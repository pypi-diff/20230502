# Comparing `tmp/nepali-0.5.6.tar.gz` & `tmp/nepali-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepali-0.5.6.tar", last modified: Thu Jul  7 07:42:27 2022, max compression
+gzip compressed data, was "nepali-1.0.0.tar", last modified: Tue May  2 15:35:41 2023, max compression
```

## Comparing `nepali-0.5.6.tar` & `nepali-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.106155 nepali-0.5.6/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1073 2022-07-07 07:42:16.000000 nepali-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-07-07 07:42:27.106155 nepali-0.5.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     4341 2022-07-07 07:42:16.000000 nepali-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.102155 nepali-0.5.6/nepali/
--rwxr-xr-x   0 runner    (1001) docker     (121)       15 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2606 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/char.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.102155 nepali-0.5.6/nepali/datetime/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12530 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10284 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     6407 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/_formarter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/_humanize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.102155 nepali-0.5.6/nepali/datetime/parser/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/parser/_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     8648 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/datetime/parser/validators.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      323 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/number.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.106155 nepali-0.5.6/nepali/templatetags/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/templatetags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1225 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/templatetags/nepalidatetime.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/templatetags/nepalinumber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.106155 nepali-0.5.6/nepali/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/tests/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (121)     6506 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/tests/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      565 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/timezone.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2421 2022-07-07 07:42:16.000000 nepali-0.5.6/nepali/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 07:42:27.102155 nepali-0.5.6/nepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-07-07 07:42:27.000000 nepali-0.5.6/nepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-07-07 07:42:27.000000 nepali-0.5.6/nepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 07:42:27.000000 nepali-0.5.6/nepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-07 07:42:27.000000 nepali-0.5.6/nepali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-07 07:42:27.000000 nepali-0.5.6/nepali.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-07 07:42:27.106155 nepali-0.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1317 2022-07-07 07:42:16.000000 nepali-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-05-02 15:35:29.000000 nepali-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-05-02 15:35:41.442139 nepali-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-02 15:35:29.000000 nepali-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3437 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/date_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_nepalimonth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_nepaliweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali/datetime/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/parser/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/parser/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216494 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/number/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/_nepalinumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/templatetags/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/templatetags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/templatetags/nepalidatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/templatetags/nepalinumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_date_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_nepalimonth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_nepaliweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117623 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_timezone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/timezone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:35:41.442139 nepali-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-02 15:35:29.000000 nepali-1.0.0/setup.py
```

### Comparing `nepali-0.5.6/LICENSE` & `nepali-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nepali-0.5.6/nepali/datetime/parser/_parser.py` & `nepali-1.0.0/nepali/datetime/parser/_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 from nepali.exceptions import InvalidDateTimeFormatException, FormatNotMatchException
 
-from.validators import validate
+from .validators import validate
 
-__all__ = ["strptime", "parse",]
+__all__ = [
+    "strptime",
+    "parse",
+]
 
 _standard_datetime_format_CACHE = None
 
+
 def strptime(datetime_str, format):
-	'''
-	Parses nepalidatetime str with the corresponding format.
-	returns nepalidatetime object.
-	'''
-	nepalidatetime_object = validate(datetime_str, format)
-	if nepalidatetime_object == None:
-		raise FormatNotMatchException('Datetime string did not match with the given format.') 
-	return nepalidatetime_object
+    """
+    Parses nepalidatetime str with the corresponding format.
+    returns nepalidatetime object.
+    """
+    nepalidatetime_object = validate(datetime_str, format)
+    if nepalidatetime_object is None:
+        raise FormatNotMatchException(
+            "Datetime string did not match with the given format."
+        )
+    return nepalidatetime_object
+
 
 def _get_standard_formats():
-	global _standard_datetime_format_CACHE
-	if _standard_datetime_format_CACHE != None:
-		return _standard_datetime_format_CACHE
-
-	STANDARD_DATE_FORMAT = [
-		'%Y-%m-%d',
-		'%d-%m-%Y',
-		'%Y %m %d',
-		'%Y %B %d',
-		'%d %B %Y',
-		'%d %B, %Y',
-		'%B %d, %Y',
-		'%Y/%m/%d',
-		'%d/%m/%Y',
-	]
-
-	STANDARD_TIME_FORMAT = [
-		'%H:%M',
-		'%I:%M %p',
-		'%I %p',
-		'%I%p',
-		'%H:%M:%S',
-		'%H:%M:%S:%f',
-	]
-
-	_standard_datetime_format_CACHE = STANDARD_DATE_FORMAT.copy()
-	for time_format in STANDARD_TIME_FORMAT:
-		for date_format in STANDARD_DATE_FORMAT:
-			_standard_datetime_format_CACHE += ['{} {}'.format(date_format, time_format)]
-			_standard_datetime_format_CACHE += ['{}, {}'.format(date_format, time_format)]
-	return _standard_datetime_format_CACHE
+    global _standard_datetime_format_CACHE
+    if _standard_datetime_format_CACHE is not None:
+        return _standard_datetime_format_CACHE
+
+    STANDARD_DATE_FORMAT = [
+        "%Y-%m-%d",
+        "%d-%m-%Y",
+        "%Y %m %d",
+        "%Y %B %d",
+        "%d %B %Y",
+        "%d %B, %Y",
+        "%B %d, %Y",
+        "%Y/%m/%d",
+        "%d/%m/%Y",
+    ]
+
+    STANDARD_TIME_FORMAT = [
+        "%H:%M",
+        "%I:%M %p",
+        "%I %p",
+        "%I%p",
+        "%H:%M:%S",
+        "%H:%M:%S:%f",
+    ]
+
+    _standard_datetime_format_CACHE = STANDARD_DATE_FORMAT.copy()
+    for time_format in STANDARD_TIME_FORMAT:
+        for date_format in STANDARD_DATE_FORMAT:
+            _standard_datetime_format_CACHE += [
+                "{} {}".format(date_format, time_format)
+            ]
+            _standard_datetime_format_CACHE += [
+                "{}, {}".format(date_format, time_format)
+            ]
+    return _standard_datetime_format_CACHE
 
 
 def parse(datetime_str):
-	"""
-	parses nepali datetime
-	eg. parse('2078-10-12') => <NepaliDateTime: 2078-10-12>
-	"""
-	standard_formats = _get_standard_formats()
-	nepalidatetime_object = None
-	for format in standard_formats:
-		nepalidatetime_object = validate(datetime_str, format=format)
-		if nepalidatetime_object != None:
-			return nepalidatetime_object
+    """
+    parses nepali datetime
+    eg. parse('2078-10-12') => <NepaliDateTime: 2078-10-12>
+    """
+    standard_formats = _get_standard_formats()
+    nepalidatetime_object = None
+    for format in standard_formats:
+        nepalidatetime_object = validate(datetime_str, format=format)
+        if nepalidatetime_object is not None:
+            return nepalidatetime_object
 
-	raise InvalidDateTimeFormatException('Invalid format to parse nepali datetime.') 
+    raise InvalidDateTimeFormatException("Invalid format to parse nepali datetime.")
```

### Comparing `nepali-0.5.6/nepali/datetime/parser/validators.py` & `nepali-1.0.0/nepali/datetime/parser/validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,149 @@
-'''
+"""
 validates parsing
-'''
+"""
 import re
-from datetime import date
 
-from nepali.char import EnglishChar, nepali_to_english_text
-from nepali.datetime import nepalidatetime
+from nepali.char import nepali_to_english_text
+from nepali.datetime import nepalidatetime, nepalimonth, nepaliweek
+from nepali.datetime.constants import MONTHS_EN, WEEKS_EN, WEEKS_ABBR_EN
 
 
 __nepali_time_re__CACHE = None
 
+
 class NepaliTimeRE(dict):
-    
     def __init__(self):
         """Create keys/values.
         Order of execution is important for dependency reasons.
         """
         base = super()
-        base.__init__({
-            # The " [1-9]" part of the regex is to make %c from ANSI C work
-            'd': r"(?P<d>3[0-2]|[1-2]\d|0[1-9]|[1-9]| [1-9])",
-            '-d': r"(?P<d>3[0-2]|[1-2]\d|0[1-9]|[1-9]| [1-9])", # same as "d"
-            'f': r"(?P<f>[0-9]{1,6})",
-            'H': r"(?P<H>2[0-3]|[0-1]\d|\d)",
-            '-H': r"(?P<H>2[0-3]|[0-1]\d|\d)",
-            'I': r"(?P<I>1[0-2]|0[1-9]|[1-9])",
-            '-I': r"(?P<I>1[0-2]|0[1-9]|[1-9])",
-            'G': r"(?P<G>\d\d\d\d)",
-            'j': r"(?P<j>36[0-6]|3[0-5]\d|[1-2]\d\d|0[1-9]\d|00[1-9]|[1-9]\d|0[1-9]|[1-9])",
-            'm': r"(?P<m>1[0-2]|0[1-9]|[1-9])",
-            '-m': r"(?P<m>1[0-2]|0[1-9]|[1-9])", # same as "m"
-            'M': r"(?P<M>[0-5]\d|\d)",
-            '-M': r"(?P<M>[0-5]\d|\d)", # same as "M"
-            'S': r"(?P<S>6[0-1]|[0-5]\d|\d)",
-            '-S': r"(?P<S>6[0-1]|[0-5]\d|\d)", # same as "S"
-            'w': r"(?P<w>[0-6])",
-
-            'y': r"(?P<y>\d\d)",
-            'Y': r"(?P<Y>\d\d\d\d)",
-            'z': r"(?P<z>[+-]\d\d:?[0-5]\d(:?[0-5]\d(\.\d{1,6})?)?|(?-i:Z))",
-
-            'A': self.__seqToRE(EnglishChar.days, 'A'),
-            'a': self.__seqToRE(EnglishChar.days_half, 'a'),
-            'B': self.__seqToRE(EnglishChar.months, 'B'),
-            'b': self.__seqToRE(EnglishChar.months, 'b'),
-            'p': self.__seqToRE(('AM', 'PM',), 'p'),
-
-            '%': '%'
-        })
-    
+        base.__init__(
+            {
+                # The " [1-9]" part of the regex is to make %c from ANSI C work
+                "d": r"(?P<d>3[0-2]|[1-2]\d|0[1-9]|[1-9]| [1-9])",
+                "-d": r"(?P<d>3[0-2]|[1-2]\d|0[1-9]|[1-9]| [1-9])",  # same as "d"
+                "f": r"(?P<f>[0-9]{1,6})",
+                "H": r"(?P<H>2[0-3]|[0-1]\d|\d)",
+                "-H": r"(?P<H>2[0-3]|[0-1]\d|\d)",
+                "I": r"(?P<I>1[0-2]|0[1-9]|[1-9])",
+                "-I": r"(?P<I>1[0-2]|0[1-9]|[1-9])",
+                "G": r"(?P<G>\d\d\d\d)",
+                "j": r"(?P<j>36[0-6]|3[0-5]\d|[1-2]\d\d|0[1-9]\d|00[1-9]|[1-9]\d|0[1-9]|[1-9])",
+                "m": r"(?P<m>1[0-2]|0[1-9]|[1-9])",
+                "-m": r"(?P<m>1[0-2]|0[1-9]|[1-9])",  # same as "m"
+                "M": r"(?P<M>[0-5]\d|\d)",
+                "-M": r"(?P<M>[0-5]\d|\d)",  # same as "M"
+                "S": r"(?P<S>6[0-1]|[0-5]\d|\d)",
+                "-S": r"(?P<S>6[0-1]|[0-5]\d|\d)",  # same as "S"
+                "w": r"(?P<w>[0-6])",
+                "y": r"(?P<y>\d\d)",
+                "Y": r"(?P<Y>\d\d\d\d)",
+                "z": r"(?P<z>[+-]\d\d:?[0-5]\d(:?[0-5]\d(\.\d{1,6})?)?|(?-i:Z))",
+                "A": self.__seqToRE(WEEKS_EN, "A"),
+                "a": self.__seqToRE(WEEKS_ABBR_EN, "a"),
+                "B": self.__seqToRE(MONTHS_EN, "B"),
+                "b": self.__seqToRE(MONTHS_EN, "b"),
+                "p": self.__seqToRE(
+                    (
+                        "AM",
+                        "PM",
+                    ),
+                    "p",
+                ),
+                "%": "%",
+            }
+        )
+
     def __seqToRE(self, to_convert, directive):
         """Convert a list to a regex string for matching a directive.
         Want possible matching values to be from longest to shortest.  This
         prevents the possibility of a match occurring for a value that also
         a substring of a larger value that should have matched (e.g., 'abc'
         matching when 'abcdef' should have been the match).
         """
         to_convert = sorted(to_convert, key=len, reverse=True)
         for value in to_convert:
-            if value != '':
+            if value != "":
                 break
         else:
-            return ''
-        regex = '|'.join(re.escape(stuff) for stuff in to_convert)
-        regex = '(?P<%s>%s' % (directive, regex)
-        return '%s)' % regex
+            return ""
+        regex = "|".join(re.escape(stuff) for stuff in to_convert)
+        regex = "(?P<%s>%s" % (directive, regex)
+        return "%s)" % regex
 
     def pattern(self, format):
-        '''
+        """
         Handle conversion from format directives to regexes.
-        '''
-        processed_format = ''
+        """
+        processed_format = ""
         regex_chars = re.compile(r"([\\.^$*+?\(\){}\[\]|])")
         format = regex_chars.sub(r"\\\1", format)
-        whitespace_replacement = re.compile(r'\s+')
-        format = whitespace_replacement.sub(r'\\s+', format)
-        while '%' in format:
-            directive_index = format.index('%')+1
+        whitespace_replacement = re.compile(r"\s+")
+        format = whitespace_replacement.sub(r"\\s+", format)
+        while "%" in format:
+            directive_index = format.index("%") + 1
             index_increment = 1
-            
-            if format[directive_index] == '-':
+
+            if format[directive_index] == "-":
                 index_increment = 2
-            
-            if format[directive_index: directive_index+index_increment] not in self:
+
+            if format[directive_index : directive_index + index_increment] not in self:
                 return None
 
-            processed_format = "%s%s%s" % (processed_format,
-                                            format[:directive_index-1],
-                                            self[format[directive_index: directive_index+index_increment]])
-            format = format[directive_index+index_increment:]
+            processed_format = "%s%s%s" % (
+                processed_format,
+                format[: directive_index - 1],
+                self[format[directive_index : directive_index + index_increment]],
+            )
+            format = format[directive_index + index_increment :]
         return "^%s%s$" % (processed_format, format)
 
     def compile(self, format):
         """Return a compiled re object for the format string."""
         return re.compile(self.pattern(format), re.IGNORECASE)
 
+
 def get_nepali_time_re_object():
     global __nepali_time_re__CACHE
-    if __nepali_time_re__CACHE == None:
+    if __nepali_time_re__CACHE is None:
         __nepali_time_re__CACHE = NepaliTimeRE()
     return __nepali_time_re__CACHE
 
 
 def extract(datetime_str, format):
-    '''
+    """
     Extracts year, month, day, hour, minute, etc from the given format.
-    
+
     eg.
     USAGE: extract("2078-01-12", format="%Y-%m-%d")
     INPUT:
-    datetime_str="2078-01-12" 
+    datetime_str="2078-01-12"
     format="%Y-%m-%d"
 
     OUTPUT:
     {
         "Y": 2078,
         "m": 1,
         "d": 12,
     }
-    '''
+    """
 
     # converting datetime_str to english if any exists
     datetime_str = nepali_to_english_text(datetime_str)
 
     re_compiled_format = get_nepali_time_re_object().compile(format=format)
     match = re_compiled_format.match(datetime_str)
-    if match == None:
+    if match is None:
         return {}
     return match.groupdict()
 
+
 def transform(data: dict):
-    '''
+    """
     transforms different format data to uniform data
 
     eg.
     INPUT:
     data = {
         "Y": 2078,
         "b": "Mangsir",
@@ -145,118 +154,114 @@
     OUTPUT:
     {
         "year": 2078,
         "month": 8,
         "day": 12,
         ...
     }
-    '''
+    """
 
     year = None
     month = day = 1
     hour = minute = second = fraction = 0
     weekday = None
 
     for date_key in data.keys():
-        if date_key == 'y':
-            year = int(data['y'])
+        if date_key == "y":
+            year = int(data["y"])
             year += 2000
-        elif date_key == 'Y':
-            year = int(data['Y'])
-        elif date_key == 'm':
-            month = int(data['m'])
-        elif date_key == 'B':
-            # TODO: change indexing process
-            month = EnglishChar.months.index(data['B'].lower().capitalize()) + 1
-        elif date_key == 'b':
-            # TODO: change indexing process
-            month = EnglishChar.months.index(data['b'].lower().capitalize()) + 1
-        elif date_key == 'd':
-            day = int(data['d'])
-        elif date_key == 'H':
-            hour = int(data['H'])
-        elif date_key == 'I':
-            hour = int(data['I'])
-            ampm = data.get('p', '').lower()
+        elif date_key == "Y":
+            year = int(data["Y"])
+        elif date_key == "m":
+            month = int(data["m"])
+        elif date_key == "B":
+            month = nepalimonth(data["B"])
+        elif date_key == "b":
+            month = nepalimonth(data["b"])
+        elif date_key == "d":
+            day = int(data["d"])
+        elif date_key == "H":
+            hour = int(data["H"])
+        elif date_key == "I":
+            hour = int(data["I"])
+            ampm = data.get("p", "").lower()
             # If there was no AM/PM indicator, we'll treat this like AM
-            if ampm in ('', 'am'):
+            if ampm in ("", "am"):
                 # We're in AM so the hour is correct unless we're
                 # looking at 12 midnight.
                 # 12 midnight == 12 AM == hour 0
                 if hour == 12:
                     hour = 0
-            elif ampm == 'pm':
+            elif ampm == "pm":
                 # We're in PM so we need to add 12 to the hour unless
                 # we're looking at 12 noon.
                 # 12 noon == 12 PM == hour 12
                 if hour != 12:
                     hour += 12
-        elif date_key == 'M':
-            minute = int(data['M'])
-        elif date_key == 'S':
-            second = int(data['S'])
-        elif date_key == 'f':
-            s = data['f']
+        elif date_key == "M":
+            minute = int(data["M"])
+        elif date_key == "S":
+            second = int(data["S"])
+        elif date_key == "f":
+            s = data["f"]
             # Pad to always return microseconds.
             s += "0" * (6 - len(s))
             fraction = int(s)
-        elif date_key == 'A':
-            # TODO: change indexing process
-            weekday = EnglishChar.days.index(data['A'].lower().capitalize()) + 1
-        elif date_key == 'a':
-            # TODO: change indexing process
-            weekday = EnglishChar.days_half.index(data['a'].lower().capitalize()) + 1
-        elif date_key == 'w':
-            weekday = int(data['w'])
+        elif date_key == "A":
+            weekday = nepaliweek(data["A"])
+        elif date_key == "a":
+            weekday = nepaliweek(data["a"])
+        elif date_key == "w":
+            weekday = int(data["w"])
             if weekday == 0:
                 weekday = 6
             else:
                 weekday -= 1
     return {
-        'year': year,
-        'month': month,
-        'day': day,
-        'hour': hour,
-        'minute': minute,
-        'second': second,
-        'microsecond': fraction,
-        'weekday': weekday,
+        "year": year,
+        "month": month,
+        "day": day,
+        "hour": hour,
+        "minute": minute,
+        "second": second,
+        "microsecond": fraction,
+        "weekday": weekday,
     }
 
 
 def validate(datetime_str, format):
-    '''
+    """
     validates datetime_str with the format
     Perform step by step test for fast performance. The steps are:
     -
     -
     returns False if validation failed
     returns nepalidatetime object if validation success.
-    '''
-    
+    """
+
     # 1. validate if format is correct.
-    if get_nepali_time_re_object().pattern(format=format) == None:
+    if get_nepali_time_re_object().pattern(format=format) is None:
         # regex pattern generation failed
         return None
-    
+
     # 2. validate if parse result if not empty
     parsed_result = extract(datetime_str, format)
-    if parsed_result.get('Y') == None and parsed_result.get('y') == None:
-        # compilation failed or year included 
+    if parsed_result.get("Y") is None and parsed_result.get("y") is None:
+        # compilation failed or year included
         return None
 
     # 3. validate if transformation
     transformed_data = transform(parsed_result)
-    if transformed_data.get('year') == None:
+    if transformed_data.get("year") is None:
         # could not transform data, not getting year
         return None
 
     # 4. create the datetime object
     return nepalidatetime(
-        year=transformed_data['year'], 
-        month=transformed_data['month'], 
-        day=transformed_data['day'], 
-        hour=transformed_data['hour'],
-        minute=transformed_data['minute'],
-        second=transformed_data['second'],
-        microsecond=transformed_data['microsecond'],
-    )
+        year=transformed_data["year"],
+        month=transformed_data["month"],
+        day=transformed_data["day"],
+        hour=transformed_data["hour"],
+        minute=transformed_data["minute"],
+        second=transformed_data["second"],
+        microsecond=transformed_data["microsecond"],
+    )
```

### Comparing `nepali-0.5.6/nepali/templatetags/nepalidatetime.py` & `nepali-1.0.0/nepali/templatetags/nepalidatetime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from django import template
 from django.utils import timezone
 
-from nepali.datetime import nepalidatetime, nepalihumanize as humanize
-from nepali.utils import to_local, to_utc, to_nepali_datetime
+from nepali.datetime import nepalihumanize as humanize
+from nepali.utils import to_nepalidatetime
 
 register = template.Library()
 
-@register.filter(name='nepalidate')
+
+@register.filter(name="nepalidate")
 def nepalidate(datetime_obj, format="%B %d, %Y, %A"):
-	nepali_datetime_obj = to_nepali_datetime(datetime_obj)
-	if nepali_datetime_obj == None: return None
-	return nepali_datetime_obj.strftime(format)
+    nepali_datetime_obj = to_nepalidatetime(datetime_obj)
+    if nepali_datetime_obj is None:
+        return None
+    return nepali_datetime_obj.strftime(format)
+
 
-@register.filter(name='nepalidate_en')
+@register.filter(name="nepalidate_en")
 def nepalidate_en(datetime_obj, format="%B %d, %Y, %A"):
-	nepali_datetime_obj = to_nepali_datetime(datetime_obj)
-	if nepali_datetime_obj == None: return None
-	return nepali_datetime_obj.strftime_en(format)
+    nepali_datetime_obj = to_nepalidatetime(datetime_obj)
+    if nepali_datetime_obj is None:
+        return None
+    return nepali_datetime_obj.strftime_en(format)
+
 
-@register.filter(name='nepalihumanize')
+@register.filter(name="nepalihumanize")
 def nepalihumanize(datetime_obj, threshold=None, format=None):
-	""" templatetag to humanize nepalidatetime """
-	nepali_datetime_obj = to_nepali_datetime(datetime_obj)
-	if nepali_datetime_obj == None: return None
-	return humanize(nepali_datetime_obj, threshold=threshold, format=format)
-	
+    """templatetag to humanize nepalidatetime"""
+    nepali_datetime_obj = to_nepalidatetime(datetime_obj)
+    if nepali_datetime_obj is None:
+        return None
+    return humanize(nepali_datetime_obj, threshold=threshold, format=format)
+
+
 @register.simple_tag
 def nepalinow(format="%B %d, %Y, %A"):
-	""" templatetag to display current datetime in nepali format """
-	return to_nepali_datetime(timezone.now()).strftime(format)
+    """templatetag to display current datetime in nepali format"""
+    return to_nepalidatetime(timezone.now()).strftime(format)
```

### Comparing `nepali-0.5.6/nepali/tests/test_datetime.py` & `nepali-1.0.0/nepali/tests/test_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,164 @@
-import datetime
 import unittest
 
-from nepali.datetime import nepalidate, nepalitime, nepalidatetime
-from nepali.timezone import NepaliTimeZone
-from nepali.utils import to_nepali_timezone
-
-class TestNepaliDateTime(unittest.TestCase):
+from nepali.char import nepali_to_english_text
+from nepali.datetime import nepalidatetime
+from nepali.datetime import parser as nepalidatetime_parser
+from nepali.datetime.parser.validators import NepaliTimeRE, extract, transform, validate
+from nepali.exceptions import FormatNotMatchException, InvalidDateTimeFormatException
+
+
+class TestNepaliDateTimeParserValidators(unittest.TestCase):
+    """
+    Tests nepali date
+    """
+
+    def setUp(self) -> None:
+        self.nepali_time_re = NepaliTimeRE()
+        return super().setUp()
+
+    # test extract
+
+    def test_simple_extract(self):
+        extracted_data = extract("2078-01-12", format="%Y-%m-%d")
+        self.assertEqual(extracted_data.get("Y"), "2078")
+        self.assertEqual(extracted_data.get("m"), "01")
+        self.assertEqual(extracted_data.get("d"), "12")
+
+    def test_complex_extract(self):
+        extracted_data = extract(
+            "Wed Wednesday 3 28 Sharwan Sharwan 04 51 2051 05 05 AM 28 23",
+            format="%a %A %w %d %b %B %m %y %Y %H %I %p %M %S",
+        )
+        self.assertEqual(extracted_data.get("a"), "Wed")
+        self.assertEqual(extracted_data.get("A"), "Wednesday")
+        self.assertEqual(extracted_data.get("w"), "3")
+        self.assertEqual(extracted_data.get("d"), "28")
+        self.assertEqual(extracted_data.get("b"), "Sharwan")
+        self.assertEqual(extracted_data.get("B"), "Sharwan")
+        self.assertEqual(extracted_data.get("m"), "04")
+        self.assertEqual(extracted_data.get("y"), "51")
+        self.assertEqual(extracted_data.get("Y"), "2051")
+        self.assertEqual(extracted_data.get("H"), "05")
+        self.assertEqual(extracted_data.get("I"), "05")
+        self.assertEqual(extracted_data.get("p"), "AM")
+        self.assertEqual(extracted_data.get("M"), "28")
+        self.assertEqual(extracted_data.get("S"), "23")
+
+    def test_nepali_to_english_text_conversion(self):
+        self.assertEqual(
+            nepali_to_english_text(
+                "बुध बुधबार ३ २८ साउन साउन ०४ ५१ २०५१ ०५ ०५ शुभप्रभात २८ २३"
+            ),
+            "Wed Wednesday 3 28 Sharwan Sharwan 04 51 2051 05 05 AM 28 23",
+        )
+
+    def test_complex_extract_in_nepali(self):
+        extracted_data = extract(
+            "बुध बुधबार ३ २८ साउन साउन ०४ ५१ २०५१ ०५ ०५ शुभप्रभात २८ २३",
+            format="%a %A %w %d %b %B %m %y %Y %H %I %p %M %S",
+        )
+        self.assertEqual(extracted_data.get("a"), "Wed")
+        self.assertEqual(extracted_data.get("A"), "Wednesday")
+        self.assertEqual(extracted_data.get("w"), "3")
+        self.assertEqual(extracted_data.get("d"), "28")
+        self.assertEqual(extracted_data.get("b"), "Sharwan")
+        self.assertEqual(extracted_data.get("B"), "Sharwan")
+        self.assertEqual(extracted_data.get("m"), "04")
+        self.assertEqual(extracted_data.get("y"), "51")
+        self.assertEqual(extracted_data.get("Y"), "2051")
+        self.assertEqual(extracted_data.get("H"), "05")
+        self.assertEqual(extracted_data.get("I"), "05")
+        self.assertEqual(extracted_data.get("p"), "AM")
+        self.assertEqual(extracted_data.get("M"), "28")
+        self.assertEqual(extracted_data.get("S"), "23")
+
+    # test transform
+    def test_transform(self):
+        data = transform(
+            {
+                "Y": "2078",
+                "b": "MAngsir",
+                "d": "12",
+                "p": "pm",
+                "I": "05",
+                "M": "25",
+                "S": "31",
+                "f": "455",
+                "a": "Wed",
+            }
+        )
+        self.assertEqual(data.get("year"), 2078)
+        self.assertEqual(data.get("month"), 8)
+        self.assertEqual(data.get("day"), 12)
+        self.assertEqual(data.get("hour"), 17)
+        self.assertEqual(data.get("minute"), 25)
+        self.assertEqual(data.get("second"), 31)
+        self.assertEqual(data.get("microsecond"), 455000)
+        self.assertEqual(data.get("weekday"), 3)
 
     #
-    # nepalidate
-
-    def test_nepalidate_now_and_today(self):
-        today = nepalidate.today()
-        now = nepalidate.now()
-        self.assertEqual(today, now, msg='nepalidate today is not equals to now.')
-
-    def test_nepalidate_comparision(self):
-        nepalidate_obj1 = nepalidate(year=2051, month=4, day=28)
-
-        # test equal date
-        nepalidate_obj2 = nepalidate(year=2051, month=4, day=28)
-        self.assertEqual(nepalidate_obj1, nepalidate_obj2, 'Same nepali date are not checked equals.')
-
-        # test different date
-        nepalidate_obj3 = nepalidate(year=2051, month=4, day=29)
-        self.assertNotEqual(nepalidate_obj1, nepalidate_obj3, 'Different nepali date are checked as equal.')
-
-        # TODO: check other comparisions (later)
-
-    def test_nepalidate_year_month_day(self):
-        nepalidate_obj = nepalidate(year=2051, month=4, day=28)
-        self.assertEqual(nepalidate_obj.year, 2051)
-        self.assertEqual(nepalidate_obj.month, 4)
-        self.assertEqual(nepalidate_obj.day, 28)
-        self.assertEqual(nepalidate_obj.weekday(), 5)
-
-    def test_nepalidate_from_date(self):
-        python_date_obj = datetime.date(year=1994, month=8, day=12)
-        nepalidate_obj = nepalidate.from_date(python_date_obj)
-        self.assertEqual(python_date_obj, nepalidate_obj.to_date(), 'nepalidate from_date and to_date are not equal.')
-
-    def test_nepalidate_from_datetime(self):
-        python_datetime_obj = datetime.datetime(year=1994, month=8, day=12, hour=4, minute=8, second=12)
-        nepalidate_obj = nepalidate.from_datetime(python_datetime_obj)
-        self.assertEqual(python_datetime_obj.date(), nepalidate_obj.to_date(), 'nepalidate from_datetime and to_datetime are not equal.')
-
-    def test_nepalidate_strftime(self):
-        nepalidate_obj = nepalidate(year=2051, month=4, day=28)
-        self.assertEqual(nepalidate_obj.strftime('%Y-%m-%d'), '२०५१-०४-२८')
-        self.assertEqual(nepalidate_obj.strftime('%a %A %w %d %b %B %m %y %Y'), 'शुक्र शुक्रबार ५ २८ साउन साउन ०४ ५१ २०५१')
-        self.assertEqual(nepalidate_obj.strftime_en('%Y-%m-%d'), '2051-04-28')
-        self.assertEqual(nepalidate_obj.strftime_en('%a %A %w %d %b %B %m %y %Y'), 'Fri Friday 5 28 Sharwan Sharwan 04 51 2051')
+    # test validate
 
-    def test_nepalidate_strptime(self):
-        nepalidatetime_obj = nepalidate.strptime('2078-01-12', format='%Y-%m-%d')
+    def test_validate(self):
+        nepalidatetime_obj = validate("2078-01-12", format="%Y-%m-%d")
         self.assertEqual(nepalidatetime_obj.year, 2078)
         self.assertEqual(nepalidatetime_obj.month, 1)
         self.assertEqual(nepalidatetime_obj.day, 12)
 
-    #
-    # nepalitime
-    
-    def test_nepalitime_now(self):
-        nepalitime_obj, dt_now = nepalitime.now(), datetime.datetime.now()
-        self.assertEqual(nepalitime_obj.hour, dt_now.hour)
-        self.assertEqual(nepalitime_obj.minute, dt_now.minute)
-        self.assertEqual(nepalitime_obj.second, dt_now.second)
-
-    #
-    # nepalidatetime
-
-    def test_nepalidatetime_from_date(self):
-        python_datetime_obj = datetime.datetime(year=1994, month=8, day=12, hour=5, minute=28, second=23)
-        nepalidatetime_obj = nepalidatetime.from_date(python_datetime_obj)
-        self.assertEqual(python_datetime_obj.date(), nepalidatetime_obj.to_date())
-
-    def test_nepalidatetime_from_datetime(self):
-        python_datetime_obj = datetime.datetime(year=1994, month=8, day=12, hour=5, minute=28, second=23, tzinfo=NepaliTimeZone())
-        nepalidatetime_obj = nepalidatetime.from_datetime(python_datetime_obj)
-        self.assertEqual(python_datetime_obj, nepalidatetime_obj.to_datetime(), msg="{} and {} are not equal.".format(python_datetime_obj, nepalidatetime_obj.to_datetime()))
-
-    def test_nepalidatetime_strftime(self):
-        nepalidatetime_obj = nepalidatetime(year=2051, month=4, day=28, hour=5, minute=28, second=23)
-        self.assertEqual(nepalidatetime_obj.strftime('%Y-%m-%d %H:%M:%S'), '२०५१-०४-२८ ०५:२८:२३')
-        self.assertEqual(nepalidatetime_obj.strftime('%a %A %w %d %b %B %m %y %Y %H %I %p %M %S'), 'शुक्र शुक्रबार ५ २८ साउन साउन ०४ ५१ २०५१ ०५ ०५ शुभप्रभात २८ २३')
-        self.assertEqual(nepalidatetime_obj.strftime_en('%Y-%m-%d %H:%M:%S'), '2051-04-28 05:28:23')
-        self.assertEqual(nepalidatetime_obj.strftime_en('%a %A %w %d %b %B %m %y %Y %H %I %p %M %S'), 'Fri Friday 5 28 Sharwan Sharwan 04 51 2051 05 05 AM 28 23')
+        nepalidatetime_obj = validate("2079-03-32", format="%Y-%m-%d")
+        self.assertEqual(nepalidatetime_obj.year, 2079)
+        self.assertEqual(nepalidatetime_obj.month, 3)
+        self.assertEqual(nepalidatetime_obj.day, 32)
+
+    def test_test_validate(self):
+        nepalidatetime_obj = validate(
+            "29 Jestha, 2078, 1:30 PM", format="%d %B, %Y, %I:%M %p"
+        )
+        self.assertEqual(nepalidatetime_obj.year, 2078)
+        self.assertEqual(nepalidatetime_obj.month, 2)
+        self.assertEqual(nepalidatetime_obj.day, 29)
+        self.assertEqual(nepalidatetime_obj.hour, 13)
+        self.assertEqual(nepalidatetime_obj.minute, 30)
+        self.assertEqual(nepalidatetime_obj.second, 0)
 
-    def test_nepalidatetime_strptime(self):
-        nepalidatetime_obj = nepalidatetime.strptime('2078-01-12 13:12', format='%Y-%m-%d %H:%M')
+    def test_validate_with_invalid_data(self):
+        self.assertEqual(validate("2078-01-12", format="%k-%m-%d"), None)
+        self.assertEqual(validate("2078-01-12", format="%m-%M-%Y"), None)
+
+
+class TestNepaliDateTimeParser(unittest.TestCase):
+    """
+    Tests nepali datetime parser.
+    """
+
+    # test strptime
+    def test_strptime(self):
+        nepalidatetime_obj = nepalidatetime_parser.strptime(
+            "2078-01-12", format="%Y-%m-%d"
+        )
         self.assertEqual(nepalidatetime_obj.year, 2078)
         self.assertEqual(nepalidatetime_obj.month, 1)
         self.assertEqual(nepalidatetime_obj.day, 12)
+
+    def test_strptime_fail(self):
+        with self.assertRaises(FormatNotMatchException):
+            nepalidatetime_parser.strptime("2078-01-12", format="%Y %d")
+
+    # test parser
+
+    def test_normal_string_parse(self):
+        parsed_datetime = nepalidatetime_parser.parse("2071-01-24")
+        test_datetime = nepalidatetime(2071, 1, 24)
+        self.assertEqual(parsed_datetime, test_datetime)
+
+    def test_complex_string_parse(self):
+        nepalidatetime_obj = nepalidatetime_parser.parse("29 Jestha, 2078, 1:30 PM")
+        self.assertEqual(nepalidatetime_obj.year, 2078)
+        self.assertEqual(nepalidatetime_obj.month, 2)
+        self.assertEqual(nepalidatetime_obj.day, 29)
         self.assertEqual(nepalidatetime_obj.hour, 13)
-        self.assertEqual(nepalidatetime_obj.minute, 12)
+        self.assertEqual(nepalidatetime_obj.minute, 30)
 
-    def test_nepalidatetime_timedelta(self):
-        nepalidatetime_obj1 = nepalidatetime(year=2051, month=4, day=28, hour=5, minute=28, second=23)
-        nepalidatetime_obj2 = nepalidatetime(year=2051, month=4, day=29, hour=5, minute=28, second=23)
-        nepalidatetime_obj1 = nepalidatetime_obj1 + datetime.timedelta(days=1)
-        self.assertEqual(nepalidatetime_obj1, nepalidatetime_obj2, msg='{} and {} are not equal'.format(nepalidatetime_obj1, nepalidatetime_obj2))
+    def test_parse_failed(self):
+        with self.assertRaises(InvalidDateTimeFormatException):
+            nepalidatetime_parser.parse("")
```

### Comparing `nepali-0.5.6/nepali.egg-info/SOURCES.txt` & `nepali-1.0.0/nepali.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 LICENSE
 README.md
 setup.py
 nepali/__init__.py
 nepali/char.py
+nepali/date_converter.py
 nepali/exceptions.py
-nepali/number.py
+nepali/phone_number.py
 nepali/timezone.py
 nepali/utils.py
 nepali.egg-info/PKG-INFO
 nepali.egg-info/SOURCES.txt
 nepali.egg-info/dependency_links.txt
-nepali.egg-info/requires.txt
 nepali.egg-info/top_level.txt
 nepali/datetime/__init__.py
-nepali/datetime/_converter.py
 nepali/datetime/_datetime.py
-nepali/datetime/_formarter.py
+nepali/datetime/_formatter.py
 nepali/datetime/_humanize.py
+nepali/datetime/_nepalimonth.py
+nepali/datetime/_nepaliweek.py
+nepali/datetime/constants.py
+nepali/datetime/utils.py
 nepali/datetime/parser/__init__.py
 nepali/datetime/parser/_parser.py
 nepali/datetime/parser/validators.py
+nepali/locations/__init__.py
+nepali/locations/_data.py
+nepali/locations/_locations.py
+nepali/locations/models.py
+nepali/locations/utils.py
+nepali/number/__init__.py
+nepali/number/_nepalinumber.py
+nepali/number/_number.py
+nepali/number/utils.py
 nepali/templatetags/__init__.py
 nepali/templatetags/nepalidatetime.py
 nepali/templatetags/nepalinumber.py
 nepali/tests/__init__.py
+nepali/tests/test_date_converter.py
 nepali/tests/test_datetime.py
 nepali/tests/test_humanize.py
-nepali/tests/test_parser.py
+nepali/tests/test_locations.py
+nepali/tests/test_nepalimonth.py
+nepali/tests/test_nepaliweek.py
+nepali/tests/test_number.py
+nepali/tests/test_parser.py
+nepali/tests/test_phone_number.py
+nepali/tests/test_timezone.py
```

### Comparing `nepali-0.5.6/setup.py` & `nepali-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 """
 setup file for nepali package
 
-- Publish version
-$ python setup.py publish
+- Building a package
+
+    pip install build
+    python -m build
 
-- Alternative
-pip install build
-python -m build
-"""
 
+- Publishing a package
+You must have twine installed in your system. `pip install twine`
 
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
+
+"""
 import os
 import sys
 import setuptools
 
 with open("README.md", "r") as fh:
-	long_description = fh.read()
+    long_description = fh.read()
 
 
-if sys.argv[-1] == 'publish':
-	if os.system("pip3 freeze | grep twine"):
-		print("twine not installed.\nUse `pip install twine`.\nExiting.")
-		sys.exit()
-	os.system("rm -rf dist")
-	os.system("python3 setup.py sdist bdist_wheel")
-	os.system("twine upload dist/*")
-	sys.exit()
+if sys.argv[-1] == "publish":
+    if os.system("pip3 freeze | grep twine"):
+        print("twine not installed.\nUse `pip install twine`.\nExiting.")
+        sys.exit()
+    os.system("rm -rf dist")
+    os.system("python3 setup.py sdist bdist_wheel")
+    os.system("twine upload dist/*")
+    sys.exit()
 
 
 setuptools.setup(
-	name="nepali",
-	version="0.5.6",
-	author="Ajesh Sen Thapa",
-	author_email="aj3sshh@gmail.com",
-	description="nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime",
-	long_description=long_description,
-	long_description_content_type="text/markdown",
-	keywords=['nepali date conversion', 'convert date', 'nepali date time', 'python convert date', 'parse nepali date time'],
-	url="https://github.com/aj3sh/nepali",
-	packages=setuptools.find_packages(),
-	test_suite='nepali.tests',
-	install_requires=[
-		'pytz'
-	],
-	classifiers=[
-
-		'Programming Language :: Python :: 3',
-		'License :: OSI Approved :: MIT License',
-		'Operating System :: OS Independent',
-	],
+    name="nepali",
+    version="1.0.0",
+    author="opensource-nepal",
+    author_email="aj3sshh@gmail.com, sugatbajracharya49@gmail.com",
+    description="nepalidatetime compatible with python's datetime feature. "
+    "Converting nepali date to english, parsing nepali datetime, "
+    "nepali timezone, and timedelta support in nepali datetime",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    keywords=[
+        "nepali date conversion",
+        "convert date",
+        "nepali date time",
+        "python convert date",
+        "parse nepali date time",
+    ],
+    url="https://github.com/opensource-nepal/py-nepali",
+    packages=setuptools.find_packages(),
+    test_suite="nepali.tests",
+    install_requires=[],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
 )
```

