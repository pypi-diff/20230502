# Comparing `tmp/dazl-8.0.0a2.tar.gz` & `tmp/dazl-8.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dazl-8.0.0a2.tar", last modified: Fri Mar 19 15:15:09 2021, max compression
+gzip compressed data, was "dazl-8.0.0a3.tar", last modified: Tue Mar 23 16:12:14 2021, max compression
```

## Comparing `dazl-8.0.0a2.tar` & `dazl-8.0.0a3.tar`

### file list

```diff
@@ -1,203 +1,204 @@
--rw-r--r--   0        0        0     2696 2021-03-18 14:00:20.333101 dazl-8.0.0a2/README.md
--rw-r--r--   0        0        0     2832 2021-03-18 14:00:20.333895 dazl-8.0.0a2/dazl/__init__.py
--rw-r--r--   0        0        0      275 2021-03-11 02:10:43.591711 dazl-8.0.0a2/dazl/__main__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592234 dazl-8.0.0a2/dazl/_gen/__init__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592532 dazl-8.0.0a2/dazl/_gen/com/__init__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592716 dazl-8.0.0a2/dazl/_gen/com/daml/__init__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592893 dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/__init__.py
--rw-r--r--   0        0        0     1783 2021-03-11 02:10:43.593150 dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/daml_lf_0_pb2.py
--rw-r--r--   0        0        0   385176 2021-03-11 02:10:43.594165 dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/daml_lf_1_pb2.py
--rw-r--r--   0        0        0     7842 2021-03-11 02:10:43.594427 dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/daml_lf_pb2.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.594585 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/__init__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.594819 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/__init__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.595003 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/__init__.py
--rw-r--r--   0        0        0    11341 2021-03-11 02:10:43.595289 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py
--rw-r--r--   0        0        0     4541 2021-03-11 02:10:43.595555 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.595726 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py
--rw-r--r--   0        0        0    16007 2021-03-11 02:10:43.595945 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py
--rw-r--r--   0        0        0     7254 2021-03-11 02:10:43.596189 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    13384 2021-03-11 02:10:43.596549 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py
--rw-r--r--   0        0        0     7388 2021-03-11 02:10:43.597010 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     5556 2021-03-11 02:10:43.597339 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py
--rw-r--r--   0        0        0     5813 2021-03-11 02:10:43.597572 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py
--rw-r--r--   0        0        0    20434 2021-03-11 02:10:43.597832 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py
--rw-r--r--   0        0        0    12769 2021-03-11 02:10:43.598090 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    17265 2021-03-11 02:10:43.598335 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py
--rw-r--r--   0        0        0     8870 2021-03-11 02:10:43.598586 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py
--rw-r--r--   0        0        0    13599 2021-03-11 02:10:43.598826 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py
--rw-r--r--   0        0        0    12841 2021-03-11 02:10:43.599155 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py
--rw-r--r--   0        0        0     5486 2021-03-11 02:10:43.599393 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py
--rw-r--r--   0        0        0     6579 2021-03-11 02:10:43.599623 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py
--rw-r--r--   0        0        0    30489 2021-03-11 02:10:43.599890 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py
--rw-r--r--   0        0        0     5382 2021-03-11 02:10:43.600127 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py
--rw-r--r--   0        0        0    23918 2021-03-11 02:10:43.600385 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py
--rw-r--r--   0        0        0     9393 2021-03-11 02:10:43.600648 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py
--rw-r--r--   0        0        0     3900 2021-03-11 02:10:43.600866 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py
--rw-r--r--   0        0        0     6204 2021-03-11 02:10:43.601082 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py
--rw-r--r--   0        0        0     3859 2021-03-11 02:10:43.601322 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py
--rw-r--r--   0        0        0     5330 2021-03-11 02:10:43.601536 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py
--rw-r--r--   0        0        0    20956 2021-03-11 02:10:43.601863 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py
--rw-r--r--   0        0        0     7887 2021-03-11 02:10:43.602261 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.602506 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/__init__.py
--rw-r--r--   0        0        0     3978 2021-03-11 02:10:43.602726 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2.py
--rw-r--r--   0        0        0     7210 2021-03-11 02:10:43.602954 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.py
--rw-r--r--   0        0        0     9735 2021-03-11 02:10:43.603316 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py
--rw-r--r--   0        0        0     5342 2021-03-11 02:10:43.603562 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py
--rw-r--r--   0        0        0     5923 2021-03-11 02:10:43.603904 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/trace_context_pb2.py
--rw-r--r--   0        0        0     9384 2021-03-11 02:10:43.604199 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py
--rw-r--r--   0        0        0    20415 2021-03-11 02:10:43.604532 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py
--rw-r--r--   0        0        0    32470 2021-03-11 02:10:43.604866 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py
--rw-r--r--   0        0        0    19448 2021-03-11 02:10:43.605156 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py
--rw-r--r--   0        0        0    39736 2021-03-11 02:10:43.605486 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py
--rw-r--r--   0        0        0     5694 2021-03-11 02:10:43.605797 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py
--rw-r--r--   0        0        0     3208 2021-03-11 02:10:43.606037 dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.606585 dazl-8.0.0a2/dazl/_gen/google/__init__.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.606931 dazl-8.0.0a2/dazl/_gen/google/rpc/__init__.py
--rw-r--r--   0        0        0     4127 2021-03-11 02:10:43.608818 dazl-8.0.0a2/dazl/_gen/google/rpc/status_pb2.py
--rw-r--r--   0        0        0     5218 2021-03-11 02:10:43.609019 dazl-8.0.0a2/dazl/_logging.py
--rw-r--r--   0        0        0     1759 2021-03-11 02:10:43.804731 dazl-8.0.0a2/dazl/cli/__init__.py
--rw-r--r--   0        0        0      566 2021-03-11 02:10:43.611554 dazl-8.0.0a2/dazl/cli/_base.py
--rw-r--r--   0        0        0     2069 2021-03-11 02:10:43.611895 dazl-8.0.0a2/dazl/cli/ls.py
--rw-r--r--   0        0        0     3384 2021-03-11 02:10:43.805003 dazl-8.0.0a2/dazl/cli/metadata.py
--rw-r--r--   0        0        0     3191 2021-03-11 02:10:43.805431 dazl-8.0.0a2/dazl/cli/tail.py
--rw-r--r--   0        0        0     1197 2021-03-11 02:10:43.613293 dazl-8.0.0a2/dazl/cli/upload.py
--rw-r--r--   0        0        0      454 2021-03-11 02:10:43.613720 dazl-8.0.0a2/dazl/cli/version.py
--rw-r--r--   0        0        0     1000 2021-03-11 02:10:43.614163 dazl-8.0.0a2/dazl/client/__init__.py
--rw-r--r--   0        0        0     1294 2021-03-18 14:00:20.335218 dazl-8.0.0a2/dazl/client/_base_model.py
--rw-r--r--   0        0        0     3484 2021-03-11 02:10:43.805746 dazl-8.0.0a2/dazl/client/_conn_settings.py
--rw-r--r--   0        0        0     1383 2021-03-18 14:00:20.335915 dazl-8.0.0a2/dazl/client/_events.py
--rw-r--r--   0        0        0    22467 2021-03-18 14:00:20.336720 dazl-8.0.0a2/dazl/client/_network_client_impl.py
--rw-r--r--   0        0        0    27609 2021-03-18 14:00:20.337763 dazl-8.0.0a2/dazl/client/_party_client_impl.py
--rw-r--r--   0        0        0     4759 2021-03-11 02:10:43.807637 dazl-8.0.0a2/dazl/client/_reader_sync.py
--rw-r--r--   0        0        0      810 2021-03-11 02:10:43.807983 dazl-8.0.0a2/dazl/client/_run_level.py
--rw-r--r--   0        0        0     2623 2021-03-18 14:00:20.338118 dazl-8.0.0a2/dazl/client/_writer_verify.py
--rw-r--r--   0        0        0    68829 2021-03-18 14:00:20.338762 dazl-8.0.0a2/dazl/client/api.py
--rw-r--r--   0        0        0    19473 2021-03-18 14:00:20.339368 dazl-8.0.0a2/dazl/client/bots.py
--rw-r--r--   0        0        0    19358 2021-03-18 14:00:20.339593 dazl-8.0.0a2/dazl/client/commands.py
--rw-r--r--   0        0        0    17485 2021-03-11 02:10:43.810153 dazl-8.0.0a2/dazl/client/config.py
--rw-r--r--   0        0        0     1288 2021-03-11 02:10:43.810302 dazl-8.0.0a2/dazl/client/errors.py
--rw-r--r--   0        0        0     7109 2021-03-11 02:10:43.810567 dazl-8.0.0a2/dazl/client/events.py
--rw-r--r--   0        0        0      938 2021-03-18 14:00:20.340111 dazl-8.0.0a2/dazl/client/ledger.py
--rw-r--r--   0        0        0      387 2021-03-18 14:00:20.340427 dazl-8.0.0a2/dazl/client/pkg_loader.py
--rw-r--r--   0        0        0      916 2021-03-11 02:10:43.621794 dazl-8.0.0a2/dazl/client/runner.py
--rw-r--r--   0        0        0     8648 2021-03-18 14:00:20.340815 dazl-8.0.0a2/dazl/client/state.py
--rw-r--r--   0        0        0     1477 2021-03-11 02:10:43.622839 dazl-8.0.0a2/dazl/damlast/__init__.py
--rw-r--r--   0        0        0      404 2021-03-11 02:10:43.623392 dazl-8.0.0a2/dazl/damlast/_base.py
--rw-r--r--   0        0        0     2776 2021-03-11 02:10:43.812202 dazl-8.0.0a2/dazl/damlast/_builtins_meta.py
--rw-r--r--   0        0        0     2052 2021-03-11 02:10:43.625248 dazl-8.0.0a2/dazl/damlast/builtins.py
--rw-r--r--   0        0        0    67449 2021-03-11 02:10:43.626282 dazl-8.0.0a2/dazl/damlast/daml_lf_1.py
--rw-r--r--   0        0        0     6256 2021-03-11 02:10:43.626819 dazl-8.0.0a2/dazl/damlast/daml_types.py
--rw-r--r--   0        0        0     1359 2021-03-11 02:10:43.812517 dazl-8.0.0a2/dazl/damlast/errors.py
--rw-r--r--   0        0        0    12487 2021-03-11 02:10:43.628084 dazl-8.0.0a2/dazl/damlast/expand.py
--rw-r--r--   0        0        0    15491 2021-03-18 14:00:20.341346 dazl-8.0.0a2/dazl/damlast/lookup.py
--rw-r--r--   0        0        0     2858 2021-03-11 02:10:43.628616 dazl-8.0.0a2/dazl/damlast/parse.py
--rw-r--r--   0        0        0    30162 2021-03-11 02:10:43.629545 dazl-8.0.0a2/dazl/damlast/pb_parse.py
--rw-r--r--   0        0        0     8021 2021-03-18 14:00:20.342216 dazl-8.0.0a2/dazl/damlast/pkgfile.py
--rw-r--r--   0        0        0     4819 2021-03-18 14:00:20.343284 dazl-8.0.0a2/dazl/damlast/protocols.py
--rw-r--r--   0        0        0     2744 2021-03-11 02:10:43.813241 dazl-8.0.0a2/dazl/damlast/types.py
--rw-r--r--   0        0        0     4654 2021-03-11 02:10:43.813599 dazl-8.0.0a2/dazl/damlast/util.py
--rw-r--r--   0        0        0    13881 2021-03-11 02:10:43.631873 dazl-8.0.0a2/dazl/damlast/visitor.py
--rw-r--r--   0        0        0    19958 2021-03-18 14:00:20.343551 dazl-8.0.0a2/dazl/ledger/__init__.py
--rw-r--r--   0        0        0    15742 2021-03-19 15:12:46.013185 dazl-8.0.0a2/dazl/ledger/api_types.py
--rw-r--r--   0        0        0    16361 2021-03-18 14:00:20.344088 dazl-8.0.0a2/dazl/ledger/config/__init__.py
--rw-r--r--   0        0        0    15856 2021-03-18 14:00:20.344264 dazl-8.0.0a2/dazl/ledger/config/access.py
--rw-r--r--   0        0        0    13799 2021-03-18 14:00:20.344427 dazl-8.0.0a2/dazl/ledger/config/argv.py
--rw-r--r--   0        0        0      126 2021-03-18 14:00:20.344719 dazl-8.0.0a2/dazl/ledger/config/exc.py
--rw-r--r--   0        0        0     2626 2021-03-18 14:00:20.344857 dazl-8.0.0a2/dazl/ledger/config/ssl.py
--rw-r--r--   0        0        0     8882 2021-03-18 14:00:20.345010 dazl-8.0.0a2/dazl/ledger/config/url.py
--rw-r--r--   0        0        0      773 2021-03-18 14:00:20.345126 dazl-8.0.0a2/dazl/ledger/errors.py
--rw-r--r--   0        0        0     1390 2021-03-18 14:00:20.345814 dazl-8.0.0a2/dazl/ledger/grpc/__init__.py
--rw-r--r--   0        0        0     1878 2021-03-18 14:00:20.345950 dazl-8.0.0a2/dazl/ledger/grpc/channel.py
--rw-r--r--   0        0        0    14080 2021-03-18 14:00:20.346393 dazl-8.0.0a2/dazl/ledger/grpc/codec_aio.py
--rw-r--r--   0        0        0    19667 2021-03-19 15:12:46.014229 dazl-8.0.0a2/dazl/ledger/grpc/conn_aio.py
--rw-r--r--   0        0        0      277 2021-03-18 14:00:20.347073 dazl-8.0.0a2/dazl/ledger/pkgcache.py
--rw-r--r--   0        0        0     8693 2021-03-18 14:00:20.347267 dazl-8.0.0a2/dazl/ledger/pkgloader_aio.py
--rw-r--r--   0        0        0     2891 2021-03-18 14:00:20.347407 dazl-8.0.0a2/dazl/ledger/pkgloader_aio_compat.py
--rw-r--r--   0        0        0     5236 2021-03-19 15:12:46.015256 dazl-8.0.0a2/dazl/ledger/stream_aio.py
--rw-r--r--   0        0        0     3680 2021-03-19 15:12:46.015712 dazl-8.0.0a2/dazl/ledger/stream_aio.pyi
--rw-r--r--   0        0        0      162 2021-03-19 15:12:46.016189 dazl-8.0.0a2/dazl/ledgerutil/__init__.py
--rw-r--r--   0        0        0     4041 2021-03-19 15:12:46.016485 dazl-8.0.0a2/dazl/ledgerutil/acs.py
--rw-r--r--   0        0        0      172 2021-03-11 02:10:43.633749 dazl-8.0.0a2/dazl/metrics/__init__.py
--rw-r--r--   0        0        0      955 2021-03-11 02:10:43.814000 dazl-8.0.0a2/dazl/metrics/api.py
--rw-r--r--   0        0        0     1578 2021-03-11 02:10:43.635018 dazl-8.0.0a2/dazl/metrics/instrumenters.py
--rw-r--r--   0        0        0     1557 2021-03-11 02:10:43.814282 dazl-8.0.0a2/dazl/metrics/prometheus.py
--rw-r--r--   0        0        0      882 2021-03-11 02:10:43.814685 dazl-8.0.0a2/dazl/model/__init__.py
--rw-r--r--   0        0        0     2043 2021-03-11 02:10:43.815212 dazl-8.0.0a2/dazl/model/core.py
--rw-r--r--   0        0        0      281 2021-03-11 02:10:43.815669 dazl-8.0.0a2/dazl/model/ledger.py
--rw-r--r--   0        0        0      393 2021-03-11 02:10:43.816116 dazl-8.0.0a2/dazl/model/lookup.py
--rw-r--r--   0        0        0      439 2021-03-11 02:10:43.816500 dazl-8.0.0a2/dazl/model/network.py
--rw-r--r--   0        0        0     1177 2021-03-11 02:10:43.816927 dazl-8.0.0a2/dazl/model/reading.py
--rw-r--r--   0        0        0     1176 2021-03-18 14:00:20.348095 dazl-8.0.0a2/dazl/model/writing.py
--rw-r--r--   0        0        0     1558 2021-03-11 02:10:43.817653 dazl-8.0.0a2/dazl/pretty/__init__.py
--rw-r--r--   0        0        0     5549 2021-03-11 02:10:43.817968 dazl-8.0.0a2/dazl/pretty/_module_builder.py
--rw-r--r--   0        0        0    33366 2021-03-11 02:10:43.818474 dazl-8.0.0a2/dazl/pretty/_render_base.py
--rw-r--r--   0        0        0      953 2021-03-11 02:10:43.644693 dazl-8.0.0a2/dazl/pretty/options.py
--rw-r--r--   0        0        0      842 2021-03-11 02:10:43.645308 dazl-8.0.0a2/dazl/pretty/pygments_daml_lexer.py
--rw-r--r--   0        0        0    16881 2021-03-11 02:10:43.818929 dazl-8.0.0a2/dazl/pretty/render_csharp.py
--rw-r--r--   0        0        0     1756 2021-03-11 02:10:43.819309 dazl-8.0.0a2/dazl/pretty/render_csv.py
--rw-r--r--   0        0        0    16122 2021-03-11 02:10:43.819695 dazl-8.0.0a2/dazl/pretty/render_daml.py
--rw-r--r--   0        0        0    14612 2021-03-11 02:10:43.820106 dazl-8.0.0a2/dazl/pretty/render_python.py
--rw-r--r--   0        0        0      216 2021-03-11 02:10:43.648874 dazl-8.0.0a2/dazl/pretty/table/__init__.py
--rw-r--r--   0        0        0      697 2021-03-11 02:10:43.649075 dazl-8.0.0a2/dazl/pretty/table/fmt_base.py
--rw-r--r--   0        0        0     1627 2021-03-11 02:10:43.649433 dazl-8.0.0a2/dazl/pretty/table/fmt_json.py
--rw-r--r--   0        0        0     5341 2021-03-11 02:10:43.649643 dazl-8.0.0a2/dazl/pretty/table/fmt_pretty.py
--rw-r--r--   0        0        0     3087 2021-03-11 02:10:43.649898 dazl-8.0.0a2/dazl/pretty/table/model.py
--rw-r--r--   0        0        0     1517 2021-03-11 02:10:43.650204 dazl-8.0.0a2/dazl/pretty/table/write.py
--rw-r--r--   0        0        0     3284 2021-03-11 02:10:43.650799 dazl-8.0.0a2/dazl/pretty/util.py
--rw-r--r--   0        0        0      991 2021-03-18 14:00:20.348860 dazl-8.0.0a2/dazl/prim/__init__.py
--rw-r--r--   0        0        0     1562 2021-03-18 14:00:20.349446 dazl-8.0.0a2/dazl/prim/basic.py
--rw-r--r--   0        0        0     1581 2021-03-11 02:10:43.651451 dazl-8.0.0a2/dazl/prim/complex.py
--rw-r--r--   0        0        0     2102 2021-03-11 02:10:43.651656 dazl-8.0.0a2/dazl/prim/contracts.py
--rw-r--r--   0        0        0     6875 2021-03-11 02:10:43.651973 dazl-8.0.0a2/dazl/prim/datetime.py
--rw-r--r--   0        0        0     1119 2021-03-11 02:10:43.820552 dazl-8.0.0a2/dazl/prim/errors.py
--rw-r--r--   0        0        0     1394 2021-03-11 02:10:43.652145 dazl-8.0.0a2/dazl/prim/json.py
--rw-r--r--   0        0        0     1362 2021-03-11 02:10:43.652362 dazl-8.0.0a2/dazl/prim/map.py
--rw-r--r--   0        0        0     1285 2021-03-11 02:10:43.652623 dazl-8.0.0a2/dazl/prim/numbers.py
--rw-r--r--   0        0        0      330 2021-03-11 02:10:43.652792 dazl-8.0.0a2/dazl/prim/party.py
--rw-r--r--   0        0        0      369 2021-03-11 02:10:43.653218 dazl-8.0.0a2/dazl/protocols/__init__.py
--rw-r--r--   0        0        0     5144 2021-03-18 14:00:20.350461 dazl-8.0.0a2/dazl/protocols/_base.py
--rw-r--r--   0        0        0     8460 2021-03-18 14:00:20.351109 dazl-8.0.0a2/dazl/protocols/autodetect.py
--rw-r--r--   0        0        0     2941 2021-03-18 14:00:20.351599 dazl-8.0.0a2/dazl/protocols/core.py
--rw-r--r--   0        0        0      884 2021-03-18 14:00:20.352124 dazl-8.0.0a2/dazl/protocols/errors.py
--rw-r--r--   0        0        0     6750 2021-03-11 02:10:43.822145 dazl-8.0.0a2/dazl/protocols/events.py
--rw-r--r--   0        0        0     2160 2021-03-11 02:10:43.822547 dazl-8.0.0a2/dazl/protocols/oauth.py
--rw-r--r--   0        0        0     4490 2021-03-18 14:00:20.352273 dazl-8.0.0a2/dazl/protocols/serializers.py
--rw-r--r--   0        0        0      141 2021-03-11 02:10:43.656066 dazl-8.0.0a2/dazl/protocols/v1/__init__.py
--rw-r--r--   0        0        0    13875 2021-03-18 14:00:20.353075 dazl-8.0.0a2/dazl/protocols/v1/grpc.py
--rw-r--r--   0        0        0     2578 2021-03-11 02:10:43.657362 dazl-8.0.0a2/dazl/protocols/v1/model/__init__.py
--rw-r--r--   0        0        0    16616 2021-03-18 14:00:20.353739 dazl-8.0.0a2/dazl/protocols/v1/pb_parse_event.py
--rw-r--r--   0        0        0     4532 2021-03-18 14:00:20.354336 dazl-8.0.0a2/dazl/protocols/v1/pb_ser_command.py
--rw-r--r--   0        0        0      194 2021-03-11 02:10:43.659880 dazl-8.0.0a2/dazl/py.typed
--rw-r--r--   0        0        0      277 2021-03-18 14:00:20.354709 dazl-8.0.0a2/dazl/query/__init__.py
--rw-r--r--   0        0        0     1479 2021-03-18 14:00:20.355076 dazl-8.0.0a2/dazl/query/query.py
--rw-r--r--   0        0        0      234 2021-03-11 02:10:43.660160 dazl-8.0.0a2/dazl/scheduler/__init__.py
--rw-r--r--   0        0        0     1284 2021-03-11 02:10:43.660300 dazl-8.0.0a2/dazl/scheduler/_base.py
--rw-r--r--   0        0        0     4816 2021-03-11 02:10:43.660474 dazl-8.0.0a2/dazl/scheduler/_invoker.py
--rw-r--r--   0        0        0     2030 2021-03-11 02:10:43.660613 dazl-8.0.0a2/dazl/scheduler/_invoker.pyi
--rw-r--r--   0        0        0      539 2021-03-11 02:10:43.661188 dazl-8.0.0a2/dazl/server/__init__.py
--rw-r--r--   0        0        0     3175 2021-03-11 02:10:43.824657 dazl-8.0.0a2/dazl/server/management.py
--rw-r--r--   0        0        0     1678 2021-03-11 02:10:43.662514 dazl-8.0.0a2/dazl/server/metrics.py
--rw-r--r--   0        0        0      376 2021-03-11 02:10:43.824944 dazl-8.0.0a2/dazl/util/__init__.py
--rw-r--r--   0        0        0    23710 2021-03-11 02:10:43.664455 dazl-8.0.0a2/dazl/util/asyncio_util.py
--rw-r--r--   0        0        0     4687 2021-03-11 02:10:43.825255 dazl-8.0.0a2/dazl/util/config_meta.py
--rw-r--r--   0        0        0      928 2021-03-11 02:10:43.667126 dazl-8.0.0a2/dazl/util/enum.py
--rw-r--r--   0        0        0     2631 2021-03-11 02:10:43.667679 dazl-8.0.0a2/dazl/util/io.py
--rw-r--r--   0        0        0      785 2021-03-11 02:10:43.668185 dazl-8.0.0a2/dazl/util/logging.py
--rw-r--r--   0        0        0     1188 2021-03-11 02:10:43.668878 dazl-8.0.0a2/dazl/util/notifications.py
--rw-r--r--   0        0        0      568 2021-03-11 02:10:43.669444 dazl-8.0.0a2/dazl/util/path_util.py
--rw-r--r--   0        0        0     2510 2021-03-11 02:10:43.670127 dazl-8.0.0a2/dazl/util/prim_natural.py
--rw-r--r--   0        0        0     3390 2021-03-11 02:10:43.825542 dazl-8.0.0a2/dazl/util/proc_util.py
--rw-r--r--   0        0        0     1316 2021-03-11 02:10:43.671521 dazl-8.0.0a2/dazl/util/termcap.py
--rw-r--r--   0        0        0     3814 2021-03-11 02:10:43.672144 dazl-8.0.0a2/dazl/util/tools.py
--rw-r--r--   0        0        0     2820 2021-03-11 02:10:43.672720 dazl-8.0.0a2/dazl/util/typing.py
--rw-r--r--   0        0        0      576 2021-03-11 02:10:43.672860 dazl-8.0.0a2/dazl/values/__init__.py
--rw-r--r--   0        0        0     6214 2021-03-11 02:10:43.673001 dazl-8.0.0a2/dazl/values/canonical.py
--rw-r--r--   0        0        0    14279 2021-03-11 02:10:43.825988 dazl-8.0.0a2/dazl/values/context.py
--rw-r--r--   0        0        0     1840 2021-03-11 02:10:43.673422 dazl-8.0.0a2/dazl/values/json.py
--rw-r--r--   0        0        0     3468 2021-03-18 14:00:20.356349 dazl-8.0.0a2/dazl/values/mapper.py
--rw-r--r--   0        0        0     9821 2021-03-11 02:10:43.674131 dazl-8.0.0a2/dazl/values/protobuf.py
--rw-r--r--   0        0        0     2837 2021-03-11 02:10:43.674352 dazl-8.0.0a2/dazl/values/pysample_encoder.py
--rw-r--r--   0        0        0     5092 2021-03-11 02:10:43.674578 dazl-8.0.0a2/dazl/values/string.py
--rw-r--r--   0        0        0     1625 2021-03-19 15:12:46.021227 dazl-8.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     4518 2021-03-19 15:15:10.600765 dazl-8.0.0a2/setup.py
--rw-r--r--   0        0        0     3824 2021-03-19 15:15:10.601111 dazl-8.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2696 2021-03-18 14:00:20.333101 dazl-8.0.0a3/README.md
+-rw-r--r--   0        0        0     2832 2021-03-18 14:00:20.333895 dazl-8.0.0a3/dazl/__init__.py
+-rw-r--r--   0        0        0      275 2021-03-11 02:10:43.591711 dazl-8.0.0a3/dazl/__main__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592234 dazl-8.0.0a3/dazl/_gen/__init__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592532 dazl-8.0.0a3/dazl/_gen/com/__init__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592716 dazl-8.0.0a3/dazl/_gen/com/daml/__init__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.592893 dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/__init__.py
+-rw-r--r--   0        0        0     1783 2021-03-11 02:10:43.593150 dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/daml_lf_0_pb2.py
+-rw-r--r--   0        0        0   385176 2021-03-11 02:10:43.594165 dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/daml_lf_1_pb2.py
+-rw-r--r--   0        0        0     7842 2021-03-11 02:10:43.594427 dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/daml_lf_pb2.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.594585 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/__init__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.594819 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/__init__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.595003 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/__init__.py
+-rw-r--r--   0        0        0    11341 2021-03-11 02:10:43.595289 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py
+-rw-r--r--   0        0        0     4541 2021-03-11 02:10:43.595555 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.595726 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/__init__.py
+-rw-r--r--   0        0        0    16007 2021-03-11 02:10:43.595945 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py
+-rw-r--r--   0        0        0     7254 2021-03-11 02:10:43.596189 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    13384 2021-03-11 02:10:43.596549 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py
+-rw-r--r--   0        0        0     7388 2021-03-11 02:10:43.597010 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5556 2021-03-11 02:10:43.597339 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py
+-rw-r--r--   0        0        0     5813 2021-03-11 02:10:43.597572 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20434 2021-03-11 02:10:43.597832 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py
+-rw-r--r--   0        0        0    12769 2021-03-11 02:10:43.598090 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    17265 2021-03-11 02:10:43.598335 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py
+-rw-r--r--   0        0        0     8870 2021-03-11 02:10:43.598586 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py
+-rw-r--r--   0        0        0    13599 2021-03-11 02:10:43.598826 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py
+-rw-r--r--   0        0        0    12841 2021-03-11 02:10:43.599155 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5486 2021-03-11 02:10:43.599393 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py
+-rw-r--r--   0        0        0     6579 2021-03-11 02:10:43.599623 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py
+-rw-r--r--   0        0        0    30489 2021-03-11 02:10:43.599890 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py
+-rw-r--r--   0        0        0     5382 2021-03-11 02:10:43.600127 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py
+-rw-r--r--   0        0        0    23918 2021-03-11 02:10:43.600385 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py
+-rw-r--r--   0        0        0     9393 2021-03-11 02:10:43.600648 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py
+-rw-r--r--   0        0        0     3900 2021-03-11 02:10:43.600866 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6204 2021-03-11 02:10:43.601082 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py
+-rw-r--r--   0        0        0     3859 2021-03-11 02:10:43.601322 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5330 2021-03-11 02:10:43.601536 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py
+-rw-r--r--   0        0        0    20956 2021-03-11 02:10:43.601863 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py
+-rw-r--r--   0        0        0     7887 2021-03-11 02:10:43.602261 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.602506 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/__init__.py
+-rw-r--r--   0        0        0     3978 2021-03-11 02:10:43.602726 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2.py
+-rw-r--r--   0        0        0     7210 2021-03-11 02:10:43.602954 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9735 2021-03-11 02:10:43.603316 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py
+-rw-r--r--   0        0        0     5342 2021-03-11 02:10:43.603562 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5923 2021-03-11 02:10:43.603904 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/trace_context_pb2.py
+-rw-r--r--   0        0        0     9384 2021-03-11 02:10:43.604199 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py
+-rw-r--r--   0        0        0    20415 2021-03-11 02:10:43.604532 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py
+-rw-r--r--   0        0        0    32470 2021-03-11 02:10:43.604866 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py
+-rw-r--r--   0        0        0    19448 2021-03-11 02:10:43.605156 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py
+-rw-r--r--   0        0        0    39736 2021-03-11 02:10:43.605486 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py
+-rw-r--r--   0        0        0     5694 2021-03-11 02:10:43.605797 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py
+-rw-r--r--   0        0        0     3208 2021-03-11 02:10:43.606037 dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.606585 dazl-8.0.0a3/dazl/_gen/google/__init__.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.606931 dazl-8.0.0a3/dazl/_gen/google/rpc/__init__.py
+-rw-r--r--   0        0        0     4127 2021-03-11 02:10:43.608818 dazl-8.0.0a3/dazl/_gen/google/rpc/status_pb2.py
+-rw-r--r--   0        0        0     5218 2021-03-11 02:10:43.609019 dazl-8.0.0a3/dazl/_logging.py
+-rw-r--r--   0        0        0     1759 2021-03-11 02:10:43.804731 dazl-8.0.0a3/dazl/cli/__init__.py
+-rw-r--r--   0        0        0      566 2021-03-11 02:10:43.611554 dazl-8.0.0a3/dazl/cli/_base.py
+-rw-r--r--   0        0        0     2069 2021-03-11 02:10:43.611895 dazl-8.0.0a3/dazl/cli/ls.py
+-rw-r--r--   0        0        0     3384 2021-03-11 02:10:43.805003 dazl-8.0.0a3/dazl/cli/metadata.py
+-rw-r--r--   0        0        0     3191 2021-03-11 02:10:43.805431 dazl-8.0.0a3/dazl/cli/tail.py
+-rw-r--r--   0        0        0     1197 2021-03-11 02:10:43.613293 dazl-8.0.0a3/dazl/cli/upload.py
+-rw-r--r--   0        0        0      454 2021-03-11 02:10:43.613720 dazl-8.0.0a3/dazl/cli/version.py
+-rw-r--r--   0        0        0     1000 2021-03-11 02:10:43.614163 dazl-8.0.0a3/dazl/client/__init__.py
+-rw-r--r--   0        0        0     1294 2021-03-18 14:00:20.335218 dazl-8.0.0a3/dazl/client/_base_model.py
+-rw-r--r--   0        0        0     3484 2021-03-11 02:10:43.805746 dazl-8.0.0a3/dazl/client/_conn_settings.py
+-rw-r--r--   0        0        0     1383 2021-03-18 14:00:20.335915 dazl-8.0.0a3/dazl/client/_events.py
+-rw-r--r--   0        0        0    22467 2021-03-18 14:00:20.336720 dazl-8.0.0a3/dazl/client/_network_client_impl.py
+-rw-r--r--   0        0        0    27609 2021-03-18 14:00:20.337763 dazl-8.0.0a3/dazl/client/_party_client_impl.py
+-rw-r--r--   0        0        0     4759 2021-03-11 02:10:43.807637 dazl-8.0.0a3/dazl/client/_reader_sync.py
+-rw-r--r--   0        0        0      810 2021-03-11 02:10:43.807983 dazl-8.0.0a3/dazl/client/_run_level.py
+-rw-r--r--   0        0        0     2623 2021-03-18 14:00:20.338118 dazl-8.0.0a3/dazl/client/_writer_verify.py
+-rw-r--r--   0        0        0    68829 2021-03-18 14:00:20.338762 dazl-8.0.0a3/dazl/client/api.py
+-rw-r--r--   0        0        0    19473 2021-03-18 14:00:20.339368 dazl-8.0.0a3/dazl/client/bots.py
+-rw-r--r--   0        0        0    19358 2021-03-18 14:00:20.339593 dazl-8.0.0a3/dazl/client/commands.py
+-rw-r--r--   0        0        0    17485 2021-03-11 02:10:43.810153 dazl-8.0.0a3/dazl/client/config.py
+-rw-r--r--   0        0        0     1288 2021-03-11 02:10:43.810302 dazl-8.0.0a3/dazl/client/errors.py
+-rw-r--r--   0        0        0     7252 2021-03-23 16:10:00.887261 dazl-8.0.0a3/dazl/client/events.py
+-rw-r--r--   0        0        0      938 2021-03-18 14:00:20.340111 dazl-8.0.0a3/dazl/client/ledger.py
+-rw-r--r--   0        0        0      387 2021-03-18 14:00:20.340427 dazl-8.0.0a3/dazl/client/pkg_loader.py
+-rw-r--r--   0        0        0      916 2021-03-11 02:10:43.621794 dazl-8.0.0a3/dazl/client/runner.py
+-rw-r--r--   0        0        0     8648 2021-03-18 14:00:20.340815 dazl-8.0.0a3/dazl/client/state.py
+-rw-r--r--   0        0        0     1477 2021-03-11 02:10:43.622839 dazl-8.0.0a3/dazl/damlast/__init__.py
+-rw-r--r--   0        0        0      404 2021-03-11 02:10:43.623392 dazl-8.0.0a3/dazl/damlast/_base.py
+-rw-r--r--   0        0        0     2776 2021-03-11 02:10:43.812202 dazl-8.0.0a3/dazl/damlast/_builtins_meta.py
+-rw-r--r--   0        0        0     2052 2021-03-11 02:10:43.625248 dazl-8.0.0a3/dazl/damlast/builtins.py
+-rw-r--r--   0        0        0    67449 2021-03-11 02:10:43.626282 dazl-8.0.0a3/dazl/damlast/daml_lf_1.py
+-rw-r--r--   0        0        0     6256 2021-03-11 02:10:43.626819 dazl-8.0.0a3/dazl/damlast/daml_types.py
+-rw-r--r--   0        0        0     1359 2021-03-11 02:10:43.812517 dazl-8.0.0a3/dazl/damlast/errors.py
+-rw-r--r--   0        0        0    12487 2021-03-11 02:10:43.628084 dazl-8.0.0a3/dazl/damlast/expand.py
+-rw-r--r--   0        0        0    17080 2021-03-23 16:10:00.888663 dazl-8.0.0a3/dazl/damlast/lookup.py
+-rw-r--r--   0        0        0     2858 2021-03-11 02:10:43.628616 dazl-8.0.0a3/dazl/damlast/parse.py
+-rw-r--r--   0        0        0    30162 2021-03-11 02:10:43.629545 dazl-8.0.0a3/dazl/damlast/pb_parse.py
+-rw-r--r--   0        0        0     8021 2021-03-18 14:00:20.342216 dazl-8.0.0a3/dazl/damlast/pkgfile.py
+-rw-r--r--   0        0        0     4819 2021-03-18 14:00:20.343284 dazl-8.0.0a3/dazl/damlast/protocols.py
+-rw-r--r--   0        0        0     2744 2021-03-11 02:10:43.813241 dazl-8.0.0a3/dazl/damlast/types.py
+-rw-r--r--   0        0        0     4654 2021-03-11 02:10:43.813599 dazl-8.0.0a3/dazl/damlast/util.py
+-rw-r--r--   0        0        0    13881 2021-03-11 02:10:43.631873 dazl-8.0.0a3/dazl/damlast/visitor.py
+-rw-r--r--   0        0        0    19958 2021-03-18 14:00:20.343551 dazl-8.0.0a3/dazl/ledger/__init__.py
+-rw-r--r--   0        0        0     2054 2021-03-23 16:10:00.888971 dazl-8.0.0a3/dazl/ledger/_offsets.py
+-rw-r--r--   0        0        0    15742 2021-03-19 15:12:46.013185 dazl-8.0.0a3/dazl/ledger/api_types.py
+-rw-r--r--   0        0        0    16361 2021-03-18 14:00:20.344088 dazl-8.0.0a3/dazl/ledger/config/__init__.py
+-rw-r--r--   0        0        0    15856 2021-03-18 14:00:20.344264 dazl-8.0.0a3/dazl/ledger/config/access.py
+-rw-r--r--   0        0        0    13799 2021-03-18 14:00:20.344427 dazl-8.0.0a3/dazl/ledger/config/argv.py
+-rw-r--r--   0        0        0      126 2021-03-18 14:00:20.344719 dazl-8.0.0a3/dazl/ledger/config/exc.py
+-rw-r--r--   0        0        0     2626 2021-03-18 14:00:20.344857 dazl-8.0.0a3/dazl/ledger/config/ssl.py
+-rw-r--r--   0        0        0     8882 2021-03-18 14:00:20.345010 dazl-8.0.0a3/dazl/ledger/config/url.py
+-rw-r--r--   0        0        0      773 2021-03-18 14:00:20.345126 dazl-8.0.0a3/dazl/ledger/errors.py
+-rw-r--r--   0        0        0     1390 2021-03-18 14:00:20.345814 dazl-8.0.0a3/dazl/ledger/grpc/__init__.py
+-rw-r--r--   0        0        0     1878 2021-03-18 14:00:20.345950 dazl-8.0.0a3/dazl/ledger/grpc/channel.py
+-rw-r--r--   0        0        0    14080 2021-03-18 14:00:20.346393 dazl-8.0.0a3/dazl/ledger/grpc/codec_aio.py
+-rw-r--r--   0        0        0    23545 2021-03-23 16:10:05.780170 dazl-8.0.0a3/dazl/ledger/grpc/conn_aio.py
+-rw-r--r--   0        0        0      277 2021-03-18 14:00:20.347073 dazl-8.0.0a3/dazl/ledger/pkgcache.py
+-rw-r--r--   0        0        0     8693 2021-03-18 14:00:20.347267 dazl-8.0.0a3/dazl/ledger/pkgloader_aio.py
+-rw-r--r--   0        0        0     2891 2021-03-18 14:00:20.347407 dazl-8.0.0a3/dazl/ledger/pkgloader_aio_compat.py
+-rw-r--r--   0        0        0     4798 2021-03-23 16:10:00.890531 dazl-8.0.0a3/dazl/ledger/stream_aio.py
+-rw-r--r--   0        0        0     3680 2021-03-19 15:12:46.015712 dazl-8.0.0a3/dazl/ledger/stream_aio.pyi
+-rw-r--r--   0        0        0      162 2021-03-19 15:12:46.016189 dazl-8.0.0a3/dazl/ledgerutil/__init__.py
+-rw-r--r--   0        0        0    16887 2021-03-23 16:10:05.781084 dazl-8.0.0a3/dazl/ledgerutil/acs.py
+-rw-r--r--   0        0        0      172 2021-03-11 02:10:43.633749 dazl-8.0.0a3/dazl/metrics/__init__.py
+-rw-r--r--   0        0        0      955 2021-03-11 02:10:43.814000 dazl-8.0.0a3/dazl/metrics/api.py
+-rw-r--r--   0        0        0     1578 2021-03-11 02:10:43.635018 dazl-8.0.0a3/dazl/metrics/instrumenters.py
+-rw-r--r--   0        0        0     1557 2021-03-11 02:10:43.814282 dazl-8.0.0a3/dazl/metrics/prometheus.py
+-rw-r--r--   0        0        0      882 2021-03-11 02:10:43.814685 dazl-8.0.0a3/dazl/model/__init__.py
+-rw-r--r--   0        0        0     2043 2021-03-11 02:10:43.815212 dazl-8.0.0a3/dazl/model/core.py
+-rw-r--r--   0        0        0      281 2021-03-11 02:10:43.815669 dazl-8.0.0a3/dazl/model/ledger.py
+-rw-r--r--   0        0        0      422 2021-03-23 16:10:00.891269 dazl-8.0.0a3/dazl/model/lookup.py
+-rw-r--r--   0        0        0      439 2021-03-11 02:10:43.816500 dazl-8.0.0a3/dazl/model/network.py
+-rw-r--r--   0        0        0     1177 2021-03-11 02:10:43.816927 dazl-8.0.0a3/dazl/model/reading.py
+-rw-r--r--   0        0        0     1176 2021-03-18 14:00:20.348095 dazl-8.0.0a3/dazl/model/writing.py
+-rw-r--r--   0        0        0     1558 2021-03-11 02:10:43.817653 dazl-8.0.0a3/dazl/pretty/__init__.py
+-rw-r--r--   0        0        0     5549 2021-03-11 02:10:43.817968 dazl-8.0.0a3/dazl/pretty/_module_builder.py
+-rw-r--r--   0        0        0    33366 2021-03-11 02:10:43.818474 dazl-8.0.0a3/dazl/pretty/_render_base.py
+-rw-r--r--   0        0        0      953 2021-03-11 02:10:43.644693 dazl-8.0.0a3/dazl/pretty/options.py
+-rw-r--r--   0        0        0      842 2021-03-11 02:10:43.645308 dazl-8.0.0a3/dazl/pretty/pygments_daml_lexer.py
+-rw-r--r--   0        0        0    16881 2021-03-11 02:10:43.818929 dazl-8.0.0a3/dazl/pretty/render_csharp.py
+-rw-r--r--   0        0        0     1756 2021-03-11 02:10:43.819309 dazl-8.0.0a3/dazl/pretty/render_csv.py
+-rw-r--r--   0        0        0    16122 2021-03-11 02:10:43.819695 dazl-8.0.0a3/dazl/pretty/render_daml.py
+-rw-r--r--   0        0        0    14612 2021-03-11 02:10:43.820106 dazl-8.0.0a3/dazl/pretty/render_python.py
+-rw-r--r--   0        0        0      216 2021-03-11 02:10:43.648874 dazl-8.0.0a3/dazl/pretty/table/__init__.py
+-rw-r--r--   0        0        0      697 2021-03-11 02:10:43.649075 dazl-8.0.0a3/dazl/pretty/table/fmt_base.py
+-rw-r--r--   0        0        0     1627 2021-03-11 02:10:43.649433 dazl-8.0.0a3/dazl/pretty/table/fmt_json.py
+-rw-r--r--   0        0        0     5341 2021-03-11 02:10:43.649643 dazl-8.0.0a3/dazl/pretty/table/fmt_pretty.py
+-rw-r--r--   0        0        0     3087 2021-03-11 02:10:43.649898 dazl-8.0.0a3/dazl/pretty/table/model.py
+-rw-r--r--   0        0        0     1517 2021-03-11 02:10:43.650204 dazl-8.0.0a3/dazl/pretty/table/write.py
+-rw-r--r--   0        0        0     3284 2021-03-11 02:10:43.650799 dazl-8.0.0a3/dazl/pretty/util.py
+-rw-r--r--   0        0        0      991 2021-03-18 14:00:20.348860 dazl-8.0.0a3/dazl/prim/__init__.py
+-rw-r--r--   0        0        0     1562 2021-03-18 14:00:20.349446 dazl-8.0.0a3/dazl/prim/basic.py
+-rw-r--r--   0        0        0     1581 2021-03-11 02:10:43.651451 dazl-8.0.0a3/dazl/prim/complex.py
+-rw-r--r--   0        0        0     2102 2021-03-11 02:10:43.651656 dazl-8.0.0a3/dazl/prim/contracts.py
+-rw-r--r--   0        0        0     6875 2021-03-11 02:10:43.651973 dazl-8.0.0a3/dazl/prim/datetime.py
+-rw-r--r--   0        0        0     1119 2021-03-11 02:10:43.820552 dazl-8.0.0a3/dazl/prim/errors.py
+-rw-r--r--   0        0        0     1394 2021-03-11 02:10:43.652145 dazl-8.0.0a3/dazl/prim/json.py
+-rw-r--r--   0        0        0     1362 2021-03-11 02:10:43.652362 dazl-8.0.0a3/dazl/prim/map.py
+-rw-r--r--   0        0        0     1285 2021-03-11 02:10:43.652623 dazl-8.0.0a3/dazl/prim/numbers.py
+-rw-r--r--   0        0        0      330 2021-03-11 02:10:43.652792 dazl-8.0.0a3/dazl/prim/party.py
+-rw-r--r--   0        0        0      369 2021-03-11 02:10:43.653218 dazl-8.0.0a3/dazl/protocols/__init__.py
+-rw-r--r--   0        0        0     5144 2021-03-18 14:00:20.350461 dazl-8.0.0a3/dazl/protocols/_base.py
+-rw-r--r--   0        0        0     8460 2021-03-18 14:00:20.351109 dazl-8.0.0a3/dazl/protocols/autodetect.py
+-rw-r--r--   0        0        0     2941 2021-03-18 14:00:20.351599 dazl-8.0.0a3/dazl/protocols/core.py
+-rw-r--r--   0        0        0      884 2021-03-18 14:00:20.352124 dazl-8.0.0a3/dazl/protocols/errors.py
+-rw-r--r--   0        0        0     6750 2021-03-11 02:10:43.822145 dazl-8.0.0a3/dazl/protocols/events.py
+-rw-r--r--   0        0        0     2160 2021-03-11 02:10:43.822547 dazl-8.0.0a3/dazl/protocols/oauth.py
+-rw-r--r--   0        0        0     4490 2021-03-18 14:00:20.352273 dazl-8.0.0a3/dazl/protocols/serializers.py
+-rw-r--r--   0        0        0      141 2021-03-11 02:10:43.656066 dazl-8.0.0a3/dazl/protocols/v1/__init__.py
+-rw-r--r--   0        0        0    13875 2021-03-18 14:00:20.353075 dazl-8.0.0a3/dazl/protocols/v1/grpc.py
+-rw-r--r--   0        0        0     2578 2021-03-11 02:10:43.657362 dazl-8.0.0a3/dazl/protocols/v1/model/__init__.py
+-rw-r--r--   0        0        0    16616 2021-03-18 14:00:20.353739 dazl-8.0.0a3/dazl/protocols/v1/pb_parse_event.py
+-rw-r--r--   0        0        0     4532 2021-03-18 14:00:20.354336 dazl-8.0.0a3/dazl/protocols/v1/pb_ser_command.py
+-rw-r--r--   0        0        0      194 2021-03-11 02:10:43.659880 dazl-8.0.0a3/dazl/py.typed
+-rw-r--r--   0        0        0      277 2021-03-18 14:00:20.354709 dazl-8.0.0a3/dazl/query/__init__.py
+-rw-r--r--   0        0        0     1479 2021-03-18 14:00:20.355076 dazl-8.0.0a3/dazl/query/query.py
+-rw-r--r--   0        0        0      234 2021-03-11 02:10:43.660160 dazl-8.0.0a3/dazl/scheduler/__init__.py
+-rw-r--r--   0        0        0     1284 2021-03-11 02:10:43.660300 dazl-8.0.0a3/dazl/scheduler/_base.py
+-rw-r--r--   0        0        0     4816 2021-03-11 02:10:43.660474 dazl-8.0.0a3/dazl/scheduler/_invoker.py
+-rw-r--r--   0        0        0     2030 2021-03-11 02:10:43.660613 dazl-8.0.0a3/dazl/scheduler/_invoker.pyi
+-rw-r--r--   0        0        0      539 2021-03-11 02:10:43.661188 dazl-8.0.0a3/dazl/server/__init__.py
+-rw-r--r--   0        0        0     3175 2021-03-11 02:10:43.824657 dazl-8.0.0a3/dazl/server/management.py
+-rw-r--r--   0        0        0     1678 2021-03-11 02:10:43.662514 dazl-8.0.0a3/dazl/server/metrics.py
+-rw-r--r--   0        0        0      376 2021-03-11 02:10:43.824944 dazl-8.0.0a3/dazl/util/__init__.py
+-rw-r--r--   0        0        0    23710 2021-03-11 02:10:43.664455 dazl-8.0.0a3/dazl/util/asyncio_util.py
+-rw-r--r--   0        0        0     4687 2021-03-11 02:10:43.825255 dazl-8.0.0a3/dazl/util/config_meta.py
+-rw-r--r--   0        0        0      928 2021-03-11 02:10:43.667126 dazl-8.0.0a3/dazl/util/enum.py
+-rw-r--r--   0        0        0     2631 2021-03-11 02:10:43.667679 dazl-8.0.0a3/dazl/util/io.py
+-rw-r--r--   0        0        0      785 2021-03-11 02:10:43.668185 dazl-8.0.0a3/dazl/util/logging.py
+-rw-r--r--   0        0        0     1188 2021-03-11 02:10:43.668878 dazl-8.0.0a3/dazl/util/notifications.py
+-rw-r--r--   0        0        0      568 2021-03-11 02:10:43.669444 dazl-8.0.0a3/dazl/util/path_util.py
+-rw-r--r--   0        0        0     2510 2021-03-11 02:10:43.670127 dazl-8.0.0a3/dazl/util/prim_natural.py
+-rw-r--r--   0        0        0     3390 2021-03-11 02:10:43.825542 dazl-8.0.0a3/dazl/util/proc_util.py
+-rw-r--r--   0        0        0     1316 2021-03-11 02:10:43.671521 dazl-8.0.0a3/dazl/util/termcap.py
+-rw-r--r--   0        0        0     3814 2021-03-11 02:10:43.672144 dazl-8.0.0a3/dazl/util/tools.py
+-rw-r--r--   0        0        0     2820 2021-03-11 02:10:43.672720 dazl-8.0.0a3/dazl/util/typing.py
+-rw-r--r--   0        0        0      576 2021-03-11 02:10:43.672860 dazl-8.0.0a3/dazl/values/__init__.py
+-rw-r--r--   0        0        0     6214 2021-03-11 02:10:43.673001 dazl-8.0.0a3/dazl/values/canonical.py
+-rw-r--r--   0        0        0    14279 2021-03-11 02:10:43.825988 dazl-8.0.0a3/dazl/values/context.py
+-rw-r--r--   0        0        0     1840 2021-03-11 02:10:43.673422 dazl-8.0.0a3/dazl/values/json.py
+-rw-r--r--   0        0        0     3468 2021-03-18 14:00:20.356349 dazl-8.0.0a3/dazl/values/mapper.py
+-rw-r--r--   0        0        0     9821 2021-03-11 02:10:43.674131 dazl-8.0.0a3/dazl/values/protobuf.py
+-rw-r--r--   0        0        0     2837 2021-03-11 02:10:43.674352 dazl-8.0.0a3/dazl/values/pysample_encoder.py
+-rw-r--r--   0        0        0     5092 2021-03-11 02:10:43.674578 dazl-8.0.0a3/dazl/values/string.py
+-rw-r--r--   0        0        0     1625 2021-03-23 16:10:05.781725 dazl-8.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4518 2021-03-23 16:12:15.816663 dazl-8.0.0a3/setup.py
+-rw-r--r--   0        0        0     3824 2021-03-23 16:12:15.817089 dazl-8.0.0a3/PKG-INFO
```

### Comparing `dazl-8.0.0a2/README.md` & `dazl-8.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/__init__.py` & `dazl-8.0.0a3/dazl/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/daml_lf_0_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/daml_lf_0_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/daml_lf_1_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/daml_lf_1_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/daml_lf_dev/daml_lf_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/daml_lf_dev/daml_lf_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/active_contracts_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/config_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/package_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/participant_pruning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/admin/party_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_completion_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/command_submission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/commands_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/completion_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_configuration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_identity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/ledger_offset_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/package_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/reset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/testing/time_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/trace_context_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/trace_context_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/transaction_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py` & `dazl-8.0.0a3/dazl/_gen/com/daml/ledger/api/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_gen/google/rpc/status_pb2.py` & `dazl-8.0.0a3/dazl/_gen/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/_logging.py` & `dazl-8.0.0a3/dazl/_logging.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/cli/__init__.py` & `dazl-8.0.0a3/dazl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/cli/_base.py` & `dazl-8.0.0a3/dazl/cli/_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/cli/ls.py` & `dazl-8.0.0a3/dazl/cli/ls.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/cli/metadata.py` & `dazl-8.0.0a3/dazl/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/cli/tail.py` & `dazl-8.0.0a3/dazl/cli/tail.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/cli/upload.py` & `dazl-8.0.0a3/dazl/cli/upload.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/__init__.py` & `dazl-8.0.0a3/dazl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_base_model.py` & `dazl-8.0.0a3/dazl/client/_base_model.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_conn_settings.py` & `dazl-8.0.0a3/dazl/client/_conn_settings.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_events.py` & `dazl-8.0.0a3/dazl/client/_events.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_network_client_impl.py` & `dazl-8.0.0a3/dazl/client/_network_client_impl.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_party_client_impl.py` & `dazl-8.0.0a3/dazl/client/_party_client_impl.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_reader_sync.py` & `dazl-8.0.0a3/dazl/client/_reader_sync.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_run_level.py` & `dazl-8.0.0a3/dazl/client/_run_level.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/_writer_verify.py` & `dazl-8.0.0a3/dazl/client/_writer_verify.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/api.py` & `dazl-8.0.0a3/dazl/client/api.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/bots.py` & `dazl-8.0.0a3/dazl/client/bots.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/commands.py` & `dazl-8.0.0a3/dazl/client/commands.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/config.py` & `dazl-8.0.0a3/dazl/client/config.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/errors.py` & `dazl-8.0.0a3/dazl/client/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/events.py` & `dazl-8.0.0a3/dazl/client/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # Copyright (c) 2017-2021 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
-
 from typing import Any, Callable, Collection, Iterator, TypeVar
+import warnings
 
-__all__ = ["EventKey", "template_reverse_globs"]
-
-from ..damlast.lookup import validate_template
+from ..damlast.lookup import (
+    matching_normalizations,
+    normalize,
+    parse_type_con_name,
+    validate_template,
+)
 from ..protocols.events import (
     BaseEvent,
     ContractArchiveEvent,
     ContractCreateEvent,
     ContractExercisedEvent,
     InitEvent,
     OffsetEvent,
     PackagesAddedEvent,
     ReadyEvent,
     TransactionEndEvent,
     TransactionStartEvent,
 )
 
+__all__ = ["EventKey", "template_reverse_globs"]
+
 T = TypeVar("T")
 
 
 def create_dispatch(
     on_init: "Callable[[InitEvent], T]",
     on_ready: "Callable[[ReadyEvent], T]",
     on_offset: "Callable[[OffsetEvent], T]",
@@ -58,45 +63,41 @@
     return handle
 
 
 def template_reverse_globs(primary_only: bool, package_id: str, type_name: str) -> "Iterator[str]":
     """
     Return an iterator over strings that glob to a specified type.
     """
-    package_id = package_id or "*"
-    type_name = type_name or "*"
+    warnings.warn(
+        "template_reverse_globs is deprecated; use either "
+        "dazl.damlast.lookup.matching_normalizations (for template_reverse_globs(False, ...)) or "
+        "dazl.damlast.lookup.normalize(for template_reverse_globs(True, ...)). "
+        "Note that the new functions do NOT support periods as a delimiter between "
+        "module names and entity names; you MUST use a colon.",
+        DeprecationWarning,
+    )
 
-    if package_id != "*":
-        if type_name != "*":
-            if ":" not in type_name:
-                # this is a historical use of template name here; assume the last dot was supposed
-                # to have been a colon instead
-                m, delim, e = type_name.rpartition(".")
-                if delim:
-                    yield f"{package_id}:{m}:{e}"
-                    if primary_only:
-                        return
-            yield f"{package_id}:{type_name}"
-            if primary_only:
-                return
-        if not primary_only or type_name == "*":
-            yield f"{package_id}:*"
-    if type_name != "*":
-        if ":" not in type_name:
-            # this is a historical use of template name here; assume the last dot was supposed
-            # to have been a colon instead
-            m, delim, e = type_name.rpartition(".")
-            if delim:
-                yield f"*:{m}:{e}"
-                if primary_only:
-                    return
-        yield f"*:{type_name}"
-        if primary_only:
-            return
-    yield "*:*"
+    # support deprecated type identifiers for usages of this old API to preserve backwards
+    # compatibility
+    use_deprecated_form = False
+    if type_name != "*" and ":" not in type_name:
+        m, delim, e = type_name.rpartition(".")
+        if delim:
+            use_deprecated_form = True
+            type_name = f"{m}:{e}"
+    t = f"{package_id}:{type_name}"
+
+    if primary_only:
+        yield normalize(t)
+    else:
+        for form in matching_normalizations(t):
+            yield form
+            if use_deprecated_form and len(form.split(":")) == 3:
+                s, _, e = form.rpartition(":")
+                yield f"{s}.{e}"
 
 
 class EventKey:
     from_event = create_dispatch(
         on_init=lambda _: EventKey.init(),
         on_ready=lambda _: EventKey.ready(),
         on_offset=lambda _: EventKey.offset(),
@@ -186,8 +187,10 @@
         if changed:
             keys.append("packages-added/changed")
         return tuple(keys)
 
     @staticmethod
     def _contract(primary_only: bool, prefix: str, template: "Any") -> Collection[str]:
         m, t = validate_template(template)
-        return tuple(f"{prefix}/{g}" for g in template_reverse_globs(primary_only, m, t))
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", DeprecationWarning)
+            return tuple(f"{prefix}/{g}" for g in template_reverse_globs(primary_only, m, t))
```

### Comparing `dazl-8.0.0a2/dazl/client/ledger.py` & `dazl-8.0.0a3/dazl/client/ledger.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/runner.py` & `dazl-8.0.0a3/dazl/client/runner.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/client/state.py` & `dazl-8.0.0a3/dazl/client/state.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/__init__.py` & `dazl-8.0.0a3/dazl/damlast/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/_builtins_meta.py` & `dazl-8.0.0a3/dazl/damlast/_builtins_meta.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/builtins.py` & `dazl-8.0.0a3/dazl/damlast/builtins.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/daml_lf_1.py` & `dazl-8.0.0a3/dazl/damlast/daml_lf_1.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/daml_types.py` & `dazl-8.0.0a3/dazl/damlast/daml_types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/errors.py` & `dazl-8.0.0a3/dazl/damlast/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/expand.py` & `dazl-8.0.0a3/dazl/damlast/expand.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/lookup.py` & `dazl-8.0.0a3/dazl/damlast/lookup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,26 @@
 # The code in here is fairly monotonous and boilerplate heavy. However, being too creative here can
 # potentially lead to performance degradations, particularly at application startup where type and
 # template lookups by name are very frequent. Please be conscious of the runtime costs of
 # modifications in this file!
 
 import threading
 from types import MappingProxyType
-from typing import AbstractSet, Any, Collection, Dict, Iterable, NoReturn, Optional, Tuple
+from typing import (
+    AbstractSet,
+    Any,
+    Collection,
+    Dict,
+    Iterable,
+    NoReturn,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 from .daml_lf_1 import (
     Archive,
     DefDataType,
     DefTemplate,
     DefValue,
     DottedName,
@@ -30,45 +41,48 @@
     TypeConName,
     ValName,
 )
 from .errors import NameNotFoundError, PackageNotFoundError
 from .protocols import SymbolLookup
 
 __all__ = [
-    "find_choice",
-    "parse_type_con_name",
-    "validate_template",
     "EmptyLookup",
     "MultiPackageLookup",
-    "PackageLookup",
     "MultiPackageLookup",
+    "PackageLookup",
+    "find_choice",
+    "matching_normalizations",
+    "normalize",
+    "parse_type_con_name",
+    "validate_template",
 ]
 
+
 STAR = PackageRef("*")
 
 
-def parse_type_con_name(val: str) -> "TypeConName":
+def parse_type_con_name(val: str) -> TypeConName:
     """
     Parse the given string as a type constructor.
     """
     pkg, name = validate_template(val)
     module_name, _, entity_name = name.rpartition(":")
     module_ref = ModuleRef(pkg, DottedName(module_name.split(".")))
     return TypeConName(module_ref, entity_name.split("."))
 
 
-def empty_lookup_impl(ref: "Any") -> "NoReturn":
+def empty_lookup_impl(ref: Any) -> NoReturn:
     pkg, _ = validate_template(ref)
     if pkg != STAR:
         raise PackageNotFoundError(pkg)
     else:
         raise NameNotFoundError(ref)
 
 
-def validate_template(template: "Any") -> "Tuple[PackageRef, str]":
+def validate_template(template: Union[None, str, TypeConName]) -> Tuple[PackageRef, str]:
     """
     Return a module and type name component from something that can be interpreted as a template.
 
     :param template:
         Any object that can be interpreted as an identifier for a template.
     :return:
         A tuple of package ID and ``Module.Name:EntityName`` (the package-scoped identifier for the
@@ -90,25 +104,59 @@
             pkgid, m, e = components
             return pkgid, f"{m}:{e}"
 
         elif len(components) == 2:
             # one colon, so assume the package ID is unspecified UNLESS the second component is a
             # wildcard; then we assume the wildcard means any module name and entity name
             m, e = components
+            if m == STAR and e != STAR:
+                # strings that look like "*:SOMETHING" are explicitly not allowed; this is almost
+                # certainly an attempt to use periods instead of colons as a delimiter between
+                # module name and entity name
+                raise ValueError("string must be in the format PKG_REF:MOD:ENTITY or MOD:ENTITY")
             return (STAR, f"{m}:{e}") if e != "*" else (PackageRef(m), "*")
 
         else:
             raise ValueError("string must be in the format PKG_REF:MOD:ENTITY or MOD:ENTITY")
 
     if isinstance(template, TypeConName):
         return package_ref(template), package_local_name(template)
     else:
         raise ValueError(f"Don't know how to convert {template!r} into a template")
 
 
+def normalize(name: Union[None, str, TypeConName], /) -> str:
+    """
+    Return the canonical form for a string that represents a template ID or partial match of a
+    template ID.
+
+    Concretely, this function converts ``"MyMod:MyTemplate"`` to ``"*:MyMod:MyTemplate"`` and leaves
+    most other strings unchanged.
+
+    :param name:
+        A template ID, expressed in either string form or as an instance of :class:`TypeConName`.
+    :return:
+        A string in canonical form (either ``PACKAGE_REF:MODULE_NAME:ENTITY_NAME`` or
+        ``PACKAGE_REF:*``, where ``PACKAGE_REF`` is also allowed to be ``*``).
+    """
+    p, m = validate_template(name)
+    return f"{p}:{m}"
+
+
+def matching_normalizations(name: Union[str, TypeConName], /) -> Sequence[str]:
+    """
+    Return strings that are possible matches for the given template ID.
+    """
+    p, m = validate_template(name)
+
+    # throw away duplicates that arise from `name` not being fully specified (p and/or m are
+    # allowed to be asterisks too)
+    return list(dict.fromkeys([f"{p}:{m}", f"{p}:*", f"*:{m}", "*:*"]))
+
+
 class EmptyLookup(SymbolLookup):
     """
     A :class:`SymbolLookup` that trivially throws for all of its functions.
 
     This can be used where a :class:`SymbolLookup` instance is useful but an implementation is not
     required.
```

### Comparing `dazl-8.0.0a2/dazl/damlast/parse.py` & `dazl-8.0.0a3/dazl/damlast/parse.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/pb_parse.py` & `dazl-8.0.0a3/dazl/damlast/pb_parse.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/pkgfile.py` & `dazl-8.0.0a3/dazl/damlast/pkgfile.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/protocols.py` & `dazl-8.0.0a3/dazl/damlast/protocols.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/types.py` & `dazl-8.0.0a3/dazl/damlast/types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/util.py` & `dazl-8.0.0a3/dazl/damlast/util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/damlast/visitor.py` & `dazl-8.0.0a3/dazl/damlast/visitor.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/__init__.py` & `dazl-8.0.0a3/dazl/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/api_types.py` & `dazl-8.0.0a3/dazl/ledger/api_types.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/config/__init__.py` & `dazl-8.0.0a3/dazl/ledger/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/config/access.py` & `dazl-8.0.0a3/dazl/ledger/config/access.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/config/argv.py` & `dazl-8.0.0a3/dazl/ledger/config/argv.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/config/ssl.py` & `dazl-8.0.0a3/dazl/ledger/config/ssl.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/config/url.py` & `dazl-8.0.0a3/dazl/ledger/config/url.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/errors.py` & `dazl-8.0.0a3/dazl/ledger/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/grpc/__init__.py` & `dazl-8.0.0a3/dazl/ledger/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/grpc/channel.py` & `dazl-8.0.0a3/dazl/ledger/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/grpc/codec_aio.py` & `dazl-8.0.0a3/dazl/ledger/grpc/codec_aio.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/grpc/conn_aio.py` & `dazl-8.0.0a3/dazl/ledger/grpc/conn_aio.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from ..._gen.com.daml.ledger.api.v1.transaction_service_pb2 import (
     GetTransactionsRequest as G_GetTransactionsRequest,
 )
 from ..._gen.com.daml.ledger.api.v1.transaction_service_pb2_grpc import TransactionServiceStub
 from ...damlast.daml_lf_1 import PackageRef, TypeConName
 from ...prim import LEDGER_STRING_REGEX, ContractData, ContractId, Party
 from ...query import Query
+from .._offsets import UNTIL_END, LedgerOffsetRange, from_offset_until_forever
 from ..api_types import ArchiveEvent, Boundary, Command, CreateEvent, ExerciseResponse, PartyInfo
 from ..config import Config
 from ..config.access import PropertyBasedAccessConfig
 from ..errors import ProtocolWarning
 from ..stream_aio import QueryStreamBase
 from .channel import create_channel
 from .codec_aio import Codec
@@ -319,25 +320,87 @@
             )
         )
 
     # endregion
 
     # region Read API
 
-    def query(self, template_id: str = "*", query: Query = None) -> QueryStream:
-        return QueryStream(self, {template_id: query}, False)
+    def query(self, template_id: str = "*", query: Query = None, /) -> QueryStream:
+        """
+        Return the create events from the active contract set service as a stream.
+
+        If you find yourself repeatedly calling :meth:`query` or :meth:`query_many` over the same
+        set of templates, you may want to consider :class:`ACS` instead, which is a utility class
+        that helps you maintain a "live" state of the ACS.
+
+        :param template_id:
+            The name of the template for which to fetch contracts.
+        :param query:
+            A filter to apply to the set of returned contracts.
+        """
+        return QueryStream(self, {template_id: query}, UNTIL_END)
+
+    def query_many(self, queries: Optional[Mapping[str, Query]] = None, /) -> QueryStream:
+        """
+        Return the create events from the active contract set service as a stream.
+
+        If you find yourself repeatedly calling :meth:`query` or :meth:`query_many` over the same
+        set of templates, you may want to consider :class:`ACS` instead, which is a utility class
+        that helps you maintain a "live" state of the ACS.
+
+        :param queries:
+            A map of template IDs to filter to apply to the set of returned contracts.
+        """
+        return QueryStream(self, queries, UNTIL_END)
+
+    def stream(
+        self, template_id: str = "*", query: Query = None, /, *, offset: Optional[str] = None
+    ) -> QueryStream:
+        """
+        Stream create/archive events.
+
+        When ``offset`` is ``None``, create events from the active contract set are returned first,
+        followed by a continuous stream of updates (creates/archives).
+
+        Otherwise, ``offset`` can be supplied to resume a stream from a prior point where a
+        ``Boundary`` was returned from a previous stream.
+
+        :param template_id:
+            The name of the template for which to fetch contracts.
+        :param query:
+            A filter to apply to the set of returned contracts. Note that this does not filter
+            :class:`ArchiveEvent`; readers of the stream MUST be able to cope with "mismatched"
+            archives that come from the result of applying a filter.
+        :param offset:
+            An optional offset at which to start receiving events. If ``None``, start from the
+            beginning.
+        """
+        return QueryStream(self, {template_id: query}, from_offset_until_forever(offset))
+
+    def stream_many(
+        self, queries: Optional[Mapping[str, Query]] = None, /, *, offset: Optional[str] = None
+    ) -> QueryStream:
+        """
+        Stream create/archive events from more than one template ID in the same stream.
 
-    def query_many(self, queries: Optional[Mapping[str, Query]] = None) -> QueryStream:
-        return QueryStream(self, queries, False)
+        When ``offset`` is ``None``, create events from the active contract set are returned first,
+        followed by a continuous stream of updates (creates/archives).
 
-    def stream(self, template_id: str = "*", query: Query = None) -> QueryStream:
-        return QueryStream(self, {template_id: query}, True)
+        Otherwise, ``offset`` can be supplied to resume a stream from a prior point where a
+        ``Boundary`` was returned from a previous stream.
 
-    def stream_many(self, queries: Optional[Mapping[str, Query]] = None) -> QueryStream:
-        return QueryStream(self, queries, True)
+        :param queries:
+            A map of template IDs to filter to apply to the set of returned contracts. Note that
+            this does not filter :class:`ArchiveEvent`; readers of the stream MUST be able to cope
+            with "mismatched" archives that come from the result of applying a filter.
+        :param offset:
+            An optional offset at which to start receiving events. If ``None``, start from the
+            beginning.
+        """
+        return QueryStream(self, queries, from_offset_until_forever(offset))
 
     # endregion
 
     # region Party Management calls
 
     async def allocate_party(
         self, identifier_hint: str = None, display_name: str = None
@@ -383,21 +446,20 @@
 
 
 class QueryStream(QueryStreamBase):
     def __init__(
         self,
         conn: Connection,
         queries: Optional[Mapping[str, Query]],
-        continue_stream: bool,
+        offset_range: LedgerOffsetRange,
     ):
         self.conn = conn
         self._queries = queries
-        self._continue_stream = continue_stream
+        self._offset_range = offset_range
 
-        self._offset = None
         self._filter = None
         self._response_stream = None
 
     async def close(self) -> None:
         if self._response_stream is not None:
             self._response_stream.cancel()
             self._response_stream = None
@@ -417,44 +479,61 @@
         :return:
             A stream of responses, where each response contains one or more events at a particular
             offset.
 
             At least one initial :class:`Boundary` is always returned, even if the stream is empty.
             In this case, the first returned object is a :class:`Boundary` with ``offset=None``.
         """
+        log = self.conn.config.logger
+
         filters = await self.conn.codec.encode_filters(self._queries)
         filters_by_party = {party: filters for party in self.conn.config.access.read_as}
         tx_filter_pb = G_TransactionFilter(filters_by_party=filters_by_party)
 
         try:
             offset = None
-            async for event in self._acs_events(tx_filter_pb):
-                if isinstance(event, CreateEvent):
-                    await self._emit_create(event)
-                elif isinstance(event, Boundary):
-                    offset = event.offset
-                    await self._emit_boundary(event)
-                else:
-                    warnings.warn(f"Received an unknown event: {event}", ProtocolWarning)
-                yield event
+            if self._offset_range.begin is None:
+                # when starting from the beginning of the ledger, the Active Contract Set service
+                # lets us catch up more quickly than having to parse every create/archive event
+                # ourselves
+                log.debug("Reading from the ACS...")
+                async for event in self._acs_events(tx_filter_pb):
+                    if isinstance(event, CreateEvent):
+                        await self._emit_create(event)
+                    elif isinstance(event, Boundary):
+                        offset = event.offset
+                        await self._emit_boundary(event)
+                    else:
+                        warnings.warn(f"Received an unknown event: {event}", ProtocolWarning)
+                    yield event
+            else:
+                log.debug(
+                    "Skipped reading from the ACS because begin offset is %r",
+                    self._offset_range.begin,
+                )
 
-            if self._continue_stream:
+            if self._offset_range != UNTIL_END:
                 # now start returning events as they come off the transaction stream; note this
                 # stream will never naturally close, so it's on the caller to call close() or to
                 # otherwise exit our current context
+                log.debug("Reading a transaction stream: %s", self._offset_range)
                 async for event in self._tx_events(tx_filter_pb, offset):
                     if isinstance(event, CreateEvent):
                         await self._emit_create(event)
                     elif isinstance(event, ArchiveEvent):
                         await self._emit_archive(event)
                     elif isinstance(event, Boundary):
                         await self._emit_boundary(event)
                     else:
                         warnings.warn(f"Received an unknown event: {event}", ProtocolWarning)
                     yield event
+            else:
+                log.debug(
+                    "Not reading from transaction stream because we were only asked for a snapshot."
+                )
         finally:
             await self.close()
 
     async def _acs_events(
         self, filter_pb: G_TransactionFilter
     ) -> AsyncIterable[Union[CreateEvent, Boundary]]:
         stub = ActiveContractsServiceStub(self.conn.channel)
```

### Comparing `dazl-8.0.0a2/dazl/ledger/pkgloader_aio.py` & `dazl-8.0.0a3/dazl/ledger/pkgloader_aio.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/pkgloader_aio_compat.py` & `dazl-8.0.0a3/dazl/ledger/pkgloader_aio_compat.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/ledger/stream_aio.py` & `dazl-8.0.0a3/dazl/ledger/stream_aio.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from collections import defaultdict
 from inspect import iscoroutine
 from typing import Any, Callable, TypeVar, Union
 import warnings
 
-from ..client.events import template_reverse_globs
 from ..damlast.daml_lf_1 import TypeConName
 from .api_types import ArchiveEvent, Boundary, CreateEvent, Event
 from .errors import CallbackReturnWarning
 
 __all__ = ["QueryStreamBase"]
 
-from ..damlast.lookup import validate_template
+from ..damlast.lookup import matching_normalizations, normalize
 
 CREATE_EVENT = "create"
 ARCHIVE_EVENT = "archive"
 BOUNDARY = "boundary"
 
 E = TypeVar("E", bound=Event)
 
@@ -135,32 +134,18 @@
 
 def _register(
     q: QueryStreamBase,
     name: str,
     template_id: Union[None, str, TypeConName],
     fn: Callable[[E], None],
 ) -> Callable[[E], None]:
-    template_search = (
-        next(template_reverse_globs(True, *validate_template(template_id)))
-        if template_id is not None
-        else None
-    )
-    if template_search == "*:*":
-        template_search = None
+    template_search = normalize(template_id)
 
     def handler(event: E):
-        if template_search is not None:
-            for match in template_reverse_globs(
-                False, *validate_template(event.contract_id.value_type)
-            ):
-                if template_search == match:
-                    fn(event)
-                    return
-            return
-        else:
+        if template_search in matching_normalizations(event.contract_id.value_type):
             fn(event)
 
     # noinspection PyProtectedMember
     q._callbacks[name].append(handler)
     return fn
```

### Comparing `dazl-8.0.0a2/dazl/ledger/stream_aio.pyi` & `dazl-8.0.0a3/dazl/ledger/stream_aio.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/metrics/api.py` & `dazl-8.0.0a3/dazl/metrics/api.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/metrics/instrumenters.py` & `dazl-8.0.0a3/dazl/metrics/instrumenters.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/metrics/prometheus.py` & `dazl-8.0.0a3/dazl/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/model/__init__.py` & `dazl-8.0.0a3/dazl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/model/core.py` & `dazl-8.0.0a3/dazl/model/core.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/model/reading.py` & `dazl-8.0.0a3/dazl/model/reading.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/model/writing.py` & `dazl-8.0.0a3/dazl/model/writing.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/__init__.py` & `dazl-8.0.0a3/dazl/pretty/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/_module_builder.py` & `dazl-8.0.0a3/dazl/pretty/_module_builder.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/_render_base.py` & `dazl-8.0.0a3/dazl/pretty/_render_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/options.py` & `dazl-8.0.0a3/dazl/pretty/options.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/pygments_daml_lexer.py` & `dazl-8.0.0a3/dazl/pretty/pygments_daml_lexer.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/render_csharp.py` & `dazl-8.0.0a3/dazl/pretty/render_csharp.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/render_csv.py` & `dazl-8.0.0a3/dazl/pretty/render_csv.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/render_daml.py` & `dazl-8.0.0a3/dazl/pretty/render_daml.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/render_python.py` & `dazl-8.0.0a3/dazl/pretty/render_python.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/table/fmt_base.py` & `dazl-8.0.0a3/dazl/pretty/table/fmt_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/table/fmt_json.py` & `dazl-8.0.0a3/dazl/pretty/table/fmt_json.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/table/fmt_pretty.py` & `dazl-8.0.0a3/dazl/pretty/table/fmt_pretty.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/table/model.py` & `dazl-8.0.0a3/dazl/pretty/table/model.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/table/write.py` & `dazl-8.0.0a3/dazl/pretty/table/write.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/pretty/util.py` & `dazl-8.0.0a3/dazl/pretty/util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/__init__.py` & `dazl-8.0.0a3/dazl/prim/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/basic.py` & `dazl-8.0.0a3/dazl/prim/basic.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/complex.py` & `dazl-8.0.0a3/dazl/prim/complex.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/contracts.py` & `dazl-8.0.0a3/dazl/prim/contracts.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/datetime.py` & `dazl-8.0.0a3/dazl/prim/datetime.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/errors.py` & `dazl-8.0.0a3/dazl/prim/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/json.py` & `dazl-8.0.0a3/dazl/prim/json.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/map.py` & `dazl-8.0.0a3/dazl/prim/map.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/prim/numbers.py` & `dazl-8.0.0a3/dazl/prim/numbers.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/_base.py` & `dazl-8.0.0a3/dazl/protocols/_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/autodetect.py` & `dazl-8.0.0a3/dazl/protocols/autodetect.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/core.py` & `dazl-8.0.0a3/dazl/protocols/core.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/errors.py` & `dazl-8.0.0a3/dazl/protocols/errors.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/events.py` & `dazl-8.0.0a3/dazl/protocols/events.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/oauth.py` & `dazl-8.0.0a3/dazl/protocols/oauth.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/serializers.py` & `dazl-8.0.0a3/dazl/protocols/serializers.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/v1/grpc.py` & `dazl-8.0.0a3/dazl/protocols/v1/grpc.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/v1/model/__init__.py` & `dazl-8.0.0a3/dazl/protocols/v1/model/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/v1/pb_parse_event.py` & `dazl-8.0.0a3/dazl/protocols/v1/pb_parse_event.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/protocols/v1/pb_ser_command.py` & `dazl-8.0.0a3/dazl/protocols/v1/pb_ser_command.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/query/query.py` & `dazl-8.0.0a3/dazl/query/query.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/scheduler/_base.py` & `dazl-8.0.0a3/dazl/scheduler/_base.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/scheduler/_invoker.py` & `dazl-8.0.0a3/dazl/scheduler/_invoker.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/scheduler/_invoker.pyi` & `dazl-8.0.0a3/dazl/scheduler/_invoker.pyi`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/server/__init__.py` & `dazl-8.0.0a3/dazl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/server/management.py` & `dazl-8.0.0a3/dazl/server/management.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/server/metrics.py` & `dazl-8.0.0a3/dazl/server/metrics.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/asyncio_util.py` & `dazl-8.0.0a3/dazl/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/config_meta.py` & `dazl-8.0.0a3/dazl/util/config_meta.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/enum.py` & `dazl-8.0.0a3/dazl/util/enum.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/io.py` & `dazl-8.0.0a3/dazl/util/io.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/logging.py` & `dazl-8.0.0a3/dazl/util/logging.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/notifications.py` & `dazl-8.0.0a3/dazl/util/notifications.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/path_util.py` & `dazl-8.0.0a3/dazl/util/path_util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/prim_natural.py` & `dazl-8.0.0a3/dazl/util/prim_natural.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/proc_util.py` & `dazl-8.0.0a3/dazl/util/proc_util.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/termcap.py` & `dazl-8.0.0a3/dazl/util/termcap.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/tools.py` & `dazl-8.0.0a3/dazl/util/tools.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/util/typing.py` & `dazl-8.0.0a3/dazl/util/typing.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/__init__.py` & `dazl-8.0.0a3/dazl/values/__init__.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/canonical.py` & `dazl-8.0.0a3/dazl/values/canonical.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/context.py` & `dazl-8.0.0a3/dazl/values/context.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/json.py` & `dazl-8.0.0a3/dazl/values/json.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/mapper.py` & `dazl-8.0.0a3/dazl/values/mapper.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/protobuf.py` & `dazl-8.0.0a3/dazl/values/protobuf.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/pysample_encoder.py` & `dazl-8.0.0a3/dazl/values/pysample_encoder.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/dazl/values/string.py` & `dazl-8.0.0a3/dazl/values/string.py`

 * *Files identical despite different names*

### Comparing `dazl-8.0.0a2/pyproject.toml` & `dazl-8.0.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2017-2021 Digital Asset (Switzerland) GmbH and/or its affiliates. All rights reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "dazl"
-version = "8.0.0a2"
+version = "8.0.0a3"
 description = "high-level Ledger API client for DAML ledgers"
 license = "Apache-2.0"
 authors = ["Davin K. Tanabe <davin.tanabe@digitalasset.com>"]
 readme = 'README.md'
 repository = "https://github.com/digital-asset/dazl-client"
 homepage = "https://github.com/digital-asset/dazl-client"
 keywords = ["daml", "blockchain", "dlt", "distributed ledger", "digital asset"]
```

### Comparing `dazl-8.0.0a2/setup.py` & `dazl-8.0.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
  'server': ['aiohttp']}
 
 entry_points = \
 {'console_scripts': ['dazl = dazl.cli:main']}
 
 setup_kwargs = {
     'name': 'dazl',
-    'version': '8.0.0a2',
+    'version': '8.0.0a3',
     'description': 'high-level Ledger API client for DAML ledgers',
     'long_description': 'dazl\n====\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/digital-asset/dazl-client/blob/master/LICENSE)\n<a href="https://circleci.com/gh/digital-asset/dazl-client">\n<img src="https://circleci.com/gh/digital-asset/dazl-client.svg?style=svg">\n</a>\n\nCopyright (c) 2017-2021 Digital Asset (Switzerland) GmbH and/or its affiliates. All Rights Reserved.\nSPDX-License-Identifier: Apache-2.0\n\n\nRich Python bindings for accessing Ledger API-based applications.\n\nDocumentation\n-------------\nThe user documentation is available online [here](https://digital-asset.github.io/dazl-client).\n\nInstallation\n------------\nIf you just want to use the library, you can install it locally with `pip`:\n```sh\npip install --user dazl\n```\n\nRequirements\n------------\n* Python 3.8+\n* GNU Make\n* [Poetry](https://python-poetry.org/) for build/dependency management\n* [DAML SDK](https://www.daml.com)\n\nExamples\n--------\n\nAll of the examples below assume you imported `dazl`, and are running a ledger with the default scenario generated with `daml new`.\n\nConnect to the ledger and submit a single command:\n\n```py\nwith dazl.simple_client(\'http://localhost:6865\', \'Alice\') as client:\n    contract = { \'issuer\' : \'Alice\', \'owner\' : \'Alice\', \'name\' : \'hello world!\' }\n    client.ready()\n    client.submit_create(\'Main.Asset\', contract)\n```\n\nConnect to the ledger as a single party, print all contracts, and close:\n\n```py\nwith dazl.simple_client(\'http://localhost:6865\', \'Alice\') as client:\n    # wait for the ACS to be fully read\n    client.ready()\n    contract_dict = client.find_active(\'*\')\nprint(contract_dict)\n```\n\nConnect to the ledger using asynchronous callbacks:\n\n```py\nfrom dazl.protocols.reading import ReadyEvent\n\nnetwork = dazl.Network()\nnetwork.set_config(url=\'http://localhost:6865\')\n\nalice = network.aio_party(\'Alice\')\n\n\n@alice.ledger_ready()\nasync def onReady(event: ReadyEvent):\n    contracts = await event.acs_find_one(\'Main.Asset\')\n    print(contracts)\n\n\nnetwork.run_until_complete()\n```\n\n\nBuilding locally\n----------------\nYou will need to have [Poetry](https://python-poetry.org) installed, and the dependencies fetched using `poetry install`. Then do:\n\n```sh\nmake build\n```\n\nIf you see errors about incompatible python versions, switch your environment to python3 using `poetry env use python3`, for instance.\n\nBuilding Documentation\n----------------------\nThe above command will build documentation in the root `docs/` dir. Committing this into source control and pushing to github will cause github-pages to be updated.\n\nTests\n-----\n\nTests in dazl are written using [pytest](https://docs.pytest.org/en/latest/). You can run them by doing:\n\n```sh\nmake test\n```\n',
     'author': 'Davin K. Tanabe',
     'author_email': 'davin.tanabe@digitalasset.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/digital-asset/dazl-client',
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 'dazl.metrics', 'dazl.model', 'dazl.pretty', 'dazl.pretty.table', 'dazl.prim',
 'dazl.protocols', 'dazl.protocols.v1', 'dazl.protocols.v1.model', 'dazl.query',
 'dazl.scheduler', 'dazl.server', 'dazl.util', 'dazl.values'] package_data = \
 {'': ['*']} install_requires = \ ['grpcio>=1.32.0', 'protobuf>=3.12.0',
 'requests', 'semver', 'toposort'] extras_require = \ {'oauth': ['google-auth',
 'oauthlib'], 'prometheus': ['prometheus_client'], 'pygments': ['pygments'],
 'server': ['aiohttp']} entry_points = \ {'console_scripts': ['dazl = dazl.cli:
-main']} setup_kwargs = { 'name': 'dazl', 'version': '8.0.0a2', 'description':
+main']} setup_kwargs = { 'name': 'dazl', 'version': '8.0.0a3', 'description':
 'high-level Ledger API client for DAML ledgers', 'long_description':
 'dazl\n====\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-
 blue.svg)](https://github.com/digital-asset/dazl-client/blob/master/
 LICENSE)\n\n[https://circleci.com/gh/digital-asset/dazl-
 client.svg?style=svg]\n\n\nCopyright (c) 2017-2021 Digital Asset (Switzerland)
 GmbH and/or its affiliates. All Rights Reserved.\nSPDX-License-Identifier:
 Apache-2.0\n\n\nRich Python bindings for accessing Ledger API-based
```

### Comparing `dazl-8.0.0a2/PKG-INFO` & `dazl-8.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dazl
-Version: 8.0.0a2
+Version: 8.0.0a3
 Summary: high-level Ledger API client for DAML ledgers
 Home-page: https://github.com/digital-asset/dazl-client
 License: Apache-2.0
 Keywords: daml,blockchain,dlt,distributed ledger,digital asset
 Author: Davin K. Tanabe
 Author-email: davin.tanabe@digitalasset.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dazl Version: 8.0.0a2 Summary: high-level Ledger
+Metadata-Version: 2.1 Name: dazl Version: 8.0.0a3 Summary: high-level Ledger
 API client for DAML ledgers Home-page: https://github.com/digital-asset/dazl-
 client License: Apache-2.0 Keywords: daml,blockchain,dlt,distributed
 ledger,digital asset Author: Davin K. Tanabe Author-email:
 davin.tanabe@digitalasset.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Provides-Extra: oauth Provides-Extra:
```

