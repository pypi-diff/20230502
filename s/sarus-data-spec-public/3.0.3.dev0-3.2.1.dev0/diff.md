# Comparing `tmp/sarus_data_spec_public-3.0.3.dev0.tar.gz` & `tmp/sarus_data_spec_public-3.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.0.3.dev0.tar", last modified: Tue Apr 25 07:20:53 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.2.1.dev0.tar", last modified: Tue May  2 11:55:46 2023, max compression
```

## Comparing `sarus_data_spec_public-3.0.3.dev0.tar` & `sarus_data_spec_public-3.2.1.dev0.tar`

### file list

```diff
@@ -1,183 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.485340 sarus_data_spec_public-3.0.3.dev0/
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-25 07:20:53.485340 sarus_data_spec_public-3.0.3.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.435334 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.438335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5582 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9709 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.439335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6687 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/config/routing.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3587 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.440335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18525 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.442335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.444335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4470 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.445335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    28484 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.446335 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8138 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.447336 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2172 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.448336 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.448336 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3552 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.449336 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.453336 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15727 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.454337 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28990 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    28830 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/protection_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     9271 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10449 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.459337 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13739 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11529 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10703 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    10747 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6519 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10106 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    10991 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.460337 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    12588 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.481339 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    73431 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28800 2023-04-25 07:20:42.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10599 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43542 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17816 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.482339 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31051 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   136116 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35122 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:20:53.484340 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-25 07:20:53.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6787 2023-04-25 07:20:53.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:20:53.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:20:53.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-25 07:20:53.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-25 07:20:53.000000 sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4878 2023-04-25 07:20:53.486340 sarus_data_spec_public-3.0.3.dev0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-04-25 07:20:30.000000 sarus_data_spec_public-3.0.3.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.590237 sarus_data_spec_public-3.2.1.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-02 11:55:46.590237 sarus_data_spec_public-3.2.1.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.538236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.540236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5582 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9892 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.541236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3622 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.542236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.543236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.546236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13941 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.547236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    28802 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.548236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8138 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.549236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.550236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.550236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.551236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.554236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7945 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.555236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    71070 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.560236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38861 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6429 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6041 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    18290 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6107 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.564236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.566236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.587237 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    73431 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28800 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17816 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.588237 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35527 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.590237 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7837 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-02 11:55:46.592237 sarus_data_spec_public-3.2.1.dev0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/setup.py
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.0.3.dev0'
+VERSION: Final[str] = '3.2.1.dev0'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/conversion.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pyarrow as pa
 
 from sarus_data_spec.manager.async_utils import (
     sync_iterator_from_async_iterator,
 )
 import sarus_data_spec.typing as st
 
+NO_SERIES_NAME = "__sarus_no_name__"
+
 
 async def async_cast_arrow_batches(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
     kind: st.DatasetCastable,
 ) -> st.DatasetCastable:
     """Convert an async record batches iterator to another Python type."""
     if kind not in t.get_args(st.DatasetCastable):
@@ -43,27 +45,36 @@
 
 
 async def async_arrow_batches_to_series(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
     """Returns the first columns of the DataFrame."""
     df = await async_arrow_batches_to_dataframe(batches_async_iterator)
-    return df[df.columns[0]]
+    first_col = df.columns[0]
+    series = df[first_col]
+    if first_col == NO_SERIES_NAME:
+        # This is a default value for a column.
+        # The series actually has no name.
+        series.name = None
+    return series
 
 
 def to_pyarrow_table(data: t.Any) -> pa.Table:
     """Convert the result of an external transform to a Pyarrow Table."""
     if not type(data) in t.get_args(st.DatasetCastable):
         raise TypeError(f"Cannot convert {type(data)} to Arrow batches.")
 
     if isinstance(data, pd.DataFrame):
         df = t.cast(pd.DataFrame, data)
         return pa.Table.from_pandas(df)
     elif isinstance(data, pd.Series):
         sr = t.cast(pd.Series, data)
+        if sr.name is None:
+            # We need to set a name otherwise pandas adds a default one.
+            sr.name = NO_SERIES_NAME
         return pa.Table.from_pandas(pd.DataFrame(sr))
     elif isinstance(data, t.Iterator):
         # We test this case last because DataFrames and Series are also
         # Iterators. We cannot easily test that an object is an Iterator of a
         # specific type. So we put the Iterator[pa.RecordBatch] last as the
         # last possible case.
         batches = t.cast(t.Iterator[pa.RecordBatch], data)
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,14 +307,19 @@
             {
                 struct_type.field(i).name: type_from_arrow(
                     struct_type.field(i).type, nullable=False
                 )
                 for i in range(struct_type.num_fields)
             }
         )
+    if pa.types.is_list(type):
+        list_type = t.cast(pa.ListType, type)
+        return sdt.List(
+            type=type_from_arrow(list_type.value_type, nullable=False)
+        )
     raise NotImplementedError('Type not implemented')
 
 
 def type_from_arrow(
     arrow_type: pa.DataType,
     nullable: bool,
 ) -> st.Type:
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     PICKLE = 'pickle'
     PROTO = 'protobuf'
 
 
 # Attributes Status
 SCHEMA_TASK = 'schema'
 SIZE_TASK = 'size'
+MULTIPLICITY_TASK = 'multiplicity'
 BOUNDS_TASK = 'bounds'
 MARGINALS_TASK = 'marginals'
 ARROW_TASK = 'arrow'
 PROTECTION_TASK = 'protection_task'
 USER_SETTINGS_TASK = 'user_settings_task'
 PUBLIC_TASK = 'public_task'
 CACHE_SCALAR_TASK = 'cache_scalar'
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 import sarus_data_spec.transform as sdtr
 import sarus_data_spec.typing as st
 
 if TYPE_CHECKING:
     from sarus_data_spec.bounds import Bounds
     from sarus_data_spec.links import Links
     from sarus_data_spec.marginals import Marginals
+    from sarus_data_spec.multiplicity import Multiplicity
     from sarus_data_spec.size import Size
 
 
 class Dataset(Referring[sp.Dataset]):
     """A python class to describe datasets"""
 
     def __init__(self, protobuf: sp.Dataset, store: bool = True) -> None:
@@ -156,14 +157,17 @@
 
     async def async_schema(self) -> st.Schema:
         return await self.manager().async_schema(self)
 
     def size(self) -> t.Optional[Size]:
         return cast('Size', self.manager().size(self))
 
+    def multiplicity(self) -> t.Optional[Multiplicity]:
+        return cast('Multiplicity', self.manager().multiplicity(self))
+
     def bounds(self) -> t.Optional[Bounds]:
         return cast('Bounds', self.manager().bounds(self))
 
     def marginals(self) -> t.Optional[Marginals]:
         return cast('Marginals', self.manager().marginals(self))
 
     def links(self) -> st.Links:
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 logger = logging.getLogger(__name__)
 
 
 class DataspecPrivacyPolicy(Enum):
     WHITE_LISTED = "Whitelisted"
     DP = "Differentially-private evaluation"
     SYNTHETIC = "Evaluated from synthetic data only"
+    PUBLIC = "Public"
 
 
 class PEPKind(Enum):
     NOT_PEP = 0
     PEP = 1
     TOKEN_PRESERVING = 2
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 import sarus_data_spec.storage.typing as storage_typing
 import sarus_data_spec.typing as st
 
 try:
     from sarus_data_spec.bounds import Bounds
     from sarus_data_spec.links import Links
     from sarus_data_spec.marginals import Marginals
+    from sarus_data_spec.multiplicity import Multiplicity
     from sarus_data_spec.size import Size
 
 except ModuleNotFoundError:
     pass
 try:
     import tensorflow as tf
 
@@ -376,14 +377,17 @@
 
     def schema(self, dataset: st.Dataset) -> Schema:
         return t.cast(Schema, sync(self.async_schema(dataset=dataset)))
 
     def size(self, dataset: st.Dataset) -> st.Size:
         return t.cast(Size, sync(self.async_size(dataset)))
 
+    def multiplicity(self, dataset: st.Dataset) -> st.Multiplicity:
+        return t.cast(Multiplicity, sync(self.async_multiplicity(dataset)))
+
     def sql(
         self,
         dataset: st.Dataset,
         query: t.Union[str, t.Mapping[t.Union[str, t.Tuple[str, ...]], str]],
         dialect: t.Optional[st.SQLDialect] = None,
         batch_size: int = 10000,
     ) -> t.Iterator[pa.RecordBatch]:
@@ -476,14 +480,17 @@
 
     async def async_schema(self, dataset: st.Dataset) -> st.Schema:
         return await self.schema_computation.task_result(dataspec=dataset)
 
     async def async_size(self, dataset: st.Dataset) -> st.Size:
         raise NotImplementedError
 
+    async def async_multiplicity(self, dataset: st.Dataset) -> st.Multiplicity:
+        raise NotImplementedError
+
     async def async_to_arrow(
         self, dataset: st.Dataset, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         """Reads asynchronous iterator of datast batches"""
         computation = t.cast(
             Computation[t.AsyncIterator[pa.RecordBatch]],
             self.dataspec_computation(dataset),
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         raise NotImplementedError
 
     async def size(self) -> st.Size:
         raise NotImplementedError
 
+    async def multiplicity(self) -> st.Multiplicity:
+        raise NotImplementedError
+
     async def bounds(self) -> st.Bounds:
         raise NotImplementedError
 
     async def marginals(self) -> st.Marginals:
         raise NotImplementedError
 
     async def sql(
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,94 @@
 from __future__ import annotations
 
 import hashlib
-import importlib
-import inspect
 import typing as t
 
 import pyarrow as pa
 
 from sarus_data_spec.arrow.admin_utils import (
     compute_admin_data,
     merge_data_and_admin,
 )
 from sarus_data_spec.arrow.conversion import to_pyarrow_table
 from sarus_data_spec.arrow.schema import type_from_arrow_schema
-from sarus_data_spec.config import ROUTING
+from sarus_data_spec.dataspec_validator.signature import (
+    SarusBoundSignature,
+    SarusSignature,
+)
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.base import (
     DatasetImplementation,
     DatasetStaticChecker,
     DataspecStaticChecker,
     ScalarImplementation,
 )
 from sarus_data_spec.schema import schema as schema_builder
 from sarus_data_spec.transform import external, transform_id
-import sarus_data_spec.manager.typing as smt
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
-from .signature import ExternalSignature
-from .utils import static_and_dynamic_arguments, static_arguments
+from .typing import NO_TRANSFORM_ID
+from .utils import static_arguments
 
 
 class ExternalScalarStaticChecker(DataspecStaticChecker):
     async def private_queries(self) -> t.List[st.PrivateQuery]:
         """Return the PrivateQueries summarizing DP characteristics."""
-        transform = self.dataspec.transform()
-        ds_args, ds_kwargs = self.dataspec.parents()
-
-        implementation = external_implementation(transform)
-        args, kwargs = static_and_dynamic_arguments(
-            transform, *ds_args, **ds_kwargs
+        implementation = external_implementation(self.dataspec.transform())
+        bound_signature = implementation.signature().bind_dataspec(
+            self.dataspec
         )
-        return await implementation.private_queries(*args, **kwargs)
+        return await implementation.private_queries(bound_signature)
 
     def is_dp(self) -> bool:
         """Checks if the transform is DP and compatible with the arguments."""
-        transform = self.dataspec.transform()
-        ds_args, ds_kwargs = self.dataspec.parents()
-
-        implementation = external_implementation(transform)
-        args, kwargs = static_and_dynamic_arguments(
-            transform, *ds_args, **ds_kwargs
+        implementation = external_implementation(self.dataspec.transform())
+        bound_signature = implementation.signature().bind_dataspec(
+            self.dataspec
         )
-        return implementation.is_dp(*args, **kwargs)
+        return implementation.is_dp(bound_signature)
 
     def is_dp_applicable(self, public_context: t.Collection[str]) -> bool:
         """Statically check if a DP transform is applicable in this position.
 
         This verification is common to all dataspecs and is true if:
             - the dataspec is transformed and its transform has an equivalent
             DP transform
             - the DP transform's required PEP arguments are PEP and aligned
             (i.e. same PEP token)
             - other dataspecs arguments are public
         """
         transform = self.dataspec.transform()
-        ds_args, ds_kwargs = self.dataspec.parents()
-
         implementation = external_implementation(transform)
-        args, kwargs = static_and_dynamic_arguments(
-            transform, *ds_args, **ds_kwargs
-        )
-
         dp_implementation = implementation.dp_equivalent()
-        if dp_implementation is None or not dp_implementation.is_dp(
-            *args, **kwargs
-        ):
-            return False
-
-        pep_args, non_pep_args = group_by_pep(
-            dp_implementation, *args, **kwargs
+        bound_signature = implementation.signature().bind_dataspec(
+            self.dataspec
         )
 
-        # All non PEP args should be public of published
-        if not all(
-            [
-                arg.uuid() in public_context or arg.is_public()
-                for arg in non_pep_args.values()
-            ]
+        if dp_implementation is None or not dp_implementation.is_dp(
+            bound_signature
         ):
             return False
 
-        # The PEP arg combination should be allowed
-        if set(pep_args.keys()) not in dp_implementation.allowed_pep_args:
-            return False
-
-        # All PEP tokens should be equal
-        pep_tokens = [arg.pep_token() for arg in pep_args.values()]
-        if not all([token == pep_tokens[0] for token in pep_tokens]):
-            return False
-
-        return True
+        return bound_signature.pep_token() is not None
 
     def dp_transform(self) -> t.Optional[st.Transform]:
         """Return the dataspec's DP equivalent transform if existing."""
         transform = self.dataspec.transform()
         op_implementation = external_implementation(transform)
         py_args, py_kwargs, ds_args_pos, ds_types = static_arguments(transform)
 
         dp_implementation = op_implementation.dp_equivalent()
         if dp_implementation is None:
             return None
 
-        dp_transform_id = dp_implementation.transform_id
+        dp_transform_id = dp_implementation.transform_id()
         assert dp_transform_id is not None
 
         # Types won't be used since budget & seed are scalars
         ds_types["budget"] = ""
         ds_types["seed"] = ""
 
         return external(
@@ -134,62 +104,36 @@
     ExternalScalarStaticChecker, DatasetStaticChecker
 ):
     def __init__(self, dataset: st.Dataset):
         super().__init__(dataset)
         self.dataset = dataset
 
     def pep_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
-        """Return the current dataspec's PEP token."""
+        """Return the dataspec's PEP token."""
         transform = self.dataspec.transform()
-        ds_args, ds_kwargs = self.dataspec.parents()
-
         implementation = external_implementation(transform)
-        args, kwargs = static_and_dynamic_arguments(
-            transform, *ds_args, **ds_kwargs
+        bound_signature = implementation.signature().bind_dataspec(
+            self.dataspec
         )
 
-        if len(implementation.allowed_pep_args) == 0:
+        input_token = bound_signature.pep_token()
+        if input_token is None:
             return None
 
-        pep_args, non_pep_args = group_by_pep(implementation, *args, **kwargs)
-
-        pep_kind = implementation.pep_kind(*args, **kwargs)
+        pep_kind = implementation.pep_kind(bound_signature)
         if pep_kind == PEPKind.NOT_PEP:
             return None
-
-        # All non PEP args should be public of published
-        if not all(
-            [
-                arg.uuid() in public_context or arg.is_public()
-                for arg in non_pep_args.values()
-            ]
-        ):
-            return None
-
-        # The PEP arg combination should be allowed
-        if set(pep_args.keys()) not in implementation.allowed_pep_args:
-            return None
-
-        # All PEP tokens should be equal
-        pep_tokens = [arg.pep_token() for arg in pep_args.values()]
-        if not all([token == pep_tokens[0] for token in pep_tokens]):
-            return None
-
-        # The result is PEP, now check if it's aligned with the input(s)
-        input_token = pep_tokens[0]
-        assert input_token is not None
-        if pep_kind == PEPKind.TOKEN_PRESERVING:
-            output_token = input_token
+        elif pep_kind == PEPKind.TOKEN_PRESERVING:
+            return input_token
         else:
             h = hashlib.md5()
             h.update(input_token.encode("ascii"))
-            h.update(self.dataspec.transform().protobuf().SerializeToString())
-            output_token = h.hexdigest()
-
-        return output_token
+            h.update(transform.protobuf().SerializeToString())
+            new_token = h.hexdigest()
+            return new_token
 
     async def schema(self) -> st.Schema:
         """Computes the schema of the dataspec.
 
         The schema is computed by computing the synthetic data value and
         converting the Pyarrow schema to a Sarus schema.q
         """
@@ -213,41 +157,29 @@
 
 class ExternalDatasetOp(DatasetImplementation):
     async def to_arrow(
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         transform = self.dataset.transform()
         implementation = external_implementation(transform)
+        bound_signature = implementation.signature().bind_dataspec(
+            self.dataset
+        )
+        await bound_signature.dynamic_validation()
 
-        signature = ExternalSignature.from_dataspec(self.dataset)
-        static_checker = ExternalDatasetStaticChecker(self.dataset)
-        if static_checker.is_dp():
-            args, kwargs = signature.args(), signature.kwargs()
-            result = await implementation.call(
-                *args, **kwargs, signature=signature
-            )
-            table = to_pyarrow_table(result)
-
-        elif self.dataset.is_pep():
-            (
-                args_values,
-                kwargs_values,
-                protected_entity,
-            ) = await signature.arguments_values_and_admin_data()
-            result = await implementation.call(*args_values, **kwargs_values)
+        if self.dataset.is_pep():
+            result = await implementation.call(bound_signature)
             ds_result = t.cast(st.DatasetCastable, result)
-            output_protected_entity = compute_admin_data(
-                protected_entity, ds_result
-            )
+            admin_data = await bound_signature.admin_data()
+            output_admin_data = compute_admin_data(admin_data, ds_result)
             data_table = to_pyarrow_table(ds_result)
-            table = merge_data_and_admin(data_table, output_protected_entity)
+            table = merge_data_and_admin(data_table, output_admin_data)
 
         else:
-            (args_values, kwargs_values) = await signature.arguments_values()
-            result = await implementation.call(*args_values, **kwargs_values)
+            result = await implementation.call(bound_signature)
             table = to_pyarrow_table(result)
 
         return async_iter(table.to_batches(max_chunksize=batch_size))
 
 
 class ExternalScalarOp(ScalarImplementation):
     async def value(self) -> t.Any:
@@ -267,182 +199,124 @@
 
     This function computes the output value without manipulating the
     corresponding Dataspec. This is useful when we need to have access
     to the value of a Dataspec before its creation:
       - for computing a Mock value and inferring if the result is
         a Scalar or a Dataset.
     """
-    signature = ExternalSignature(transform, ds_args, ds_kwargs)
     implementation = external_implementation(transform)
-    args, kwargs = signature.args(), signature.kwargs()
+    bound_signature = implementation.signature().bind(
+        transform, *ds_args, **ds_kwargs
+    )
+    await bound_signature.dynamic_validation()
 
-    if implementation.is_dp(*args, **kwargs):
-        data = await implementation.call(*args, **kwargs, signature=signature)
+    if implementation.is_dp(bound_signature):
+        data = await implementation.call(bound_signature)
 
     else:
-        (args_values, kwargs_values) = await signature.arguments_values()
-        data = await implementation.call(*args_values, **kwargs_values)
+        data = await implementation.call(bound_signature)
 
     return data
 
 
 class ExternalOpImplementation:
     """External PEP op implementation class.
 
     This class wraps together several elements of an external op
     implementation:
         - `call` is the function that computes the output value from the
           input(s) value(s).
     """
 
-    transform_id: str
-    _dp_equivalent: t.Optional[t.Type[ExternalOpImplementation]] = None
-    allowed_pep_args: t.List[t.Set[str]] = []
+    _transform_id: str = NO_TRANSFORM_ID
+    _dp_equivalent_id: t.Optional[str] = None
+    _non_dp_equivalent_id: t.Optional[str] = None
+    _signature: t.Optional[SarusSignature] = None
+
+    def transform_id(self) -> str:
+        return self._transform_id
+
+    def dp_equivalent_id(self) -> t.Optional[str]:
+        return self._dp_equivalent_id
 
     def dp_equivalent(self) -> t.Optional[ExternalOpImplementation]:
-        if not self._dp_equivalent:
+        if not self._dp_equivalent_id:
             return None
-        return self._dp_equivalent()
 
-    @staticmethod
-    async def call(*args: t.Any, **kwargs: t.Any) -> t.Any:
+        return external_implementation_from_id(self._dp_equivalent_id)
+
+    def signature(self) -> SarusSignature:
+        if self._signature is not None:
+            return self._signature
+
+        if self._non_dp_equivalent_id is None:
+            raise ValueError(
+                f"External implementation {self.transform_id()} has no "
+                "signature defined and no non-DP equivalent."
+            )
+
+        non_dp_signature = external_implementation_from_id(
+            self._non_dp_equivalent_id
+        ).signature()
+        return non_dp_signature.make_dp()
+
+    async def call(self, bound_signature: SarusBoundSignature) -> t.Any:
         raise NotImplementedError
 
-    def pep_kind(self, *args: t.Any, **kwargs: t.Any) -> PEPKind:
+    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         """Return the PEP properties of the transform.
 
         It takes the transform arguments as input because it can depend on some
         transform parameters. For instance, it is not PEP if we are aggregating
         the rows (axis=0) and it is PEP if we are aggregating the columns
         (axis=1).
-
-        NB: This function should have the same signature as the call function.
         """
         # Default implementation
         return PEPKind.NOT_PEP
 
-    def is_dp(self, *args: t.Any, **kwargs: t.Any) -> bool:
+    def is_dp(self, bound_signature: SarusBoundSignature) -> bool:
         """Return True if the DP transform is compatible with the arguments.
 
         It takes the transform arguments as input because it can depend on some
         transform parameters. For instance, if we are aggregating the rows
         (axis=0), then there might be an equivalent DP transform but if we are
         aggregating the columns there might not (axis=1).
-
-        NB: This function should have the same signature as the call function.
         """
+        # Default implementation
         return False
 
     async def private_queries(
-        self,
-        *args: t.Any,
-        budget: t.Optional[st.Scalar] = None,
-        seed: t.Optional[st.Scalar] = None,
-        **kwargs: t.Any,
+        self, signature: SarusBoundSignature
     ) -> t.List[st.PrivateQuery]:
         """Takes as input the args of the transform (static and dynamic)."""
-        if budget is None or seed is None:
+        if not signature.is_dp():
             return []
-        # Evaluate budget and seed
-        budget_value = await budget.async_value()
-        seed_value = await seed.async_value()
-        queries, _ = await self.private_queries_and_task(
-            *args, budget=budget_value, seed=seed_value, **kwargs
-        )
+        queries, _ = await self.private_queries_and_task(signature)
         return queries
 
-    @staticmethod
     async def private_queries_and_task(
-        *args: t.Any, **kwargs: t.Any
+        self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
         raise NotImplementedError
 
 
-def make_all_named_arguments(
-    op_implementation: smt.ExternalOpImplementation,
-    args: t.Collection[t.Any],
-    kwargs: t.Dict[str, t.Any],
-) -> t.Dict[str, t.Any]:
-    """Attribute a name to all arguments serialized in the protobuf by using
-    the implementation's `call` method signature.
-    """
-    n_args = len(args)
-    argument_names = list(
-        inspect.signature(op_implementation.call).parameters.keys()
-    )
-    """
-    Example :
-    In [1]: def foo(a, b=3):
-    ...:     return a+b
-
-    In [2]: list(inspect.signature(foo).parameters.keys())
-    Out[2]: ['a', 'b']
-    """
-    for arg_name, arg_val in zip(argument_names[:n_args], args):
-        # put all args in kwargs
-        kwargs[arg_name] = arg_val
-
-    return kwargs
-
-
-def group_by_pep(
-    op_implementation: smt.ExternalOpImplementation,
-    *args: t.Any,
-    **kwargs: t.Any,
-) -> t.Tuple[t.Dict[str, st.DataSpec], t.Dict[str, st.DataSpec]]:
-    """Get Dataspec arguments and split them between PEP and non PEP.
-
-    This also identifies positional arguments by names based on the `call`
-    signature.
-    """
-    kwargs = make_all_named_arguments(op_implementation, args, kwargs)
-
-    # Keep only dataspec args and split PEP from non PEP
-    dataspec_args = {
-        arg_name: arg
-        for arg_name, arg in kwargs.items()
-        if isinstance(arg, st.DataSpec)
-    }
-    pep_args = {
-        arg_name: arg
-        for arg_name, arg in dataspec_args.items()
-        if arg.is_pep()
-    }
-    non_pep_args = {
-        arg_name: arg
-        for arg_name, arg in dataspec_args.items()
-        if arg_name not in pep_args
-    }
-    return pep_args, non_pep_args
-
-
 def external_implementation(
     transform: st.Transform,
-) -> smt.ExternalOpImplementation:
+) -> ExternalOpImplementation:
     """Return the implementation of an external op from a DataSpec.
 
     The mapping is done by the config file.
     """
     assert transform and transform.is_external()
-    library, op_name = transform_id(transform).split(".")
-    if op_name not in ROUTING["external"][library]:
-        raise NotImplementedError(
-            f"Routing: {op_name} not in {list(ROUTING['external'][library].keys())}"  # noqa: E501
-        )
+    id = transform_id(transform)
+    return external_implementation_from_id(id)
 
-    implementation_name = ROUTING["external"][library][op_name]
-    module = importlib.import_module(
-        f"sarus_data_spec.manager.ops.processor.external.{library}"
-    )
-    op_implementation = getattr(module, implementation_name)
 
-    if not isinstance(op_implementation, type):
-        op_implementation = type(
-            implementation_name,
-            (ExternalOpImplementation,),
-            {
-                "call": staticmethod(op_implementation),
-                "transform_id": transform_id,
-            },
-        )
+def external_implementation_from_id(id: str) -> ExternalOpImplementation:
+    # Imported here to avoid circular imports
+    from . import ROUTING
 
-    return t.cast(smt.ExternalOpImplementation, op_implementation())
+    library, op_name = id.split(".")
+    op_implementation = t.cast(
+        ExternalOpImplementation, ROUTING[library][op_name]
+    )
+    return op_implementation
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import logging
 import typing as t
 
 import numpy as np
 import pandas as pd
-import pandas._typing as pdt
 
 from sarus_data_spec.constants import MAX_MAX_MULT
+from sarus_data_spec.dataspec_validator.signature import SarusBoundSignature
 from sarus_data_spec.protobuf.utilities import unwrap
 import sarus_data_spec.typing as st
 
 from ..external_op import ExternalOpImplementation
-from ..signature import ExternalSignature
 
 logger = logging.getLogger(__name__)
 
 try:
     from sarus_statistics.ops.bounds.op import BoundOp
     from sarus_statistics.ops.histograms.op import CountOp
     from sarus_statistics.ops.max_multiplicity.op import MaxMultiplicityOp
     from sarus_statistics.ops.mean.op import MeanOp
     from sarus_statistics.ops.median.op import MedianOp
     from sarus_statistics.ops.std.op import StdOp
     from sarus_statistics.ops.sum.op import SumOp
-    from sarus_statistics.protobuf.size_pb2 import MaxMultiplicity
+    from sarus_statistics.protobuf.multiplicity_pb2 import (
+        MultiplicityParameters,
+    )
 except ModuleNotFoundError:
     pass  # warning raised in typing
 
 try:
     from sarus_differential_privacy.query import ComposedPrivateQuery
 except ModuleNotFoundError:
     pass  # warning raised in typing
@@ -55,25 +56,27 @@
 
 
 DEFAULT_MAX_MAX_MULT = 1
 NUMERIC_TYPES = ('integer', 'float', 'boolean')
 
 
 class pd_shape_dp(ExternalOpImplementation):
-    allowed_pep_args: t.List[t.Set[str]] = [{"parent_ds"}]
-    transform_id: str = "pandas.PD_SHAPE_DP"
+    _transform_id = "pandas.PD_SHAPE_DP"
+    _non_dp_equivalent_id = "pandas.PD_SHAPE"
 
-    def is_dp(self, *args: t.Any, **kwargs: t.Any) -> bool:
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
         return True
 
-    @staticmethod
-    async def private_queries_and_task(  # type: ignore[override]
-        parent_ds: st.Dataset, budget: t.Any, **kwargs: t.Any
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
         """Return the PrivateQueries summarizing DP characteristics."""
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
+
         if len(budget) != 1:
             raise NotImplementedError(
                 "The PrivacyParams contains more than 1 point in the privacy "
                 "profile."
             )
 
         parent_schema = await parent_ds.manager().async_schema(parent_ds)
@@ -106,52 +109,40 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    @staticmethod
-    async def call(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        budget: st.Scalar,
-        seed: st.Scalar,
-        signature: ExternalSignature,
-    ) -> t.Any:
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
             - `pe`: theprotected entity used by `sarus_statistics` primitives
         """
         # Evaluate arguments
-        dataframe, _ = await signature._value_and_pe("parent_ds", 0)
-        (
-            budget_value,
-            _,
-        ) = await signature._value_and_pe("budget")
-        seed_value, _ = await signature._value_and_pe("seed")
+        parent_ds = signature.static_kwargs()["this"]
+        (dataframe, budget, seed) = await signature.collect_args()
 
         # Get QB task parametrization
-        _, tasks = await pd_shape_dp.private_queries_and_task(
-            parent_ds, budget_value
-        )
+        _, tasks = await self.private_queries_and_task(signature)
 
-        epsilon = budget_value[0].epsilon
+        epsilon = budget[0].epsilon
         n_rows, n_cols = dataframe.shape
 
         # Compute DP value
         tasks = [unwrap(subtask) for subtask in tasks.subtasks]
-        max_mult_task, shape_task = t.cast(MaxMultiplicity, tasks[0]), t.cast(
-            GenericTask, tasks[1]
-        )
-        random_generator = np.random.default_rng(abs(seed_value))
+        max_mult_task, shape_task = t.cast(
+            MultiplicityParameters, tasks[0]
+        ), t.cast(GenericTask, tasks[1])
+        random_generator = np.random.default_rng(abs(seed))
         max_mul = MaxMultiplicityOp(
             parent_ds,
             epsilon,  # parameter for quantiles
             max_mult_task.noise_user_count,
             max_mult_task.noise_multiplicity,
             max_mult_task.max_max_multiplicity,
         ).value(random_generator)
@@ -164,37 +155,30 @@
         dp_shape = (n_rows, n_cols)
 
         # Compute private query
         return dp_shape
 
 
 class pd_sum_dp(ExternalOpImplementation):
-    allowed_pep_args: t.List[t.Set[str]] = [{"parent_ds"}]
-    transform_id: str = "pandas.PD_SUM_DP"
+    _transform_id = "pandas.PD_SUM_DP"
+    _non_dp_equivalent_id = "pandas.PD_SUM"
 
-    def is_dp(  # type: ignore[override]
-        self,
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = None,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        min_count: int = 0,
-        budget: t.Any = None,
-        seed: t.Optional[int] = None,
-        **kwargs: t.Any,
-    ) -> bool:
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
+        """`axis = 0` and `numeric_only` is `True`"""
+        axis = signature["axis"].static_value()
+        numeric_only = signature["numeric_only"].static_value()
+        if signature["this"].python_type() == str(pd.Series):
+            numeric_only = True
         return (axis == 0) and (numeric_only is True)
 
-    @staticmethod
-    async def private_queries_and_task(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        budget: t.Any,
-        **kwargs: t.Any,
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
         if len(budget) != 1:
             raise NotImplementedError(
                 "The PrivacyParams contains more than 1 point in the privacy "
                 "profile."
             )
 
         epsilon = budget[0].epsilon
@@ -238,50 +222,23 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    @staticmethod
-    async def call(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = None,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        min_count: int = 0,
-        budget: t.Optional[st.Scalar] = None,
-        seed: t.Optional[st.Scalar] = None,
-        signature: t.Optional[ExternalSignature] = None,
-        **kwargs: t.Any,
-    ) -> t.Any:
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
-        if not signature:
-            raise ValueError("Signature is None.")
+        parent_ds: st.Dataset = signature["this"].static_value()
+        dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
+        budget_value = await signature["budget"].collect()
+        seed_value = await signature["seed"].collect()
+        skipna = await signature["skipna"].collect()
 
-        dataframe, _ = await signature._value_and_pe("parent_ds", 0)
-        (
-            budget_value,
-            _,
-        ) = await signature._value_and_pe("budget")
-        seed_value, _ = await signature._value_and_pe("seed")
-
-        assert type(dataframe) in [pd.DataFrame, pd.Series]
-        assert numeric_only
-        assert axis == 0
-        assert level is None
-        assert min_count == 0
-        assert seed_value
-        assert budget_value
-
-        _, tasks = await pd_sum_dp.private_queries_and_task(
-            parent_ds=parent_ds,
-            budget=budget_value,
-        )
+        _, tasks = await self.private_queries_and_task(signature)
 
         epsilon = budget_value[0].epsilon
         # Compute DP value
         tasks = [unwrap(subtask) for subtask in tasks.subtasks]
         max_mult_task, sum_tasks = tasks[0], tasks[1:]
         random_generator = np.random.default_rng(abs(seed_value))
         max_mul = MaxMultiplicityOp(
@@ -325,41 +282,39 @@
                 parent_ds,
                 sum_parameters.parameters['noise'],
             )
             sum_dp_dict[column_name] = sum_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
-        sum_dp = pd.Series(sum_dp_dict)
+        if signature["this"].python_type() == str(pd.DataFrame):
+            sum_dp = pd.Series(sum_dp_dict)
+        else:
+            sum_dp = list(sum_dp_dict.values()).pop()
+
         return sum_dp
 
 
 class pd_mean_dp(ExternalOpImplementation):
-    allowed_pep_args: t.List[t.Set[str]] = [{"parent_ds"}]
-    transform_id: str = "pandas.PD_MEAN_DP"
+    _transform_id = "pandas.PD_MEAN_DP"
+    _non_dp_equivalent_id = "pandas.PD_MEAN"
 
-    def is_dp(  # type: ignore[override]
-        self,
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = 0,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        budget: t.Any = None,
-        seed: t.Optional[int] = None,
-        **kwargs: t.Any,
-    ) -> bool:
-        return axis == 0 and numeric_only is True
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
+        """`axis = 0` and `numeric_only` is `True`"""
+        axis = signature["axis"].static_value()
+        numeric_only = signature["numeric_only"].static_value()
+        if signature["this"].python_type() == str(pd.Series):
+            numeric_only = True
+        return (axis == 0) and (numeric_only is True)
 
-    @staticmethod
-    async def private_queries_and_task(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        budget: t.Any,
-        **kwargs: t.Any,
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
         if len(budget) != 1:
             raise NotImplementedError(
                 "The PrivacyParams contains more than 1 point in the privacy "
                 "profile."
             )
 
         epsilon = budget[0].epsilon
@@ -401,50 +356,25 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    @staticmethod
-    async def call(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = 0,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        budget: t.Optional[st.Scalar] = None,
-        seed: t.Optional[st.Scalar] = None,
-        signature: t.Optional[ExternalSignature] = None,
-        **kwargs: t.Any,
-    ) -> t.Any:
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
-        if not signature:
-            raise ValueError("Signature is None.")
+        parent_ds: st.Dataset = signature["this"].static_value()
+        dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
+        budget_value = await signature["budget"].collect()
+        seed_value = await signature["seed"].collect()
+        skipna = await signature["skipna"].collect()
+        pe = (await signature.admin_data()).to_pandas()
+
+        _, tasks = await self.private_queries_and_task(signature)
 
-        dataframe, pe_table = await signature._value_and_pe("parent_ds", 0)
-        (
-            budget_value,
-            _,
-        ) = await signature._value_and_pe("budget")
-        pe = pe_table.to_pandas()
-        seed_value, _ = await signature._value_and_pe("seed")
-
-        assert type(dataframe) in [pd.DataFrame, pd.Series]
-        assert pe.shape[0] == dataframe.shape[0]
-        assert numeric_only
-        assert axis == 0
-        assert level is None
-        assert seed_value
-        assert budget_value
-
-        _, tasks = await pd_mean_dp.private_queries_and_task(
-            parent_ds=parent_ds,
-            budget=budget_value,
-        )
         tasks = [unwrap(subtask) for subtask in tasks.subtasks]
         max_mult_task, mean_tasks = tasks[0], tasks[1:]
 
         # Compute DP value
         random_generator = np.random.default_rng(abs(seed_value))
         epsilon = budget_value[0].epsilon
         max_mul = MaxMultiplicityOp(
@@ -485,41 +415,39 @@
                 parent_ds,
                 mean_parameters.parameters['noise'],
             )
             mean_dp_dict[column_name] = mean_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
-        mean_dp = pd.Series(mean_dp_dict)
+        if signature["this"].python_type() == str(pd.DataFrame):
+            mean_dp = pd.Series(mean_dp_dict)
+        else:
+            mean_dp = list(mean_dp_dict.values()).pop()
+
         return mean_dp
 
 
 class pd_median_dp(ExternalOpImplementation):
-    allowed_pep_args: t.List[t.Set[str]] = [{"parent_ds"}]
-    transform_id: str = "pandas.PD_MEDIAN_DP"
+    _transform_id = "pandas.PD_MEDIAN_DP"
+    _non_dp_equivalent_id = "pandas.PD_MEDIAN"
 
-    def is_dp(  # type: ignore[override]
-        self,
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = 0,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        budget: t.Any = None,
-        seed: t.Optional[int] = None,
-        **kwargs: t.Any,
-    ) -> bool:
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
+        """`axis = 0` and `numeric_only` is `True`"""
+        axis = signature["axis"].static_value()
+        if signature["this"].python_type() == str(pd.Series):
+            numeric_only = True
+        numeric_only = signature["numeric_only"].static_value()
         return axis == 0 and numeric_only is True
 
-    @staticmethod
-    async def private_queries_and_task(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        budget: t.Any,
-        **kwargs: t.Any,
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
         if len(budget) != 1:
             raise NotImplementedError(
                 "The PrivacyParams contains more than 1 point in the privacy "
                 "profile."
             )
 
         epsilon = budget[0].epsilon
@@ -562,50 +490,24 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    @staticmethod
-    async def call(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = 0,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        budget: t.Optional[st.Scalar] = None,
-        seed: t.Optional[st.Scalar] = None,
-        signature: t.Optional[ExternalSignature] = None,
-        **kwargs: t.Any,
-    ) -> t.Any:
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
-        if not signature:
-            raise ValueError("Signature is None.")
+        parent_ds: st.Dataset = signature["this"].static_value()
+        dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
+        budget_value = await signature["budget"].collect()
+        seed_value = await signature["seed"].collect()
+        skipna = await signature["skipna"].collect()
+        pe = (await signature.admin_data()).to_pandas()
 
-        dataframe, pe_table = await signature._value_and_pe("parent_ds", 0)
-        (
-            budget_value,
-            _,
-        ) = await signature._value_and_pe("budget")
-        pe = pe_table.to_pandas()
-        seed_value, _ = await signature._value_and_pe("seed")
-
-        assert type(dataframe) in [pd.DataFrame, pd.Series]
-        assert pe.shape[0] == dataframe.shape[0]
-        assert numeric_only
-        assert axis == 0
-        assert level is None
-        assert seed_value
-        assert budget_value
-
-        _, tasks = await pd_median_dp.private_queries_and_task(
-            parent_ds=parent_ds,
-            budget=budget_value,
-        )
+        _, tasks = await self.private_queries_and_task(signature)
         tasks = [unwrap(subtask) for subtask in tasks.subtasks]
         max_mult_task, median_tasks = tasks[0], tasks[1:]
 
         random_generator = np.random.default_rng(abs(seed_value))
         epsilon = budget_value[0].epsilon
 
         # Compute DP value
@@ -647,42 +549,39 @@
                 parent_ds,
                 median_parameters.parameters['noise'],
             )
             median_dp_dict[column_name] = median_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
-        median_dp = pd.Series(median_dp_dict)
+        if signature["this"].python_type() == str(pd.DataFrame):
+            median_dp = pd.Series(median_dp_dict)
+        else:
+            median_dp = list(median_dp_dict.values()).pop()
+
         return median_dp
 
 
 class pd_std_dp(ExternalOpImplementation):
-    allowed_pep_args: t.List[t.Set[str]] = [{"parent_ds"}]
-    transform_id: str = "pandas.PD_STD_DP"
+    _transform_id = "pandas.PD_STD_DP"
+    _non_dp_equivalent_id = "pandas.PD_STD"
 
-    def is_dp(  # type: ignore[override]
-        self,
-        parent_ds: t.Any,
-        axis: t.Optional[pdt.Axis] = 0,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        ddof: int = 1,
-        budget: t.Any = None,
-        seed: t.Optional[int] = None,
-        **kwargs: t.Any,
-    ) -> bool:
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
+        """`axis = 0` and `numeric_only` is `True`"""
+        axis = signature["axis"].static_value()
+        numeric_only = signature["numeric_only"].static_value()
+        if signature["this"].python_type() == str(pd.Series):
+            numeric_only = True
         return axis == 0 and numeric_only is True
 
-    @staticmethod
-    async def private_queries_and_task(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        budget: t.Any,
-        **kwargs: t.Any,
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
         if len(budget) != 1:
             raise NotImplementedError(
                 "The PrivacyParams contains more than 1 point in the privacy "
                 "profile."
             )
 
         epsilon = budget[0].epsilon
@@ -725,51 +624,24 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    @staticmethod
-    async def call(  # type: ignore[override]
-        parent_ds: st.Dataset,
-        axis: t.Optional[pdt.Axis] = 0,
-        skipna: bool = True,
-        level: t.Optional[pdt.Level] = None,
-        numeric_only: t.Optional[bool] = None,
-        ddof: int = 1,
-        budget: t.Optional[st.Scalar] = None,
-        seed: t.Optional[st.Scalar] = None,
-        signature: t.Optional[ExternalSignature] = None,
-        **kwargs: t.Any,
-    ) -> t.Any:
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
-        if not signature:
-            raise ValueError("Signature is None.")
+        parent_ds: st.Dataset = signature["this"].static_value()
+        dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
+        budget_value = await signature["budget"].collect()
+        seed_value = await signature["seed"].collect()
+        skipna = await signature["skipna"].collect()
+        pe = (await signature.admin_data()).to_pandas()
 
-        dataframe, pe_table = await signature._value_and_pe("parent_ds", 0)
-        (
-            budget_value,
-            _,
-        ) = await signature._value_and_pe("budget")
-        pe = pe_table.to_pandas()
-        seed_value, _ = await signature._value_and_pe("seed")
-
-        assert type(dataframe) in [pd.DataFrame, pd.Series]
-        assert pe.shape[0] == dataframe.shape[0]
-        assert numeric_only
-        assert axis == 0
-        assert level is None
-        assert seed_value
-        assert budget_value
-
-        _, tasks = await pd_std_dp.private_queries_and_task(
-            parent_ds=parent_ds,
-            budget=budget_value,
-        )
+        _, tasks = await self.private_queries_and_task(signature)
         tasks = [unwrap(subtask) for subtask in tasks.subtasks]
         max_mult_task, std_tasks = tasks[0], tasks[1:]
 
         epsilon = budget_value[0].epsilon
         random_generator = np.random.default_rng(abs(seed_value))
 
         # Compute DP value
@@ -813,9 +685,13 @@
                 std_parameters.parameters['noise_square'],
                 std_parameters.parameters['noise_count'],
             )
             std_dp_dict[column_name] = std_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
-        std_dp = pd.Series(std_dp_dict)
+        if signature["this"].python_type() == str(pd.DataFrame):
+            std_dp = pd.Series(std_dp_dict)
+        else:
+            std_dp = list(std_dp_dict.values()).pop()
+
         return std_dp
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         AttributesBudget,
         AttributesBudgetStaticChecker,
         AutomaticBudget,
         AutomaticBudgetStaticChecker,
         SDBudget,
         SDBudgetStaticChecker,
     )
+
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("Transforms: Transforms with budgets not available.")
 try:
     from sarus_data_spec.manager.ops.processor.standard.synthetic import (  # noqa: E501
         SamplingRatios,
         SamplingRatiosStaticChecker,
@@ -247,14 +248,17 @@
 
     async def schema(self) -> st.Schema:
         return await self.static_checker.schema()
 
     async def size(self) -> st.Size:
         return await self.implementation.size()
 
+    async def multiplicity(self) -> st.Multiplicity:
+        return await self.implementation.multiplicity()
+
     async def bounds(self) -> st.Bounds:
         return await self.implementation.bounds()
 
     async def marginals(self) -> st.Marginals:
         return await self.implementation.marginals()
 
     async def sql(
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     sampled_size,
 )
 from sarus_data_spec.manager.ops.processor.standard.standard_op import (  # noqa: E501
     StandardDatasetImplementation,
     StandardDatasetStaticChecker,
 )
 from sarus_data_spec.marginals import marginals as marginals_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.path import straight_path
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.typing as st
 
 try:
@@ -81,14 +82,20 @@
         return size_builder(
             self.dataset,
             differentiated_sampled_size(
                 parent_size.statistics(), size_dict, curr_path=[DATA]
             ),
         )
 
+    async def multiplicity(self) -> st.Multiplicity:
+        parent_multiplicity = await self.parent_multiplicity()
+        return multiplicity_builder(
+            self.dataset, parent_multiplicity.statistics()
+        )
+
     async def bounds(self) -> st.Bounds:
         parent_bounds = await self.parent_bounds()
         previous_schema = await self.parent_schema()
         if len(previous_schema.tables()) == 1:
             size_ratio = new_sampling_ratio(
                 self.dataset, parent_bounds.statistics()
             )
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from sarus_data_spec.manager.ops.processor.standard.visitor_selector import (  # noqa: E501
     filter_primary_keys,
     select_rows,
     update_fks,
 )
 from sarus_data_spec.marginals import marginals as marg_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.statistics as sds
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 
@@ -109,14 +110,22 @@
         schema = await self.dataset.manager().async_schema(self.dataset)
         sizes = await self.parent_size()
         new_stats = update_statistics(
             stats=sizes.statistics(), new_type=schema.data_type()
         )
         return size_builder(dataset=self.dataset, statistics=new_stats)
 
+    async def multiplicity(self) -> st.Multiplicity:
+        schema = await self.dataset.manager().async_schema(self.dataset)
+        multiplicities = await self.parent_multiplicity()
+        new_stats = update_statistics(
+            stats=multiplicities.statistics(), new_type=schema.data_type()
+        )
+        return multiplicity_builder(dataset=self.dataset, statistics=new_stats)
+
     async def bounds(self) -> st.Bounds:
         schema = await self.dataset.manager().async_schema(self.dataset)
         bounds = await self.parent_bounds()
         new_stats = update_statistics(
             stats=bounds.statistics(), new_type=schema.data_type()
         )
         return bounds_builder(dataset=self.dataset, statistics=new_stats)
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     StandardDatasetImplementation,
     StandardDatasetStaticChecker,
 )
 from sarus_data_spec.manager.ops.processor.standard.visitor_selector import (  # noqa : E501
     select_rows,
 )
 from sarus_data_spec.marginals import marginals as marg_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.path import Path
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 
@@ -97,14 +98,23 @@
     async def size(self) -> st.Size:
         sizes = await self.parent_size()
         path = Path(self.dataset.transform().protobuf().spec.get_item.path)
         new_stats = sizes.statistics().nodes_statistics(path)
         assert len(new_stats) == 1
         return size_builder(dataset=self.dataset, statistics=new_stats[0])
 
+    async def multiplicity(self) -> st.Multiplicity:
+        multiplicities = await self.parent_multiplicity()
+        path = Path(self.dataset.transform().protobuf().spec.get_item.path)
+        new_stats = multiplicities.statistics().nodes_statistics(path)
+        assert len(new_stats) == 1
+        return multiplicity_builder(
+            dataset=self.dataset, statistics=new_stats[0]
+        )
+
     async def bounds(self) -> st.Bounds:
         bounds = await self.parent_bounds()
         path = Path(self.dataset.transform().protobuf().spec.get_item.path)
         new_stats = bounds.statistics().nodes_statistics(path)
         assert len(new_stats) == 1
         return bounds_builder(dataset=self.dataset, statistics=new_stats[0])
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 from sarus_data_spec.manager.ops.processor.standard.visitor_selector import (  # noqa: E501
     filter_primary_keys,
     select_columns,
     update_fks,
 )
 from sarus_data_spec.marginals import marginals as marg_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.statistics as sds
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 
@@ -91,14 +92,22 @@
         schema = await self.dataset.manager().async_schema(self.dataset)
         sizes = await self.parent_size()
         new_stats = update_statistics(
             stats=sizes.statistics(), new_type=schema.data_type()
         )
         return size_builder(dataset=self.dataset, statistics=new_stats)
 
+    async def multiplicity(self) -> st.Multiplicity:
+        schema = await self.dataset.manager().async_schema(self.dataset)
+        multiplicities = await self.parent_multiplicity()
+        new_stats = update_statistics(
+            stats=multiplicities.statistics(), new_type=schema.data_type()
+        )
+        return multiplicity_builder(dataset=self.dataset, statistics=new_stats)
+
     async def bounds(self) -> st.Bounds:
         schema = await self.dataset.manager().async_schema(self.dataset)
         bounds = await self.parent_bounds()
         new_stats = update_statistics(
             stats=bounds.statistics(), new_type=schema.data_type()
         )
         return bounds_builder(dataset=self.dataset, statistics=new_stats)
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.processor.standard.standard_op import (  # noqa: E501
     StandardDatasetImplementation,
     StandardDatasetStaticChecker,
 )
 from sarus_data_spec.marginals import marginals as marginals_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.typing as st
 
 try:
     from sarus_data_spec.manager.ops.processor.standard.sampling.sql import (  # noqa: E501
@@ -66,14 +67,20 @@
         size_ratio = new_sampling_ratio(self.dataset, parent_size.statistics())
         if size_ratio >= 1:
             return parent_size
         return size_builder(
             self.dataset, sampled_size(parent_size.statistics(), size_ratio)
         )
 
+    async def multiplicity(self) -> st.Multiplicity:
+        parent_multiplicity = await self.parent_multiplicity()
+        return multiplicity_builder(
+            self.dataset, parent_multiplicity.statistics()
+        )
+
     async def bounds(self) -> st.Bounds:
         parent_bounds = await self.parent_bounds()
         size_ratio = new_sampling_ratio(
             self.dataset, parent_bounds.statistics()
         )
         if size_ratio >= 1:
             return parent_bounds
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sarus_data_spec.constants import DATASET_SLUGNAME
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.processor.standard.standard_op import (  # noqa: E501
     StandardDatasetImplementation,
     StandardDatasetStaticChecker,
 )
 from sarus_data_spec.marginals import marginals as marg_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.typing as st
 
 
 class ShuffleStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
@@ -49,14 +50,20 @@
 
     async def size(self) -> st.Size:
         sizes = await self.parent_size()
         return size_builder(
             dataset=self.dataset, statistics=sizes.statistics()
         )
 
+    async def multiplicity(self) -> st.Multiplicity:
+        multiplicities = await self.parent_multiplicity()
+        return multiplicity_builder(
+            dataset=self.dataset, statistics=multiplicities.statistics()
+        )
+
     async def bounds(self) -> st.Bounds:
         bounds = await self.parent_bounds()
         return bounds_builder(
             dataset=self.dataset, statistics=bounds.statistics()
         )
 
     async def marginals(self) -> st.Marginals:
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,19 @@
         return await parent.manager().async_value(parent)
 
     async def parent_size(self) -> st.Size:
         parent = self.parent(kind='dataset')
         assert isinstance(parent, Dataset)
         return await parent.manager().async_size(parent)
 
+    async def parent_multiplicity(self) -> st.Multiplicity:
+        parent = self.parent(kind='dataset')
+        assert isinstance(parent, Dataset)
+        return await parent.manager().async_multiplicity(parent)
+
     async def parent_bounds(self) -> st.Bounds:
         parent = self.parent(kind='dataset')
         assert isinstance(parent, Dataset)
         return await parent.manager().async_bounds(parent)
 
     async def parent_marginals(self) -> st.Marginals:
         parent = self.parent(kind='dataset')
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 
 import pyarrow as pa
 
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.bounds import bounds as bounds_builder
 from sarus_data_spec.marginals import marginals as marginals_builder
+from sarus_data_spec.multiplicity import multiplicity as multiplicity_builder
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.typing as st
 
 try:
     from sarus_synthetic_data.synthetic_generator.generator import (
         SyntheticGenerator,
     )
@@ -308,14 +309,20 @@
         table = convert_array_to_table(datatype, sample)
         return async_iter_arrow(table.to_batches(max_chunksize=batch_size))
 
     async def size(self) -> st.Size:
         parent_size = await self.parent_size()
         return size_builder(self.dataset, parent_size.statistics())
 
+    async def multiplicity(self) -> st.Multiplicity:
+        parent_multiplicity = await self.parent_multiplicity()
+        return multiplicity_builder(
+            self.dataset, parent_multiplicity.statistics()
+        )
+
     async def bounds(self) -> st.Bounds:
         parent_bounds = await self.parent_bounds()
         return bounds_builder(self.dataset, parent_bounds.statistics())
 
     async def marginals(self) -> st.Marginals:
         parent_marginals = await self.parent_marginals()
         return marginals_builder(self.dataset, parent_marginals.statistics())
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/path.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ConstraintKind,
     VariantConstraint,
 )
 from sarus_data_spec.protobuf.dataset_pb2 import Dataset
 from sarus_data_spec.protobuf.links_pb2 import Links
 from sarus_data_spec.protobuf.manager_pb2 import Manager
 from sarus_data_spec.protobuf.marginals_pb2 import Marginals
+from sarus_data_spec.protobuf.multiplicity_pb2 import Multiplicity
 from sarus_data_spec.protobuf.path_pb2 import Path
 from sarus_data_spec.protobuf.predicate_pb2 import Predicate
 from sarus_data_spec.protobuf.proto_container_pb2 import ProtoContainer
 from sarus_data_spec.protobuf.relation_pb2 import Relation
 from sarus_data_spec.protobuf.scalar_pb2 import Scalar
 from sarus_data_spec.protobuf.schema_pb2 import Schema
 from sarus_data_spec.protobuf.size_pb2 import Size
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/size.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/status.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/type.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,17 @@
 
     async def async_schema(self) -> Schema:
         ...
 
     def size(self) -> t.Optional[Size]:
         ...
 
+    def multiplicity(self) -> t.Optional[Multiplicity]:
+        ...
+
     def bounds(self) -> t.Optional[Bounds]:
         ...
 
     def marginals(self) -> t.Optional[Marginals]:
         ...
 
     def to_arrow(self, batch_size: int = 10000) -> t.Iterator[pa.RecordBatch]:
@@ -474,14 +477,28 @@
         """Return the type of the underlying protobuf."""
         ...
 
     def dataset(self) -> Dataset:
         ...
 
     def statistics(self) -> Statistics:
+        ...
+
+
+class Multiplicity(Referring[sp.Multiplicity], t.Protocol):
+    """A python abstract class to describe size"""
+
+    def prototype(self) -> t.Type[sp.Multiplicity]:
+        """Return the type of the underlying protobuf."""
+        ...
+
+    def dataset(self) -> Dataset:
+        ...
+
+    def statistics(self) -> Statistics:
         ...
 
 
 class Schema(Referring[sp.Schema], t.Protocol):
     """A python abstract class to describe schemas"""
 
     def prototype(self) -> t.Type[sp.Schema]:
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.3.dev0/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 sarus_data_spec/bounds.py
 sarus_data_spec/constants.py
 sarus_data_spec/dataset.py
 sarus_data_spec/deprecation.py
 sarus_data_spec/factory.py
 sarus_data_spec/json_serialisation.py
 sarus_data_spec/marginals.py
+sarus_data_spec/multiplicity.py
 sarus_data_spec/path.py
 sarus_data_spec/predicate.py
 sarus_data_spec/py.typed
 sarus_data_spec/scalar.py
 sarus_data_spec/schema.py
 sarus_data_spec/size.py
 sarus_data_spec/statistics.py
@@ -29,26 +30,27 @@
 sarus_data_spec/arrow/array.py
 sarus_data_spec/arrow/conversion.py
 sarus_data_spec/arrow/pandas_utils.py
 sarus_data_spec/arrow/schema.py
 sarus_data_spec/arrow/type.py
 sarus_data_spec/config/__init__.py
 sarus_data_spec/config/privacy_properties.yaml
-sarus_data_spec/config/routing.yaml
 sarus_data_spec/context/__init__.py
 sarus_data_spec/context/public.py
 sarus_data_spec/context/state.py
 sarus_data_spec/context/typing.py
 sarus_data_spec/dataspec_rewriter/__init__.py
 sarus_data_spec/dataspec_rewriter/base.py
 sarus_data_spec/dataspec_rewriter/simple_rules.py
 sarus_data_spec/dataspec_rewriter/typing.py
 sarus_data_spec/dataspec_validator/__init__.py
 sarus_data_spec/dataspec_validator/base.py
+sarus_data_spec/dataspec_validator/parameter_kind.py
 sarus_data_spec/dataspec_validator/privacy_limit.py
+sarus_data_spec/dataspec_validator/signature.py
 sarus_data_spec/dataspec_validator/simple_rules.py
 sarus_data_spec/dataspec_validator/typing.py
 sarus_data_spec/manager/__init__.py
 sarus_data_spec/manager/async_utils.py
 sarus_data_spec/manager/base.py
 sarus_data_spec/manager/typing.py
 sarus_data_spec/manager/computations/__init__.py
@@ -63,24 +65,36 @@
 sarus_data_spec/manager/ops/processor/__init__.py
 sarus_data_spec/manager/ops/processor/routing.py
 sarus_data_spec/manager/ops/processor/external/__init__.py
 sarus_data_spec/manager/ops/processor/external/external_op.py
 sarus_data_spec/manager/ops/processor/external/imblearn.py
 sarus_data_spec/manager/ops/processor/external/numpy.py
 sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-sarus_data_spec/manager/ops/processor/external/protection_utils.py
-sarus_data_spec/manager/ops/processor/external/signature.py
-sarus_data_spec/manager/ops/processor/external/sklearn.py
 sarus_data_spec/manager/ops/processor/external/skopt.py
 sarus_data_spec/manager/ops/processor/external/std.py
+sarus_data_spec/manager/ops/processor/external/typing.py
 sarus_data_spec/manager/ops/processor/external/utils.py
 sarus_data_spec/manager/ops/processor/external/xgboost.py
 sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
 sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
 sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
 sarus_data_spec/manager/ops/processor/standard/__init__.py
 sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
 sarus_data_spec/manager/ops/processor/standard/extract.py
 sarus_data_spec/manager/ops/processor/standard/filter.py
 sarus_data_spec/manager/ops/processor/standard/get_item.py
 sarus_data_spec/manager/ops/processor/standard/project.py
 sarus_data_spec/manager/ops/processor/standard/sample.py
@@ -111,14 +125,17 @@
 sarus_data_spec/protobuf/links_pb2.pyi
 sarus_data_spec/protobuf/manager.proto
 sarus_data_spec/protobuf/manager_pb2.py
 sarus_data_spec/protobuf/manager_pb2.pyi
 sarus_data_spec/protobuf/marginals.proto
 sarus_data_spec/protobuf/marginals_pb2.py
 sarus_data_spec/protobuf/marginals_pb2.pyi
+sarus_data_spec/protobuf/multiplicity.proto
+sarus_data_spec/protobuf/multiplicity_pb2.py
+sarus_data_spec/protobuf/multiplicity_pb2.pyi
 sarus_data_spec/protobuf/path.proto
 sarus_data_spec/protobuf/path_pb2.py
 sarus_data_spec/protobuf/path_pb2.pyi
 sarus_data_spec/protobuf/predicate.proto
 sarus_data_spec/protobuf/predicate_pb2.py
 sarus_data_spec/protobuf/predicate_pb2.pyi
 sarus_data_spec/protobuf/proto_container.proto
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/setup.cfg` & `sarus_data_spec_public-3.2.1.dev0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 	sarus_data_spec.base
 	sarus_data_spec.bounds
 	sarus_data_spec.constants
 	sarus_data_spec.dataset
 	sarus_data_spec.deprecation
 	sarus_data_spec.factory
 	sarus_data_spec.marginals
+	sarus_data_spec.multiplicity
 	sarus_data_spec.path
 	sarus_data_spec.predicate
 	sarus_data_spec.scalar
 	sarus_data_spec.schema
 	sarus_data_spec.size
 	sarus_data_spec.statistics
 	sarus_data_spec.status
@@ -75,40 +76,55 @@
 	sarus_data_spec.manager.ops.processor.standard.synthetic
 	sarus_data_spec.manager.ops.processor.external.external_op
 	sarus_data_spec.manager.ops.processor.external.imblearn
 	sarus_data_spec.manager.ops.processor.external.numpy
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas_dp
 	sarus_data_spec.manager.ops.processor.external.pandas_profiling
-	sarus_data_spec.manager.ops.processor.external.protection_utils
 	sarus_data_spec.manager.ops.processor.external.sklearn
+	sarus_data_spec.manager.ops.processor.external.sklearn.cluster
+	sarus_data_spec.manager.ops.processor.external.sklearn.compose
+	sarus_data_spec.manager.ops.processor.external.sklearn.decomposition
+	sarus_data_spec.manager.ops.processor.external.sklearn.ensemble
+	sarus_data_spec.manager.ops.processor.external.sklearn.impute
+	sarus_data_spec.manager.ops.processor.external.sklearn.inspection
+	sarus_data_spec.manager.ops.processor.external.sklearn.lib
+	sarus_data_spec.manager.ops.processor.external.sklearn.linear_model
+	sarus_data_spec.manager.ops.processor.external.sklearn.metrics
+	sarus_data_spec.manager.ops.processor.external.sklearn.model_selection
+	sarus_data_spec.manager.ops.processor.external.sklearn.pipeline
+	sarus_data_spec.manager.ops.processor.external.sklearn.preprocessing
+	sarus_data_spec.manager.ops.processor.external.sklearn.svm
 	sarus_data_spec.manager.ops.processor.external.skopt
-	sarus_data_spec.manager.ops.processor.external.signature
 	sarus_data_spec.manager.ops.processor.external.std
+	sarus_data_spec.manager.ops.processor.external.typing
 	sarus_data_spec.manager.ops.processor.external.utils
 	sarus_data_spec.manager.ops.processor.external.xgboost
 	sarus_data_spec.dataspec_rewriter.typing
 	sarus_data_spec.dataspec_rewriter.base
 	sarus_data_spec.dataspec_rewriter.simple_rules
 	sarus_data_spec.dataspec_validator.typing
 	sarus_data_spec.dataspec_validator.base
 	sarus_data_spec.dataspec_validator.simple_rules
+	sarus_data_spec.dataspec_validator.signature
+	sarus_data_spec.dataspec_validator.parameter_kind
 	sarus_data_spec.dataspec_validator.privacy_limit
 	sarus_data_spec.context.typing
 	sarus_data_spec.context.public
 	sarus_data_spec.context.state
 	sarus_data_spec.protobuf.typing
 	sarus_data_spec.protobuf.utilities
 	sarus_data_spec.protobuf.attribute_pb2
 	sarus_data_spec.protobuf.bounds_pb2
 	sarus_data_spec.protobuf.constraint_pb2
 	sarus_data_spec.protobuf.dataset_pb2
 	sarus_data_spec.protobuf.links_pb2
 	sarus_data_spec.protobuf.manager_pb2
 	sarus_data_spec.protobuf.marginals_pb2
+	sarus_data_spec.protobuf.multiplicity_pb2
 	sarus_data_spec.protobuf.path_pb2
 	sarus_data_spec.protobuf.predicate_pb2
 	sarus_data_spec.protobuf.proto_container_pb2
 	sarus_data_spec.protobuf.relation_pb2
 	sarus_data_spec.protobuf.scalar_pb2
 	sarus_data_spec.protobuf.schema_pb2
 	sarus_data_spec.protobuf.size_pb2
```

### Comparing `sarus_data_spec_public-3.0.3.dev0/setup.py` & `sarus_data_spec_public-3.2.1.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.0.3.dev0')
+    setup(version='3.2.1.dev0')
```

