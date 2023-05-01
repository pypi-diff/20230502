# Comparing `tmp/pandas_stubs-2.0.0.230412.tar.gz` & `tmp/pandas_stubs-2.0.1.230501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_stubs-2.0.0.230412.tar", max compression
+gzip compressed data, was "pandas_stubs-2.0.1.230501.tar", max compression
```

## Comparing `pandas_stubs-2.0.0.230412.tar` & `pandas_stubs-2.0.1.230501.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.0.0.230412/LICENSE
--rw-r--r--   0        0        0     3717 2023-04-05 02:20:38.238520 pandas_stubs-2.0.0.230412/pandas-stubs/__init__.pyi
--rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.0.0.230412/pandas-stubs/_config/__init__.pyi
--rw-r--r--   0        0        0     4145 2023-02-26 16:00:15.410944 pandas_stubs-2.0.0.230412/pandas-stubs/_config/config.pyi
--rw-r--r--   0        0        0      251 2022-08-08 01:00:32.265011 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/__init__.pyi
--rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/indexing.pyi
--rw-r--r--   0        0        0     8318 2023-02-23 17:31:11.760589 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/interval.pyi
--rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/json.pyi
--rw-r--r--   0        0        0      866 2023-02-27 22:18:36.850339 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/lib.pyi
--rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/missing.pyi
--rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/ops_dispatch.pyi
--rw-r--r--   0        0        0      421 2023-02-04 17:09:12.289425 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/properties.pyi
--rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/sparse.pyi
--rw-r--r--   0        0        0      573 2022-12-28 15:28:49.657656 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/__init__.pyi
--rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/base.pyi
--rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/conversion.pyi
--rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/dtypes.pyi
--rw-r--r--   0        0        0     3543 2023-02-23 17:31:11.762588 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/nattype.pyi
--rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/np_datetime.pyi
--rw-r--r--   0        0        0     8230 2023-02-23 17:31:11.763588 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/offsets.pyi
--rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/parsing.pyi
--rw-r--r--   0        0        0     6525 2023-02-23 17:31:11.764590 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/period.pyi
--rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/strptime.pyi
--rw-r--r--   0        0        0    14082 2023-04-05 02:20:38.239523 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timedeltas.pyi
--rw-r--r--   0        0        0    10731 2023-02-23 17:31:11.766587 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timestamps.pyi
--rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/tzconversion.pyi
--rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/vectorized.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/window/__init__.pyi
--rw-r--r--   0        0        0     4126 2023-02-04 17:09:12.293389 pandas_stubs-2.0.0.230412/pandas-stubs/_testing/__init__.pyi
--rw-r--r--   0        0        0    15476 2023-04-12 19:14:53.205397 pandas_stubs-2.0.0.230412/pandas-stubs/_typing.pyi
--rw-r--r--   0        0        0      124 2023-04-12 21:59:05.354817 pandas_stubs-2.0.0.230412/pandas-stubs/_version.pyi
--rw-r--r--   0        0        0       94 2022-08-08 01:00:32.471998 pandas_stubs-2.0.0.230412/pandas-stubs/api/__init__.pyi
--rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.0.0.230412/pandas-stubs/api/extensions/__init__.pyi
--rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.0.0.230412/pandas-stubs/api/indexers/__init__.pyi
--rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-2.0.0.230412/pandas-stubs/api/interchange/__init__.pyi
--rw-r--r--   0        0        0     1959 2022-12-28 15:28:49.665655 pandas_stubs-2.0.0.230412/pandas-stubs/api/types/__init__.pyi
--rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.0.0.230412/pandas-stubs/arrays/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.0.0.230412/pandas-stubs/core/__init__.pyi
--rw-r--r--   0        0        0      471 2022-08-08 01:00:32.505997 pandas_stubs-2.0.0.230412/pandas-stubs/core/accessor.pyi
--rw-r--r--   0        0        0     2295 2023-03-04 20:30:27.571571 pandas_stubs-2.0.0.230412/pandas-stubs/core/algorithms.pyi
--rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.0.0.230412/pandas-stubs/core/api.pyi
--rw-r--r--   0        0        0     1846 2023-02-27 22:18:36.852304 pandas_stubs-2.0.0.230412/pandas-stubs/core/arraylike.pyi
--rw-r--r--   0        0        0      726 2022-08-10 19:03:04.648579 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/__init__.pyi
--rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/arrow/dtype.pyi
--rw-r--r--   0        0        0     2168 2023-04-01 02:35:39.716027 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/base.pyi
--rw-r--r--   0        0        0      954 2023-02-27 22:18:36.854305 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/boolean.pyi
--rw-r--r--   0        0        0     7407 2023-02-27 22:18:36.855305 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/categorical.pyi
--rw-r--r--   0        0        0     2841 2023-02-27 22:18:36.855305 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimelike.pyi
--rw-r--r--   0        0        0     2216 2022-12-28 15:28:49.669665 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimes.pyi
--rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/floating.pyi
--rw-r--r--   0        0        0     1010 2023-02-27 03:32:24.827813 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/integer.pyi
--rw-r--r--   0        0        0     2428 2023-02-27 22:18:36.856321 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/interval.pyi
--rw-r--r--   0        0        0      964 2023-02-27 22:18:36.857336 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/masked.pyi
--rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/numeric.pyi
--rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/numpy_.pyi
--rw-r--r--   0        0        0     1661 2023-02-04 17:09:12.300387 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/period.pyi
--rw-r--r--   0        0        0      210 2022-12-28 15:28:49.674654 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/__init__.pyi
--rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/accessor.pyi
--rw-r--r--   0        0        0     2309 2023-02-27 22:18:36.857336 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/array.pyi
--rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/dtype.pyi
--rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/string_.pyi
--rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/timedeltas.pyi
--rw-r--r--   0        0        0     2681 2023-04-01 02:35:39.717031 pandas_stubs-2.0.0.230412/pandas-stubs/core/base.pyi
--rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.0.0.230412/pandas-stubs/core/common.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/__init__.pyi
--rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/align.pyi
--rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/api.pyi
--rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/common.pyi
--rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/engines.pyi
--rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/eval.pyi
--rw-r--r--   0        0        0     2265 2022-08-08 01:00:32.699007 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/expr.pyi
--rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/expressions.pyi
--rw-r--r--   0        0        0     2324 2022-08-08 01:00:32.722048 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/ops.pyi
--rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/parsing.pyi
--rw-r--r--   0        0        0     3061 2022-08-08 01:00:32.745044 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/pytables.pyi
--rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/scope.pyi
--rw-r--r--   0        0        0     1621 2022-08-08 01:00:32.764271 pandas_stubs-2.0.0.230412/pandas-stubs/core/config_init.pyi
--rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.0.0.230412/pandas-stubs/core/construction.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/__init__.pyi
--rw-r--r--   0        0        0     1625 2022-12-28 15:28:49.680655 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/api.pyi
--rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/base.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/cast.pyi
--rw-r--r--   0        0        0     2377 2023-02-23 17:31:11.770587 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/common.pyi
--rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/concat.pyi
--rw-r--r--   0        0        0     1687 2023-02-27 22:18:36.858307 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/dtypes.pyi
--rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/generic.pyi
--rw-r--r--   0        0        0      610 2022-12-28 15:28:49.684666 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/inference.pyi
--rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/missing.pyi
--rw-r--r--   0        0        0    65003 2023-04-12 19:14:53.207397 pandas_stubs-2.0.0.230412/pandas-stubs/core/frame.pyi
--rw-r--r--   0        0        0    14954 2023-04-12 19:14:53.208396 pandas_stubs-2.0.0.230412/pandas-stubs/core/generic.pyi
--rw-r--r--   0        0        0      120 2022-08-08 01:00:32.927699 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/__init__.pyi
--rw-r--r--   0        0        0      261 2023-02-04 17:09:12.306444 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/base.pyi
--rw-r--r--   0        0        0      246 2022-08-10 19:03:04.661580 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/categorical.pyi
--rw-r--r--   0        0        0    12835 2023-03-04 20:30:27.574572 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/generic.pyi
--rw-r--r--   0        0        0     4139 2023-03-04 20:30:27.574572 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/groupby.pyi
--rw-r--r--   0        0        0     1647 2023-02-04 17:09:12.308388 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/grouper.pyi
--rw-r--r--   0        0        0     2721 2023-02-04 17:09:12.308388 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/ops.pyi
--rw-r--r--   0        0        0     1673 2022-08-10 19:03:04.663578 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexers.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/__init__.pyi
--rw-r--r--   0        0        0    12913 2023-04-05 02:20:38.241521 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/accessors.pyi
--rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/api.pyi
--rw-r--r--   0        0        0    10393 2023-04-12 19:14:53.209396 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/base.pyi
--rw-r--r--   0        0        0     1741 2023-02-23 17:31:11.776589 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/category.pyi
--rw-r--r--   0        0        0      812 2023-02-23 17:31:11.777589 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimelike.pyi
--rw-r--r--   0        0        0     4393 2023-04-05 02:20:38.243522 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimes.pyi
--rw-r--r--   0        0        0       80 2023-02-23 17:31:11.778625 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/extension.pyi
--rw-r--r--   0        0        0      429 2022-08-08 01:00:33.113434 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/frozen.pyi
--rw-r--r--   0        0        0    13062 2023-04-05 02:20:38.243522 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/interval.pyi
--rw-r--r--   0        0        0     5428 2023-04-01 02:35:39.720026 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/multi.pyi
--rw-r--r--   0        0        0     2933 2023-02-23 17:31:11.781588 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/period.pyi
--rw-r--r--   0        0        0     2853 2023-04-05 02:20:38.244521 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/range.pyi
--rw-r--r--   0        0        0     2713 2023-02-23 17:31:11.783587 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/timedeltas.pyi
--rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexing.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/__init__.pyi
--rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/dataframe_protocol.pyi
--rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/from_dataframe.pyi
--rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.0.0.230412/pandas-stubs/core/missing.pyi
--rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/__init__.pyi
--rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/array_ops.pyi
--rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/common.pyi
--rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/dispatch.pyi
--rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/docstrings.pyi
--rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/invalid.pyi
--rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/mask_ops.pyi
--rw-r--r--   0        0        0     6266 2023-03-04 20:30:27.575571 pandas_stubs-2.0.0.230412/pandas-stubs/core/resample.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/__init__.pyi
--rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/api.pyi
--rw-r--r--   0        0        0     2872 2023-04-12 19:14:53.210397 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/concat.pyi
--rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/encoding.pyi
--rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/melt.pyi
--rw-r--r--   0        0        0     3089 2022-12-28 15:28:49.701655 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/merge.pyi
--rw-r--r--   0        0        0     4113 2023-02-23 17:31:11.784589 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/pivot.pyi
--rw-r--r--   0        0        0     7900 2023-04-05 02:20:38.246521 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/tile.pyi
--rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/util.pyi
--rw-r--r--   0        0        0    62534 2023-04-12 19:14:53.212397 pandas_stubs-2.0.0.230412/pandas-stubs/core/series.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.0.0.230412/pandas-stubs/core/sparse/__init__.pyi
--rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.0.0.230412/pandas-stubs/core/strings.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/__init__.pyi
--rw-r--r--   0        0        0     2781 2023-02-23 17:31:11.787588 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/datetimes.pyi
--rw-r--r--   0        0        0      873 2023-02-23 17:31:11.787588 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/numeric.pyi
--rw-r--r--   0        0        0     1074 2023-02-04 17:09:12.322446 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/timedeltas.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.0.0.230412/pandas-stubs/core/util/__init__.pyi
--rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.0.0.230412/pandas-stubs/core/util/hashing.pyi
--rw-r--r--   0        0        0      274 2022-08-08 01:00:33.545825 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/__init__.pyi
--rw-r--r--   0        0        0     2484 2022-12-28 15:28:49.706655 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/ewm.pyi
--rw-r--r--   0        0        0     3838 2023-02-04 17:09:12.323425 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/expanding.pyi
--rw-r--r--   0        0        0     5796 2023-02-04 17:09:12.324423 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/rolling.pyi
--rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.0.0.230412/pandas-stubs/errors/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.0.0.230412/pandas-stubs/io/__init__.pyi
--rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.0.0.230412/pandas-stubs/io/api.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.0.0.230412/pandas-stubs/io/clipboard/__init__.pyi
--rw-r--r--   0        0        0     6938 2023-04-12 19:14:53.213395 pandas_stubs-2.0.0.230412/pandas-stubs/io/clipboards.pyi
--rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.0.0.230412/pandas-stubs/io/common.pyi
--rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/__init__.pyi
--rw-r--r--   0        0        0     7653 2023-04-12 19:14:53.214395 pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/_base.pyi
--rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/_util.pyi
--rw-r--r--   0        0        0      335 2022-08-29 12:14:24.788360 pandas_stubs-2.0.0.230412/pandas-stubs/io/feather_format.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/__init__.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/css.pyi
--rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/format.pyi
--rw-r--r--   0        0        0    11408 2023-03-04 20:30:27.577572 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style.pyi
--rw-r--r--   0        0        0     2436 2023-03-04 20:30:27.578572 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style_render.pyi
--rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.0.0.230412/pandas-stubs/io/gbq.pyi
--rw-r--r--   0        0        0     1382 2023-02-04 17:09:12.326429 pandas_stubs-2.0.0.230412/pandas-stubs/io/html.pyi
--rw-r--r--   0        0        0      170 2022-08-29 12:14:24.789359 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/__init__.pyi
--rw-r--r--   0        0        0     4110 2023-02-04 17:09:12.327388 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_json.pyi
--rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_normalize.pyi
--rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_table_schema.pyi
--rw-r--r--   0        0        0      282 2022-08-29 12:14:24.791359 pandas_stubs-2.0.0.230412/pandas-stubs/io/orc.pyi
--rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.0.0.230412/pandas-stubs/io/parquet.pyi
--rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers/__init__.pyi
--rw-r--r--   0        0        0    15581 2023-04-12 19:14:53.215395 pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers/readers.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers.pyi
--rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.0.0.230412/pandas-stubs/io/pickle.pyi
--rw-r--r--   0        0        0     6725 2023-02-23 17:31:11.791589 pandas_stubs-2.0.0.230412/pandas-stubs/io/pytables.pyi
--rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/__init__.pyi
--rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sas7bdat.pyi
--rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sas_xport.pyi
--rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sasreader.pyi
--rw-r--r--   0        0        0      250 2022-08-29 12:14:24.795362 pandas_stubs-2.0.0.230412/pandas-stubs/io/spss.pyi
--rw-r--r--   0        0        0     4871 2023-02-23 17:31:11.794588 pandas_stubs-2.0.0.230412/pandas-stubs/io/sql.pyi
--rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.0.0.230412/pandas-stubs/io/stata.pyi
--rw-r--r--   0        0        0     1015 2023-02-04 17:09:12.330386 pandas_stubs-2.0.0.230412/pandas-stubs/io/xml.pyi
--rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.0.0.230412/pandas-stubs/plotting/__init__.pyi
--rw-r--r--   0        0        0    12852 2023-02-23 17:31:11.796591 pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_core.pyi
--rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_misc.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.0.0.230412/pandas-stubs/py.typed
--rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.0.0.230412/pandas-stubs/testing.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.614504 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/__init__.pyi
--rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/api.pyi
--rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/frequencies.pyi
--rw-r--r--   0        0        0      118 2022-08-29 12:14:32.889752 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/holiday.pyi
--rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/offsets.pyi
--rw-r--r--   0        0        0      255 2022-12-28 15:28:49.723655 pandas_stubs-2.0.0.230412/pandas-stubs/util/__init__.pyi
--rw-r--r--   0        0        0     1230 2023-02-04 17:09:12.332423 pandas_stubs-2.0.0.230412/pandas-stubs/util/_decorators.pyi
--rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.0.0.230412/pandas-stubs/util/_doctools.pyi
--rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.0.0.230412/pandas-stubs/util/_exceptions.pyi
--rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.0.0.230412/pandas-stubs/util/_print_versions.pyi
--rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.0.0.230412/pandas-stubs/util/_tester.pyi
--rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.0.0.230412/pandas-stubs/util/_validators.pyi
--rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.0.0.230412/pandas-stubs/util/version/__init__.pyi
--rw-r--r--   0        0        0     6935 2023-04-12 21:58:43.256511 pandas_stubs-2.0.0.230412/pyproject.toml
--rw-r--r--   0        0        0     8415 2023-04-12 21:57:46.990004 pandas_stubs-2.0.0.230412/README.md
--rw-r--r--   0        0        0    10415 1970-01-01 00:00:00.000000 pandas_stubs-2.0.0.230412/setup.py
--rw-r--r--   0        0        0     9685 1970-01-01 00:00:00.000000 pandas_stubs-2.0.0.230412/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.0.1.230501/LICENSE
+-rw-r--r--   0        0        0     3717 2023-04-05 02:20:38.238520 pandas_stubs-2.0.1.230501/pandas-stubs/__init__.pyi
+-rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.0.1.230501/pandas-stubs/_config/__init__.pyi
+-rw-r--r--   0        0        0     4145 2023-02-26 16:00:15.410944 pandas_stubs-2.0.1.230501/pandas-stubs/_config/config.pyi
+-rw-r--r--   0        0        0      251 2022-08-08 01:00:32.265011 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/__init__.pyi
+-rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/indexing.pyi
+-rw-r--r--   0        0        0     8318 2023-04-30 02:38:30.381115 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/interval.pyi
+-rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/json.pyi
+-rw-r--r--   0        0        0      866 2023-02-27 22:18:36.850339 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/lib.pyi
+-rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/missing.pyi
+-rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/ops_dispatch.pyi
+-rw-r--r--   0        0        0      421 2023-02-04 17:09:12.289425 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/properties.pyi
+-rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/sparse.pyi
+-rw-r--r--   0        0        0      573 2022-12-28 15:28:49.657656 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/__init__.pyi
+-rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/base.pyi
+-rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/conversion.pyi
+-rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/dtypes.pyi
+-rw-r--r--   0        0        0     3543 2023-02-23 17:31:11.762588 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/nattype.pyi
+-rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/np_datetime.pyi
+-rw-r--r--   0        0        0     8230 2023-02-23 17:31:11.763588 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/offsets.pyi
+-rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/parsing.pyi
+-rw-r--r--   0        0        0     6525 2023-02-23 17:31:11.764590 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/period.pyi
+-rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/strptime.pyi
+-rw-r--r--   0        0        0    14082 2023-04-05 02:20:38.239523 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timedeltas.pyi
+-rw-r--r--   0        0        0    10731 2023-02-23 17:31:11.766587 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timestamps.pyi
+-rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/tzconversion.pyi
+-rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/vectorized.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/window/__init__.pyi
+-rw-r--r--   0        0        0     4126 2023-02-04 17:09:12.293389 pandas_stubs-2.0.1.230501/pandas-stubs/_testing/__init__.pyi
+-rw-r--r--   0        0        0    15505 2023-04-25 19:40:11.552225 pandas_stubs-2.0.1.230501/pandas-stubs/_typing.pyi
+-rw-r--r--   0        0        0      124 2023-05-01 21:56:21.743993 pandas_stubs-2.0.1.230501/pandas-stubs/_version.pyi
+-rw-r--r--   0        0        0       94 2022-08-08 01:00:32.471998 pandas_stubs-2.0.1.230501/pandas-stubs/api/__init__.pyi
+-rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.0.1.230501/pandas-stubs/api/extensions/__init__.pyi
+-rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.0.1.230501/pandas-stubs/api/indexers/__init__.pyi
+-rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-2.0.1.230501/pandas-stubs/api/interchange/__init__.pyi
+-rw-r--r--   0        0        0     1959 2022-12-28 15:28:49.665655 pandas_stubs-2.0.1.230501/pandas-stubs/api/types/__init__.pyi
+-rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.0.1.230501/pandas-stubs/arrays/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.0.1.230501/pandas-stubs/core/__init__.pyi
+-rw-r--r--   0        0        0      471 2022-08-08 01:00:32.505997 pandas_stubs-2.0.1.230501/pandas-stubs/core/accessor.pyi
+-rw-r--r--   0        0        0     2309 2023-05-01 21:55:22.558166 pandas_stubs-2.0.1.230501/pandas-stubs/core/algorithms.pyi
+-rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.0.1.230501/pandas-stubs/core/api.pyi
+-rw-r--r--   0        0        0     1846 2023-02-27 22:18:36.852304 pandas_stubs-2.0.1.230501/pandas-stubs/core/arraylike.pyi
+-rw-r--r--   0        0        0      726 2022-08-10 19:03:04.648579 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/__init__.pyi
+-rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/arrow/dtype.pyi
+-rw-r--r--   0        0        0     2168 2023-04-01 02:35:39.716027 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/base.pyi
+-rw-r--r--   0        0        0      954 2023-02-27 22:18:36.854305 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/boolean.pyi
+-rw-r--r--   0        0        0     7407 2023-02-27 22:18:36.855305 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/categorical.pyi
+-rw-r--r--   0        0        0     2841 2023-02-27 22:18:36.855305 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimelike.pyi
+-rw-r--r--   0        0        0     2216 2022-12-28 15:28:49.669665 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimes.pyi
+-rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/floating.pyi
+-rw-r--r--   0        0        0     1010 2023-02-27 03:32:24.827813 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/integer.pyi
+-rw-r--r--   0        0        0     2689 2023-05-01 21:55:22.558166 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/interval.pyi
+-rw-r--r--   0        0        0      964 2023-02-27 22:18:36.857336 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/masked.pyi
+-rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/numeric.pyi
+-rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/numpy_.pyi
+-rw-r--r--   0        0        0     1661 2023-02-04 17:09:12.300387 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/period.pyi
+-rw-r--r--   0        0        0      210 2022-12-28 15:28:49.674654 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/__init__.pyi
+-rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/accessor.pyi
+-rw-r--r--   0        0        0     2309 2023-02-27 22:18:36.857336 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/array.pyi
+-rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/dtype.pyi
+-rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/string_.pyi
+-rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/timedeltas.pyi
+-rw-r--r--   0        0        0     2681 2023-04-01 02:35:39.717031 pandas_stubs-2.0.1.230501/pandas-stubs/core/base.pyi
+-rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.0.1.230501/pandas-stubs/core/common.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/__init__.pyi
+-rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/align.pyi
+-rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/api.pyi
+-rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/common.pyi
+-rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/engines.pyi
+-rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/eval.pyi
+-rw-r--r--   0        0        0     2265 2022-08-08 01:00:32.699007 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/expr.pyi
+-rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/expressions.pyi
+-rw-r--r--   0        0        0     2324 2022-08-08 01:00:32.722048 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/ops.pyi
+-rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/parsing.pyi
+-rw-r--r--   0        0        0     3061 2022-08-08 01:00:32.745044 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/pytables.pyi
+-rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/scope.pyi
+-rw-r--r--   0        0        0     1621 2022-08-08 01:00:32.764271 pandas_stubs-2.0.1.230501/pandas-stubs/core/config_init.pyi
+-rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.0.1.230501/pandas-stubs/core/construction.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/__init__.pyi
+-rw-r--r--   0        0        0     1625 2022-12-28 15:28:49.680655 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/api.pyi
+-rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/base.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/cast.pyi
+-rw-r--r--   0        0        0     2377 2023-02-23 17:31:11.770587 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/common.pyi
+-rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/concat.pyi
+-rw-r--r--   0        0        0     1687 2023-02-27 22:18:36.858307 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/dtypes.pyi
+-rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/generic.pyi
+-rw-r--r--   0        0        0      610 2022-12-28 15:28:49.684666 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/inference.pyi
+-rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/missing.pyi
+-rw-r--r--   0        0        0    65002 2023-05-01 14:59:34.187821 pandas_stubs-2.0.1.230501/pandas-stubs/core/frame.pyi
+-rw-r--r--   0        0        0    15017 2023-04-25 19:40:11.553225 pandas_stubs-2.0.1.230501/pandas-stubs/core/generic.pyi
+-rw-r--r--   0        0        0      120 2022-08-08 01:00:32.927699 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/__init__.pyi
+-rw-r--r--   0        0        0      261 2023-02-04 17:09:12.306444 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/base.pyi
+-rw-r--r--   0        0        0      246 2022-08-10 19:03:04.661580 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/categorical.pyi
+-rw-r--r--   0        0        0    12835 2023-03-04 20:30:27.574572 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/generic.pyi
+-rw-r--r--   0        0        0     4139 2023-03-04 20:30:27.574572 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/groupby.pyi
+-rw-r--r--   0        0        0     1647 2023-02-04 17:09:12.308388 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/grouper.pyi
+-rw-r--r--   0        0        0     2721 2023-02-04 17:09:12.308388 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/ops.pyi
+-rw-r--r--   0        0        0     1673 2022-08-10 19:03:04.663578 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexers.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/__init__.pyi
+-rw-r--r--   0        0        0    12913 2023-04-05 02:20:38.241521 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/accessors.pyi
+-rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/api.pyi
+-rw-r--r--   0        0        0    10393 2023-04-12 19:14:53.209396 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/base.pyi
+-rw-r--r--   0        0        0     1741 2023-02-23 17:31:11.776589 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/category.pyi
+-rw-r--r--   0        0        0      812 2023-02-23 17:31:11.777589 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimelike.pyi
+-rw-r--r--   0        0        0     4393 2023-04-05 02:20:38.243522 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimes.pyi
+-rw-r--r--   0        0        0       80 2023-02-23 17:31:11.778625 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/extension.pyi
+-rw-r--r--   0        0        0      429 2022-08-08 01:00:33.113434 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/frozen.pyi
+-rw-r--r--   0        0        0    13292 2023-05-01 21:55:22.559166 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/interval.pyi
+-rw-r--r--   0        0        0     5428 2023-04-01 02:35:39.720026 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/multi.pyi
+-rw-r--r--   0        0        0     2933 2023-02-23 17:31:11.781588 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/period.pyi
+-rw-r--r--   0        0        0     2853 2023-04-05 02:20:38.244521 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/range.pyi
+-rw-r--r--   0        0        0     2713 2023-02-23 17:31:11.783587 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/timedeltas.pyi
+-rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexing.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/__init__.pyi
+-rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/dataframe_protocol.pyi
+-rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/from_dataframe.pyi
+-rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.0.1.230501/pandas-stubs/core/missing.pyi
+-rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/__init__.pyi
+-rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/array_ops.pyi
+-rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/common.pyi
+-rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/dispatch.pyi
+-rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/docstrings.pyi
+-rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/invalid.pyi
+-rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/mask_ops.pyi
+-rw-r--r--   0        0        0     6266 2023-03-04 20:30:27.575571 pandas_stubs-2.0.1.230501/pandas-stubs/core/resample.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/__init__.pyi
+-rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/api.pyi
+-rw-r--r--   0        0        0     2872 2023-04-12 19:14:53.210397 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/concat.pyi
+-rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/encoding.pyi
+-rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/melt.pyi
+-rw-r--r--   0        0        0     3089 2022-12-28 15:28:49.701655 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/merge.pyi
+-rw-r--r--   0        0        0     4113 2023-02-23 17:31:11.784589 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/pivot.pyi
+-rw-r--r--   0        0        0     7900 2023-04-05 02:20:38.246521 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/tile.pyi
+-rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/util.pyi
+-rw-r--r--   0        0        0    63031 2023-05-01 21:55:22.560166 pandas_stubs-2.0.1.230501/pandas-stubs/core/series.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.0.1.230501/pandas-stubs/core/sparse/__init__.pyi
+-rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.0.1.230501/pandas-stubs/core/strings.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/__init__.pyi
+-rw-r--r--   0        0        0     2781 2023-02-23 17:31:11.787588 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/datetimes.pyi
+-rw-r--r--   0        0        0     1140 2023-04-25 19:40:11.555225 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/numeric.pyi
+-rw-r--r--   0        0        0     1074 2023-02-04 17:09:12.322446 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/timedeltas.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.0.1.230501/pandas-stubs/core/util/__init__.pyi
+-rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.0.1.230501/pandas-stubs/core/util/hashing.pyi
+-rw-r--r--   0        0        0      274 2022-08-08 01:00:33.545825 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/__init__.pyi
+-rw-r--r--   0        0        0     2484 2022-12-28 15:28:49.706655 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/ewm.pyi
+-rw-r--r--   0        0        0     3838 2023-02-04 17:09:12.323425 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/expanding.pyi
+-rw-r--r--   0        0        0     5796 2023-02-04 17:09:12.324423 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/rolling.pyi
+-rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.0.1.230501/pandas-stubs/errors/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.0.1.230501/pandas-stubs/io/__init__.pyi
+-rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.0.1.230501/pandas-stubs/io/api.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.0.1.230501/pandas-stubs/io/clipboard/__init__.pyi
+-rw-r--r--   0        0        0     7153 2023-04-25 19:40:11.555225 pandas_stubs-2.0.1.230501/pandas-stubs/io/clipboards.pyi
+-rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.0.1.230501/pandas-stubs/io/common.pyi
+-rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/__init__.pyi
+-rw-r--r--   0        0        0     7816 2023-04-25 19:40:11.556233 pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/_base.pyi
+-rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/_util.pyi
+-rw-r--r--   0        0        0      446 2023-04-25 19:40:11.557224 pandas_stubs-2.0.1.230501/pandas-stubs/io/feather_format.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/css.pyi
+-rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/format.pyi
+-rw-r--r--   0        0        0    11408 2023-03-04 20:30:27.577572 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style.pyi
+-rw-r--r--   0        0        0     2436 2023-03-04 20:30:27.578572 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style_render.pyi
+-rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.0.1.230501/pandas-stubs/io/gbq.pyi
+-rw-r--r--   0        0        0     1493 2023-04-25 19:40:11.557224 pandas_stubs-2.0.1.230501/pandas-stubs/io/html.pyi
+-rw-r--r--   0        0        0      170 2022-08-29 12:14:24.789359 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/__init__.pyi
+-rw-r--r--   0        0        0     4377 2023-04-25 19:40:11.558224 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_json.pyi
+-rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_normalize.pyi
+-rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_table_schema.pyi
+-rw-r--r--   0        0        0      393 2023-04-25 19:40:11.558224 pandas_stubs-2.0.1.230501/pandas-stubs/io/orc.pyi
+-rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.0.1.230501/pandas-stubs/io/parquet.pyi
+-rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers/__init__.pyi
+-rw-r--r--   0        0        0    16138 2023-04-25 19:40:11.559237 pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers/readers.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers.pyi
+-rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.0.1.230501/pandas-stubs/io/pickle.pyi
+-rw-r--r--   0        0        0     6725 2023-02-23 17:31:11.791589 pandas_stubs-2.0.1.230501/pandas-stubs/io/pytables.pyi
+-rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/__init__.pyi
+-rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sas7bdat.pyi
+-rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sas_xport.pyi
+-rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sasreader.pyi
+-rw-r--r--   0        0        0      361 2023-04-25 19:40:11.560224 pandas_stubs-2.0.1.230501/pandas-stubs/io/spss.pyi
+-rw-r--r--   0        0        0     5312 2023-04-25 19:40:11.560224 pandas_stubs-2.0.1.230501/pandas-stubs/io/sql.pyi
+-rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.0.1.230501/pandas-stubs/io/stata.pyi
+-rw-r--r--   0        0        0     1126 2023-04-25 19:40:11.561224 pandas_stubs-2.0.1.230501/pandas-stubs/io/xml.pyi
+-rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.0.1.230501/pandas-stubs/plotting/__init__.pyi
+-rw-r--r--   0        0        0    12852 2023-02-23 17:31:11.796591 pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_core.pyi
+-rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_misc.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.0.1.230501/pandas-stubs/py.typed
+-rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.0.1.230501/pandas-stubs/testing.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.614504 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/__init__.pyi
+-rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/api.pyi
+-rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/frequencies.pyi
+-rw-r--r--   0        0        0     4142 2023-05-01 21:55:22.561166 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/holiday.pyi
+-rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/offsets.pyi
+-rw-r--r--   0        0        0      255 2022-12-28 15:28:49.723655 pandas_stubs-2.0.1.230501/pandas-stubs/util/__init__.pyi
+-rw-r--r--   0        0        0     1230 2023-02-04 17:09:12.332423 pandas_stubs-2.0.1.230501/pandas-stubs/util/_decorators.pyi
+-rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.0.1.230501/pandas-stubs/util/_doctools.pyi
+-rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.0.1.230501/pandas-stubs/util/_exceptions.pyi
+-rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.0.1.230501/pandas-stubs/util/_print_versions.pyi
+-rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.0.1.230501/pandas-stubs/util/_tester.pyi
+-rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.0.1.230501/pandas-stubs/util/_validators.pyi
+-rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.0.1.230501/pandas-stubs/util/version/__init__.pyi
+-rw-r--r--   0        0        0     6935 2023-05-01 21:55:48.619914 pandas_stubs-2.0.1.230501/pyproject.toml
+-rw-r--r--   0        0        0     8415 2023-04-12 21:57:46.990004 pandas_stubs-2.0.1.230501/README.md
+-rw-r--r--   0        0        0    10415 1970-01-01 00:00:00.000000 pandas_stubs-2.0.1.230501/setup.py
+-rw-r--r--   0        0        0     9685 1970-01-01 00:00:00.000000 pandas_stubs-2.0.1.230501/PKG-INFO
```

### Comparing `pandas_stubs-2.0.0.230412/LICENSE` & `pandas_stubs-2.0.1.230501/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_config/config.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_config/config.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/interval.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/lib.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/lib.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/missing.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/dtypes.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/nattype.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/nattype.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/offsets.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/period.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timedeltas.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timestamps.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timestamps.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/vectorized.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/vectorized.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_testing/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/_typing.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/_typing.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     us: DatetimeDictArg
     ns: DatetimeDictArg
 
 # dtypes
 NpDtype: TypeAlias = str | np.dtype[np.generic] | type[str | complex | bool | object]
 Dtype: TypeAlias = ExtensionDtype | NpDtype
 DtypeArg: TypeAlias = Dtype | dict[Any, Dtype]
+DtypeBackend: TypeAlias = Literal["pyarrow", "numpy_nullable"]
 BooleanDtypeArg: TypeAlias = (
     # Builtin bool type and its string alias
     type[bool]  # noqa: Y030
     | Literal["bool"]
     # Pandas nullable boolean type and its string alias
     | pd.BooleanDtype
     | Literal["boolean"]
@@ -282,16 +283,14 @@
     | np.datetime64
     | np.timedelta64
     | bool
     | int
     | float
     | Timestamp
     | Timedelta
-    | np.integer
-    | np.float_
 )
 Scalar: TypeAlias = IndexIterScalar | complex
 ScalarT = TypeVar("ScalarT", bound=Scalar)
 # Refine the definitions below in 3.9 to use the specialized type.
 np_ndarray_int64: TypeAlias = npt.NDArray[np.int64]
 np_ndarray_int: TypeAlias = npt.NDArray[np.signedinteger]
 np_ndarray_anyint: TypeAlias = npt.NDArray[np.integer]
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/api/extensions/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/api/extensions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/api/types/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/api/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/algorithms.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/algorithms.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def unique(values: Series) -> np.ndarray | ExtensionArray: ...
 @overload
 def unique(values: np.ndarray | list) -> np.ndarray: ...
 @overload
 def unique(values: ExtensionArray) -> ExtensionArray: ...
 @overload
 def factorize(
-    values: Sequence,
+    values: Sequence | np.recarray,
     sort: bool = ...,
     use_na_sentinel: bool = ...,
     size_hint: int | None = ...,
 ) -> tuple[np.ndarray, np.ndarray]: ...
 @overload
 def factorize(
     values: Index | Series,
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/api.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arraylike.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arraylike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/base.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/boolean.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/boolean.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/categorical.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/categorical.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimelike.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimes.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/integer.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/integer.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/interval.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/interval.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+from typing import overload
+
 import numpy as np
-from pandas import Index
+from pandas import (
+    Index,
+    Series,
+)
 from pandas.core.arrays.base import ExtensionArray as ExtensionArray
 from typing_extensions import Self
 
 from pandas._libs.interval import (
     Interval as Interval,
     IntervalMixin as IntervalMixin,
 )
 from pandas._typing import (
     Axis,
+    Scalar,
     TakeIndexer,
+    np_ndarray_bool,
 )
 
 class IntervalArray(IntervalMixin, ExtensionArray):
     ndim: int = ...
     can_hold_na: bool = ...
     def __new__(
         cls, data, closed=..., dtype=..., copy: bool = ..., verify_integrity: bool = ...
@@ -66,9 +73,14 @@
     def mid(self) -> Index: ...
     @property
     def is_non_overlapping_monotonic(self) -> bool: ...
     def __array__(self, dtype=...) -> np.ndarray: ...
     def __arrow_array__(self, type=...): ...
     def to_tuples(self, na_tuple: bool = ...): ...
     def repeat(self, repeats, axis: Axis | None = ...): ...
-    def contains(self, other): ...
+    @overload
+    def contains(self, other: Series) -> Series[bool]: ...
+    @overload
+    def contains(
+        self, other: Scalar | ExtensionArray | Index | np.ndarray
+    ) -> np_ndarray_bool: ...
     def overlaps(self, other: Interval) -> bool: ...
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/masked.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/masked.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/numpy_.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/numpy_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/period.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/accessor.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/accessor.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/array.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/array.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/string_.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/string_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/timedeltas.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/base.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/common.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/eval.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/eval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/expr.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/expr.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/ops.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/pytables.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/scope.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/scope.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/config_init.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/config_init.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/construction.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/construction.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/api.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/base.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/common.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/dtypes.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/inference.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/inference.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/missing.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/frame.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/frame.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -541,27 +541,27 @@
     ) -> None: ...
     def memory_usage(self, index: _bool = ..., deep: _bool = ...) -> Series: ...
     def transpose(self, *args, copy: _bool = ...) -> DataFrame: ...
     @property
     def T(self) -> DataFrame: ...
     def __getattr__(self, name: str) -> Series: ...
     @overload
-    def __getitem__(self, idx: Scalar | Hashable) -> Series: ...
-    @overload
-    def __getitem__(self, rows: slice) -> DataFrame: ...
-    @overload
     def __getitem__(
         self,
-        idx: Series[_bool]
+        key: Series[_bool]
         | DataFrame
         | Index
         | np_ndarray_str
         | np_ndarray_bool
         | list[_ScalarOrTupleT],
     ) -> DataFrame: ...
+    @overload
+    def __getitem__(self, key: slice) -> DataFrame: ...
+    @overload
+    def __getitem__(self, key: Scalar | Hashable) -> Series: ...
     def isetitem(
         self, loc: int | Sequence[int], value: Scalar | ArrayLike | list[Any]
     ) -> None: ...
     def __setitem__(self, key, value): ...
     @overload
     def query(self, expr: _str, *, inplace: Literal[True], **kwargs) -> None: ...
     @overload
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/generic.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/generic.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ArrayLike,
     Axis,
     AxisIndex,
     CompressionOptions,
     CSVQuoting,
     Dtype,
     DtypeArg,
+    DtypeBackend,
     FilePath,
     FileWriteMode,
     FillnaOptions,
     HashableT1,
     HashableT2,
     HDFCompLib,
     IgnoreRaise,
@@ -369,14 +370,15 @@
     def infer_objects(self) -> NDFrame: ...
     def convert_dtypes(
         self: NDFrameT,
         infer_objects: _bool = ...,
         convert_string: _bool = ...,
         convert_integer: _bool = ...,
         convert_boolean: _bool = ...,
+        dtype_backend: DtypeBackend = ...,
     ) -> NDFrameT: ...
     def fillna(
         self,
         value=...,
         *,
         method=...,
         axis=...,
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/generic.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/generic.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/groupby.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/groupby.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/grouper.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/grouper.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/ops.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexers.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexers.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/accessors.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/accessors.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/api.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/base.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/category.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/category.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimelike.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimes.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/interval.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/interval.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         closed: IntervalClosedType = ...,
         name: Hashable = ...,
         copy: bool = ...,
         dtype: IntervalDtype | None = ...,
     ) -> IntervalIndex[Interval[pd.Timedelta]]: ...
     @overload
     @classmethod
-    def from_tuples(
+    def from_tuples(  # pyright: ignore[reportOverlappingOverload]
         cls,
         data: Sequence[tuple[int, int]],
         closed: IntervalClosedType = ...,
         name: Hashable = ...,
         copy: bool = ...,
         dtype: IntervalDtype | None = ...,
     ) -> IntervalIndex[pd.Interval[int]]: ...
@@ -213,15 +213,15 @@
         closed: IntervalClosedType = ...,
         name: Hashable = ...,
         copy: bool = ...,
         dtype: IntervalDtype | None = ...,
     ) -> IntervalIndex[pd.Interval[pd.Timedelta]]: ...
     def to_tuples(self, na_tuple: bool = ...) -> pd.Index: ...
     @overload
-    def __contains__(self, key: IntervalT) -> bool: ...  # type: ignore[misc]
+    def __contains__(self, key: IntervalT) -> bool: ...  # type: ignore[misc] # pyright: ignore[reportOverlappingOverload]
     @overload
     def __contains__(self, key: object) -> Literal[False]: ...
     def astype(self, dtype: DtypeArg, copy: bool = ...) -> IntervalIndex: ...
     @property
     def inferred_type(self) -> str: ...
     def memory_usage(self, deep: bool = ...) -> int: ...
     @property
@@ -288,51 +288,51 @@
     @overload  # type: ignore[override]
     def __lt__(
         self, other: IntervalT | IntervalIndex[IntervalT]
     ) -> np_ndarray_bool: ...
     @overload
     def __lt__(self, other: pd.Series[IntervalT]) -> pd.Series[bool]: ...
     @overload  # type: ignore[override]
-    def __eq__(self, other: IntervalT | IntervalIndex[IntervalT]) -> np_ndarray_bool: ...  # type: ignore[misc]
+    def __eq__(self, other: IntervalT | IntervalIndex[IntervalT]) -> np_ndarray_bool: ...  # type: ignore[misc] # pyright: ignore[reportOverlappingOverload]
     @overload
     def __eq__(self, other: pd.Series[IntervalT]) -> pd.Series[bool]: ...  # type: ignore[misc]
     @overload
     def __eq__(self, other: object) -> Literal[False]: ...
     @overload  # type: ignore[override]
-    def __ne__(self, other: IntervalT | IntervalIndex[IntervalT]) -> np_ndarray_bool: ...  # type: ignore[misc]
+    def __ne__(self, other: IntervalT | IntervalIndex[IntervalT]) -> np_ndarray_bool: ...  # type: ignore[misc] # pyright: ignore[reportOverlappingOverload]
     @overload
     def __ne__(self, other: pd.Series[IntervalT]) -> pd.Series[bool]: ...  # type: ignore[misc]
     @overload
     def __ne__(self, other: object) -> Literal[True]: ...
 
 # misc here because int and float overlap but interval has distinct types
 # int gets hit first and so the correct type is returned
 @overload
-def interval_range(  # type: ignore[misc]
+def interval_range(  # type: ignore[misc] # pyright: ignore[reportOverlappingOverload]
     start: int = ...,
     end: int = ...,
     periods: int | None = ...,
     freq: int | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[int]]: ...
 
 # Overlaps since int is a subclass of float
 @overload
-def interval_range(  # pyright: reportOverlappingOverload=false
+def interval_range(  # pyright: ignore[reportOverlappingOverload]
     start: int,
     *,
     end: None = ...,
     periods: int | None = ...,
     freq: int | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[int]]: ...
 @overload
-def interval_range(  # pyright: reportOverlappingOverload=false
+def interval_range(  # pyright: ignore[reportOverlappingOverload]
     *,
     start: None = ...,
     end: int,
     periods: int | None = ...,
     freq: int | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/multi.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/multi.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/period.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/range.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/range.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/timedeltas.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexing.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/dataframe_protocol.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/dataframe_protocol.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/array_ops.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/array_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/mask_ops.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/mask_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/resample.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/resample.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/api.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/concat.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/concat.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/encoding.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/encoding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/melt.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/melt.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/merge.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/merge.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/pivot.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/pivot.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/tile.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/tile.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/series.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/series.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from pandas import (
     Period,
     Timedelta,
     Timestamp,
 )
 from pandas.core.arrays.base import ExtensionArray
 from pandas.core.arrays.categorical import CategoricalAccessor
+from pandas.core.arrays.interval import IntervalArray
 from pandas.core.groupby.generic import (
     _SeriesGroupByNonScalar,
     _SeriesGroupByScalar,
 )
 from pandas.core.indexers import BaseIndexer
 from pandas.core.indexes.accessors import (
     CombinedDatetimelikeProperties,
@@ -72,15 +73,18 @@
 )
 from typing_extensions import (
     Never,
     TypeAlias,
 )
 import xarray as xr
 
-from pandas._libs.interval import Interval
+from pandas._libs.interval import (
+    Interval,
+    _OrderableT,
+)
 from pandas._libs.missing import NAType
 from pandas._libs.tslibs import BaseOffset
 from pandas._typing import (
     S1,
     AggFuncTypeBase,
     AggFuncTypeDictFrame,
     AggFuncTypeSeriesToFrame,
@@ -92,14 +96,15 @@
     AxisIndex,
     BooleanDtypeArg,
     BytesDtypeArg,
     CalculationMethod,
     CategoryDtypeArg,
     ComplexDtypeArg,
     CompressionOptions,
+    DtypeBackend,
     DtypeObj,
     FilePath,
     FillnaOptions,
     FloatDtypeArg,
     GroupByObjectNonScalar,
     HashableT1,
     HashableT2,
@@ -240,51 +245,57 @@
         name: Hashable | None = ...,
         copy: bool = ...,
         fastpath: bool = ...,
     ) -> TimedeltaSeries: ...
     @overload
     def __new__(
         cls,
-        data: IntervalIndex[Interval[int]],
+        data: IntervalIndex[Interval[int]] | Interval[int] | Sequence[Interval[int]],
         index: Axes | None = ...,
         dtype=...,
         name: Hashable | None = ...,
         copy: bool = ...,
         fastpath: bool = ...,
-    ) -> Series[Interval[int]]: ...
+    ) -> IntervalSeries[int]: ...
     @overload
     def __new__(
         cls,
-        data: IntervalIndex[Interval[float]],
+        data: IntervalIndex[Interval[float]]
+        | Interval[float]
+        | Sequence[Interval[float]],
         index: Axes | None = ...,
         dtype=...,
         name: Hashable | None = ...,
         copy: bool = ...,
         fastpath: bool = ...,
-    ) -> Series[Interval[float]]: ...
+    ) -> IntervalSeries[float]: ...
     @overload
     def __new__(
         cls,
-        data: IntervalIndex[Interval[Timestamp]],
+        data: IntervalIndex[Interval[Timestamp]]
+        | Interval[Timestamp]
+        | Sequence[Interval[Timestamp]],
         index: Axes | None = ...,
         dtype=...,
         name: Hashable | None = ...,
         copy: bool = ...,
         fastpath: bool = ...,
-    ) -> Series[Interval[Timestamp]]: ...
+    ) -> IntervalSeries[Timestamp]: ...
     @overload
     def __new__(
         cls,
-        data: IntervalIndex[Interval[Timedelta]],
+        data: IntervalIndex[Interval[Timedelta]]
+        | Interval[Timedelta]
+        | Sequence[Interval[Timedelta]],
         index: Axes | None = ...,
         dtype=...,
         name: Hashable | None = ...,
         copy: bool = ...,
         fastpath: bool = ...,
-    ) -> Series[Interval[Timedelta]]: ...
+    ) -> IntervalSeries[Timedelta]: ...
     @overload
     def __new__(
         cls,
         data: object | _ListLike | Series[S1] | dict[int, S1] | dict[_str, S1] | None,
         dtype: type[S1],
         index: Axes | None = ...,
         name: Hashable | None = ...,
@@ -1129,14 +1140,15 @@
     def infer_objects(self) -> Series[S1]: ...
     def convert_dtypes(
         self,
         infer_objects: _bool = ...,
         convert_string: _bool = ...,
         convert_integer: _bool = ...,
         convert_boolean: _bool = ...,
+        dtype_backend: DtypeBackend = ...,
     ) -> Series[S1]: ...
     @overload
     def ffill(
         self,
         *,
         axis: AxisIndex | None = ...,
         inplace: Literal[True],
@@ -1605,15 +1617,15 @@
     def mean(
         self,
         axis: AxisIndex | None = ...,
         skipna: _bool = ...,
         level: None = ...,
         numeric_only: _bool = ...,
         **kwargs,
-    ) -> np.float64: ...
+    ) -> float: ...
     def median(
         self,
         axis: AxisIndex | None = ...,
         skipna: _bool = ...,
         level: None = ...,
         numeric_only: _bool = ...,
         **kwargs,
@@ -1991,7 +2003,11 @@
     def __sub__(self, other: PeriodSeries) -> OffsetSeries: ...  # type: ignore[override]
 
 class OffsetSeries(Series):
     @overload  # type: ignore[override]
     def __radd__(self, other: Period) -> PeriodSeries: ...
     @overload
     def __radd__(self, other: BaseOffset) -> OffsetSeries: ...
+
+class IntervalSeries(Series, Generic[_OrderableT]):
+    @property
+    def array(self) -> IntervalArray: ...
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/strings.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/strings.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/datetimes.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/numeric.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/numeric.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -3,39 +3,45 @@
     overload,
 )
 
 import numpy as np
 import pandas as pd
 from typing_extensions import TypeAlias
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
+    DtypeBackend,
     IgnoreRaiseCoerce,
     Scalar,
     npt,
 )
 
 _Downcast: TypeAlias = Literal["integer", "signed", "unsigned", "float"] | None
 
 @overload
 def to_numeric(
     arg: Scalar,
     errors: Literal["raise", "coerce"] = ...,
     downcast: _Downcast = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> float: ...
 @overload
 def to_numeric(
     arg: Scalar,
     errors: Literal["ignore"],
     downcast: _Downcast = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> Scalar: ...
 @overload
 def to_numeric(
     arg: list | tuple | np.ndarray,
     errors: IgnoreRaiseCoerce = ...,
     downcast: _Downcast = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> npt.NDArray: ...
 @overload
 def to_numeric(
     arg: pd.Series,
     errors: IgnoreRaiseCoerce = ...,
     downcast: _Downcast = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> pd.Series: ...
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/timedeltas.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/window/ewm.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/window/ewm.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/window/expanding.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/window/expanding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/core/window/rolling.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/core/window/rolling.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/errors/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/errors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/api.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/clipboards.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/clipboards.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,33 @@
     Any,
     Literal,
     overload,
 )
 
 from pandas.core.frame import DataFrame
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
     CompressionOptions,
     CSVEngine,
     CSVQuoting,
     DtypeArg,
+    DtypeBackend,
     ListLikeHashable,
     StorageOptions,
     UsecolsArgType,
 )
 
 from pandas.io.parsers import TextFileReader
 
 @overload
 def read_clipboard(
     sep: str | None = ...,
     *,
+    dtype_backend: DtypeBackend | NoDefault = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
     names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
     usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
@@ -81,14 +84,15 @@
     float_precision: Literal["high", "legacy", "round_trip"] | None = ...,
     storage_options: StorageOptions | None = ...,
 ) -> TextFileReader: ...
 @overload
 def read_clipboard(
     sep: str | None = ...,
     *,
+    dtype_backend: DtypeBackend | NoDefault = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
     names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
     usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
@@ -138,14 +142,15 @@
     float_precision: Literal["high", "legacy", "round_trip"] | None = ...,
     storage_options: StorageOptions | None = ...,
 ) -> TextFileReader: ...
 @overload
 def read_clipboard(
     sep: str | None = ...,
     *,
+    dtype_backend: DtypeBackend | NoDefault = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
     names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
     usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/_base.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/_base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 from odf.opendocument import OpenDocument
 from openpyxl.workbook.workbook import Workbook
 from pandas.core.frame import DataFrame
 import pyxlsb.workbook
 from typing_extensions import Self
 from xlrd.book import Book
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
     Dtype,
+    DtypeBackend,
     FilePath,
     ListLikeHashable,
     ReadBuffer,
     StorageOptions,
     UsecolsArgType,
     WriteExcelBuffer,
 )
@@ -62,14 +64,15 @@
     | dict[str, Sequence[int] | list[str]] = ...,
     date_parser: Callable | None = ...,
     thousands: str | None = ...,
     decimal: str = ...,
     comment: str | None = ...,
     skipfooter: int = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> dict[int | str, DataFrame]: ...
 @overload
 def read_excel(
     io: FilePath
     | ReadBuffer[bytes]
     | bytes
     | ExcelFile
@@ -100,14 +103,15 @@
     | dict[str, Sequence[int] | list[str]] = ...,
     date_parser: Callable | None = ...,
     thousands: str | None = ...,
     decimal: str = ...,
     comment: str | None = ...,
     skipfooter: int = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 
 class ExcelWriter:
     def __init__(
         self,
         path: FilePath | WriteExcelBuffer | ExcelWriter,
         engine: Literal["auto", "openpyxl", "odf", "xlsxwriter"] | None = ...,
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style_render.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style_render.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/gbq.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/gbq.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/html.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/html.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from typing import (
     Any,
     Literal,
 )
 
 from pandas.core.frame import DataFrame
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
+    DtypeBackend,
     FilePath,
     HashableT1,
     HashableT2,
     HashableT3,
     HashableT4,
     HashableT5,
     ReadBuffer,
@@ -45,8 +47,9 @@
     | list[str]
     | dict[HashableT5, str]
     | dict[HashableT5, list[str]]
     | None = ...,
     keep_default_na: bool = ...,
     displayed_only: bool = ...,
     extract_links: Literal["header", "footer", "body", "all"] | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> list[DataFrame]: ...
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_json.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_json.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,19 @@
     Literal,
     overload,
 )
 
 from pandas.core.frame import DataFrame
 from pandas.core.series import Series
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
     CompressionOptions,
     DtypeArg,
+    DtypeBackend,
     FilePath,
     HashableT,
     JsonFrameOrient,
     JsonSeriesOrient,
     NDFrameT,
     ReadBuffer,
     StorageOptions,
@@ -39,14 +41,15 @@
     ]
     | None = ...,
     lines: Literal[True],
     chunksize: int,
     compression: CompressionOptions = ...,
     nrows: int | None = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> JsonReader[Series]: ...
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonFrameOrient | None = ...,
     typ: Literal["frame"] = ...,
@@ -62,14 +65,15 @@
     ]
     | None = ...,
     lines: Literal[True],
     chunksize: int,
     compression: CompressionOptions = ...,
     nrows: int | None = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> JsonReader[DataFrame]: ...
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonSeriesOrient | None = ...,
     typ: Literal["series"],
@@ -85,14 +89,15 @@
     ]
     | None = ...,
     lines: bool = ...,
     chunksize: None = ...,
     compression: CompressionOptions = ...,
     nrows: int | None = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> Series: ...
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonFrameOrient | None = ...,
     typ: Literal["frame"] = ...,
@@ -108,14 +113,15 @@
     ]
     | None = ...,
     lines: bool = ...,
     chunksize: None = ...,
     compression: CompressionOptions = ...,
     nrows: int | None = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 
 class JsonReader(abc.Iterator, Generic[NDFrameT]):
     def read(self) -> NDFrameT: ...
     def close(self) -> None: ...
     def __iter__(self) -> JsonReader[NDFrameT]: ...
     def __next__(self) -> NDFrameT: ...
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers/readers.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers/readers.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,21 @@
     Literal,
     overload,
 )
 
 from pandas.core.frame import DataFrame
 from typing_extensions import Self
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
     CompressionOptions,
     CSVEngine,
     CSVQuoting,
     DtypeArg,
+    DtypeBackend,
     FilePath,
     ListLikeHashable,
     ReadCsvBuffer,
     StorageOptions,
     UsecolsArgType,
 )
 
@@ -63,14 +65,15 @@
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
     date_parser: Callable = ...,
+    date_format: str | Mapping[int | str, str] | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: Literal[True],
     chunksize: int | None = ...,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -86,14 +89,15 @@
     on_bad_lines: Literal["error", "warn", "skip"]
     | Callable[[list[str]], list[str] | None] = ...,
     delim_whitespace: bool = ...,
     low_memory: bool = ...,
     memory_map: bool = ...,
     float_precision: Literal["high", "legacy", "round_trip"] | None = ...,
     storage_options: StorageOptions | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> TextFileReader: ...
 @overload
 def read_csv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
@@ -122,14 +126,15 @@
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
     date_parser: Callable = ...,
+    date_format: str | Mapping[int | str, str] | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: bool = ...,
     chunksize: int,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -145,14 +150,15 @@
     on_bad_lines: Literal["error", "warn", "skip"]
     | Callable[[list[str]], list[str] | None] = ...,
     delim_whitespace: bool = ...,
     low_memory: bool = ...,
     memory_map: bool = ...,
     float_precision: Literal["high", "legacy", "round_trip"] | None = ...,
     storage_options: StorageOptions | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> TextFileReader: ...
 @overload
 def read_csv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
@@ -181,14 +187,15 @@
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
     date_parser: Callable = ...,
+    date_format: str | Mapping[int | str, str] | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: Literal[False] = ...,
     chunksize: None = ...,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -204,14 +211,15 @@
     on_bad_lines: Literal["error", "warn", "skip"]
     | Callable[[list[str]], list[str] | None] = ...,
     delim_whitespace: bool = ...,
     low_memory: bool = ...,
     memory_map: bool = ...,
     float_precision: Literal["high", "legacy", "round_trip"] | None = ...,
     storage_options: StorageOptions | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 @overload
 def read_table(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
@@ -389,36 +397,39 @@
 @overload
 def read_fwf(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     colspecs: Sequence[tuple[int, int]] | Literal["infer"] | None = ...,
     widths: Sequence[int] | None = ...,
     infer_nrows: int = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
     iterator: Literal[True],
     chunksize: int | None = ...,
     **kwds: Any,
 ) -> TextFileReader: ...
 @overload
 def read_fwf(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     colspecs: Sequence[tuple[int, int]] | Literal["infer"] | None = ...,
     widths: Sequence[int] | None = ...,
     infer_nrows: int = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
     iterator: bool = ...,
     chunksize: int,
     **kwds: Any,
 ) -> TextFileReader: ...
 @overload
 def read_fwf(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     colspecs: Sequence[tuple[int, int]] | Literal["infer"] | None = ...,
     widths: Sequence[int] | None = ...,
     infer_nrows: int = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
     iterator: Literal[False] = ...,
     chunksize: None = ...,
     **kwds: Any,
 ) -> DataFrame: ...
 
 class TextFileReader(abc.Iterator):
     engine: CSVEngine
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/pickle.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/pickle.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/pytables.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sasreader.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sasreader.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/sql.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/sql.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 
 from pandas.core.base import PandasObject
 from pandas.core.frame import DataFrame
 import sqlalchemy.engine
 import sqlalchemy.sql.expression
 from typing_extensions import TypeAlias
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
     DtypeArg,
+    DtypeBackend,
     npt,
 )
 
 _SQLConnection: TypeAlias = str | sqlalchemy.engine.Connectable | sqlite3.Connection
 
 _SQLStatement: TypeAlias = (
     str | sqlalchemy.sql.expression.Selectable | sqlalchemy.sql.expression.TextClause
@@ -34,71 +36,79 @@
     schema: str | None = ...,
     index_col: str | list[str] | None = ...,
     coerce_float: bool = ...,
     parse_dates: list[str] | dict[str, str] | dict[str, dict[str, Any]] | None = ...,
     columns: list[str] | None = ...,
     *,
     chunksize: int,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> Generator[DataFrame, None, None]: ...
 @overload
 def read_sql_table(
     table_name: str,
     con: _SQLConnection,
     schema: str | None = ...,
     index_col: str | list[str] | None = ...,
     coerce_float: bool = ...,
     parse_dates: list[str] | dict[str, str] | dict[str, dict[str, Any]] | None = ...,
     columns: list[str] | None = ...,
     chunksize: None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 @overload
 def read_sql_query(
     sql: _SQLStatement,
     con: _SQLConnection,
     index_col: str | list[str] | None = ...,
     coerce_float: bool = ...,
     params: list[str] | tuple[str, ...] | dict[str, str] | None = ...,
     parse_dates: list[str] | dict[str, str] | dict[str, dict[str, Any]] | None = ...,
     *,
     chunksize: int,
     dtype: DtypeArg | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> Generator[DataFrame, None, None]: ...
 @overload
 def read_sql_query(
     sql: _SQLStatement,
     con: _SQLConnection,
     index_col: str | list[str] | None = ...,
     coerce_float: bool = ...,
     params: list[str] | tuple[str, ...] | dict[str, str] | None = ...,
     parse_dates: list[str] | dict[str, str] | dict[str, dict[str, Any]] | None = ...,
     chunksize: None = ...,
     dtype: DtypeArg | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 @overload
 def read_sql(
     sql: _SQLStatement,
     con: _SQLConnection,
     index_col: str | list[str] | None = ...,
     coerce_float: bool = ...,
     params: list[str] | tuple[str, ...] | dict[str, str] | None = ...,
     parse_dates: list[str] | dict[str, str] | dict[str, dict[str, Any]] | None = ...,
     columns: list[str] = ...,
     *,
     chunksize: int,
+    dtype: DtypeArg | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> Generator[DataFrame, None, None]: ...
 @overload
 def read_sql(
     sql: _SQLStatement,
     con: _SQLConnection,
     index_col: str | list[str] | None = ...,
     coerce_float: bool = ...,
     params: list[str] | tuple[str, ...] | dict[str, str] | None = ...,
     parse_dates: list[str] | dict[str, str] | dict[str, dict[str, Any]] | None = ...,
     columns: list[str] = ...,
     chunksize: None = ...,
+    dtype: DtypeArg | None = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 
 class PandasSQL(PandasObject):
     def read_sql(self, *args, **kwargs): ...
     def to_sql(
         self,
         frame: DataFrame,
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/stata.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/stata.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/io/xml.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/io/xml.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from collections.abc import Sequence
 
 from pandas.core.frame import DataFrame
 
+from pandas._libs.lib import NoDefault
 from pandas._typing import (
     CompressionOptions,
     ConvertersArg,
     DtypeArg,
+    DtypeBackend,
     FilePath,
     ParseDatesArg,
     ReadBuffer,
     StorageOptions,
     XMLParsers,
 )
 
@@ -27,8 +29,9 @@
     # encoding can not be None for lxml and StringIO input
     encoding: str | None = ...,
     parser: XMLParsers = ...,
     stylesheet: FilePath | ReadBuffer[bytes] | ReadBuffer[str] | None = ...,
     iterparse: dict[str, list[str]] | None = ...,
     compression: CompressionOptions = ...,
     storage_options: StorageOptions = ...,
+    dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
```

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/plotting/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/plotting/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_core.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_core.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_misc.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_misc.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/tseries/offsets.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/tseries/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/util/_decorators.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/util/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/util/_validators.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/util/_validators.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pandas-stubs/util/version/__init__.pyi` & `pandas_stubs-2.0.1.230501/pandas-stubs/util/version/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/pyproject.toml` & `pandas_stubs-2.0.1.230501/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-stubs"
-version = "2.0.0.230412"
+version = "2.0.1.230501"
 description = "Type annotations for pandas"
 authors = ["The Pandas Development Team <pandas-dev@python.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pandas.pydata.org"
 repository = "https://github.com/pandas-dev/pandas-stubs"
 classifiers = [
@@ -34,19 +34,19 @@
 python = ">=3.8"
 types-pytz = ">= 2022.1.1"
 
 [tool.poetry.dev-dependencies]
 mypy = "1.2.0"
 pyarrow = ">=10.0.1"
 pytest = ">=7.1.2"
-pyright = ">= 1.1.300"
+pyright = ">= 1.1.305"
 poethepoet = ">=0.16.5"
 loguru = ">=0.6.0"
-pandas = "2.0.0"
-numpy = ">=1.24.1"
+pandas = "2.0.1"
+numpy = ">=1.24.3"
 typing-extensions = ">=4.4.0"
 matplotlib = ">=3.5.1"
 pre-commit = ">=2.19.0"
 black = ">=23.3.0"
 isort = ">=5.12.0"
 openpyxl = ">=3.0.10"
 tables = { version = ">=3.7.0" , python = "<4"}  # 3.8.0 depends on blosc2 which caps python to <4
```

### Comparing `pandas_stubs-2.0.0.230412/README.md` & `pandas_stubs-2.0.1.230501/README.md`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.0.230412/setup.py` & `pandas_stubs-2.0.1.230501/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                   'util/version/*']}
 
 install_requires = \
 ['types-pytz>=2022.1.1']
 
 setup_kwargs = {
     'name': 'pandas-stubs',
-    'version': '2.0.0.230412',
+    'version': '2.0.1.230501',
     'description': 'Type annotations for pandas',
     'long_description': '# pandas-stubs: Public type stubs for pandas\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![Conda Latest Release](https://anaconda.org/conda-forge/pandas-stubs/badges/version.svg)](https://anaconda.org/conda-forge/pandas-stubs)\n[![Package Status](https://img.shields.io/pypi/status/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![License](https://img.shields.io/pypi/l/pandas-stubs.svg)](https://github.com/pandas-dev/pandas-stubs/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pandas-stubs?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pandas-stubs)\n[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydata/pandas)\n[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n\n## What is it?\n\nThese are public type stubs for [**pandas**](http://pandas.pydata.org/), following the\nconvention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of\npandas.  In general, these stubs are narrower than what is possibly allowed by pandas,\nbut follow a convention of suggesting best recommended practices for using pandas.\n\nThe stubs are likely incomplete in terms of covering the published API of pandas.  NOTE: The current 2.0.x releases of pandas-stubs do not support all of the new features of pandas 2.0.  See this [tracker](https://github.com/pandas-dev/pandas-stubs/issues/624) to understand the current compatibility with version 2.0.\n\nThe stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension\n[pylance](https://github.com/microsoft/pylance-release#readme).\n\n## Usage\n\nLet’s take this example piece of code in file `round.py`\n\n```python\nimport pandas as pd\n\ndecimals = pd.DataFrame({\'TSLA\': 2, \'AMZN\': 1})\nprices = pd.DataFrame(data={\'date\': [\'2021-08-13\', \'2021-08-07\', \'2021-08-21\'],\n                            \'TSLA\': [720.13, 716.22, 731.22], \'AMZN\': [3316.50, 3200.50, 3100.23]})\nrounded_prices = prices.round(decimals=decimals)\n```\n\nMypy won\'t see any issues with that, but after installing pandas-stubs and running it again:\n\n```sh\nmypy round.py\n```\n\nwe get the following error message:\n\n```text\nround.py:6: error: Argument "decimals" to "round" of "DataFrame" has incompatible type "DataFrame"; expected "Union[int, Dict[Any, Any], Series[Any]]"  [arg-type]\nFound 1 error in 1 file (checked 1 source file)\n```\n\nAnd, if you use pyright:\n\n```sh\npyright round.py\n```\n\nyou get the following error message:\n\n```text\n round.py:6:40 - error: Argument of type "DataFrame" cannot be assigned to parameter "decimals" of type "int | Dict[Unknown, Unknown] | Series[Unknown]" in function "round"\n  \xa0\xa0Type "DataFrame" cannot be assigned to type "int | Dict[Unknown, Unknown] | Series[Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "int"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Dict[Unknown, Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Series[Unknown]" (reportGeneralTypeIssues)\n```\n\nAnd after confirming with the [docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.round.html)\nwe can fix the code:\n\n```python\ndecimals = pd.Series({\'TSLA\': 2, \'AMZN\': 1})\n```\n\n## Version Numbering Convention\n\nThe version number x.y.z.yymmdd corresponds to a test done with pandas version x.y.z, with the stubs released on the date mm/yy/dd.\nIt is anticipated that the stubs will be released more frequently than pandas as the stubs are expected to evolve due to more\npublic visibility.\n\n## Where to get it\n\nThe source code is currently hosted on GitHub at: <https://github.com/pandas-dev/pandas-stubs>\n\nBinary installers for the latest released version are available at the [Python\nPackage Index (PyPI)](https://pypi.org/project/pandas-stubs) and on [conda-forge](https://conda-forge.org/).\n\n```sh\n# conda\nconda install pandas-stubs\n```\n\n```sh\n# or PyPI\npip install pandas-stubs\n```\n\n## Dependencies\n\n- [pandas: powerful Python data analysis toolkit](https://pandas.pydata.org/)\n- [typing-extensions >= 4.2.0 - supporting the latest typing extensions](https://github.com/python/typing_extensions#readme)\n\n## Installation from sources\n\n- Make sure you have `python >= 3.8` installed.\n- Install poetry\n\n```sh\n# conda\nconda install poetry\n```\n\n```sh\n# or PyPI\npip install poetry\n```\n\n- Install the project dependencies\n\n```sh\npoetry update -vvv\n```\n\n- Build and install the distribution\n\n```sh\npoetry run poe build_dist\npoetry run poe install_dist\n```\n\n## License\n\n[BSD 3](LICENSE)\n\n## Documentation\n\nDocumentation is a work-in-progress.  \n\n## Background\n\nThese stubs are the result of a strategic effort led by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs) with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).\n\nThese stubs were initially forked from the Microsoft project at <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).\n\nWe are indebted to Microsoft and that project for providing the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs>, which created the framework for testing the stubs.\n\n## Differences between type declarations in pandas and pandas-stubs\n\nThe <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API\'s.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.\n\nThe <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.\n\nIf issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.\n\n## Getting help\n\nAsk questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  \n\n## Discussion and Development\n\nMost development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.\n\n## Contributing to pandas-stubs\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.\n',
     'author': 'The Pandas Development Team',
     'author_email': 'pandas-dev@python.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pandas.pydata.org',
```

### Comparing `pandas_stubs-2.0.0.230412/PKG-INFO` & `pandas_stubs-2.0.1.230501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-stubs
-Version: 2.0.0.230412
+Version: 2.0.1.230501
 Summary: Type annotations for pandas
 Home-page: https://pandas.pydata.org
 License: BSD-3-Clause
 Author: The Pandas Development Team
 Author-email: pandas-dev@python.org
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
```

