# Comparing `tmp/ph-1.1.3.tar.gz` & `tmp/ph-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ph-1.1.3.tar", last modified: Thu Nov  3 12:55:07 2022, max compression
+gzip compressed data, was "ph-1.1.4.tar", last modified: Tue May  2 19:27:37 2023, max compression
```

## Comparing `ph-1.1.3.tar` & `ph-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2022-11-03 12:55:07.015111 ph-1.1.3/
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)     1077 2021-06-27 12:07:31.000000 ph-1.1.3/LICENSE
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)    27143 2022-11-03 12:55:07.015111 ph-1.1.3/PKG-INFO
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)    26374 2022-07-16 20:01:07.000000 ph-1.1.3/README.md
-drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2022-11-03 12:55:07.011111 ph-1.1.3/ph/
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)    48451 2022-06-30 09:53:50.000000 ph-1.1.3/ph/__init__.py
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)       22 2022-11-03 12:54:06.000000 ph-1.1.3/ph/_version.py
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)    97434 2022-11-03 12:53:43.000000 ph-1.1.3/ph/tabulate.py
-drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2022-11-03 12:55:07.015111 ph-1.1.3/ph.egg-info/
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)    27143 2022-11-03 12:55:06.000000 ph-1.1.3/ph.egg-info/PKG-INFO
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)      229 2022-11-03 12:55:07.000000 ph-1.1.3/ph.egg-info/SOURCES.txt
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)        1 2022-11-03 12:55:06.000000 ph-1.1.3/ph.egg-info/dependency_links.txt
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)       31 2022-11-03 12:55:06.000000 ph-1.1.3/ph.egg-info/entry_points.txt
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)      299 2022-11-03 12:55:06.000000 ph-1.1.3/ph.egg-info/requires.txt
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)        3 2022-11-03 12:55:06.000000 ph-1.1.3/ph.egg-info/top_level.txt
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)       38 2022-11-03 12:55:07.015111 ph-1.1.3/setup.cfg
--rw-r--r--   0 pdr081   (129968) ansatt    (4601)     2082 2022-06-27 20:36:16.000000 ph-1.1.3/setup.py
+drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2023-05-02 19:27:37.223857 ph-1.1.4/
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)     1077 2021-06-27 12:07:31.000000 ph-1.1.4/LICENSE
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)    27143 2023-05-02 19:27:37.223857 ph-1.1.4/PKG-INFO
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)    26374 2022-07-16 20:01:07.000000 ph-1.1.4/README.md
+drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2023-05-02 19:27:37.223857 ph-1.1.4/ph/
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)    51203 2023-05-02 19:26:06.000000 ph-1.1.4/ph/__init__.py
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)       22 2023-05-02 19:25:02.000000 ph-1.1.4/ph/_version.py
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)    97434 2022-11-03 12:53:43.000000 ph-1.1.4/ph/tabulate.py
+drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2023-05-02 19:27:37.223857 ph-1.1.4/ph.egg-info/
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)    27143 2023-05-02 19:27:37.000000 ph-1.1.4/ph.egg-info/PKG-INFO
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)      246 2023-05-02 19:27:37.000000 ph-1.1.4/ph.egg-info/SOURCES.txt
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)        1 2023-05-02 19:27:37.000000 ph-1.1.4/ph.egg-info/dependency_links.txt
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)       31 2023-05-02 19:27:37.000000 ph-1.1.4/ph.egg-info/entry_points.txt
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)      299 2023-05-02 19:27:37.000000 ph-1.1.4/ph.egg-info/requires.txt
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)        3 2023-05-02 19:27:37.000000 ph-1.1.4/ph.egg-info/top_level.txt
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)       38 2023-05-02 19:27:37.223857 ph-1.1.4/setup.cfg
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)     2082 2022-06-27 20:36:16.000000 ph-1.1.4/setup.py
+drwxr-xr-x   0 pdr081   (129968) ansatt    (4601)        0 2023-05-02 19:27:37.223857 ph-1.1.4/tests/
+-rw-r--r--   0 pdr081   (129968) ansatt    (4601)    29004 2022-06-27 20:36:16.000000 ph-1.1.4/tests/test_ph.py
```

### Comparing `ph-1.1.3/LICENSE` & `ph-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ph-1.1.3/PKG-INFO` & `ph-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ph
-Version: 1.1.3
+Version: 1.1.4
 Summary: ph - the tabular data shell tool
 Home-page: https://github.com/pgdr/ph
 Author: PG Drange
 Author-email: Pal.Drange@uib.no
 Maintainer: PG Drange <Pal.Drange@uib.no>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pgdr/ph/issues
```

### Comparing `ph-1.1.3/README.md` & `ph-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ph-1.1.3/ph/__init__.py` & `ph-1.1.4/ph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,29 @@
     try:
         import gpxpy
     except ImportError:
         sys.exit("ph gpx needs gpxpy, pip install ph[gpx]")
 
     def from_trackpoint(tp=None):
         if tp is None:
-            return "time", "latitude", "longitude", "elevation", "distance"
+            return (
+                "time",
+                "latitude",
+                "longitude",
+                "elevation",
+                "distance",
+            )
         p = tp.point
-        return str(p.time), p.latitude, p.longitude, p.elevation, tp.distance_from_start
+        return (
+            str(p.time),
+            p.latitude,
+            p.longitude,
+            p.elevation,
+            tp.distance_from_start,
+        )
 
     with open(fname, "r") as fin:
         gpx = gpxpy.parse(fin)
     data = gpx.get_points_data()
     columns = from_trackpoint()
     dfdata = [from_trackpoint(tp) for tp in data]
     return pd.DataFrame(dfdata, columns=columns)
@@ -248,15 +260,17 @@
     if dset is None:
         print("type,name")
         print("\n".join("{},{}".format("real", k) for k in REALDATA))
         print("\n".join("{},{}".format("toy", k) for k in TOYDATA))
         sys.exit()
 
     if dset not in TOYDATA.keys() | REALDATA.keys():
-        sys.exit("Unknown dataset {}.  See ph help dataset.".format(dset))
+        sys.exit(
+            "Unknown dataset {}.  See ph help dataset.".format(dset)
+        )
     if dset in TOYDATA:
         data = TOYDATA[dset]()
     else:
         data = REALDATA[dset]()
     try:
         df = pd.DataFrame(data.data, columns=data.feature_names)
     except AttributeError:
@@ -265,14 +279,21 @@
         df["target"] = pd.Series(data.target)
     except Exception:
         pass
     pipeout(df)
 
 
 @register
+def drop_duplicates(*cols):
+    """Drop duplicates"""
+    df = pipein()
+    pipeout(df.drop_duplicates(cols))
+
+
+@register
 def diff(*cols, periods=1, axis=0):
     """Calculate the difference of an element compared with another element
     in the csv file (default is element in previous row).
 
     Argument: --periods=1
 
     Periods to shift for calculating difference, default 1.  Accepts
@@ -315,23 +336,31 @@
            cat a.csv | ph dropna --thresh=5  # keep cols with >= 5 non-na
            cat a.csv | ph dropna --how=all   # delete only if all vals na
 
     """
     try:
         axis = int(axis)
         if axis not in (0, 1):
-            sys.exit("ph dropna --axis=0 or --axis=1, not {}".format(axis))
+            sys.exit(
+                "ph dropna --axis=0 or --axis=1, not {}".format(axis)
+            )
     except ValueError:
-        sys.exit("ph dropna --axis=0 or --axis=1, not {}".format(axis))
+        sys.exit(
+            "ph dropna --axis=0 or --axis=1, not {}".format(axis)
+        )
 
     if thresh is not None:
         try:
             thresh = int(thresh)
         except ValueError:
-            sys.exit("ph dropna --thresh=0 or --thresh=1, not {}".format(thresh))
+            sys.exit(
+                "ph dropna --thresh=0 or --thresh=1, not {}".format(
+                    thresh
+                )
+            )
 
     df = pipein()
     try:
         df = df.dropna(axis=axis, how=how, thresh=thresh)
     except Exception as err:
         sys.exit(str(err))
     pipeout(df)
@@ -362,15 +391,19 @@
     skiprows = kwargs.get("skiprows")
     if skiprows is not None:
         try:
             skiprows = int(skiprows)
             if skiprows < 0:
                 raise ValueError("Negative")
         except ValueError:
-            sys.exit("skiprows must be a non-negative int, not {}".format(skiprows))
+            sys.exit(
+                "skiprows must be a non-negative int, not {}".format(
+                    skiprows
+                )
+            )
         kwargs["skiprows"] = skiprows
 
     if kwargs.get("sep") == "\\t":
         kwargs["sep"] = "\t"
 
     try:
         return READERS[ftype](sys.stdin, **kwargs)
@@ -403,19 +436,25 @@
            cat a.csv | ph fillna --method=pad --limit=5
 
     """
     if limit is not None:
         try:
             limit = int(limit)
         except ValueError:
-            sys.exit("--limit=x must be an integer, not {}".format(limit))
+            sys.exit(
+                "--limit=x must be an integer, not {}".format(limit)
+            )
     METHODS = ("backfill", "bfill", "pad", "ffill")
     if method is not None:
         if method not in METHODS:
-            sys.exit("method must be one of {}, not {}".format(METHODS, method))
+            sys.exit(
+                "method must be one of {}, not {}".format(
+                    METHODS, method
+                )
+            )
         pipeout(pipein().fillna(method=method, limit=limit))
     elif value is not None:
         value = __tryparse(value)
         pipeout(pipein().fillna(value=value, limit=limit))
     else:
         sys.exit("'ph fillna' needs exactly one of value and method")
 
@@ -454,38 +493,50 @@
     df = pipein()
 
     if case is True or case in TRUTHY:
         case = True
     elif case in FALSY:
         case = False
     else:
-        sys.exit("ph grep:  Unknown --case={} should be True or False".format(case))
+        sys.exit(
+            "ph grep:  Unknown --case={} should be True or False".format(
+                case
+            )
+        )
 
     if regex is True or regex in TRUTHY:
         regex = True
     elif regex in FALSY:
         regex = False
     else:
-        sys.exit("ph grep:  Unknown --regex={} should be True or False".format(regex))
+        sys.exit(
+            "ph grep:  Unknown --regex={} should be True or False".format(
+                regex
+            )
+        )
 
     if column is not None:
         _assert_col(df, column, "grep")
 
     expr = " ".join(str(e) for e in expr)  # force string input
 
     try:
         import numpy
     except ImportError:
         sys.exit("numpy needed for grep.  pip install numpy")
 
     retval = df[
         numpy.logical_or.reduce(
             [
-                df[col].astype(str).str.contains(expr, case=case, na=na, regex=regex)
-                for col in (df.columns if column is None else [column])
+                df[col]
+                .astype(str)
+                .str.contains(expr, case=case, na=na, regex=regex)
+                for col in (
+                    df.columns if column is None else [column]
+                )
             ]
         )
     ]
     pipeout(retval)
 
 
 @register
@@ -517,15 +568,17 @@
     new_name = col + "_rhs"
     suffix = ""
     name = lambda: (new_name + "_" + str(suffix)).rstrip("_")
     while name() in df.columns:
         if not suffix:
             suffix = 1
         suffix += 1
-    df[[col, name()]] = df[col].astype(str).str.split(pat=pat, n=1, expand=True)
+    df[[col, name()]] = (
+        df[col].astype(str).str.split(pat=pat, n=1, expand=True)
+    )
     pipeout(df)
 
 
 @register
 def strip(*cols, lstrip=False, rstrip=False):
     """Strip (trim) a string.
 
@@ -560,15 +613,17 @@
 
     """
     prefix = str(prefix)
     plen = len(prefix)
     df = pipein()
     _assert_col(df, col, "removeprefix")
     df[col] = df[col].apply(
-        lambda s: str(s)[plen:] if str(s).startswith(prefix) else str(s)
+        lambda s: str(s)[plen:]
+        if str(s).startswith(prefix)
+        else str(s)
     )
     pipeout(df)
 
 
 @register
 def removesuffix(col, suffix=" "):
     """Remove suffix of contents of a column.
@@ -579,15 +634,17 @@
 
     """
     suffix = str(suffix)
     plen = len(suffix)
     df = pipein()
     _assert_col(df, col, "removesuffix")
     df[col] = df[col].apply(
-        lambda s: str(s)[:-plen] if str(s).endswith(suffix) else str(s)
+        lambda s: str(s)[:-plen]
+        if str(s).endswith(suffix)
+        else str(s)
     )
     pipeout(df)
 
 
 @register
 def astype(type, column=None, newcolumn=None):
     """Cast a column to a different type.
@@ -620,44 +677,48 @@
 
     Usage:  cat a.csv | ph dtypes
             cat a.csv | ph dtypes float64
 
     """
     if t is None:
         df = pipein()
-        newdf = pd.DataFrame(pd.Series(df.columns), columns=["column"])
+        newdf = pd.DataFrame(
+            pd.Series(df.columns), columns=["column"]
+        )
         newdf["dtype"] = pd.Series([str(e) for e in df.dtypes])
         pipeout(newdf.T, header=False)
     else:
         df = pipein().select_dtypes(t)
         pipeout(df)
 
 
 @register
 def pivot(columns, index=None, values=None):
     """Reshape csv organized by given index / column values.
 
-    Suppose b.csv is
-foo,bar,baz,zoo
-one,A,1,x
-one,B,2,y
-one,C,3,z
-two,A,4,q
-two,B,5,w
-two,C,6,t
-
-    Usage: cat b.csv | ph pivot bar --index=foo --values=baz
-
-      A    B    C
---  ---  ---  ---
- 0    1    2    3
- 1    4    5    6
+        Suppose b.csv is
+    foo,bar,baz,zoo
+    one,A,1,x
+    one,B,2,y
+    one,C,3,z
+    two,A,4,q
+    two,B,5,w
+    two,C,6,t
+
+        Usage: cat b.csv | ph pivot bar --index=foo --values=baz
+
+          A    B    C
+    --  ---  ---  ---
+     0    1    2    3
+     1    4    5    6
 
     """
-    pipeout(pipein().pivot(index=index, columns=columns, values=values))
+    pipeout(
+        pipein().pivot(index=index, columns=columns, values=values)
+    )
 
 
 @register
 def crosstab(column):
     """Perform a very simplistic crosstabulation on one column of the input csv.
 
     Usage:  cat b.csv | ph crosstab foo
@@ -689,22 +750,32 @@
     else:
         sys.exit("--as_index=True or False, not {}".format(as_index))
 
     grouped = df.groupby(columns, as_index=as_index)
     try:
         fn = getattr(grouped, how)
     except AttributeError:
-        sys.exit("Unknown --how={}, should be sum, mean, ...".format(how))
+        sys.exit(
+            "Unknown --how={}, should be sum, mean, ...".format(how)
+        )
     retval = fn()
 
     pipeout(retval)
 
 
 @register
-def rolling(window, *columns, how="sum", win_type=None, std=None, beta=None, tau=None):
+def rolling(
+    window,
+    *columns,
+    how="sum",
+    win_type=None,
+    std=None,
+    beta=None,
+    tau=None
+):
     """Rolling window calculations using provided `how` function.
 
     Usage: cat a.csv | ph rolling 3
            cat a.csv | ph rolling 5 --how=mean
            cat a.csv | ph rolling 5 colA colB --how=mean
            cat a.csv | ph rolling 5 --win_type=gaussian --std=7.62
     """
@@ -719,27 +790,31 @@
     noncols = [c for c in df.columns if c not in columns]
 
     rollin = df[columns].rolling(window, win_type=win_type)
     nonrollin = df[noncols]
     try:
         fn = getattr(rollin, how)
     except AttributeError:
-        sys.exit("Unknown --how={}, should be sum, mean, ...".format(how))
+        sys.exit(
+            "Unknown --how={}, should be sum, mean, ...".format(how)
+        )
 
     if {std, beta, tau} != {None}:
         retval = fn(std=std, beta=beta, tau=tau)
     else:
         retval = fn()
 
     df = pd.concat([retval, nonrollin], axis=1)
     for col in orig_columns:
         if col not in df.columns:
             op = "ph rolling"
             sys.exit(
-                '{}: Could not perform rolling window on column "{}"'.format(op, col)
+                '{}: Could not perform rolling window on column "{}"'.format(
+                    op, col
+                )
             )
     df = df[orig_columns]
     pipeout(df)
 
 
 @register
 def ewm(
@@ -785,15 +860,19 @@
         span=span,
         halflife=halflife,
         alpha=alpha,
     )
     try:
         fn = getattr(ewm_, how)
     except AttributeError:
-        sys.exit("Unknown --how={}, should be mean, var, std, corr, cov..".format(how))
+        sys.exit(
+            "Unknown --how={}, should be mean, var, std, corr, cov..".format(
+                how
+            )
+        )
 
     retval = fn()
 
     pipeout(retval)
 
 
 @register
@@ -817,23 +896,31 @@
 
     """
 
     df = pipein()
 
     if quantile is not None:
         if how != "quantile":
-            sys.exit("Use both or none of --how=quantile and --quantile=<float>")
+            sys.exit(
+                "Use both or none of --how=quantile and --quantile=<float>"
+            )
     if how == "quantile" and quantile is None:
 
-        sys.exit("--how=quantile needs --quantile=<float>, e.g. --quantile=0.25")
+        sys.exit(
+            "--how=quantile needs --quantile=<float>, e.g. --quantile=0.25"
+        )
     expanding_ = df.expanding(min_periods=min_periods, axis=axis)
     try:
         fn = getattr(expanding_, how)
     except AttributeError:
-        sys.exit("Unknown --how={}, should be sum, mean, max, quantile..".format(how))
+        sys.exit(
+            "Unknown --how={}, should be sum, mean, max, quantile..".format(
+                how
+            )
+        )
 
     if how == "quantile":
         retval = fn(quantile)
     else:
         retval = fn()
 
     pipeout(retval)
@@ -962,20 +1049,29 @@
     Warning:  This is probably not what you want.
 
     """
     df = pipein()
     if col is None:
         df = (df - df.min()) / (df.max() - df.min())
     else:
-        df[col] = (df[col] - df[col].min()) / (df[col].max() - df[col].min())
+        df[col] = (df[col] - df[col].min()) / (
+            df[col].max() - df[col].min()
+        )
     pipeout(df)
 
 
 @register
-def date(col=None, unit=None, origin="unix", errors="raise", dayfirst=False, **kwargs):
+def date(
+    col=None,
+    unit=None,
+    origin="unix",
+    errors="raise",
+    dayfirst=False,
+    **kwargs
+):
     """Assemble datetime from multiple columns or from one column
 
     --unit can be D, s, us, ns (defaults to ns, ns from origin)
 
     --origin can be unix, julian, or time offset, e.g. '2000-01-01'
 
     --errors can be raise, coerce, ignore (see pandas.to_datetime)
@@ -990,34 +1086,47 @@
            cat a.csv | ph date  # if a.csv contains year, month, date
            cat a.csv | ph date x --format="%Y-%m-%d"
            cat a.csv | ph date x --utc=True
 
     """
     DATE_ERRORS = ("ignore", "raise", "coerce")
     if errors not in DATE_ERRORS:
-        sys.exit("Errors must be one of {}, not {}.".format(DATE_ERRORS, errors))
+        sys.exit(
+            "Errors must be one of {}, not {}.".format(
+                DATE_ERRORS, errors
+            )
+        )
 
     dayfirst = dayfirst in TRUTHY
 
     date_parser = None
     if "format" in kwargs:
         date_parser = lambda d: [
-            datetime.datetime.strptime(str(e), kwargs["format"]) for e in d
+            datetime.datetime.strptime(str(e), kwargs["format"])
+            for e in d
         ]
     if kwargs.get("utc") in TRUTHY:
-        date_parser = lambda d: [datetime.datetime.utcfromtimestamp(e) for e in d]
+        date_parser = lambda d: [
+            datetime.datetime.utcfromtimestamp(e) for e in d
+        ]
     df = pipein()
     try:
         if col is None:
-            df = pd.to_datetime(df, unit=unit, origin=origin, errors=errors)
+            df = pd.to_datetime(
+                df, unit=unit, origin=origin, errors=errors
+            )
         else:
             _assert_col(df, col, "date")
             if date_parser is None:
                 df[col] = pd.to_datetime(
-                    df[col], unit=unit, origin=origin, errors=errors, dayfirst=dayfirst
+                    df[col],
+                    unit=unit,
+                    origin=origin,
+                    errors=errors,
+                    dayfirst=dayfirst,
                 )
             else:
                 df[col] = date_parser(df[col])
     except Exception as err:
         sys.exit(err)
 
     pipeout(df)
@@ -1079,15 +1188,17 @@
     if index not in TRUTHY + FALSY:
         sys.exit("Index must be True or False, not {}".format(index))
     index = index in TRUTHY
 
     if ftype == "fwf":
         # pandas has not yet implemented to_fwf
         df = pipein()
-        content = tabulate_(df.values.tolist(), list(df.columns), tablefmt="plain")
+        content = tabulate_(
+            df.values.tolist(), list(df.columns), tablefmt="plain"
+        )
         if fname:
             with open(fname, "w") as wout:
                 wout.write(content)
         else:
             print(content)
         sys.exit()
 
@@ -1136,15 +1247,19 @@
     skiprows = kwargs.get("skiprows")
     if skiprows is not None:
         try:
             skiprows = int(skiprows)
             if skiprows < 0:
                 raise ValueError("Negative")
         except ValueError:
-            sys.exit("skiprows must be a non-negative int, not {}".format(skiprows))
+            sys.exit(
+                "skiprows must be a non-negative int, not {}".format(
+                    skiprows
+                )
+            )
         kwargs["skiprows"] = skiprows
 
     if kwargs.get("sep") == "\\t":
         kwargs["sep"] = "\t"
 
     if ftype == "clipboard":
         pipeout(READERS["clipboard"](**kwargs))
@@ -1174,15 +1289,17 @@
             df = pd.read_csv(fname)
             dfs.append(df)
         retval = pd.concat(dfs, axis=axis)
         pipeout(retval)
 
 
 @register
-def merge(fname1, fname2, how="inner", on=None, left=None, right=None):
+def merge(
+    fname1, fname2, how="inner", on=None, left=None, right=None
+):
     """Merging two csv files.
 
     If the two files have a common column name, then the merge will be
     on that column.  If the files have several common column names, use
     --on=key for merging on a specific column.
 
     If you want to merge on columns with different names, use
@@ -1194,33 +1311,49 @@
     Usage: ph merge a.csv b.csv --on=ijk
            ph merge a.csv b.csv --on ijk --how=inner
            ph merge a.csv b.csv --left=key_a --right=key_b
 
     """
     hows = ("left", "right", "outer", "inner")
     if how not in hows:
-        sys.exit("Unknown merge --how={}, must be one of {}".format(how, hows))
+        sys.exit(
+            "Unknown merge --how={}, must be one of {}".format(
+                how, hows
+            )
+        )
     try:
         df1 = pd.read_csv(fname1)
         df2 = pd.read_csv(fname2)
     except Exception as err:
         sys.exit(str(err))
-    if set([on, left, right]) == set([None]) and not set(df1.columns).intersection(set(df2.columns)):
-        sys.exit("No common columns to perform merge on.  Merge options: on, or: left=None, right=None.")
+    if set([on, left, right]) == set([None]) and not set(
+        df1.columns
+    ).intersection(set(df2.columns)):
+        sys.exit(
+            "No common columns to perform merge on.  Merge options: on, or: left=None, right=None."
+        )
     if set([on, left, right]) == set([None]):
         pipeout(pd.merge(df1, df2, how=how))
     else:
         if left is None and right is None:
             pipeout(pd.merge(df1, df2, how=how, on=on))
         elif left is not None and right is not None:
             _assert_col(df1, left, "merge")
             _assert_col(df2, right, "merge")
-            pipeout(pd.merge(df1, df2, how=how, left_on=left, right_on=right))
+            pipeout(
+                pd.merge(
+                    df1, df2, how=how, left_on=left, right_on=right
+                )
+            )
         else:
-            sys.exit("Specify columns in both files.  left was {}, right was {}".format(left, right))
+            sys.exit(
+                "Specify columns in both files.  left was {}, right was {}".format(
+                    left, right
+                )
+            )
 
 
 @register
 def tab():
     """Equivalent to `ph to tsv`.
 
     Usage: cat a.csv | ph tab
@@ -1253,15 +1386,17 @@
     fmt = kwargs.get("format")
     index = True
     if "--noindex" in args:
         index = False
     if "--headers" in args:
         headers = "keys"
     df = pipein()
-    out = tabulate_(df, tablefmt=fmt, headers=headers, showindex=index)
+    out = tabulate_(
+        df, tablefmt=fmt, headers=headers, showindex=index
+    )
     _safe_out(out)
 
 
 @register
 def show(noindex=False):
     """Similar to ph tabulate --headers [--noindex].
 
@@ -1415,15 +1550,19 @@
     skiprows = kwargs.get("skiprows")
     if skiprows is not None:
         try:
             skiprows = int(skiprows)
             if skiprows < 0:
                 raise ValueError("Negative")
         except ValueError:
-            sys.exit("skiprows must be a non-negative int, not {}".format(skiprows))
+            sys.exit(
+                "skiprows must be a non-negative int, not {}".format(
+                    skiprows
+                )
+            )
         kwargs["skiprows"] = skiprows
 
     try:
         if ftype == "clipboard":
             df = reader(**kwargs)
         elif ftype in ("excel", "xls", "odf"):
             try:
@@ -1438,19 +1577,23 @@
                 except Exception:
                     errormsg = "Specify --sheet_name"
                 sys.exit(errormsg)
         else:
             df = reader(fname, **kwargs)
     except AttributeError as err:
         sys.exit(
-            "{} is not supported in your Pandas installation\n{}".format(ftype, err)
+            "{} is not supported in your Pandas installation\n{}".format(
+                ftype, err
+            )
         )
     except ImportError as err:
         sys.exit(
-            "{} is not supported in your Pandas installation\n{}".format(ftype, err)
+            "{} is not supported in your Pandas installation\n{}".format(
+                ftype, err
+            )
         )
     except FileNotFoundError as err:
         sys.exit("File not found: {}".format(err))
     pipeout(df)
 
 
 _ATTRS_WITH_SERIES_OUTPUT = (
@@ -1531,14 +1674,40 @@
         pass
     except OverflowError:
         x_ = float("inf")
     return x_
 
 
 @register
+def fft(*cols):
+    """Perform fft on the datas.
+
+    Usage: ph fft [col1 col2 col3]
+
+    """
+    import numpy as np, scipy
+
+    df = pipein()
+    F = []
+
+    if not cols:
+        cols = list(df.columns)
+    for c in cols:
+        col = np.array(df[c].fillna(0))
+        N = len(col)
+        f = [x.real for x in scipy.fft.fft(col, n=len(col), norm="forward")]
+        F.append(list(f[4: N // 2]))
+
+
+    data = { k : F[idx] for idx,k in enumerate(cols) }
+
+    pipeout(pd.DataFrame(data))
+
+
+@register
 def replace(old, new, column=None, newcolumn=None):
     """Replace a value (in a column) with a new value.
 
     Usage: cat a.csv | ph replace 8 100 # replace in all columns
            cat a.csv | ph replace 8 100 --column=y
            cat a.csv | ph replace 8 100 --column=y --newcolumn=z
 
@@ -1552,15 +1721,17 @@
     if column is None:
         if newcolumn is not None:
             sys.exit("Cannot use newcolumn and not column.")
         df = df.replace(to_replace=old, value=new, inplace=False)
     elif column not in df:
         sys.exit("Column {} does not exist.".format(column))
     else:
-        df[newcolumn] = df[column].replace(to_replace=old, value=new, inplace=False)
+        df[newcolumn] = df[column].replace(
+            to_replace=old, value=new, inplace=False
+        )
     pipeout(df)
 
 
 @register
 def rename(before, after):
     """Rename a column name.
 
@@ -1620,21 +1791,40 @@
     Usage: cat a.csv | ph spencer
 
     Experimental feature for computing Spencer's 15-weight average.
     Smooths out curves by removing high frequency noise.  Will
     ultimately lose some data on each end of the timeseries.
 
     """
-    _SPENCER = (-3, -6, -5, 3, 21, 46, 67, 74, 67, 46, 21, 3, -5, -6, -3)
+    _SPENCER = (
+        -3,
+        -6,
+        -5,
+        3,
+        21,
+        46,
+        67,
+        74,
+        67,
+        46,
+        21,
+        3,
+        -5,
+        -6,
+        -3,
+    )
     _SPENCER_SUM = sum(_SPENCER)
 
     def spencer_(lst):
         for i in range(7, len(lst) - 8):
             seq = lst[i - 7 : i + 8]
-            yield sum(seq[i] * _SPENCER[i] / _SPENCER_SUM for i in range(15))
+            yield sum(
+                seq[i] * _SPENCER[i] / _SPENCER_SUM
+                for i in range(15)
+            )
 
     df = pipein()
     _assert_cols(df, cols, "spencer")
     prefix = [float("nan")] * 7
     suffix = [float("nan")] * 8
     if not cols:
         cols = list(df.columns)
@@ -1728,15 +1918,17 @@
 @register
 def shape():
     """Print the shape of the csv file, i.e. num cols and num rows.
 
     The output will have two rows and two columns, with header "rows,columns".
 
     """
-    print("rows,columns\n" + ",".join([str(x) for x in pipein().shape]))
+    print(
+        "rows,columns\n" + ",".join([str(x) for x in pipein().shape])
+    )
 
 
 @register
 def empty():
     """Print a csv file with one column containing True or False.
 
     The output depends on whether the csv input was empty.
@@ -1753,23 +1945,26 @@
 
     Adds a left-most column `index`.
     """
     pipeout(pipein().reset_index())
 
 
 @register
-def sort(col):
-    """Sort csv input by column.
+def sort(*col):
+    """Sort csv input by column(s).
+
+    This is the only way to sort on multiple columns since sort is not stable.
 
     Usage: cat iris.csv | ph sort setosa
+           cat iris.csv | ph sort setosa verginica
 
     """
     df = pipein()
-    _assert_col(df, col, "sort")
-    pipeout(df.sort_values(col))
+    _assert_cols(df, col, "sort")
+    pipeout(df.sort_values(list(col)))
 
 
 @register
 def polyfit(x, y, deg=1):
     """Perform linear/polynomial regression.
 
     Usage: cat a.csv | ph polyfix x y
@@ -1785,15 +1980,17 @@
     if not isinstance(deg, int) or deg <= 0:
         sys.exit("deg={} should be a positive int".format(deg))
     try:
         import numpy
     except ImportError:
         sys.exit("numpy needed for polyfit.  pip install numpy")
 
-    polynomial = numpy.polynomial.Polynomial.fit(df[x], df[y], deg=deg)
+    polynomial = numpy.polynomial.Polynomial.fit(
+        df[x], df[y], deg=deg
+    )
     df["polyfit_{}".format(deg)] = df[x].map(polynomial)
     pipeout(df)
 
 
 def __process(attr):
     if attr in COMMANDS:
         return False
```

### Comparing `ph-1.1.3/ph/tabulate.py` & `ph-1.1.4/ph/tabulate.py`

 * *Files identical despite different names*

### Comparing `ph-1.1.3/ph.egg-info/PKG-INFO` & `ph-1.1.4/ph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ph
-Version: 1.1.3
+Version: 1.1.4
 Summary: ph - the tabular data shell tool
 Home-page: https://github.com/pgdr/ph
 Author: PG Drange
 Author-email: Pal.Drange@uib.no
 Maintainer: PG Drange <Pal.Drange@uib.no>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pgdr/ph/issues
```

### Comparing `ph-1.1.3/setup.py` & `ph-1.1.4/setup.py`

 * *Files identical despite different names*

