# Comparing `tmp/tsx-0.1.1-py3-none-any.whl.zip` & `tmp/tsx-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5643 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       58 b- defN 22-Nov-30 13:09 tsx/__init__.py
--rw-rw-rw-  2.0 fat     7868 b- defN 22-Dec-24 09:52 tsx/ts.py
--rw-rw-rw-  2.0 fat     1089 b- defN 22-Dec-24 09:53 tsx-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3590 b- defN 22-Dec-24 09:53 tsx-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Dec-24 09:53 tsx-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 22-Dec-24 09:53 tsx-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      501 b- defN 22-Dec-24 09:53 tsx-0.1.1.dist-info/RECORD
-7 files, 13202 bytes uncompressed, 4763 bytes compressed:  63.9%
+Zip file size: 5807 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       58 b- defN 23-May-02 20:29 tsx/__init__.py
+-rw-rw-rw-  2.0 fat     8163 b- defN 23-May-02 20:49 tsx/ts.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-May-02 21:05 tsx-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3756 b- defN 23-May-02 21:05 tsx-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 21:05 tsx-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-02 21:05 tsx-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      501 b- defN 23-May-02 21:05 tsx-0.1.2.dist-info/RECORD
+7 files, 13663 bytes uncompressed, 4927 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: tsx/__init__.py
 Comment: 
 
 Filename: tsx/ts.py
 Comment: 
 
-Filename: tsx-0.1.1.dist-info/LICENSE
+Filename: tsx-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: tsx-0.1.1.dist-info/METADATA
+Filename: tsx-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: tsx-0.1.1.dist-info/WHEEL
+Filename: tsx-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: tsx-0.1.1.dist-info/top_level.txt
+Filename: tsx-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tsx-0.1.1.dist-info/RECORD
+Filename: tsx-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsx/ts.py

```diff
@@ -95,54 +95,64 @@
                 float_val = dt.timestamp()
                 return float_val
             except Exception:
                 pass
         return cls._from_number(float(ts), prec)
 
     def __new__(
-        cls,
-        ts: Union[int, float, str],
-        prec: Literal["s", "ms", "us", "ns"] = "s",
-        utc: bool = True,
+            cls,
+            ts: Union[int, float, str],
+            prec: Literal["s", "ms", "us", "ns"] = "s",
+            utc: bool = True,
     ):
         float_val = cls._parse_to_float(ts, prec, utc)
         return float.__new__(cls, float_val)
 
+    def as_dt(self, tz: tzinfo = timezone.utc) -> datetime:
+        """
+        Returns an "aware" datetime object in UTC by default
+        """
+        return datetime.fromtimestamp(self, tz=tz)
+
+    def as_local_dt(self) -> datetime:
+        """
+        Returns an "aware" datetime object in local time
+        Note: We need to call astimezone as fromtimestamp returns a naive datetime otherwise
+        """
+        return datetime.fromtimestamp(self, tz=None).astimezone()
+
     @property
     def as_iso(self) -> str:
-        dt = datetime.fromtimestamp(self, tz=timezone.utc)
-        s = dt.isoformat()
+        s = self.as_dt().isoformat()
         s = s.replace("+00:00", "Z")
         return s
 
     @property
     def as_iso_date(self) -> str:
         """Returns Extended ISO date format"""
-        dt = datetime.fromtimestamp(self, tz=timezone.utc)
-        s = dt.strftime("%Y-%m-%d")
+        s = self.as_dt().strftime("%Y-%m-%d")
         return s
 
     @property
     def as_iso_date_basic(self) -> str:
         """Returns Basic ISO date format"""
-        dt = datetime.fromtimestamp(self, tz=timezone.utc)
-        s = dt.strftime("%Y%m%d")
+        s = self.as_dt().strftime("%Y%m%d")
         return s
 
     def as_iso_tz(self, tz: Union[str, tzinfo]) -> str:
         if isinstance(tz, str):
             tz = pytz.timezone(tz)
-        dt = datetime.fromtimestamp(self, tz=tz)
+        dt = self.as_dt(tz=tz)
         s = dt.isoformat()
         s = s.replace("+00:00", "Z")
         return s
 
     @property
     def as_iso_basic(self) -> str:
-        dt = datetime.fromtimestamp(self, tz=timezone.utc)
+        dt = self.as_dt()
         s = dt.strftime("%Y%m%d-%H%M%S")
         return s
 
     as_file_ts = as_iso_basic
     as_file_date = as_iso_date_basic
 
     @property
@@ -205,15 +215,15 @@
     def weekday(self, utc: bool = True) -> int:
         """
         Return the day of the week as an integer, where Monday is 0 and Sunday is 6. See also isoweekday().
         """
         if utc:
             return int((self - FIRST_MONDAY_TS) / (24 * 3600)) % 7
         else:
-            dt = datetime.fromtimestamp(self)
+            dt = self.as_local_dt()
             return dt.weekday()
 
     def isoweekday(self, utc: bool = True) -> int:
         """
         Return the day of the week as an integer, where Monday is 1 and Sunday is 7. See also weekday().
         """
         return self.weekday(utc) + 1
```

## Comparing `tsx-0.1.1.dist-info/LICENSE` & `tsx-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsx-0.1.1.dist-info/METADATA` & `tsx-0.1.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-Metadata-Version: 2.1
-Name: tsx
-Version: 0.1.1
-Summary: TimeStam eXtensions for Python
-Home-page: https://github.com/asuiu/tsx
-Author: Andrei Suiu
-Author-email: andrei.suiu@gmail.com
-License: GPL
-Keywords: timestamp time date datetime ISO 8601
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: System :: Logging
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Internet :: Log Analysis
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typing-extensions (>=3.7.4)
-Requires-Dist: python-dateutil (>=2.8.2)
-Requires-Dist: pytz (>=2020.1)
-Requires-Dist: ciso8601 (>=2.3.0)
-
-# tsx
-
-
-
-**T**ime **S**tamp e**X**tensions for Python
-
-
-
-This library was created as a response to the known Python datetime standard library flaw that violates ISO
-
-8601. ( [Example](https://stackoverflow.com/questions/19654578/python-utc-datetime-objects-iso-format-doesnt-include-z-zulu-or-zero-offset) )
-
-
-
-Under the hood, it uses external dateparser library that's fully compatible with ISO 8601, and it simplifies working
-
-with date & time stamps.
-
-
-
-It also handles properly the Daylight Saving Time (summer time).
-
-
-
-### Installation
-
-
-
-`pip pinstall tsx`
-
-
-
-### Usage:
-
-
-
-The library is pretty simple, its central class is `TS`, which inhertis Python builtin `float`,
-
-so every timestamp in fact is a float representing number of seconds since Epoch.
-
-
-
-The `TSMsec` is the same `TS` with only difference that it's constructor by default expects msec precision, i.e. number
-
-of msecs since epoch,
-
-but internally it will store the same float as number of seconds since Epoch.
-
-
-
-```python
-
-TS(ts: Union[int, float, str], prec: Literal["s", "ms"] = "s")`
-
-
-
-TSMsec(ts: Union[int, float, str], prec: Literal["s", "ms"] = "ms")
-
-```
-
-
-
-- `prec` - is precision of the `ts` argument.
-
-    - If `prec=="s"` - the `ts` argument will be interpreted as nr of seconds since epoch,
-
-    - If `prec=="ms"` - the `ts` argument will be interpreted as nr of milliseconds since epoch
-
-
-
-### Example:
-
-
-
-```python
-
-ts = TS(ts="1519855200.123856", prec="s")
-
-
-
-ts == 1519855200.123856
-
-ts.as_iso == '2018-02-28T22:00:00.123856Z'
-
-ts.as_iso_tz(pytz.timezone("Europe/Bucharest")) == '2018-03-01T00:00:00.123856+02:00'
-
-
-
-TS("2018-02-28T22:00:00.123Z")
-
-TS("2018-02-28T22:00:00.123")
-
-
-
-TS("2018-02-28T22:00:00.123+00:00")
-
-```
-
-
-
-```python
-
-ts = TS.now()
-
-
-
-ts.as_sec == 1234567890.123
-
-ts.as_ms == 1234567890123
-
-ts.as_file_date == '20090213'
-
-ts.as_file_ts == '20090213-233130'
-
-```
-
-
-
-### Changelog
-
-
-
-##### 0.1.0
-
-
-
-- Added the `utc:bool=True` parameter to TS constructor, which if set to `True` (by default) will force the timestamp to
-
-  be interpreted as UTC, thus `TS('2018-02-28T22:00:00') will be interpreted as UTC, and not as local time, even if it
-
-  doesn't have explicit TZ info.
-
-- Improved speed of TS.from_iso(). For Python <3.11 it uses [`ciso8601`](https://github.com/closeio/ciso8601) which is
-
-  the fastest ISO 8601 parser, and for Python >= 3.11 it uses the builtin `datetime.fromisoformat()`.
-
-- some minor parsing speed improvements
-
-- added public time utility variables `FIRST_MONDAY_TS`, `DAY_SEC`, `DAY_MSEC`, `WEEK_SEC`
+Metadata-Version: 2.1
+Name: tsx
+Version: 0.1.2
+Summary: TimeStam eXtensions for Python
+Home-page: https://github.com/asuiu/tsx
+Author: Andrei Suiu
+Author-email: andrei.suiu@gmail.com
+License: GPL
+Keywords: timestamp time date datetime ISO 8601
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing-extensions (>=3.7.4)
+Requires-Dist: python-dateutil (>=2.8.2)
+Requires-Dist: pytz (>=2020.1)
+Requires-Dist: ciso8601 (>=2.3.0)
+
+# tsx
+
+
+
+**T**ime **S**tamp e**X**tensions for Python
+
+
+
+This library was created as a response to the known Python datetime standard library flaw that violates ISO
+
+8601. ( [Example](https://stackoverflow.com/questions/19654578/python-utc-datetime-objects-iso-format-doesnt-include-z-zulu-or-zero-offset) )
+
+
+
+Under the hood, it uses external dateparser library that's fully compatible with ISO 8601, and it simplifies working
+
+with date & time stamps.
+
+
+
+It also handles properly the Daylight Saving Time (summer time).
+
+
+
+### Installation
+
+
+
+`pip pinstall tsx`
+
+
+
+### Usage:
+
+
+
+The library is pretty simple, its central class is `TS`, which inhertis Python builtin `float`,
+
+so every timestamp in fact is a float representing number of seconds since Epoch.
+
+
+
+The `TSMsec` is the same `TS` with only difference that it's constructor by default expects msec precision, i.e. number
+
+of msecs since epoch,
+
+but internally it will store the same float as number of seconds since Epoch.
+
+
+
+```python
+
+TS(ts: Union[int, float, str], prec: Literal["s", "ms"] = "s")`
+
+
+
+TSMsec(ts: Union[int, float, str], prec: Literal["s", "ms"] = "ms")
+
+```
+
+
+
+- `prec` - is precision of the `ts` argument.
+
+    - If `prec=="s"` - the `ts` argument will be interpreted as nr of seconds since epoch,
+
+    - If `prec=="ms"` - the `ts` argument will be interpreted as nr of milliseconds since epoch
+
+
+
+### Example:
+
+
+
+```python
+
+ts = TS(ts="1519855200.123856", prec="s")
+
+
+
+ts == 1519855200.123856
+
+ts.as_iso == '2018-02-28T22:00:00.123856Z'
+
+ts.as_iso_tz(pytz.timezone("Europe/Bucharest")) == '2018-03-01T00:00:00.123856+02:00'
+
+
+
+TS("2018-02-28T22:00:00.123Z")
+
+TS("2018-02-28T22:00:00.123")
+
+
+
+TS("2018-02-28T22:00:00.123+00:00")
+
+```
+
+
+
+```python
+
+ts = TS.now()
+
+
+
+ts.as_sec == 1234567890.123
+
+ts.as_ms == 1234567890123
+
+ts.as_file_date == '20090213'
+
+ts.as_file_ts == '20090213-233130'
+
+```
+
+
+
+### Changelog
+
+
+
+##### 0.1.0
+
+
+
+- Added the `utc:bool=True` parameter to TS constructor, which if set to `True` (by default) will force the timestamp to
+
+  be interpreted as UTC, thus `TS('2018-02-28T22:00:00') will be interpreted as UTC, and not as local time, even if it
+
+  doesn't have explicit TZ info.
+
+- Improved speed of TS.from_iso(). For Python <3.11 it uses [`ciso8601`](https://github.com/closeio/ciso8601) which is
+
+  the fastest ISO 8601 parser, and for Python >= 3.11 it uses the builtin `datetime.fromisoformat()`.
+
+- some minor parsing speed improvements
+
+- added public time utility variables `FIRST_MONDAY_TS`, `DAY_SEC`, `DAY_MSEC`, `WEEK_SEC`
```

