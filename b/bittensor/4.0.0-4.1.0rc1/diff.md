# Comparing `tmp/bittensor-4.0.0.tar.gz` & `tmp/bittensor-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-4.0.0.tar", last modified: Thu Apr 20 17:18:38 2023, max compression
+gzip compressed data, was "bittensor-4.1.0rc1.tar", last modified: Tue May  2 18:48:14 2023, max compression
```

## Comparing `bittensor-4.0.0.tar` & `bittensor-4.1.0rc1.tar`

### file list

```diff
@@ -1,192 +1,102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.120097 bittensor-4.0.0/
--rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14522 2023-04-20 17:18:38.120097 bittensor-4.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    10559 2023-03-23 20:47:08.000000 bittensor-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/benchmarks/
--rw-rw-r--   0 root         (0) root         (0)    11819 2023-03-23 20:47:08.000000 bittensor-4.0.0/benchmarks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2251 2022-10-11 20:17:46.000000 bittensor-4.0.0/benchmarks/core_server.py
--rw-rw-r--   0 root         (0) root         (0)     2392 2022-07-09 15:48:08.000000 bittensor-4.0.0/benchmarks/multitron_server.py
--rw-rw-r--   0 root         (0) root         (0)     2404 2022-07-09 15:48:08.000000 bittensor-4.0.0/benchmarks/template_miner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/bin/
--rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.0.0/bin/btcli
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/bittensor/
--rw-rw-r--   0 root         (0) root         (0)     8756 2023-04-20 17:12:16.000000 bittensor-4.0.0/bittensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_axon/
--rw-rw-r--   0 root         (0) root         (0)    27767 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_axon/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    44809 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_axon/axon_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_cli/
--rw-rw-r--   0 root         (0) root         (0)     7347 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4316 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/cli_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_cli/commands/
--rw-rw-r--   0 root         (0) root         (0)      741 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    24295 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/delegates.py
--rw-rw-r--   0 root         (0) root         (0)     7578 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/inspect.py
--rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/list.py
--rw-rw-r--   0 root         (0) root         (0)     7197 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/metagraph.py
--rw-rw-r--   0 root         (0) root         (0)     6973 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/misc.py
--rw-rw-r--   0 root         (0) root         (0)    16251 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/overview.py
--rw-rw-r--   0 root         (0) root         (0)     5434 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/query.py
--rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/register.py
--rw-rw-r--   0 root         (0) root         (0)     6979 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/run.py
--rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/stake.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_cli/commands/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    11142 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/unstake.py
--rw-rw-r--   0 root         (0) root         (0)     6583 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/utils.py
--rw-rw-r--   0 root         (0) root         (0)    17528 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/wallets.py
--rw-rw-r--   0 root         (0) root         (0)     7587 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/commands/weights.py
--rw-rw-r--   0 root         (0) root         (0)    45041 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_cli/naka_cli_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_config/
--rw-rw-r--   0 root         (0) root         (0)     6080 2022-11-24 17:43:32.000000 bittensor-4.0.0/bittensor/_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6168 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_config/config_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_dataset/
--rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26969 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_dataset/dataset_impl.py
--rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_dataset/dataset_mock.py
--rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_dataset/thread_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_dendrite/
--rw-rw-r--   0 root         (0) root         (0)     9507 2022-12-13 00:25:39.000000 bittensor-4.0.0/bittensor/_dendrite/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    61529 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_dendrite/dendrite_impl.py
--rw-rw-r--   0 root         (0) root         (0)    37034 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_dendrite/dendrite_mock.py
--rw-rw-r--   0 root         (0) root         (0)     2906 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_dendrite/manager_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_endpoint/
--rw-rw-r--   0 root         (0) root         (0)     7561 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_endpoint/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6780 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_endpoint/endpoint_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_ipfs/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_ipfs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.0.0/bittensor/_ipfs/ipfs_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_keyfile/
--rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_keyfile/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_keyfile/keyfile_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_logging/
--rw-rw-r--   0 root         (0) root         (0)    13273 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_metagraph/
--rw-rw-r--   0 root         (0) root         (0)    11783 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_metagraph/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18406 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_metagraph/metagraph_impl.py
--rw-rw-r--   0 root         (0) root         (0)     8650 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_metagraph/metagraph_mock.py
--rw-rw-r--   0 root         (0) root         (0)    26417 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_metagraph/naka_metagraph_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/
--rw-rw-r--   0 root         (0) root         (0)     1665 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_neuron/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/audio/
--rw-rw-r--   0 root         (0) root         (0)     1150 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_neuron/audio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/text/
--rw-rw-r--   0 root         (0) root         (0)     1114 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_neuron/text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/text/core_server/
--rw-rw-r--   0 root         (0) root         (0)    33808 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_neuron/text/core_server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      143 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_neuron/text/core_server/main.py
--rw-rw-r--   0 root         (0) root         (0)    34918 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_neuron/text/core_server/nucleus_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_neuron/text/core_validator/
--rw-rw-r--   0 root         (0) root         (0)    87279 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_neuron/text/core_validator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1357 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_neuron/text/core_validator/main.py
--rw-rw-r--   0 root         (0) root         (0)    26915 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_neuron/text/log_utilities.py
--rw-rw-r--   0 root         (0) root         (0)    11272 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_neuron/text/neuron_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_prometheus/
--rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_prometheus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_proto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_proto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    58390 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_proto/bittensor_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     4168 2022-11-22 20:12:34.000000 bittensor-4.0.0/bittensor/_proto/bittensor_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_receptor/
--rw-rw-r--   0 root         (0) root         (0)     3881 2022-11-24 17:43:32.000000 bittensor-4.0.0/bittensor/_receptor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    36988 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_receptor/receptor_impl.py
--rw-rw-r--   0 root         (0) root         (0)    17491 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_receptor/receptor_pool_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.112097 bittensor-4.0.0/bittensor/_serializer/
--rw-rw-r--   0 root         (0) root         (0)     5910 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_serializer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11375 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_serializer/serializer_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_subtensor/
--rw-rw-r--   0 root         (0) root         (0)    14546 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26242 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/chain_data.py
--rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_subtensor/extrinsics/
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/delegation.py
--rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/prometheus.py
--rw-rw-r--   0 root         (0) root         (0)    14404 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/registration.py
--rw-rw-r--   0 root         (0) root         (0)    10091 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/serving.py
--rw-rw-r--   0 root         (0) root         (0)     6243 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/set_weights.py
--rw-rw-r--   0 root         (0) root         (0)    18046 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/staking.py
--rw-rw-r--   0 root         (0) root         (0)     7596 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    15089 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/extrinsics/unstaking.py
--rw-rw-r--   0 root         (0) root         (0)    85974 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_subtensor/naka_subtensor_impl.py
--rw-rw-r--   0 root         (0) root         (0)    46360 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/subtensor_impl.py
--rw-rw-r--   0 root         (0) root         (0)    14153 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/_subtensor/subtensor_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_synapse/
--rw-rw-r--   0 root         (0) root         (0)    14697 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14073 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/synapse_impl.py
--rw-rw-r--   0 root         (0) root         (0)    11996 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_causallm_impl.py
--rw-rw-r--   0 root         (0) root         (0)    11623 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_causallmnext_impl.py
--rw-rw-r--   0 root         (0) root         (0)    15284 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_lasthiddenstate_impl.py
--rw-rw-r--   0 root         (0) root         (0)    13066 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_synapse/text_seq2seq_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_threadpool/
--rw-rw-r--   0 root         (0) root         (0)     4618 2022-10-11 20:24:30.000000 bittensor-4.0.0/bittensor/_threadpool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.0.0/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_tokenizer/
--rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.0.0/bittensor/_tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_wallet/
--rw-rw-r--   0 root         (0) root         (0)     7408 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_wallet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    37669 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_wallet/naka_wallet_impl.py
--rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/_wallet/wallet_impl.py
--rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_wallet/wallet_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/_wandb/
--rw-rw-r--   0 root         (0) root         (0)     7739 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/_wandb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/bittensor/utils/
--rw-rw-r--   0 root         (0) root         (0)     8544 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/balance.py
--rw-rw-r--   0 root         (0) root         (0)     4277 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/codes.py
--rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/networking.py
--rw-rw-r--   0 root         (0) root         (0)     3241 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/register_cuda.py
--rw-rw-r--   0 root         (0) root         (0)    36240 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/registration.py
--rw-rw-r--   0 root         (0) root         (0)    33186 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/registratrion_old.py
--rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/utils/stats.py
--rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.0.0/bittensor/utils/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.0.0/bittensor/utils/tokenizer_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5908 2023-04-20 17:07:36.000000 bittensor-4.0.0/bittensor/utils/weight_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.108097 bittensor-4.0.0/bittensor.egg-info/
--rw-rw-r--   0 root         (0) root         (0)    14522 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5657 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)     1046 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       27 2023-04-20 17:18:38.000000 bittensor-4.0.0/bittensor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:18:38.120097 bittensor-4.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-03-23 20:47:08.000000 bittensor-4.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6049 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/tests/integration_tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/integration_tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      183 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/constant.py
--rw-rw-r--   0 root         (0) root         (0)    82396 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_cli.py
--rw-rw-r--   0 root         (0) root         (0)    10989 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_cli_no_network.py
--rw-rw-r--   0 root         (0) root         (0)     3535 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_dataset.py
--rw-rw-r--   0 root         (0) root         (0)    21138 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_dendrite.py
--rw-rw-r--   0 root         (0) root         (0)      925 2023-02-21 14:16:57.000000 bittensor-4.0.0/tests/integration_tests/test_ipfs.py
--rw-rw-r--   0 root         (0) root         (0)     7593 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/integration_tests/test_keyfile.py
--rw-rw-r--   0 root         (0) root         (0)     2640 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_metagraph.py
--rw-rw-r--   0 root         (0) root         (0)     1566 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/integration_tests/test_priority_thread_pool.py
--rw-rw-r--   0 root         (0) root         (0)     1589 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_prometheus.py
--rw-rw-r--   0 root         (0) root         (0)    20112 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_server_compression.py
--rw-rw-r--   0 root         (0) root         (0)    27891 2023-04-20 17:07:36.000000 bittensor-4.0.0/tests/integration_tests/test_subtensor.py
--rw-rw-r--   0 root         (0) root         (0)    10005 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/integration_tests/test_wallet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.116097 bittensor-4.0.0/tests/unit_tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.120097 bittensor-4.0.0/tests/unit_tests/bittensor_tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    62356 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_axon.py
--rw-rw-r--   0 root         (0) root         (0)    15186 2022-12-09 22:03:09.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_balance.py
--rw-rw-r--   0 root         (0) root         (0)     5426 2022-10-31 21:50:09.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_config.py
--rw-rw-r--   0 root         (0) root         (0)     6658 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_endpoint.py
--rw-rw-r--   0 root         (0) root         (0)    14448 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_forward_backward.py
--rw-rw-r--   0 root         (0) root         (0)     2136 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_metagraph.py
--rw-rw-r--   0 root         (0) root         (0)    14798 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_neuron.py
--rw-rw-r--   0 root         (0) root         (0)    37744 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_receptor.py
--rw-rw-r--   0 root         (0) root         (0)    18650 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_receptor_pool.py
--rw-rw-r--   0 root         (0) root         (0)    13476 2022-10-11 20:17:46.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_serialization.py
--rw-rw-r--   0 root         (0) root         (0)     6471 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_subtensor.py
--rw-rw-r--   0 root         (0) root         (0)     8103 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_synapse.py
--rw-rw-r--   0 root         (0) root         (0)    10781 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_wallet.py
--rw-rw-r--   0 root         (0) root         (0)     1666 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/test_wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:18:38.120097 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4938 2023-03-23 20:47:08.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_network_utils.py
--rw-rw-r--   0 root         (0) root         (0)    37677 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_tokenizer_utils.py
--rw-rw-r--   0 root         (0) root         (0)    23823 2023-04-20 17:07:37.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2948 2022-12-06 18:07:11.000000 bittensor-4.0.0/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/
+-rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3359 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.639414 bittensor-4.1.0rc1/bin/
+-rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.1.0rc1/bin/btcli
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.639414 bittensor-4.1.0rc1/bittensor/
+-rw-rw-r--   0 root         (0) root         (0)    14528 2023-05-02 18:42:06.000000 bittensor-4.1.0rc1/bittensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.639414 bittensor-4.1.0rc1/bittensor/_axon/
+-rw-rw-r--   0 root         (0) root         (0)    17744 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_axon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.639414 bittensor-4.1.0rc1/bittensor/_cli/
+-rw-rw-r--   0 root         (0) root         (0)     6688 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_cli/cli_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_cli/commands/
+-rw-rw-r--   0 root         (0) root         (0)      649 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    25104 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/delegates.py
+-rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/inspect.py
+-rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/list.py
+-rw-rw-r--   0 root         (0) root         (0)     7193 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/metagraph.py
+-rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    16429 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/overview.py
+-rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/register.py
+-rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/stake.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    11156 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/unstake.py
+-rw-rw-r--   0 root         (0) root         (0)     7733 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    17664 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/wallets.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_cli/commands/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_config/
+-rw-rw-r--   0 root         (0) root         (0)     6034 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5957 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_config/config_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_dataset/
+-rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27097 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_dataset/dataset_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_dataset/dataset_mock.py
+-rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1/bittensor/_dataset/thread_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_ipfs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/bittensor/_ipfs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.1.0rc1/bittensor/_ipfs/ipfs_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_keyfile/
+-rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/bittensor/_keyfile/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_keyfile/keyfile_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_logging/
+-rw-rw-r--   0 root         (0) root         (0)    13107 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_metagraph/
+-rw-rw-r--   0 root         (0) root         (0)    12460 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1/bittensor/_metagraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_prometheus/
+-rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_prometheus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_proto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/bittensor/_proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    30214 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_proto/bittensor_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     4422 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_proto/bittensor_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_serializer/
+-rw-rw-r--   0 root         (0) root         (0)     6078 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_serializer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10782 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_serializer/serializer_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_subtensor/
+-rw-rw-r--   0 root         (0) root         (0)    14289 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26232 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/chain_data.py
+-rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_subtensor/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/delegation.py
+-rw-rw-r--   0 root         (0) root         (0)    27011 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-rw-r--   0 root         (0) root         (0)    14454 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    10152 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/serving.py
+-rw-rw-r--   0 root         (0) root         (0)     6387 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-rw-r--   0 root         (0) root         (0)    18492 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/staking.py
+-rw-rw-r--   0 root         (0) root         (0)     7595 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    15591 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-rw-r--   0 root         (0) root         (0)    45559 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_subtensor/subtensor_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    18974 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/_subtensor/subtensor_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_threadpool/
+-rw-rw-r--   0 root         (0) root         (0)     4517 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_threadpool/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.1.0rc1/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_tokenizer/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1/bittensor/_tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/_wallet/
+-rw-rw-r--   0 root         (0) root         (0)     7293 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/_wallet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/_wallet/wallet_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/bittensor/_wallet/wallet_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/bittensor/utils/
+-rw-rw-r--   0 root         (0) root         (0)     8575 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3443 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/utils/_register_cuda.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/utils/balance.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/utils/codes.py
+-rw-rw-r--   0 root         (0) root         (0)      518 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/utils/formatting.py
+-rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/utils/networking.py
+-rw-rw-r--   0 root         (0) root         (0)    36116 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/utils/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    33174 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1/bittensor/utils/registratrion_old.py
+-rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/bittensor/utils/stats.py
+-rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1/bittensor/utils/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/bittensor/utils/tokenizer_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     9986 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1/bittensor/utils/weight_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:48:14.639414 bittensor-4.1.0rc1/bittensor.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4901 2023-05-02 18:48:14.000000 bittensor-4.1.0rc1/bittensor.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2600 2023-05-02 18:48:14.000000 bittensor-4.1.0rc1/bittensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 18:48:14.000000 bittensor-4.1.0rc1/bittensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)     1027 2023-05-02 18:48:14.000000 bittensor-4.1.0rc1/bittensor.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       10 2023-05-02 18:48:14.000000 bittensor-4.1.0rc1/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 18:48:14.643414 bittensor-4.1.0rc1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1/setup.py
```

### Comparing `bittensor-4.0.0/LICENSE` & `bittensor-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bin/btcli` & `bittensor-4.1.0rc1/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_cli/__init__.py` & `bittensor-4.1.0rc1/bittensor/_cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import sys
 import argparse
 import bittensor
 from . import cli_impl
 from .commands import *
 from typing import List, Optional
-from .naka_cli_impl import CLI as naka_CLI
 console = bittensor.__console__
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
 
 class cli:
@@ -44,79 +43,74 @@
         r""" Creates a new bittensor.cli from passed arguments.
             Args:
                 config (:obj:`bittensor.Config`, `optional`): 
                     bittensor.cli.config()
                 args (`List[str]`, `optional`): 
                     The arguments to parse from the command line.
         """
-        if config == None: 
-            config = cli.config(args)
+        if config == None:  
+            config = cli.config( args )
         cli.check_config( config )
-        if config.subtensor:
-            network = config.subtensor.get('network', bittensor.defaults.subtensor.network)
-
-        if network == 'nakamoto':
-            # Use nakamoto version of the CLI
-            return naka_CLI(config=config)
-        else:
-            return cli_impl.CLI( config = config)
-
-    @staticmethod   
-    def config(args: List[str]) -> 'bittensor.config':
-        """ From the argument parser, add config to bittensor.executor and local config 
-            Return: bittensor.config object
+        
+        return cli_impl.CLI( config = config)
+        
+    @staticmethod
+    def __create_parser__() -> 'argparse.ArgumentParser':
+        """ Creates the argument parser for the bittensor cli.
         """
         parser = argparse.ArgumentParser(
             description=f"bittensor cli v{bittensor.__version__}",
             usage="btcli <command> <command args>",
             add_help=True)
 
         cmd_parsers = parser.add_subparsers(dest='command')
-        RunCommand.add_args( cmd_parsers )
-        HelpCommand.add_args( cmd_parsers ) 
         ListCommand.add_args( cmd_parsers )
-        QueryCommand.add_args( cmd_parsers )
         StakeCommand.add_args( cmd_parsers )
         UpdateCommand.add_args( cmd_parsers )
         InspectCommand.add_args( cmd_parsers ) 
         WeightsCommand.add_args( cmd_parsers )
         UnStakeCommand.add_args( cmd_parsers )
         OverviewCommand.add_args( cmd_parsers )
         RegisterCommand.add_args( cmd_parsers )
         TransferCommand.add_args( cmd_parsers )
         NominateCommand.add_args( cmd_parsers )
         NewHotkeyCommand.add_args( cmd_parsers )
         MetagraphCommand.add_args( cmd_parsers )
-        SetWeightsCommand.add_args( cmd_parsers )
         NewColdkeyCommand.add_args( cmd_parsers )
-        NewHotkeyCommand.add_args( cmd_parsers )
         MyDelegatesCommand.add_args( cmd_parsers )
         ListSubnetsCommand.add_args( cmd_parsers )
         RegenHotkeyCommand.add_args( cmd_parsers )
         RegenColdkeyCommand.add_args( cmd_parsers )
         DelegateStakeCommand.add_args( cmd_parsers )
         DelegateUnstakeCommand.add_args( cmd_parsers )
         ListDelegatesCommand.add_args( cmd_parsers )
         RegenColdkeypubCommand.add_args( cmd_parsers )
         RecycleRegisterCommand.add_args( cmd_parsers )
 
+        return parser
+
+    @staticmethod   
+    def config(args: List[str]) -> 'bittensor.config':
+        """ From the argument parser, add config to bittensor.executor and local config 
+            Return: bittensor.config object
+        """
+        parser = cli.__create_parser__()
+
         # If no arguments are passed, print help text.
         if len(args) == 0:
             parser.print_help()
             sys.exit()
 
         return bittensor.config( parser, args=args )
 
     @staticmethod   
     def check_config (config: 'bittensor.Config'):
         """ Check if the essential config exist under different command
         """
-        if config.command == "run":
-            RunCommand.check_config( config )
-        elif config.command == "transfer":
+        if config.command == "transfer":
             TransferCommand.check_config( config )
         elif config.command == "register":
             RegisterCommand.check_config( config )
         elif config.command == "unstake":
             UnStakeCommand.check_config( config )
         elif config.command == "stake":
             StakeCommand.check_config( config )
@@ -132,24 +126,18 @@
             RegenColdkeypubCommand.check_config( config )
         elif config.command == "regen_hotkey":
             RegenHotkeyCommand.check_config( config )
         elif config.command == "metagraph":
             MetagraphCommand.check_config( config )
         elif config.command == "weights":
             WeightsCommand.check_config( config )
-        elif config.command == "set_weights":
-            SetWeightsCommand.check_config( config )
         elif config.command == "list":
             ListCommand.check_config( config )
         elif config.command == "inspect":
             InspectCommand.check_config( config )
-        elif config.command == "query":
-            QueryCommand.check_config( config )
-        elif config.command == "help":
-            HelpCommand.check_config( config )
         elif config.command == "update":
             UpdateCommand.check_config( config )
         elif config.command == "nominate":
             NominateCommand.check_config( config )
         elif config.command == "list_delegates":
             ListDelegatesCommand.check_config( config )
         elif config.command == "list_subnets":
```

### Comparing `bittensor-4.0.0/bittensor/_cli/cli_impl.py` & `bittensor-4.1.0rc1/bittensor/_cli/cli_impl.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,15 @@
             except:
                 raise RuntimeError("To avoid internet based version checking pass --no_version_checking while running the CLI.")
         self.config = config
 
     def run ( self ):
         """ Execute the command from config 
         """
-        if self.config.command == "run":
-            RunCommand.run( self )
-        elif self.config.command == "transfer":
+        if self.config.command == "transfer":
             TransferCommand.run( self )
         elif self.config.command == "register":
             RegisterCommand.run( self )
         elif self.config.command == "unstake":
             UnStakeCommand.run( self )
         elif self.config.command == "stake":
             StakeCommand.run( self )
@@ -64,22 +62,16 @@
             RegenColdkeypubCommand.run( self )
         elif self.config.command == "regen_hotkey":
             RegenHotkeyCommand.run( self )
         elif self.config.command == "metagraph":
             MetagraphCommand.run( self )
         elif self.config.command == "weights":
             WeightsCommand.run( self )
-        elif self.config.command == "set_weights":
-            SetWeightsCommand.run( self )
         elif self.config.command == "inspect":
             InspectCommand.run( self )
-        elif self.config.command == "query":
-            QueryCommand.run( self )
-        elif self.config.command == "help":
-            HelpCommand.run( self )
         elif self.config.command == 'update':
             UpdateCommand.run( self )
         elif self.config.command == 'nominate':
             NominateCommand.run( self )
         elif self.config.command == 'delegate':
             DelegateStakeCommand.run( self )
         elif self.config.command == 'undelegate':
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/__init__.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from .run import RunCommand
 from .stake import StakeCommand
 from .unstake import UnStakeCommand
 from .overview import OverviewCommand
 from .register import RegisterCommand, RecycleRegisterCommand
 from .delegates import NominateCommand, ListDelegatesCommand, DelegateStakeCommand, DelegateUnstakeCommand, MyDelegatesCommand
 from .wallets import NewColdkeyCommand, NewHotkeyCommand, RegenColdkeyCommand, RegenColdkeypubCommand, RegenHotkeyCommand
 from .transfer import TransferCommand
 from .inspect import InspectCommand
 from .metagraph import MetagraphCommand
 from .list import ListCommand
-from .weights import SetWeightsCommand, WeightsCommand
-from .query import QueryCommand
-from .misc import HelpCommand, UpdateCommand, ListSubnetsCommand
+from .weights import WeightsCommand
+from .misc import UpdateCommand, ListSubnetsCommand
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/delegates.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/delegates.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,47 +22,45 @@
 import bittensor
 from typing import List, Optional
 from rich.table import Table
 from rich.prompt import Prompt
 from rich.prompt import Confirm
 from rich.console import Text
 from tqdm import tqdm
+from substrateinterface.exceptions import SubstrateRequestException
+from .utils import get_delegates_details, DelegatesDetails
 
 import os
 import bittensor
-from typing import List
+from typing import List, Dict, Optional
 
 def _get_coldkey_wallets_for_path( path: str ) -> List['bittensor.wallet']:
     try:
         wallet_names = next(os.walk(os.path.expanduser(path)))[1]
         return [ bittensor.wallet( path= path, name=name ) for name in wallet_names ]
     except StopIteration:
         # No wallet files found.
         wallets = []
     return wallets
 
 console = bittensor.__console__
 
 # Uses rich console to pretty print a table of delegates.
-def show_delegates( delegates: List['bittensor.DelegateInfo'], prev_delegates: List['bittensor.DelegateInfo'], width: Optional[int] = None):
+def show_delegates( delegates: List['bittensor.DelegateInfo'], prev_delegates: Optional[List['bittensor.DelegateInfo']], width: Optional[int] = None):
     """ Pretty prints a table of delegates sorted by total stake.
     """
     delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
     prev_delegates_dict = {}
-    for prev_delegate in prev_delegates:
-        prev_delegates_dict[prev_delegate.hotkey_ss58] = prev_delegate
-    try:
-        package_dir = os.path.dirname(bittensor.__file__)
-        root_dir = os.path.dirname(package_dir)
-        filename = os.path.join(root_dir, 'delegates.json')
-        if os.path.exists(filename):
-            registered_delegate_info = json.load( open(filename, 'r') )
-        else:
-            registered_delegate_info = {}
-    except:
+    if prev_delegates is not None:
+        for prev_delegate in prev_delegates:
+            prev_delegates_dict[prev_delegate.hotkey_ss58] = prev_delegate
+
+    registered_delegate_info: Optional[Dict[str, DelegatesDetails]] = get_delegates_details(url = bittensor.__delegates_details_url__)
+    if registered_delegate_info is None:
+        bittensor.__console__.print( ':warning:[yellow]Could not get delegate info from chain.[/yellow]')
         registered_delegate_info = {}
 
     table = Table(show_footer=True, width=width, pad_edge=False, box=None, expand=True)
     table.add_column("[overline white]INDEX",  str(len(delegates)), footer_style = "overline white", style='bold white')
     table.add_column("[overline white]DELEGATE", style='rgb(50,163,219)', no_wrap=True, justify='left')
     table.add_column("[overline white]SS58",  str(len(delegates)), footer_style = "overline white", style='bold yellow')
     table.add_column("[overline white]NOMINATORS", justify='center', style='green', no_wrap=True)
@@ -81,17 +79,17 @@
         owner_stake = next(
             map(lambda x: x[1], # get stake
                 filter(lambda x: x[0] == delegate.owner_ss58, delegate.nominators) # filter for owner
             ),
             bittensor.Balance.from_rao(0) # default to 0 if no owner stake.
         )
         if delegate.hotkey_ss58 in registered_delegate_info:
-            delegate_name = registered_delegate_info[delegate.hotkey_ss58]['name']
-            delegate_url = registered_delegate_info[delegate.hotkey_ss58]['url']
-            delegate_description =  registered_delegate_info[delegate.hotkey_ss58]['description']
+            delegate_name = registered_delegate_info[delegate.hotkey_ss58].name
+            delegate_url = registered_delegate_info[delegate.hotkey_ss58].url
+            delegate_description =  registered_delegate_info[delegate.hotkey_ss58].description
         else:
             delegate_name = ''
             delegate_url = ''
             delegate_description = ''
 
         if delegate.hotkey_ss58 in prev_delegates_dict:
             prev_stake = prev_delegates_dict[delegate.hotkey_ss58].total_stake
@@ -102,15 +100,15 @@
                 if rate_change_in_stake > 0:
                     rate_change_in_stake_str = "[green]{:.2f}%[/green]".format(rate_change_in_stake)
                 elif rate_change_in_stake < 0:
                     rate_change_in_stake_str = "[red]{:.2f}%[/red]".format(rate_change_in_stake)
                 else:
                     rate_change_in_stake_str = "[grey0]0%[/grey0]"
         else:
-            rate_change_in_stake_str = "[grey0]0%[/grey0]"
+            rate_change_in_stake_str = "[grey0]NA[/grey0]"
 
         table.add_row(
             str(i),
             Text(delegate_name, style=f'link {delegate_url}'),
             f'{delegate.hotkey_ss58:8.8}...',
             str(len([nom for nom in delegate.nominators if nom[1].rao > 0])),
             f'{owner_stake!s:13.13}',
@@ -186,18 +184,24 @@
     @staticmethod   
     def check_config( config: 'bittensor.Config' ):
         if not config.get('delegate_ss58key'):
             # Check for delegates.
             with bittensor.__console__.status(":satellite: Loading delegates..."):
                 subtensor = bittensor.subtensor( config = config )
                 delegates: List[bittensor.DelegateInfo] = subtensor.get_delegates()
-                prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
+                try:
+                    prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
+                except SubstrateRequestException:
+                    prev_delegates = None
+
+            if prev_delegates is None:
+                bittensor.__console__.print(":warning: [yellow]Could not fetch delegates history[/yellow]")
 
             if len(delegates) == 0:
-                console.print(":cross_mark:[red]There are no delegates on {}[/red]".format(subtensor.network))
+                console.print(":cross_mark: [red]There are no delegates on {}[/red]".format(subtensor.network))
                 sys.exit(1)
             
             delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
             show_delegates( delegates, prev_delegates = prev_delegates)
             delegate_index = Prompt.ask("Enter delegate index")
             config.delegate_ss58key = str(delegates[int(delegate_index)].hotkey_ss58)
             console.print("Selected: [yellow]{}[/yellow]".format(config.delegate_ss58key))
@@ -209,15 +213,15 @@
         # Get amount.
         if not config.get('amount') and not config.get('stake_all'):
             if not Confirm.ask("Stake all Tao from account: [bold]'{}'[/bold]?".format(config.wallet.get('name', bittensor.defaults.wallet.name))):
                 amount = Prompt.ask("Enter Tao amount to stake")
                 try:
                     config.amount = float(amount)
                 except ValueError:
-                    console.print(":cross_mark:[red]Invalid Tao amount[/red] [bold white]{}[/bold white]".format(amount))
+                    console.print(":cross_mark: [red]Invalid Tao amount[/red] [bold white]{}[/bold white]".format(amount))
                     sys.exit()
             else:
                 config.stake_all = True
 
 class DelegateUnstakeCommand:
 
     @staticmethod
@@ -285,18 +289,24 @@
             config.wallet.name = str(wallet_name)
 
         if not config.get('delegate_ss58key'):
             # Check for delegates.
             with bittensor.__console__.status(":satellite: Loading delegates..."):
                 subtensor = bittensor.subtensor( config = config )
                 delegates: List[bittensor.DelegateInfo] = subtensor.get_delegates()
-                prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
+                try:
+                    prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
+                except SubstrateRequestException:
+                    prev_delegates = None
+
+            if prev_delegates is None:
+                bittensor.__console__.print(":warning: [yellow]Could not fetch delegates history[/yellow]")
 
             if len(delegates) == 0:
-                console.print(":cross_mark:[red]There are no delegates on {}[/red]".format(subtensor.network))
+                console.print(":cross_mark: [red]There are no delegates on {}[/red]".format(subtensor.network))
                 sys.exit(1)
             
             delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
             show_delegates( delegates, prev_delegates = prev_delegates)
             delegate_index = Prompt.ask("Enter delegate index")
             config.delegate_ss58key = str(delegates[int(delegate_index)].hotkey_ss58)
             console.print("Selected: [yellow]{}[/yellow]".format(config.delegate_ss58key))
@@ -304,30 +314,37 @@
         # Get amount.
         if not config.get('amount') and not config.get('unstake_all'):
             if not Confirm.ask("Unstake all Tao to account: [bold]'{}'[/bold]?".format(config.wallet.get('name', bittensor.defaults.wallet.name))):
                 amount = Prompt.ask("Enter Tao amount to unstake")
                 try:
                     config.amount = float(amount)
                 except ValueError:
-                    console.print(":cross_mark:[red]Invalid Tao amount[/red] [bold white]{}[/bold white]".format(amount))
+                    console.print(":cross_mark: [red]Invalid Tao amount[/red] [bold white]{}[/bold white]".format(amount))
                     sys.exit()
             else:
                 config.unstake_all = True
 
 class ListDelegatesCommand:
 
     @staticmethod
     def run( cli ):
         r"""
         List all delegates on the network.
         """
         subtensor = bittensor.subtensor( config = cli.config )
         with bittensor.__console__.status(":satellite: Loading delegates..."):
             delegates: bittensor.DelegateInfo = subtensor.get_delegates()
-            prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
+            try:
+                prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
+            except SubstrateRequestException:
+                prev_delegates = None
+
+        if prev_delegates is None:
+            bittensor.__console__.print(":warning: [yellow]Could not fetch delegates history[/yellow]")
+        
         show_delegates( delegates, prev_delegates = prev_delegates, width = cli.config.get('width', None) )
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         list_delegates_parser = parser.add_parser(
             'list_delegates', 
             help='''List all delegates on the network'''
@@ -405,15 +422,15 @@
 
 class MyDelegatesCommand:
 
     @staticmethod
     def run( cli ):
         '''Delegates stake to a chain delegate.'''
         config = cli.config.copy()
-        if config.all == True:
+        if config.get('all', d=None) == True:
             wallets = _get_coldkey_wallets_for_path( config.wallet.path )
         else:
             wallets = [bittensor.wallet( config = config )]
         subtensor: bittensor.Subtensor = bittensor.subtensor( config = config )
 
         table = Table(show_footer=True, pad_edge=False, box=None, expand=True)
         table.add_column("[overline white]Wallet", footer_style = "overline white", style='bold white')
@@ -437,23 +454,17 @@
             for delegate in delegates:
                 for coldkey_addr, staked in delegate[0].nominators:
                     if coldkey_addr == wallet.coldkeypub.ss58_address and staked.tao > 0:
                         my_delegates[ delegate[0].hotkey_ss58 ] = staked
 
             delegates.sort(key=lambda delegate: delegate[0].total_stake, reverse=True)
             
-            try:
-                package_dir = os.path.dirname(bittensor.__file__)
-                root_dir = os.path.dirname(package_dir)
-                filename = os.path.join(root_dir, 'delegates.json')
-                if os.path.exists(filename):
-                    registered_delegate_info = json.load( open(filename, 'r') )
-                else:
-                    registered_delegate_info = {}
-            except:
+            registered_delegate_info: Optional[DelegatesDetails] = get_delegates_details(url = bittensor.__delegates_details_url__)
+            if registered_delegate_info is None:
+                bittensor.__console__.print( ':warning:[yellow]Could not get delegate info from chain.[/yellow]')
                 registered_delegate_info = {}
 
             for i, delegate in enumerate( delegates ):
                 owner_stake = next(
                     map(lambda x: x[1], # get stake
                         filter(lambda x: x[0] == delegate[0].owner_ss58, delegate[0].nominators) # filter for owner
                     ),
@@ -514,14 +525,14 @@
             default=False,
         )
         bittensor.wallet.add_args( delegate_stake_parser )
         bittensor.subtensor.add_args( delegate_stake_parser )
 
     @staticmethod   
     def check_config( config: 'bittensor.Config' ):
-        if not config.all and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.get( 'all', d=None ) and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/inspect.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 import json
 import argparse
 import bittensor
 from tqdm import tqdm
 from rich.table import Table
 from rich.prompt import Prompt
-from .utils import check_netuid_set
+from .utils import check_netuid_set, get_delegates_details, DelegatesDetails
 console = bittensor.__console__
 
 import os
 import bittensor
-from typing import List, Tuple
+from typing import List, Tuple, Optional, Dict
 
 def _get_coldkey_wallets_for_path( path: str ) -> List['bittensor.wallet']:
     try:
         wallet_names = next(os.walk(os.path.expanduser(path)))[1]
         return [ bittensor.wallet( path= path, name=name ) for name in wallet_names ]
     except StopIteration:
         # No wallet files found.
@@ -54,31 +54,25 @@
     return hotkey_wallets
 
 class InspectCommand:
     @staticmethod
     def run (cli):
         r""" Inspect a cold, hot pair.
         """
-        if cli.config.all == True:
+        if cli.config.get('all', d=False) == True:
             wallets = _get_coldkey_wallets_for_path( cli.config.wallet.path )
         else:
             wallets = [bittensor.wallet( config = cli.config )]
         subtensor = bittensor.subtensor( config = cli.config )
 
         netuids = subtensor.get_all_subnet_netuids()
 
-        try:
-            package_dir = os.path.dirname(bittensor.__file__)
-            root_dir = os.path.dirname(package_dir)
-            filename = os.path.join(root_dir, 'delegates.json')
-            if os.path.exists(filename):
-                registered_delegate_info = json.load( open(filename, 'r') )
-            else:
-                registered_delegate_info = {}
-        except:
+        registered_delegate_info: Optional[Dict[str, DelegatesDetails]] = get_delegates_details(url = bittensor.__delegates_details_url__)
+        if registered_delegate_info is None:
+            bittensor.__console__.print( ':warning:[yellow]Could not get delegate info from chain.[/yellow]')
             registered_delegate_info = {}
 
         neuron_state_dict = {}
         for netuid in tqdm( netuids ):
             neuron_state_dict[netuid] = subtensor.neurons_lite( netuid )
 
         table = Table(show_footer=True, pad_edge=False, box=None, expand=True)
@@ -104,15 +98,15 @@
                 '',
                 '',
                 '',
                 '',
             )
             for dele, staked in delegates:
                 if dele.hotkey_ss58 in registered_delegate_info:
-                    delegate_name = registered_delegate_info[dele.hotkey_ss58]['name']
+                    delegate_name = registered_delegate_info[dele.hotkey_ss58].name
                 else:
                     delegate_name = dele.hotkey_ss58
                 table.add_row(
                     '',
                     '',
                     str(delegate_name),
                     str(staked),
@@ -141,15 +135,15 @@
                
         bittensor.__console__.print(table)
             
                 
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if not config.all and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.get( 'all', d=None ) and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         inspect_parser = parser.add_parser(
             'inspect',
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/list.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/metagraph.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/metagraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class MetagraphCommand:
     @staticmethod
     def run (cli):
         r""" Prints an entire metagraph."""
         console = bittensor.__console__
         subtensor = bittensor.subtensor( config = cli.config )
         console.print(":satellite: Syncing with chain: [white]{}[/white] ...".format(cli.config.subtensor.network))
-        metagraph = subtensor.metagraph( netuid = cli.config.netuid )
+        metagraph: bittensor.metagraph = subtensor.metagraph( netuid = cli.config.netuid )
         metagraph.save()
         difficulty = subtensor.difficulty( cli.config.netuid )
         subnet_emission = bittensor.Balance.from_tao(subtensor.get_emission_value_by_subnet(cli.config.netuid))
         total_issuance = bittensor.Balance.from_tao(subtensor.total_issuance())
 
         TABLE_DATA = [] 
         total_stake = 0.0
@@ -42,17 +42,18 @@
         total_validator_trust = 0.0
         total_trust = 0.0
         total_consensus = 0.0
         total_incentive = 0.0
         total_dividends = 0.0
         total_emission = 0  
         for uid in metagraph.uids:
-            ep = metagraph.endpoint_objs[uid]
+            neuron = metagraph.neurons[uid]
+            ep = metagraph.axons[uid]
             row = [
-                str(ep.uid), 
+                str(neuron.uid), 
                 '{:.5f}'.format( metagraph.total_stake[uid]),
                 '{:.5f}'.format( metagraph.ranks[uid]),
                 '{:.5f}'.format( metagraph.trust[uid]), 
                 '{:.5f}'.format( metagraph.consensus[uid]),
                 '{:.5f}'.format( metagraph.incentive[uid]),
                 '{:.5f}'.format( metagraph.dividends[uid]),
                 '{}'.format( int(metagraph.emission[uid] * 1000000000)),
@@ -72,15 +73,15 @@
             total_incentive += metagraph.incentive[uid]
             total_dividends += metagraph.dividends[uid]
             total_emission += int(metagraph.emission[uid] * 1000000000)
             TABLE_DATA.append(row)
         total_neurons = len(metagraph.uids)                
         table = Table(show_footer=False)
         table.title = (
-            "[white]Metagraph: net: {}:{}, block: {}, N: {}/{}, tau: {}/block, stake: {}, issuance: {}, difficulty: {}".format(subtensor.network, metagraph.netuid, metagraph.block.item(), sum(metagraph.active.tolist()), metagraph.n.item(), bittensor.Balance.from_tao(metagraph.tau.item()), bittensor.Balance.from_tao(total_stake), total_issuance, difficulty )
+            "[white]Metagraph: net: {}:{}, block: {}, N: {}/{}, stake: {}, issuance: {}, difficulty: {}".format(subtensor.network, metagraph.netuid, metagraph.block.item(), sum(metagraph.active.tolist()), metagraph.n.item(), bittensor.Balance.from_tao(total_stake), total_issuance, difficulty )
         )
         table.add_column("[overline white]UID",  str(total_neurons), footer_style = "overline white", style='yellow')
         table.add_column("[overline white]STAKE(\u03C4)", '\u03C4{:.5f}'.format(total_stake), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]RANK", '{:.5f}'.format(total_rank), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]TRUST", '{:.5f}'.format(total_trust), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]CONSENSUS", '{:.5f}'.format(total_consensus), footer_style = "overline white", justify='right', style='green', no_wrap=True)
         table.add_column("[overline white]INCENTIVE", '{:.5f}'.format(total_incentive), footer_style = "overline white", justify='right', style='green', no_wrap=True)
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/misc.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,45 +23,46 @@
 from rich.prompt import Prompt
 from rich.table import Table
 console = bittensor.__console__
 
 class HelpCommand:
     @staticmethod
     def run (cli):
-        cli.config.to_defaults()
         sys.argv = [sys.argv[0], '--help']
-        # Run miner.
-        if cli.config.model == 'core_server':
-            bittensor.neurons.core_server.neuron().run()
-        elif cli.config.model == 'core_validator':
-            bittensor.neurons.core_validator.neuron().run()
-        elif cli.config.model == 'multitron_server':
-            bittensor.neurons.multitron_server.neuron().run()
+        # # Run miner.
+        # if cli.config.model == 'core_server':
+        #     bittensor.neurons.core_server.neuron().run()
+        # elif cli.config.model == 'core_validator':
+        #     bittensor.neurons.core_validator.neuron().run()
+        # elif cli.config.model == 'multitron_server':
+        #     bittensor.neurons.multitron_server.neuron().run()
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.model == 'None':
-            model = Prompt.ask('Enter miner name', choices = list(bittensor.neurons.__text_neurons__.keys()), default = 'core_server')
-            config.model = model
+        pass
+        # if config.model == 'None':
+        #     model = Prompt.ask('Enter miner name', choices = list(bittensor.neurons.__text_neurons__.keys()), default = 'core_server')
+        #     config.model = model
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
-        help_parser = parser.add_parser(
-            'help', 
-            add_help=False,
-            help='''Displays the help '''
-        )
-        help_parser.add_argument(
-            '--model', 
-            type=str, 
-            choices= list(bittensor.neurons.__text_neurons__.keys()), 
-            default='None', 
-        )
-        help_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
-        bittensor.subtensor.add_args( help_parser )
+        pass
+        # help_parser = parser.add_parser(
+        #     'help', 
+        #     add_help=False,
+        #     help='''Displays the help '''
+        # )
+        # help_parser.add_argument(
+        #     '--model', 
+        #     type=str, 
+        #     choices= list(bittensor.neurons.__text_neurons__.keys()), 
+        #     default='None', 
+        # )
+        # help_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
+        # bittensor.subtensor.add_args( help_parser )
 
 class UpdateCommand:
     @staticmethod
     def run (cli):
         if cli.config.no_prompt or cli.config.answer == 'Y':
             os.system(' (cd ~/.bittensor/bittensor/ ; git checkout master ; git pull --ff-only )')
             os.system('pip install -e ~/.bittensor/bittensor/')
@@ -101,16 +102,16 @@
 
         for subnet in subnets:
             total_neurons += subnet.max_n
             # netuid, N, Max N, difficulty, network connect, tempo, emission, burn rate
             rows.append((
                 str(subnet.netuid),
                 str(subnet.subnetwork_n),
-                str(bittensor.utils.registration.millify(subnet.max_n)),
-                str(bittensor.utils.registration.millify(subnet.difficulty)),
+                str(bittensor.utils.formatting.millify(subnet.max_n)),
+                str(bittensor.utils.formatting.millify(subnet.difficulty)),
                 str(subnet.tempo),
                 str([ f'{cr[0]}: {cr[1] * 100:.1f}%' for cr in subnet.connection_requirements.items()] if len(subnet.connection_requirements) > 0 else None ),
                 f'{subnet.emission_value / bittensor.utils.RAOPERTAO * 100:0.2f}%',
                 f'{subnet.burn!s:8.8}',
             ))
 
         table = Table(show_footer=True, width=cli.config.get('width', None), pad_edge=True, box=None, show_edge=True)
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/overview.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         wallet = bittensor.wallet( config = cli.config )
         subtensor: 'bittensor.Subtensor' = bittensor.subtensor( config = cli.config )
 
         all_hotkeys = []
         total_balance = bittensor.Balance(0)
         
         # We are printing for every coldkey.
-        if cli.config.all:
+        if cli.config.get( 'all', d=None ):
             cold_wallets = get_coldkey_wallets_for_path(cli.config.wallet.path)
             for cold_wallet in tqdm(cold_wallets, desc="Pulling balances"):
                 if cold_wallet.coldkeypub_file.exists_on_device() and not cold_wallet.coldkeypub_file.is_encrypted():
                     total_balance = total_balance + subtensor.get_balance( cold_wallet.coldkeypub.ss58_address )
             all_hotkeys = get_all_wallets_for_path( cli.config.wallet.path )
         else:
             # We are only printing keys for a single coldkey
@@ -98,15 +98,15 @@
                     # Remove netuid from overview if no neurons are found.
                     netuids.remove(netuid)
 
         # Setup outer table.
         grid = Table.grid(pad_edge=False)
 
         title: str = ""
-        if not cli.config.all:
+        if not cli.config.get( 'all', d=None ):
             title = ( "[bold white italic]Wallet - {}:{}".format(cli.config.wallet.name, wallet.coldkeypub.ss58_address) )
         else:
             title = ( "[bold whit italic]All Wallets:" )
 
         # Add title
         grid.add_row(Align(title, vertical="middle", align="center"))
 
@@ -329,14 +329,17 @@
         )
         overview_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )  
         bittensor.wallet.add_args( overview_parser )
         bittensor.subtensor.add_args( overview_parser )
 
     @staticmethod   
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt and not config.all:
+        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt and not config.get( 'all', d=None ):
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.netuid != []:
-            config.netuid = [int(netuid) for netuid in config.netuid]
+            if not isinstance(config.netuid, list):
+                config.netuid = [int(config.netuid)]
+            else:
+                config.netuid = [int(netuid) for netuid in config.netuid]
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/query.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/weights.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
+# Copyright © 2023 Opentensor Foundation
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
@@ -11,103 +12,86 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
-import sys
 import argparse
 import bittensor
 from rich.prompt import Prompt
+from rich.table import Table
+from rich.prompt import Confirm
+from .utils import check_netuid_set
 console = bittensor.__console__
 
-class QueryCommand:
+class WeightsCommand:
     @staticmethod
     def run (cli):
-        wallet = bittensor.wallet(config = cli.config)
+        r""" Prints an weights to screen.
+        """
+        console = bittensor.__console__
         subtensor = bittensor.subtensor( config = cli.config )
-
-        # Verify subnet exists
-        if not hasattr(cli.config, 'netuid'):
-            bittensor.__console__.print(f"[red]Please specify subnet with --netuid.[/red]")
-            sys.exit(1)
-
-        if not subtensor.subnet_exists( netuid = cli.config.netuid ):
-            bittensor.__console__.print(f"[red]Subnet {cli.config.netuid} does not exist.[/red]")
-            sys.exit(1)
-
-        dendrite = bittensor.dendrite( wallet = wallet )
-        stats = {}
-        for uid in cli.config.uids:
-            neuron = subtensor.neuron_for_uid( uid = uid, netuid = cli.config.netuid )
-            endpoint = bittensor.endpoint.from_neuron( neuron )
-            _, c, t = dendrite.text( endpoints = endpoint, inputs = 'hello world', synapses = [bittensor.synapse.TextCausalLMNext()])
-            latency = "{}".format(t[0].tolist()[0]) if c[0].tolist()[0] == 1 else 'N/A'
-            bittensor.__console__.print("\tUid: [bold white]{}[/bold white]\n\tLatency: [bold white]{}[/bold white]\n\tCode: [bold {}]{}[/bold {}]\n\n".format(
-                    uid, 
-                    latency, 
-                    bittensor.utils.codes.code_to_loguru_color( c[0].item() ), 
-                    bittensor.utils.codes.code_to_string( c[0].item() ), 
-                    bittensor.utils.codes.code_to_loguru_color( c[0].item() )
-                ), highlight=True)
-            stats[uid] = latency
-        print (stats)
-        dendrite.__del__()
+        wallet = bittensor.wallet( config = cli.config )
+        metagraph = subtensor.metagraph( netuid = cli.config.get('netuid') )
+        metagraph.save()
+
+        table = Table()
+        rows = []
+        table.add_column("[bold white]uid", style='white', no_wrap=False)
+        for uid in metagraph.uids.tolist():
+            table.add_column("[bold white]{}".format(uid), style='white', no_wrap=False)
+            if cli.config.all_weights:
+                rows.append(["[bold white]{}".format(uid) ] + ['{:.3f}'.format(v) for v in metagraph.W[uid].tolist()])
+            else:
+                if metagraph.coldkeys[uid] == wallet.coldkeypub.ss58_address:
+                    if not cli.config.all_hotkeys:
+                        if metagraph.hotkeys[uid] == wallet.hotkey.ss58_address:
+                            rows.append(["[bold white]{}".format(uid) ] + ['{:.3f}'.format(v) for v in metagraph.W[uid].tolist()])
+                    else:
+                        rows.append(["[bold white]{}".format(uid) ] + ['{:.3f}'.format(v) for v in metagraph.W[uid].tolist()])
+
+        for row in rows:
+            table.add_row(*row)
+        table.box = None
+        table.pad_edge = False
+        table.width = None
+        with console.pager():
+            console.print(table)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-
         if config.subtensor.get('network') == bittensor.defaults.subtensor.network and not config.no_prompt:
             config.subtensor.network = Prompt.ask("Enter subtensor network", choices=bittensor.__networks__, default = bittensor.defaults.subtensor.network)
 
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
-            wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
-            config.wallet.name = str(wallet_name)
+        check_netuid_set( config, subtensor = bittensor.subtensor( config = config ) )
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
-            hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
-            config.wallet.hotkey = str(hotkey)
-                  
-        if not config.uids:
-            prompt = Prompt.ask("Enter uids to query [i.e. 0 10 1999]", default = 'All')
-            if prompt == 'All':
-                config.uids = list( range(2000) )
+        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+            if not Confirm.ask("Show all weights?"):
+                wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
+                config.wallet.name = str(wallet_name)
+                config.all_weights = False
+                if not Confirm.ask("Show all hotkeys?"):
+                    hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
+                    config.wallet.hotkey = str(hotkey)
+                    config.all_hotkeys = False
+                else:
+                    config.all_hotkeys = True
             else:
-                try:
-                    config.uids = [int(el) for el in prompt.split(' ')]
-                except Exception as e:
-                    console.print(":cross_mark:[red] Failed to parse uids[/red] [bold white]{}[/bold white], must be space separated list of ints".format(prompt))
-                    sys.exit()
+                config.all_weights = True
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
-        query_parser = parser.add_parser(
-            'query', 
-            help='''Query a uid with your current wallet'''
-        )
-        query_parser.add_argument(
-            "-u", '--uids',
-            type=list, 
-            nargs='+',
-            dest='uids', 
-            choices=list(range(2000)), 
-            help='''Uids to query'''
+        weights_parser = parser.add_parser(
+            'weights', 
+            help='''Show weights from chain.'''
         )
-        query_parser.add_argument(
+        weights_parser.add_argument(
             '--no_prompt', 
             dest='no_prompt', 
             action='store_true', 
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
-        query_parser.add_argument(
-            '--netuid',
-            type=int,
-            help='netuid for subnet to serve this neuron on',
-            default=argparse.SUPPRESS,
-        )
-        query_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
-        bittensor.wallet.add_args( query_parser )
-        bittensor.subtensor.add_args( query_parser )
-        bittensor.dendrite.add_args( query_parser )
-        bittensor.logging.add_args( query_parser )
+        weights_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
+        bittensor.wallet.add_args( weights_parser )
+        bittensor.subtensor.add_args( weights_parser )
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/register.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/stake.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/transfer.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/unstake.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/unstake.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
     @classmethod   
     def check_config( cls, config: 'bittensor.Config' ):        
         if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if not config.hotkey_ss58address and config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
+        if not config.get('hotkey_ss58address') and config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
                     
         # Get amount.
-        if not config.hotkey_ss58address and not config.get('amount') and not config.get('unstake_all') and not config.get('max_stake'):
+        if not config.get('hotkey_ss58address') and not config.get('amount') and not config.get('unstake_all') and not config.get('max_stake'):
             hotkeys: str = ''
             if config.get('all_hotkeys'):
                 hotkeys = "all hotkeys"
             elif config.get('hotkeys'):
                 hotkeys = str(config.hotkeys).replace('[', '').replace(']', '')
             else:
                 hotkeys = str(config.wallet.hotkey)
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/utils.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import os
 import torch
 import bittensor
-from typing import List, Dict
+from typing import List, Dict, Any, Optional
 from rich.prompt import Confirm, Prompt, PromptBase
+import requests
+from dataclasses import dataclass
 console = bittensor.__console__
 
 class IntListPrompt(PromptBase):
     """ Prompt for a list of integers. """
     
     def check_choice( self, value: str ) -> bool:
         assert self.choices is not None
@@ -122,8 +124,43 @@
 
 def get_all_wallets_for_path( path:str ) -> List['bittensor.wallet']:
     all_wallets = []
     cold_wallets = get_coldkey_wallets_for_path(path)
     for cold_wallet in cold_wallets:
         if cold_wallet.coldkeypub_file.exists_on_device() and not cold_wallet.coldkeypub_file.is_encrypted():
             all_wallets.extend( get_hotkey_wallets_for_wallet(cold_wallet) )
-    return all_wallets
+    return all_wallets
+
+@dataclass
+class DelegatesDetails:
+    name: str
+    url: str
+    description: str
+    signature: str
+
+    @classmethod
+    def from_json(cls, json: Dict[str, any]) -> 'DelegatesDetails':
+        return cls(
+            name=json['name'],
+            url=json['url'],
+            description=json['description'],
+            signature=json['signature'],
+        )
+
+def _get_delegates_details_from_github(requests_get, url: str) -> Dict[str, DelegatesDetails]:
+    response = requests_get(url)
+    
+
+    if response.status_code == 200:
+        all_delegates: Dict[str, Any] = response.json()
+        all_delegates_details = {}
+        for delegate_hotkey, delegates_details in all_delegates.items():
+            all_delegates_details[delegate_hotkey] = DelegatesDetails.from_json(delegates_details)
+        return all_delegates_details
+    else:
+        return {}
+    
+def get_delegates_details(url: str) -> Optional[Dict[str, DelegatesDetails]]: 
+    try:
+        return _get_delegates_details_from_github(requests.get, url)
+    except Exception:
+        return None # Fail silently
```

### Comparing `bittensor-4.0.0/bittensor/_cli/commands/wallets.py` & `bittensor-4.1.0rc1/bittensor/_cli/commands/wallets.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,24 @@
    
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
         
-        if config.mnemonic == None and config.seed == None and config.json == None:
+        if config.mnemonic == None and config.get( 'seed', d=None ) == None and config.get( 'json', d=None ) == None:
             prompt_answer = Prompt.ask("Enter mnemonic, seed, or json file location")
             if prompt_answer.startswith("0x"):
                 config.seed = prompt_answer
             elif len(prompt_answer.split(" ")) > 1:
                 config.mnemonic = prompt_answer
             else:
                 config.json = prompt_answer
 
-        if config.json and config.json_password == None:
+        if config.get( 'json', d=None ) and config.get( 'json_password', d=None ) == None:
             config.json_password = Prompt.ask("Enter json backup password", password=True)
     
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         regen_coldkey_parser = parser.add_parser(
             'regen_coldkey',
             help='''Regenerates a coldkey from a passed value'''
@@ -209,24 +209,24 @@
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
         
-        if config.mnemonic == None and config.seed == None and config.json == None:
+        if config.mnemonic == None and config.get( 'seed', d=None ) == None and config.get( 'json', d=None ) == None:
             prompt_answer = Prompt.ask("Enter mnemonic, seed, or json file location")
             if prompt_answer.startswith("0x"):
                 config.seed = prompt_answer
             elif len(prompt_answer.split(" ")) > 1:
                 config.mnemonic = prompt_answer
             else:
                 config.json = prompt_answer
 
-        if config.json and config.json_password == None:
+        if config.get( 'json', d=None ) and config.get( 'json_password', d=None ) == None:
             config.json_password = Prompt.ask("Enter json backup password", password=True)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         regen_hotkey_parser = parser.add_parser(
             'regen_hotkey',
             help='''Regenerates a hotkey from a passed mnemonic'''
```

### Comparing `bittensor-4.0.0/bittensor/_config/__init__.py` & `bittensor-4.1.0rc1/bittensor/_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,13 +142,12 @@
     def full():
         """ From the parser, add arguments to multiple bittensor sub-modules
         """
         parser = ArgumentParser()
         bittensor.wallet.add_args( parser )
         bittensor.subtensor.add_args( parser )
         bittensor.axon.add_args( parser )
-        bittensor.dendrite.add_args( parser )
         bittensor.metagraph.add_args( parser )
         bittensor.dataset.add_args( parser )
         bittensor.prometheus.add_args( parser )
         return bittensor.config( parser )
```

### Comparing `bittensor-4.0.0/bittensor/_config/config_impl.py` & `bittensor-4.1.0rc1/bittensor/_config/config_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 
     def update_with_kwargs( self, kwargs ):
         """ Add config to self
         """
         for key,val in kwargs.items():
             self[key] = val
 
+    def merge(self, b):
+        """ Merge two configs
+        """
+        self = _merge(self, b)
+
     def to_prometheus(self):
         """
             Sends the config to the inprocess prometheus server if it exists.
         """
         try:
             prometheus_info = Info('config', 'Config Values')
             config_info = pandas.json_normalize(json.loads(json.dumps(self)), sep='.').to_dict(orient='records')[0]
@@ -85,19 +90,14 @@
                 bittensor.defaults.dataset.num_batches = self.dataset.num_batches
                 bittensor.defaults.dataset.num_workers = self.dataset.num_workers
                 bittensor.defaults.dataset.dataset_names = self.dataset.dataset_names
                 bittensor.defaults.dataset.data_dir = self.dataset.data_dir
                 bittensor.defaults.dataset.save_dataset = self.dataset.save_dataset
                 bittensor.defaults.dataset.max_datasets = self.dataset.max_datasets
 
-            if 'dendrite' in self.keys():
-                bittensor.defaults.dendrite.timeout = self.dendrite.timeout
-                bittensor.defaults.dendrite.max_active_receptors = self.dendrite.max_active_receptors
-                bittensor.defaults.dendrite.requires_grad = self.dendrite.requires_grad
-
             if  'logging' in self.keys():
                 bittensor.defaults.logging.debug = self.logging.debug
                 bittensor.defaults.logging.trace = self.logging.trace
                 bittensor.defaults.logging.record_log = self.logging.record_log
                 bittensor.defaults.logging.logging_dir = self.logging.logging_dir
             
             if 'subtensor' in self.keys():
```

### Comparing `bittensor-4.0.0/bittensor/_dataset/__init__.py` & `bittensor-4.1.0rc1/bittensor/_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_dataset/dataset_impl.py` & `bittensor-4.1.0rc1/bittensor/_dataset/dataset_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,19 @@
         Return:
             text (str):
                 The text that we get from the file (from disk or IPFS).     
         """
         text = None
         response = self.get_ipfs_directory(self.text_dir, file_meta)
         if (response != None) and (response.status_code == 200):
-            text = response.text
+            try:
+                text = json.loads(response.text)['Data']
+            except json.decoder.JSONDecodeError:
+                text = response.text
+
             self.IPFS_fails = 0
             
             if self.save_dataset and self.dataset_hashes[file_meta['Folder']]['Size'] < self.backup_dataset_cap_size:
                 self.save_hash( file_meta, text )
                 self.dataset_hashes[file_meta['Folder']]['Size'] += file_meta['Size']
             
         else:
```

### Comparing `bittensor-4.0.0/bittensor/_dataset/dataset_mock.py` & `bittensor-4.1.0rc1/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_dataset/thread_queue.py` & `bittensor-4.1.0rc1/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_ipfs/ipfs_impl.py` & `bittensor-4.1.0rc1/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_keyfile/__init__.py` & `bittensor-4.1.0rc1/bittensor/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_keyfile/keyfile_impl.py` & `bittensor-4.1.0rc1/bittensor/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_logging/__init__.py` & `bittensor-4.1.0rc1/bittensor/_logging/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,31 +15,33 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import sys
-
-import argparse
 import copy
-
-from loguru import logger
-
+import torch
+import argparse
 import bittensor
 import bittensor.utils.codes as codes
 
+from loguru import logger
 logger = logger.opt(colors=True)
-
 # Remove default sink.
 try:
     logger.remove( 0 )
 except Exception:
     pass
 
+import re
+def _remove_loguru_ansi_directive( text:str ) -> str:
+    pattern = r'<.*?>'
+    return re.sub(pattern, '', text)
+
 class logging:
     """ Standardize logging for bittensor
     """
     __has_been_inited__:bool = False
     __debug_on__:bool = False
     __trace_on__:bool = False
     __std_sink__:int = None
@@ -88,14 +90,15 @@
             logger.remove( cls.__std_sink__ )
         if cls.__file_sink__ != None:
             logger.remove( cls.__file_sink__ )
 
         # Add filtered sys.stdout.
         cls.__std_sink__ = logger.add (
             sys.stdout,
+            level = 0,
             filter = cls.log_filter,
             colorize = True,
             enqueue = True,
             backtrace = True,
             diagnose = True,
             format = cls.log_formatter
         )
@@ -178,56 +181,48 @@
         """ Set trace back for the specific cls class 
         """
         if not cls.__has_been_inited__:
             cls()
         cls.__trace_on__ = trace_on
 
     @classmethod
+    def get_level( cls ) -> int:
+        return 5 if cls.__trace_on__ else 10 if cls.__debug_on__ else 20
+
+    @classmethod
     def log_filter(cls, record ):
         """ Filter out debug log if debug is not on
         """
-        if cls.__debug_on__ or cls.__trace_on__:
+        if cls.get_level() <= record["level"].no:
             return True
         else:
             return False
 
     @classmethod
     def log_save_filter(cls, record ):
-        if cls.__debug_on__ or cls.__trace_on__:
+        if cls.get_level() < record["level"].no:
             return True
         else:
-            return record["level"].name != "DEBUG"
+            return False
 
     @classmethod
     def log_formatter(cls, record):
         """ Log with different format according to record['extra']
         """
         extra = record['extra']
         if 'rpc' in extra:
-            log_format = "<blue>{time:YYYY-MM-DD HH:mm:ss.SSS}</blue> | " + extra['code_str'] + " | {extra[prefix]} | {extra[direction]} | {extra[arrow]} | {extra[uid_str]} | {extra[inputs]} | {extra[call_time]} | {extra[key_str]} | {extra[rpc_message]} | {extra[synapse]} \n"
-            return log_format
-        elif 'receptor' in extra:
-            log_format = "<blue>{time:YYYY-MM-DD HH:mm:ss.SSS}</blue> | " + extra['action'] + " | uid:{extra[uid]} | {extra[ip_str]} | hotkey:{extra[hotkey]} | coldkey:{extra[coldkey]} \n"
-            return log_format
+            return "<blue>{time:YYYY-MM-DD HH:mm:ss.SSS}</blue> | " + extra['code_str'] + " | {extra[prefix]} | {extra[direction]} | {extra[arrow]} | {extra[uid_str]} | {extra[inputs]} | {extra[call_time]} | {extra[key_str]} | {extra[rpc_message]} | {extra[synapse]} \n"
         else:
-            if cls.__trace_on__:
-                return "{time:YYYY-MM-DD HH:mm:ss.SSS} | <level>{level: ^16}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> | {message}\n"
-            else:
-                return "{time:YYYY-MM-DD HH:mm:ss.SSS} | <level>{level: ^16}</level> | {message}\n"
-
+            return "<blue>{time:YYYY-MM-DD HH:mm:ss.SSS}</blue> | <level>{level: ^16}</level> | {message}\n"
    
     @classmethod
     def log_save_formatter(cls, record):
         extra = record['extra']
         if 'rpc' in extra:
-            log_format = "{time:YYYY-MM-DD HH:mm:ss.SSS} | " + extra['code_str'] + " | {extra[prefix]} | {extra[direction]} | {extra[arrow]} | {extra[uid_str]} | {extra[inputs]} | {extra[call_time]} | {extra[key_str]} | {extra[rpc_message]} \n"
-            return log_format
-        if 'receptor' in extra:
-            log_format = "{time:YYYY-MM-DD HH:mm:ss.SSS} | " + extra['action'] + " | uid:{extra[uid]} | {extra[ip_str]} | hotkey:{extra[hotkey]} | coldkey:{extra[coldkey]} \n"
-            return log_format
+            return "{time:YYYY-MM-DD HH:mm:ss.SSS} | " + extra['code_str'] + " | {extra[prefix]} | {extra[direction]} | {extra[arrow]} | {extra[uid_str]} | {extra[inputs]} | {extra[call_time]} | {extra[key_str]} | {extra[rpc_message]} \n"
         else:
             if cls.__trace_on__:
                 return "{time:YYYY-MM-DD HH:mm:ss.SSS} | <level>{level: ^16}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> | {message}\n"
             else:
                 return "{time:YYYY-MM-DD HH:mm:ss.SSS} | <level>{level: ^16}</level> | {message}\n"
 
 
@@ -246,15 +241,15 @@
                  message:str = '',
                  synapse:'bittensor.Synapse' = None
         ):
         """ Debug logging for the communication between endpoints with axon/dendrite 
         """
 
         if axon:
-            prefix = "Axon"
+            prefix = "Synapse"
         else:
             prefix = "Dendrite"
         prefix = prefix.center(len('Dendrite'))
 
         if forward:
             direction = "Forward"
         else:
@@ -301,55 +296,64 @@
                     code_str=code_str, 
                     inputs = inputs, 
                     rpc_message = rpc_message,
                     synapse = synapse
         )
 
     @classmethod
-    def update_receptor_log( cls, endpoint: 'bittensor.Endpoint' ):
-        """ Debug logging for updating the connection with endpoint
+    def _format( cls, prefix:object, sufix:object = None ):
+        """ Format logging message
         """
-        logger.debug( 'endpoint', receptor=True, action = '<blue>' + 'Update'.center(16) + '</blue>', uid=str(endpoint.uid).center(4), hotkey=endpoint.hotkey,  coldkey=endpoint.coldkey, ip_str=endpoint.ip_str().center(27) )
+        if isinstance( prefix, torch.Tensor ):
+            prefix = prefix.detach()
+        if sufix != None:
+            if isinstance( sufix, torch.Tensor ):
+                sufix = 'shape: {}'.format( str(sufix.shape) ) + " data: {}".format( str( sufix.detach() ) )
+            else:
+                sufix = "{}".format( str( sufix ) )
+        else:
+            sufix = ""
+        log_msg = str( prefix ).ljust(30) + str( sufix )
+        return _remove_loguru_ansi_directive( log_msg )
 
     @classmethod
-    def success( cls, prefix:str, sufix:str ):
+    def success( cls, prefix:object, sufix:object = None ):
         """ Success logging 
         """
-        if not cls.__has_been_inited__:
-            cls()
-        prefix = prefix + ":"
-        prefix = prefix.ljust(20)
-        log_msg = prefix + sufix
-        logger.success( log_msg )
+        if not cls.__has_been_inited__: cls()
+        logger.success( cls._format( prefix, sufix ) )
 
     @classmethod
-    def warning( cls, prefix:str, sufix:str ):
+    def warning( cls, prefix:object, sufix:object = None ):
         """ Warning logging
         """
-        if not cls.__has_been_inited__:
-            cls()
-        prefix = prefix + ":"
-        prefix = prefix.ljust(20)
-        log_msg = prefix + sufix 
-        logger.warning( log_msg )
+        if not cls.__has_been_inited__: cls()
+        logger.warning( cls._format( prefix, sufix ) )
 
     @classmethod
-    def error( cls, prefix:str, sufix:str ):
+    def error( cls, prefix:object, sufix:object= None  ):
         """ Error logging
         """
-        if not cls.__has_been_inited__:
-            cls()
-        prefix = prefix + ":"
-        prefix = prefix.ljust(20)
-        log_msg = prefix + sufix 
-        logger.error( log_msg )
+        if not cls.__has_been_inited__: cls()
+        logger.error( cls._format( prefix, sufix ) )
 
     @classmethod
-    def info( cls, prefix:str, sufix:str ):
+    def info( cls, prefix:object, sufix:object = None ):
         """ Info logging
         """
-        if not cls.__has_been_inited__:
-            cls()
-        prefix = prefix + ":"
-        prefix = prefix.ljust(20)
-        log_msg = prefix + sufix
-        logger.info( log_msg )
+        if not cls.__has_been_inited__: cls()
+        logger.info( cls._format( prefix, sufix ) )
+
+
+    @classmethod
+    def debug( cls, prefix:object, sufix:object = None ):
+        """ Info logging
+        """
+        if not cls.__has_been_inited__: cls()
+        logger.debug( cls._format( prefix, sufix ) )
+
+    @classmethod
+    def trace( cls, prefix:object, sufix:object = None ):
+        """ Info logging
+        """
+        if not cls.__has_been_inited__: cls()
+        logger.trace( cls._format( prefix, sufix ) )
```

### Comparing `bittensor-4.0.0/bittensor/_metagraph/metagraph_mock.py` & `bittensor-4.1.0rc1/bittensor/_metagraph/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-""" Maintains mocked chain state as a torch.nn.Module.
+""" Maintains chain state as a torch.nn.Module.
 """
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
@@ -15,137 +14,184 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
 import os
-
-from typing import List
-from loguru import logger
-
-import pandas
+import json
 import torch
-from . import metagraph_impl
 import bittensor
+
+import torch.nn.functional as f
 import bittensor.utils.networking as net
-import scalecodec
-import binascii
-import random
-
-RAOPERTAO = 1000000000
-U64MAX = 18446744073709551615
-
-class MockMetagraph( metagraph_impl.Metagraph ):
-    r""" MOCKED VERSION OF THE METAGRAPH
-
-    """
-    def __init__( self ) -> None:
-        r""" Initializes a new Metagraph torch chain interface object.
-        """
-        super(MockMetagraph, self).__init__(network="mock", netuid=-1)
-        tn = torch.tensor( 2000, dtype=torch.int64 )
-        tblock = torch.tensor( 0, dtype=torch.int64 )
-        tuids = torch.tensor( list( range( 2000 )), dtype=torch.int64 )
-        tactive = torch.tensor( [ 1 for _ in range (2000)], dtype=torch.int64 )
-
-        ttotal_stake = torch.tensor( [ 1.0 for _ in range (2000) ], dtype=torch.float32 )
-
-        tranks = torch.tensor(  [1.0/2000 for _ in range (2000) ], dtype=torch.float32 )
-        ttrust = torch.tensor( [ 1.0 for _ in range (2000) ], dtype=torch.float32 )
-        tconsensus = torch.tensor( [1.0 for _ in range (2000) ], dtype=torch.float32 )
-        tvalidator_trust = torch.tensor( [ 1.0 for _ in range (2000) ], dtype=torch.float32 )
-        tincentive = torch.tensor( [1.0/2000 for _ in range (2000) ], dtype=torch.float32 )
-        temission = torch.tensor( [1.0/2000 for _ in range (2000) ], dtype=torch.float32 )
-        tdividends = torch.tensor( [1.0/2000 for _ in range (2000) ], dtype=torch.float32 )
-        tlast_update = torch.tensor( [0 for _ in range (2000) ], dtype=torch.int64 )
-        tvalidator_permit = torch.tensor( [False for _ in range (2000) ], dtype=torch.bool )
-        tbonds = torch.tensor( [ [1 for _ in range (2000) ] for _ in range (2000) ], dtype=torch.int64 )
-        tweights = torch.tensor( [ [1.0/2000 for _ in range (2000) ] for _ in range (2000) ], dtype=torch.float32 )
-        self._endpoint_objs = [ bittensor.endpoint.dummy() for _ in range (2000) ]
-        tendpoints = torch.tensor( [ end.to_tensor().tolist() for end in self._endpoint_objs ], dtype=torch.int64 )
-        self.n = torch.nn.Parameter( tn, requires_grad=False )
-        self.block = torch.nn.Parameter( tblock, requires_grad=False )
-        self.uids = torch.nn.Parameter( tuids, requires_grad=False )
-
-        self.stake = [{ 
-            scalecodec.ss58_encode( 
-                random.randint(0, U64MAX).to_bytes(32, 'big', signed=False), bittensor.__ss58_format__
-            ): bittensor.Balance.from_rao(1.0) for _ in range(random.randint(0, 10)) # random addresses to Balance(1.0)
-        } for _ in range(2000) ] # 1 dict of addresses -> Balance per uid
-        self.total_stake = torch.nn.Parameter( ttotal_stake, requires_grad=False )
-
-        self.ranks = torch.nn.Parameter( tranks, requires_grad=False )
-        self.trust = torch.nn.Parameter( ttrust, requires_grad=False )
-        self.consensus = torch.nn.Parameter( tconsensus, requires_grad=False )
-        self.validator_trust = torch.nn.Parameter( tvalidator_trust, requires_grad=False )
-        self.incentive = torch.nn.Parameter( tincentive, requires_grad=False )
-        self.emission = torch.nn.Parameter( temission, requires_grad=False )
-        self.dividends = torch.nn.Parameter( tdividends, requires_grad=False )
-        self.active = torch.nn.Parameter( tactive, requires_grad=False )
-        self.last_update = torch.nn.Parameter( tlast_update, requires_grad=False )
-        self.validator_permit = torch.nn.Parameter( tvalidator_permit, requires_grad=False )
-        self.weights = torch.nn.Parameter( tweights, requires_grad=False )
-        self.bonds = torch.nn.Parameter( tbonds, requires_grad=False )
-        self.endpoints = torch.nn.Parameter( tendpoints, requires_grad=False )
-
-        print("---- MOCKED METAGRAPH INITIALIZED ----")
-
-    def clear( self ) -> 'bittensor.Metagraph':
-        r""" Erases Metagraph state.
-        """
+
+from os import listdir
+from os.path import isfile, join
+from bittensor import Balance
+from typing import List, Optional, Dict, Union
+
+
+# Return directory path from network and netuid
+def get_save_dir(  network: str, netuid: int ) -> str: 
+    return os.path.expanduser(f"~/.bittensor/metagraphs/network-{str(network)}/netuid-{str(netuid)}/")
+
+def latest_block_path( dir_path: str ) -> int:
+        latest_block = -1
+        latest_file_full_path = None
+        for filename in listdir(dir_path):
+            full_path_filename = os.path.expanduser(join(dir_path, filename))
+            try:
+                block_number = int(filename.split('-')[1].split('.')[0])
+                if block_number > latest_block:
+                    latest_block = block_number
+                    latest_file_full_path = full_path_filename
+            except Exception as e:
+                pass
+        if not latest_file_full_path: 
+            raise ValueError( f"Metagraph not found at: {dir_path}" )
+        else:
+            return latest_file_full_path
+        
+class metagraph( torch.nn.Module ):
+
+    @property
+    def S(self) -> torch.FloatTensor: return self.total_stake
+    @property
+    def R(self) -> torch.FloatTensor: return self.ranks
+    @property
+    def I(self) -> torch.FloatTensor: return self.incentive
+    @property
+    def E(self) -> torch.FloatTensor: return self.emission
+    @property
+    def C(self) -> torch.FloatTensor: return self.consensus
+    @property
+    def T(self) -> torch.FloatTensor: return self.trust
+    @property
+    def Tv(self) -> torch.FloatTensor: return self.validator_trust
+    @property
+    def D(self) -> torch.FloatTensor: return self.dividends
+    @property
+    def B(self) -> torch.FloatTensor: return self.bonds
+    @property
+    def W(self) -> torch.FloatTensor: return self.weights
+    @property
+    def hotkeys( self ) -> List[str]: return [ axon.hotkey for axon in self.axons ]
+    @property
+    def coldkeys( self ) -> List[str]: return [ axon.coldkey for axon in self.axons ]
+    @property
+    def addresses( self ) -> List[str]: return [ axon.ip_str() for axon in self.axons ]
+
+    def __str__(self): return "Metagraph(netuid:{}, n:{}, block:{}, network:{})".format(self.netuid, self.n.item(), self.block.item(), self.network)
+        
+    def __repr__(self): return self.__str__()
+
+    def metadata(self) -> dict: return {"netuid": self.netuid, "n": self.n.item(), "block": self.block.item(), "network": self.network, "version": bittensor.__version__ }
+
+    def __init__(self, netuid: int, network: str = 'finney', lite:bool = True, sync: bool = True ) -> 'metagraph':    
+        super(metagraph, self).__init__()
+        self.netuid = netuid
+        self.network = network
         self.version = torch.nn.Parameter( torch.tensor( [ bittensor.__version_as_int__ ], dtype=torch.int64), requires_grad=False )
         self.n = torch.nn.Parameter( torch.tensor( [0], dtype=torch.int64), requires_grad = False )
-        self.tau = torch.nn.Parameter( torch.tensor( [1], dtype=torch.float32), requires_grad = False )
         self.block = torch.nn.Parameter( torch.tensor( [0], dtype=torch.int64), requires_grad = False )
-
-        self.stake = []
+        self.stake = torch.nn.Parameter( torch.tensor( [], dtype=torch.float32 ), requires_grad=False )
         self.total_stake = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
-
         self.ranks = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.trust = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.consensus = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.validator_trust = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.incentive = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.emission = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.dividends = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.active = torch.nn.Parameter(  torch.tensor( [], dtype=torch.int64), requires_grad=False )
         self.last_update = torch.nn.Parameter(  torch.tensor( [], dtype=torch.int64), requires_grad=False )
         self.validator_permit = torch.nn.Parameter(  torch.tensor( [], dtype=torch.bool), requires_grad=False )
         self.weights = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.bonds = torch.nn.Parameter(  torch.tensor( [], dtype=torch.int64), requires_grad=False )
-        self.endpoints = torch.nn.Parameter( torch.tensor( [], dtype=torch.int64), requires_grad=False )
         self.uids = torch.nn.Parameter( torch.tensor([], dtype = torch.int64),requires_grad=False )
-        self._endpoint_objs = None
+        self.axons = []
+        if sync:
+            self.sync( block = None, lite = lite )
+
+    def sync ( self, block: Optional[int] = None, lite: bool = True ) -> 'metagraph':
+        subtensor = bittensor.subtensor( network = self.network )
+        if lite:
+            self.neurons = subtensor.neurons_lite( netuid = self.netuid )
+        else:
+            self.neurons = subtensor.neurons( netuid = self.netuid )
+        self.lite = lite
+        self.n = torch.nn.Parameter( torch.tensor( len(self.neurons), dtype=torch.int64 ), requires_grad=False )
+        self.version = torch.nn.Parameter( torch.tensor( [bittensor.__version_as_int__], dtype=torch.int64 ), requires_grad=False )
+        self.block = torch.nn.Parameter( torch.tensor( subtensor.block, dtype=torch.int64 ), requires_grad=False )
+        self.uids = torch.nn.Parameter( torch.tensor( [ neuron.uid for neuron in self.neurons ], dtype=torch.int64 ), requires_grad=False )
+        self.trust = torch.nn.Parameter( torch.tensor( [ neuron.trust for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.consensus = torch.nn.Parameter( torch.tensor( [ neuron.consensus for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.incentive = torch.nn.Parameter( torch.tensor( [ neuron.incentive for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.dividends = torch.nn.Parameter( torch.tensor( [ neuron.dividends for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.ranks = torch.nn.Parameter( torch.tensor( [ neuron.rank for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.emission = torch.nn.Parameter( torch.tensor( [ neuron.emission for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.active = torch.nn.Parameter( torch.tensor( [ neuron.active for neuron in self.neurons ], dtype=torch.int64 ), requires_grad=False )
+        self.last_update = torch.nn.Parameter( torch.tensor( [ neuron.last_update for neuron in self.neurons ], dtype=torch.int64 ), requires_grad=False )
+        self.validator_permit = torch.nn.Parameter( torch.tensor( [ neuron.validator_permit for neuron in self.neurons ], dtype=torch.bool ), requires_grad=False )
+        self.validator_trust = torch.nn.Parameter( torch.tensor( [ neuron.validator_trust for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.total_stake = torch.nn.Parameter( torch.tensor( [ neuron.total_stake.tao for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.stake = torch.nn.Parameter( torch.tensor( [ neuron.stake for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
+        self.axons = [ n.axon_info for n in self.neurons ]
+        if not lite:
+            weights_array = []
+            for n in self.neurons:
+                w_uids, w_weights = zip(*n.weights)
+                weights_array.append( bittensor.utils.weight_utils.convert_weight_uids_and_vals_to_tensor( len(self.neurons), w_uids, w_weights ).tolist() )
+            self.weights = torch.nn.Parameter( torch.stack( weights_array ), requires_grad=False )
+        if not lite:
+            bonds_array = []
+            for n in self.neurons:
+                b_uids, b_bonds = zip(*n.bonds)
+                bonds_array.append( bittensor.utils.weight_utils.convert_bond_uids_and_vals_to_tensor( len(self.neurons), b_uids, b_bonds ).tolist() )
+            self.bonds = torch.nn.Parameter( torch.stack( bonds_array ), requires_grad=False )
+
+    def save( self ) -> 'metagraph':
+        r""" Saves this metagraph object's state_dict under bittensor root dir."""
+        save_directory = get_save_dir( self.network, self.netuid  )
+        os.makedirs( save_directory, exist_ok=True )
+        graph_file = save_directory + f'/block-{self.block.item()}.pt'
+        state_dict = self.state_dict()
+        state_dict['axons'] = self.axons
+        torch.save(state_dict, graph_file) 
+        state_dict = torch.load( graph_file )
         return self
 
-    def load( self, network:str = None  ) -> 'bittensor.Metagraph':
-        r""" Loads this metagraph object's state_dict from bittensor root dir.
-            Args: 
-                network: (:obj:`str`, required):
-                    Name of state_dict to load, defaults to kusanagi
-        """
-        try:
-            if network == None:
-                network = 'mock'
-            metagraph_path = '~/.bittensor/' + str(network) + '.pt'
-            metagraph_path = os.path.expanduser(metagraph_path)
-            if os.path.isfile(metagraph_path):
-                self.load_from_path( path = metagraph_path )
-            else:
-                logger.warning('Did not load metagraph from path: {}, file does not exist. Run metagraph.save() first.', metagraph_path)
-        except Exception as e:
-            logger.exception(e)
+    def load( self ) -> 'metagraph':
+        r""" Loads this metagraph object's state_dict from bittensor root dir. """
+        self.load_from_path( get_save_dir( self.network, self.netuid ) )
+    
+    def load_from_path( self, dir_path:str ) -> 'metagraph':
+        r""" Loads this metagraph object with state_dict under the specified path."""
+        graph_file = latest_block_path( dir_path )
+        state_dict = torch.load( graph_file )
+        # self.info = bittensor.SubnetInfo.from_parameter_dict( state_dict['info'] ) if 'info' in state_dict else None
+        # self.version = torch.nn.Parameter( state_dict['version'], requires_grad=False )
+        self.n = torch.nn.Parameter( state_dict['n'], requires_grad=False )
+        self.block = torch.nn.Parameter( state_dict['block'], requires_grad=False )
+        self.uids = torch.nn.Parameter( state_dict['uids'], requires_grad=False )
+        self.stake = torch.nn.Parameter( state_dict['stake'], requires_grad=False )
+        self.total_stake = torch.nn.Parameter( state_dict['total_stake'], requires_grad=False )
+        self.ranks = torch.nn.Parameter( state_dict['ranks'], requires_grad=False )
+        self.trust = torch.nn.Parameter( state_dict['trust'], requires_grad=False )
+        self.consensus = torch.nn.Parameter( state_dict['consensus'], requires_grad=False )
+        self.validator_trust = torch.nn.Parameter( state_dict['validator_trust'], requires_grad=False )
+        self.incentive = torch.nn.Parameter( state_dict['incentive'], requires_grad=False )
+        self.emission = torch.nn.Parameter( state_dict['emission'], requires_grad=False )
+        self.dividends = torch.nn.Parameter( state_dict['dividends'], requires_grad=False )
+        self.active = torch.nn.Parameter( state_dict['active'], requires_grad=False )
+        self.last_update = torch.nn.Parameter( state_dict['last_update'], requires_grad=False )
+        self.validator_permit = torch.nn.Parameter( state_dict['validator_permit'], requires_grad=False )
+        self.uids = torch.nn.Parameter( state_dict['uids'], requires_grad=False )
+        self.axons = state_dict['axons']
+        if 'weights' in state_dict:
+            self.weights = torch.nn.Parameter( state_dict['weights'], requires_grad=False )
+        if 'bonds' in state_dict:
+            self.bonds = torch.nn.Parameter( state_dict['bonds'], requires_grad=False )
         return self
 
-    def save( self, network:str = None ) -> 'bittensor.Metagraph':
-        r""" Saves this metagraph object's state_dict under bittensor root dir.
-            Args: 
-                network: (:obj:`str`, required):
-                    Name of state_dict, defaults to kusanagi
-        """
-        if network == None:
-            network = 'mock'
-        return self.save_to_path( path = '~/.bittensor/', filename = 'mock.pt')
 
-    def sync ( self, block: int = None, cached: bool = True ) -> 'bittensor.Metagraph':
-        return self
```

### Comparing `bittensor-4.0.0/bittensor/_neuron/audio/__init__.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # The MIT License (MIT)
-# Copyright © 2021 Yuma Rao
+# Copyright © 2023 Opentensor Foundation
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all copies or substantial portions of 
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-# DEALINGS IN THE SOFTWARE.
-
-# NOT AVAILABLE UNTIL BITTENSOR 4.0
+# DEALINGS IN THE SOFTWARE.
```

### Comparing `bittensor-4.0.0/bittensor/_neuron/text/log_utilities.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,20 +507,22 @@
         self.step_time.observe( step_time )
         self.gauges.labels('step_time').set( step_time )
         self.gauges.labels("loss").set( loss )
 
     def log_epoch_end(
         self,
         uid: int,
-        metagraph: 'bittensor.Metagraph'
+        metagraph: 'bittensor.Metagraph',
+        current_block: int,
     ):
         r""" All prometheus logging at the end of epoch. 
         """
         self.gauges.labels("epoch").inc()
         self.gauges.labels("set_weights").inc()
+        self.gauges.labels('set_weights_block').set(current_block)
         self.gauges.labels("stake").set( metagraph.total_stake[uid] )
         self.gauges.labels("rank").set( metagraph.ranks[uid] )
         self.gauges.labels("trust").set( metagraph.trust[uid] )
         self.gauges.labels("incentive").set( metagraph.incentive[uid] )
         self.gauges.labels("dividends").set( metagraph.dividends[uid] )
         self.gauges.labels("emission").set( metagraph.emission[uid] )
```

### Comparing `bittensor-4.0.0/bittensor/_prometheus/__init__.py` & `bittensor-4.1.0rc1/bittensor/_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-4.1.0rc1/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,99 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from bittensor._proto import bittensor_pb2 as bittensor_dot___proto_dot_bittensor__pb2
 
 
-class BittensorStub(object):
-    """Service definition for tensor processing servers.
-    """
+class TextPromptingStub(object):
+    """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Forward = channel.unary_unary(
-                '/Bittensor/Forward',
-                request_serializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.SerializeToString,
-                response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.FromString,
+                '/TextPrompting/Forward',
+                request_serializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingRequest.SerializeToString,
+                response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingResponse.FromString,
                 )
         self.Backward = channel.unary_unary(
-                '/Bittensor/Backward',
-                request_serializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.SerializeToString,
-                response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.FromString,
+                '/TextPrompting/Backward',
+                request_serializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingRequest.SerializeToString,
+                response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingResponse.FromString,
                 )
 
 
-class BittensorServicer(object):
-    """Service definition for tensor processing servers.
-    """
+class TextPromptingServicer(object):
+    """Missing associated documentation comment in .proto file."""
 
     def Forward(self, request, context):
-        """Forward tensor request. 
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Backward(self, request, context):
-        """Backward tensor request i.e. gradient.
-        """
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_BittensorServicer_to_server(servicer, server):
+def add_TextPromptingServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Forward': grpc.unary_unary_rpc_method_handler(
                     servicer.Forward,
-                    request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.FromString,
-                    response_serializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.SerializeToString,
+                    request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingRequest.FromString,
+                    response_serializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingResponse.SerializeToString,
             ),
             'Backward': grpc.unary_unary_rpc_method_handler(
                     servicer.Backward,
-                    request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.FromString,
-                    response_serializer=bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.SerializeToString,
+                    request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingRequest.FromString,
+                    response_serializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'Bittensor', rpc_method_handlers)
+            'TextPrompting', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class Bittensor(object):
-    """Service definition for tensor processing servers.
-    """
+class TextPrompting(object):
+    """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def Forward(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/Bittensor/Forward',
-            bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.SerializeToString,
-            bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.FromString,
+        return grpc.experimental.unary_unary(request, target, '/TextPrompting/Forward',
+            bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingRequest.SerializeToString,
+            bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Backward(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/Bittensor/Backward',
-            bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.SerializeToString,
-            bittensor_dot___proto_dot_bittensor__pb2.TensorMessage.FromString,
+        return grpc.experimental.unary_unary(request, target, '/TextPrompting/Backward',
+            bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingRequest.SerializeToString,
+            bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `bittensor-4.0.0/bittensor/_serializer/__init__.py` & `bittensor-4.1.0rc1/bittensor/_serializer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
             dtype = bittensor.proto.DataType.FLOAT64
         elif tdtype == torch.int32:
             dtype = bittensor.proto.DataType.INT32
         elif tdtype == torch.int64:
             dtype = bittensor.proto.DataType.INT64
         elif tdtype == torch.float16:
             dtype = bittensor.proto.DataType.FLOAT16
+        elif tdtype == torch.bool:
+            dtype = bittensor.proto.DataType.BOOL
         else:
             dtype = bittensor.proto.DataType.UNKNOWN
         return dtype
 
     @staticmethod
     def bittensor_dtype_to_torch_dtype(bdtype):
         """ Translates between bittensor.dtype and torch.dtypes.
@@ -104,14 +106,16 @@
             dtype = torch.float64
         elif bdtype == bittensor.proto.DataType.INT32:
             dtype = torch.int32
         elif bdtype == bittensor.proto.DataType.INT64:
             dtype=torch.int64
         elif bdtype == bittensor.proto.DataType.FLOAT16:
             dtype=torch.float16
+        elif bdtype == bittensor.proto.DataType.BOOL:
+            dtype=torch.bool
         else:
             raise bittensor.serializer.DeserializationException(
                 'Unknown bittensor.Dtype or no equivalent torch.dtype for bittensor.dtype = {}'
                 .format(bdtype))
         return dtype
 
     @staticmethod
```

### Comparing `bittensor-4.0.0/bittensor/_serializer/serializer_impl.py` & `bittensor-4.1.0rc1/bittensor/_serializer/serializer_impl.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     @staticmethod
     def empty():
         """Returns an empty bittensor.proto.Tensor message with the version"""
         torch_proto = bittensor.proto.Tensor(version= bittensor.__version_as_int__)
         return torch_proto
 
-    def serialize (self, tensor_obj: object, modality: bittensor.proto.Modality= bittensor.proto.Modality.TEXT, from_type: int = bittensor.proto.TensorType.TORCH) -> bittensor.proto.Tensor:
+    def serialize (self, tensor_obj: object, from_type: int = bittensor.proto.TensorType.TORCH ) -> bittensor.proto.Tensor:
         """Serializes a torch object to bittensor.proto.Tensor wire format.
 
         Args:
             tensor_obj (:obj:`object`, `required`): 
                 general tensor object i.e. torch.Tensor or tensorflow.Tensor
 
             from_type (`obj`: bittensor.proto.TensorType, `Optional`): 
@@ -55,28 +55,28 @@
                 Raised if the serializer does not implement the conversion between the passed type and a bittensor.proto.Tensor
 
             SerializationException: (Exception): 
                 Raised when the subclass serialization throws an error for the passed object.
         """
         # TODO (const): add deserialization types for torch -> tensorflow 
         if from_type == bittensor.proto.TensorType.TORCH:
-            return self.serialize_from_torch( torch_tensor = tensor_obj, modality = modality)
+            return self.serialize_from_torch( torch_tensor = tensor_obj )
 
         elif from_type == bittensor.proto.TensorType.NUMPY:
-            return self.serialize_from_numpy( numpy_tensor = tensor_obj, modality = modality)
+            return self.serialize_from_numpy( numpy_tensor = tensor_obj )
 
         elif from_type == bittensor.proto.TensorType.TENSORFLOW:
-            return self.serialize_from_tensorflow( tensorflow_tensor = tensor_obj, modality = modality)
+            return self.serialize_from_tensorflow( tensorflow_tensor = tensor_obj )
 
         else:
             raise bittensor.serializer.SerializationTypeNotImplementedException("Serialization from type {} not implemented.".format(from_type))
 
         raise NotImplementedError
 
-    def deserialize (self, tensor_pb2: bittensor.proto.Tensor, to_type: int) -> object:
+    def deserialize (self, tensor_pb2: bittensor.proto.Tensor, to_type: int = bittensor.proto.TensorType.TORCH ) -> object:
         """Serializes a torch object to bittensor.proto.Tensor wire format.
 
         Args:
             tensor_pb2 (`obj`: bittensor.proto.Tensor, `required`): 
                 Serialized tensor as bittensor.proto.proto. 
 
             to_type (`obj`: bittensor.proto.TensorType, `required`): 
@@ -102,52 +102,48 @@
 
         elif to_type == bittensor.proto.TensorType.TENSORFLOW:
             return self.deserialize_to_tensorflow( tensor_pb2 )
 
         else:
             raise bittensor.serializer.SerializationTypeNotImplementedException("Deserialization to type {} not implemented.".format(to_type))
 
-    def serialize_from_tensorflow(self, tensorflow_tensor: torch.Tensor, modality: bittensor.proto.Modality) -> bittensor.proto.Tensor:
+    def serialize_from_tensorflow( self, tensorflow_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ tensorflow -> bittensor.proto.Tensor """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
-    def serialize_from_torch(self, torch_tensor: torch.Tensor, modality: bittensor.proto.Modality) -> bittensor.proto.Tensor:
+    def serialize_from_torch( self, torch_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ torch -> bittensor.proto.Tensor """
         raise bittensor.serializer.SerializationTypeNotImplementedException
     
-    def serialize_from_numpy(self, numpy_tensor: torch.Tensor, modality: bittensor.proto.Modality) -> bittensor.proto.Tensor:
+    def serialize_from_numpy( self, numpy_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ numpy -> bittensor.proto.Tensor """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
-    def deserialize_to_torch(self, tensor_pb2: bittensor.proto.Tensor) -> torch.Tensor:
+    def deserialize_to_torch( self, tensor_pb2: bittensor.proto.Tensor ) -> torch.Tensor:
         """ bittensor.proto.Tensor -> torch """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
-    def deserialize_to_tensorflow(self, tensor_pb2: bittensor.proto.Tensor) -> object:
+    def deserialize_to_tensorflow( self, tensor_pb2: bittensor.proto.Tensor ) -> object:
         """ bittensor.proto.Tensor -> tensorflow """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
-    def deserialize_to_numpy(self, tensor_pb2: bittensor.proto.Tensor) -> object:
+    def deserialize_to_numpy( self, tensor_pb2: bittensor.proto.Tensor ) -> object:
         """ bittensor.proto.Tensor -> numpy """
         raise bittensor.serializer.SerializationTypeNotImplementedException
 
 
 class MSGPackSerializer( Serializer ):
     """ Make conversion between torch and bittensor.proto.torch
     """
-    def serialize_from_torch(self, torch_tensor: torch.Tensor, modality: bittensor.proto.Modality) -> bittensor.proto.Tensor:
+    def serialize_from_torch( self, torch_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ Serializes a torch.Tensor to an bittensor Tensor proto.
 
         Args:
             torch_tensor (torch.Tensor): 
                 Torch tensor to serialize.
-
-            modality (bittensor.proto.Modality): 
-                Datatype modality. i.e. TENSOR, TEXT, IMAGE
-
         Returns:
             bittensor.proto.Tensor: 
                 The serialized torch tensor as bittensor.proto.proto. 
         """
         dtype = bittensor.serializer.torch_dtype_to_bittensor_dtype(torch_tensor.dtype)
         shape = list(torch_tensor.shape)
         torch_numpy = torch_tensor.cpu().detach().numpy().copy()
@@ -155,15 +151,14 @@
         torch_proto = bittensor.proto.Tensor (
                                     version = bittensor.__version_as_int__,
                                     buffer = data_buffer,
                                     shape = shape,
                                     dtype = dtype,
                                     serializer = bittensor.proto.Serializer.MSGPACK,
                                     tensor_type = bittensor.proto.TensorType.TORCH,
-                                    modality = modality,
                                     requires_grad = torch_tensor.requires_grad
                                 )
         return torch_proto
 
     def deserialize_to_torch(self, torch_proto: bittensor.proto.Tensor) -> torch.Tensor:
         """Deserializes an bittensor.proto.Tensor to a torch.Tensor object.
 
@@ -181,24 +176,20 @@
         torch_object = torch.as_tensor(numpy_object).view(shape).requires_grad_(torch_proto.requires_grad)
         return torch_object.type(dtype)
 
 
 class CMPPackSerializer( Serializer ):
     """ Make conversion between torch and bittensor.proto.torch in float16
     """
-    def serialize_from_torch(self, torch_tensor: torch.Tensor, modality: bittensor.proto.Modality) -> bittensor.proto.Tensor:
+    def serialize_from_torch(self, torch_tensor: torch.Tensor ) -> bittensor.proto.Tensor:
         """ Serializes a torch.Tensor to an bittensor Tensor proto in float16
 
         Args:
             torch_tensor (torch.Tensor): 
                 Torch tensor to serialize.
-
-            modality (bittensor.proto.Modality): 
-                Datatype modality. i.e. TENSOR, TEXT, IMAGE
-
         Returns:
             bittensor.proto.Tensor: 
                 The serialized torch tensor as bittensor.proto.proto. 
         """
         dtype = bittensor.serializer.torch_dtype_to_bittensor_dtype(torch_tensor.dtype)
         shape = list(torch_tensor.shape)
         torch_numpy = torch_tensor.cpu().detach().half().numpy().copy()
@@ -206,15 +197,14 @@
         torch_proto = bittensor.proto.Tensor (
                                     version = bittensor.__version_as_int__,
                                     buffer = data_buffer,
                                     shape = shape,
                                     dtype = dtype,
                                     serializer = bittensor.proto.Serializer.CMPPACK,
                                     tensor_type = bittensor.proto.TensorType.TORCH,
-                                    modality = modality,
                                     requires_grad = torch_tensor.requires_grad
                                 )
         return torch_proto
 
     def deserialize_to_torch(self, torch_proto: bittensor.proto.Tensor) -> torch.Tensor:
         """Deserializes an bittensor.proto.Tensor to a torch.Tensor object.
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/__init__.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,36 +12,34 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
-import argparse
-import copy
-import os
 
+import os
+import copy
+import argparse
 import bittensor
+
 from loguru import logger
 from substrateinterface import SubstrateInterface
 from torch.cuda import is_available as is_cuda_available
-
-from bittensor.utils import strtobool_with_default
-from .naka_subtensor_impl import Subtensor as Nakamoto_subtensor
 from . import subtensor_impl, subtensor_mock
 
 logger = logger.opt(colors=True)
 
 GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME = 'node-subtensor'
 
 class subtensor:
     """Factory Class for both bittensor.Subtensor and Mock_Subtensor Classes
 
     The Subtensor class handles interactions with the substrate subtensor chain.
-    By default, the Subtensor class connects to the Nakamoto which serves as the main bittensor network.
+    By default, the Subtensor class connects to the Finney which serves as the main bittensor network.
     
     """
     
     def __new__(
             cls, 
             config: 'bittensor.config' = None,
             network: str = None,
@@ -181,15 +179,14 @@
             ## Registration args for CUDA registration.
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.use_cuda', '--' + prefix_str + 'cuda', '--' + prefix_str + 'cuda.use_cuda', default=argparse.SUPPRESS, help='''Set flag to use CUDA to register.''', action="store_true", required=False )
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.no_cuda', '--' + prefix_str + 'no_cuda', '--' + prefix_str + 'cuda.no_cuda', dest=prefix_str + 'subtensor.register.cuda.use_cuda', default=argparse.SUPPRESS, help='''Set flag to not use CUDA for registration''', action="store_false", required=False )
 
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.dev_id', '--' + prefix_str + 'cuda.dev_id',  type=int, nargs='+', default=argparse.SUPPRESS, help='''Set the CUDA device id(s). Goes by the order of speed. (i.e. 0 is the fastest).''', required=False )
             parser.add_argument( '--' + prefix_str + 'subtensor.register.cuda.TPB', '--' + prefix_str + 'cuda.TPB', type=int, default=bittensor.defaults.subtensor.register.cuda.TPB, help='''Set the number of Threads Per Block for CUDA.''', required=False )
 
-            parser.add_argument('--netuid', type=int, help='netuid for subnet to serve this neuron on', default=argparse.SUPPRESS)        
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
     @classmethod
     def add_defaults(cls, defaults ):
         """ Adds parser defaults to object from enviroment variables.
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/chain_data.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/chain_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             "type": "struct",
             "type_mapping": [
                 ["hotkey", "AccountId"],
                 ["coldkey", "AccountId"],
                 ["uid", "Compact<u16>"],
                 ["netuid", "Compact<u16>"],
                 ["active", "bool"],
-                ["axon_info", "AxonInfo"],
+                ["axon_info", "axon_info"],
                 ["prometheus_info", "PrometheusInfo"],
                 ["stake", "Vec<(AccountId, Compact<u64>)>"],
                 ["rank", "Compact<u16>"],
                 ["emission", "Compact<u64>"],
                 ["incentive", "Compact<u16>"],
                 ["consensus", "Compact<u16>"],
                 ["trust", "Compact<u16>"],
@@ -97,30 +97,30 @@
             "type": "struct",
             "type_mapping": [
                 ["hotkey", "AccountId"],
                 ["coldkey", "AccountId"],
                 ["uid", "Compact<u16>"],
                 ["netuid", "Compact<u16>"],
                 ["active", "bool"],
-                ["axon_info", "AxonInfo"],
+                ["axon_info", "axon_info"],
                 ["prometheus_info", "PrometheusInfo"],
                 ["stake", "Vec<(AccountId, Compact<u64>)>"],
                 ["rank", "Compact<u16>"],
                 ["emission", "Compact<u64>"],
                 ["incentive", "Compact<u16>"],
                 ["consensus", "Compact<u16>"],
                 ["trust", "Compact<u16>"],
                 ["validator_trust", "Compact<u16>"],
                 ["dividends", "Compact<u16>"],
                 ["last_update", "Compact<u64>"],
                 ["validator_permit", "bool"],
                 ["pruning_score", "Compact<u16>"]
             ],
         },
-        "AxonInfo": {
+        "axon_info": {
             "type": "struct",
             "type_mapping": [
                 ["block", "u64"],
                 ["version", "u32"],
                 ["ip", "u128"],
                 ["port", "u16"],
                 ["ip_type", "u8"],
@@ -200,15 +200,15 @@
     validator_trust: float
     dividends: float
     last_update: int
     validator_permit: bool
     weights: List[List[int]]
     bonds: List[List[int]]
     prometheus_info: 'PrometheusInfo'
-    axon_info: 'AxonInfo'
+    axon_info: 'axon_info'
     pruning_score: int
     is_null: bool = False
 
     @classmethod
     def fix_decoded_values(cls, neuron_info_decoded: Any) -> 'NeuronInfo':
         r""" Fixes the values of the NeuronInfo object.
         """
@@ -224,15 +224,15 @@
         neuron_info_decoded['emission'] = neuron_info_decoded['emission'] / RAOPERTAO
         neuron_info_decoded['incentive'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['incentive'])
         neuron_info_decoded['consensus'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['consensus'])
         neuron_info_decoded['trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['trust'])
         neuron_info_decoded['validator_trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['validator_trust'])
         neuron_info_decoded['dividends'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['dividends'])
         neuron_info_decoded['prometheus_info'] = PrometheusInfo.fix_decoded_values(neuron_info_decoded['prometheus_info'])
-        neuron_info_decoded['axon_info'] = AxonInfo.fix_decoded_values(neuron_info_decoded['axon_info'])
+        neuron_info_decoded['axon_info'] = bittensor.axon_info.from_neuron_info( neuron_info_decoded )
 
         return cls(**neuron_info_decoded)
     
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> 'NeuronInfo':
         r""" Returns a NeuronInfo object from a vec_u8.
         """
@@ -292,16 +292,16 @@
     @staticmethod
     def _neuron_dict_to_namespace(neuron_dict) -> 'NeuronInfo':
         # TODO: Legacy: remove?
         if neuron_dict['hotkey'] == '5C4hrfjw9DjXZTzV3MwzrrAr9P1MJhSrvWGWqi1eSuyUpnhM':
             return NeuronInfo._null_neuron()
         else:
             neuron = NeuronInfo( **neuron_dict )
-            neuron.stake = Balance.from_rao(neuron.total_stake)
             neuron.stake_dict = { hk: Balance.from_rao(stake) for hk, stake in neuron.stake.items() }
+            neuron.stake = Balance.from_rao(neuron.total_stake)
             neuron.total_stake = neuron.stake
             neuron.rank = neuron.rank / U16_MAX
             neuron.trust = neuron.trust / U16_MAX
             neuron.consensus = neuron.consensus / U16_MAX
             neuron.validator_trust = neuron.validator_trust / U16_MAX
             neuron.incentive = neuron.incentive / U16_MAX
             neuron.dividends = neuron.dividends / U16_MAX
@@ -331,15 +331,15 @@
     validator_trust: float
     dividends: float
     last_update: int
     validator_permit: bool
     #weights: List[List[int]]
     #bonds: List[List[int]] No weights or bonds in lite version
     prometheus_info: 'PrometheusInfo'
-    axon_info: 'AxonInfo'
+    axon_info: 'axon_info'
     pruning_score: int
     is_null: bool = False
 
     @classmethod
     def fix_decoded_values(cls, neuron_info_decoded: Any) -> 'NeuronInfoLite':
         r""" Fixes the values of the NeuronInfoLite object.
         """
@@ -356,16 +356,15 @@
         neuron_info_decoded['emission'] = neuron_info_decoded['emission'] / RAOPERTAO
         neuron_info_decoded['incentive'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['incentive'])
         neuron_info_decoded['consensus'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['consensus'])
         neuron_info_decoded['trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['trust'])
         neuron_info_decoded['validator_trust'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['validator_trust'])
         neuron_info_decoded['dividends'] = bittensor.utils.U16_NORMALIZED_FLOAT(neuron_info_decoded['dividends'])
         neuron_info_decoded['prometheus_info'] = PrometheusInfo.fix_decoded_values(neuron_info_decoded['prometheus_info'])
-        neuron_info_decoded['axon_info'] = AxonInfo.fix_decoded_values(neuron_info_decoded['axon_info'])
-
+        neuron_info_decoded['axon_info'] = bittensor.axon_info.from_neuron_info(neuron_info_decoded)
         return cls(**neuron_info_decoded)
     
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> 'NeuronInfoLite':
         r""" Returns a NeuronInfoLite object from a vec_u8.
         """
         if len(vec_u8) == 0:
@@ -438,30 +437,30 @@
             neuron.incentive = neuron.incentive / U16_MAX
             neuron.dividends = neuron.dividends / U16_MAX
             neuron.emission = neuron.emission / RAOPERTAO
                 
             return neuron
 
 @dataclass
-class AxonInfo:
+class axon_info:
     r"""
     Dataclass for axon info.
     """
     block: int
     version: int
     ip: str
     port: int
     ip_type: int
     protocol: int
     placeholder1: int # placeholder for future use
     placeholder2: int
 
     @classmethod
-    def fix_decoded_values(cls, axon_info_decoded: Dict) -> 'AxonInfo':
-        r""" Returns an AxonInfo object from an axon_info_decoded dictionary.
+    def fix_decoded_values(cls, axon_info_decoded: Dict) -> 'axon_info':
+        r""" Returns an axon_info object from an axon_info_decoded dictionary.
         """
         axon_info_decoded['ip'] = bittensor.utils.networking.int_to_ip(int(axon_info_decoded['ip']))
                                                                        
         return cls(**axon_info_decoded)
 
 @dataclass
 class PrometheusInfo:
@@ -639,15 +638,15 @@
             blocks_since_epoch = decoded['blocks_since_last_step'],
             tempo = decoded['tempo'],
             modality = decoded['network_modality'],
             connection_requirements = {
                 str(int(netuid)): bittensor.utils.U16_NORMALIZED_FLOAT(int(req)) for netuid, req in decoded['network_connect']
             },
             emission_value= decoded['emission_values'],
-            burn = Balance(0)#Balance.from_rao(decoded['burn'])
+            burn = Balance.from_rao(decoded['burn'])
         )
     
     def to_parameter_dict( self ) -> 'torch.nn.ParameterDict':
         r""" Returns a torch tensor of the subnet info.
         """
         return torch.nn.ParameterDict( 
             self.__dict__
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/errors.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import bittensor
 
 import torch
 import time
 from rich.prompt import Confirm
 from typing import List, Dict, Union, Optional
 import bittensor.utils.networking as net
+from bittensor.utils.registration import POWSolution, create_pow
 from ..errors import *
 
 def register_extrinsic (
     subtensor: 'bittensor.Subtensor',
     wallet: 'bittensor.Wallet',
     netuid: int,
     wait_for_inclusion: bool = False,
@@ -101,40 +102,40 @@
         bittensor.__console__.print(":satellite: Registering...({}/{})".format(attempts, max_allowed_attempts))
         # Solve latest POW.
         if cuda:
             if not torch.cuda.is_available():
                 if prompt:
                     bittensor.__console__.error('CUDA is not available.')
                 return False
-            pow_result = bittensor.utils.create_pow( subtensor, wallet, netuid, output_in_place, cuda, dev_id, TPB, num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose )
+            pow_result: Optional[POWSolution] = create_pow( subtensor, wallet, netuid, output_in_place, cuda, dev_id, TPB, num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose )
         else:
-            pow_result = bittensor.utils.create_pow( subtensor, wallet, netuid, output_in_place, num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose )
+            pow_result: Optional[POWSolution] = create_pow( subtensor, wallet, netuid, output_in_place, num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose )
 
         # pow failed
         if not pow_result:
             # might be registered already on this subnet
             if (wallet.is_registered( subtensor = subtensor, netuid = netuid )):
                 bittensor.__console__.print(f":white_heavy_check_mark: [green]Already registered on netuid:{netuid}[/green]")
                 return True
             
         # pow successful, proceed to submit pow to chain for registration
         else:
             with bittensor.__console__.status(":satellite: Submitting POW..."):
                 # check if pow result is still valid
-                while bittensor.utils.POWNotStale(subtensor, pow_result):
+                while not pow_result.is_stale(subtensor=subtensor):
                     with subtensor.substrate as substrate:
                         # create extrinsic call
                         call = substrate.compose_call( 
                             call_module='SubtensorModule',  
                             call_function='register', 
                             call_params={ 
                                 'netuid': netuid,
-                                'block_number': pow_result['block_number'], 
-                                'nonce': pow_result['nonce'], 
-                                'work': bittensor.utils.hex_bytes_to_u8_list( pow_result['work'] ), 
+                                'block_number': pow_result.block_number, 
+                                'nonce': pow_result.nonce, 
+                                'work': [int(byte_) for byte_ in pow_result.seal],
                                 'hotkey': wallet.hotkey.ss58_address, 
                                 'coldkey': wallet.coldkeypub.ss58_address,
                             } 
                         )
                         extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.hotkey )
                         response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion=wait_for_inclusion, wait_for_finalization=wait_for_finalization )
                         
@@ -268,8 +269,8 @@
                 bittensor.__console__.print("Balance:\n  [blue]{}[/blue] :arrow_right: [green]{}[/green]".format( old_balance, new_balance ))
                 is_registered = wallet.is_registered( subtensor = subtensor, netuid = netuid )
                 if is_registered:
                     bittensor.__console__.print(":white_heavy_check_mark: [green]Registered[/green]")
                     return True
                 else:
                     # neuron not found, try again
-                    bittensor.__console__.print(":cross_mark: [red]Unknown error. Neuron not found.[/red]")
+                    bittensor.__console__.print(":cross_mark: [red]Unknown error. Neuron not found.[/red]")
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/serving.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,45 +62,41 @@
     Returns:
         success (bool):
             flag is true if extrinsic was finalized or uncluded in the block. 
             If we did not wait for finalization / inclusion, the response is true.
     """
     # Decrypt hotkey
     wallet.hotkey
-
     params = {
         'version': bittensor.__version_as_int__,
         'ip': net.ip_to_int(ip),
         'port': port,
         'ip_type': net.ip_version(ip),
         'netuid': netuid,
         'coldkey': wallet.coldkeypub.ss58_address,
         'protocol': protocol,
         'placeholder1': placeholder1,
         'placeholder2': placeholder2,
     }
-
     with bittensor.__console__.status(":satellite: Checking Axon..."):
         neuron = subtensor.get_neuron_for_pubkey_and_subnet( wallet.hotkey.ss58_address, netuid = netuid )
         neuron_up_to_date = not neuron.is_null and params == {
             'version': neuron.axon_info.version,
             'ip': net.ip_to_int(neuron.axon_info.ip),
             'port': neuron.axon_info.port,
             'ip_type': neuron.axon_info.ip_type,
             'netuid': neuron.netuid,
             'coldkey': neuron.coldkey,
             'protocol': neuron.axon_info.protocol,
             'placeholder1': neuron.axon_info.placeholder1,
             'placeholder2': neuron.axon_info.placeholder2,
         }
-
     output = params.copy()
     output['coldkey'] = wallet.coldkeypub.ss58_address
     output['hotkey'] = wallet.hotkey.ss58_address
-
     if neuron_up_to_date:
         bittensor.__console__.print(f":white_heavy_check_mark: [green]Axon already Served[/green]\n"
                                     f"[green not bold]- coldkey: [/green not bold][white not bold]{output['coldkey']}[/white not bold] \n"
                                     f"[green not bold]- hotkey: [/green not bold][white not bold]{output['hotkey']}[/white not bold] \n"
                                     f"[green not bold]- Status: [/green not bold] |"
                                     f"[green not bold] ip: [/green not bold][white not bold]{net.int_to_ip(output['ip'])}[/white not bold] |"
                                     f"[green not bold] ip_type: [/green not bold][white not bold]{output['ip_type']}[/white not bold] |"
@@ -142,22 +138,25 @@
                     bittensor.__console__.print(':cross_mark: [green]Failed to Serve axon[/green] error: {}'.format(response.error_message))
                     return False
             else:
                 return True
 
 def serve_axon_extrinsic (
     subtensor: 'bittensor.Subtensor',
+    netuid: int,
     axon: 'bittensor.Axon',
     use_upnpc: bool = False,
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = True,
     prompt: bool = False,
 ) -> bool:
     r""" Serves the axon to the network.
     Args:
+        netuid ( int ):
+            The netuid being served on. 
         axon (bittensor.Axon):
             Axon to serve.
         use_upnpc (:type:bool, `optional`): 
             If true, the axon attempts port forward through your router before 
             subscribing.                
         wait_for_inclusion (bool):
             If set, waits for the extrinsic to enter a block before returning true, 
@@ -201,14 +200,14 @@
         external_ip = axon.external_ip
     
     # ---- Subscribe to chain ----
     serve_success = subtensor.serve(
             wallet = axon.wallet,
             ip = external_ip,
             port = external_port,
-            netuid = axon.netuid,
-            protocol = axon.protocol,
+            netuid = netuid,
+            protocol = 4,
             wait_for_inclusion = wait_for_inclusion,
             wait_for_finalization = wait_for_finalization,
             prompt = prompt
     )
     return serve_success
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,18 +105,21 @@
                     return True
                 else:
                     bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error:{}".format(response.error_message))
                     bittensor.logging.warning(  prefix = 'Set weights', sufix = '<red>Failed: </red>' + str(response.error_message) )
                     return False
 
         except Exception as e:
+
+            # TODO( devs ): lets remove all of the bittensor.__console__ calls and replace with loguru.
             bittensor.__console__.print(":cross_mark: [red]Failed[/red]: error:{}".format(e))
             bittensor.logging.warning(  prefix = 'Set weights', sufix = '<red>Failed: </red>' + str(e) )
             return False
 
+    # TODO( devs ): this code is dead.
     if response.is_success:
         bittensor.__console__.print("Set weights:\n[bold white]  weights: {}\n  uids: {}[/bold white ]".format( [float(v/4294967295) for v in weight_vals], weight_uids ))
         message = '<green>Success: </green>' + f'Set {len(uids)} weights, top 5 weights' + str(list(zip(uids.tolist()[:5], [round (w,4) for w in weights.tolist()[:5]] )))
         logger.debug('Set weights:'.ljust(20) +  message)
         return True
     
     return False
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/staking.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 from rich.prompt import Confirm
+from time import sleep
 from typing import List, Dict, Union, Optional
 from bittensor.utils.balance import Balance
 from ..errors import *
 
 def add_stake_extrinsic(
         subtensor: 'bittensor.Subtensor', 
         wallet: 'bittensor.wallet',
@@ -64,15 +65,15 @@
     wallet.coldkey
 
     # Default to wallet's own hotkey if the value is not passed.
     if hotkey_ss58 is None:
         hotkey_ss58 = wallet.hotkey.ss58_address 
 
     # Flag to indicate if we are using the wallet's own hotkey.
-    own_hotkey: bool = (wallet.hotkey.ss58_address == hotkey_ss58)
+    own_hotkey: bool
 
     with bittensor.__console__.status(":satellite: Syncing with chain: [white]{}[/white] ...".format(subtensor.network)):
         old_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
         # Get hotkey owner
         hotkey_owner = subtensor.get_hotkey_owner( hotkey_ss58 )
         own_hotkey = (wallet.coldkeypub.ss58_address == hotkey_owner)
         if not own_hotkey:
@@ -236,15 +237,15 @@
     else:
         # Staking more than 1000 rao to the wallets.
         ## Reduce the amount to stake to each wallet to keep the balance above 1000 rao.
         percent_reduction = 1 - (1000 / total_staking_rao)
         amounts = [Balance.from_tao(amount.tao * percent_reduction) for amount in amounts]
     
     successful_stakes = 0
-    for hotkey_ss58, amount, old_stake in zip(hotkey_ss58s, amounts, old_stakes):
+    for idx, (hotkey_ss58, amount, old_stake) in enumerate(zip(hotkey_ss58s, amounts, old_stakes)):
         staking_all = False
         # Convert to bittensor.Balance
         if amount == None:
             # Stake it all.
             staking_balance = bittensor.Balance.from_tao( old_balance.tao )
             staking_all = True
         else:
@@ -267,17 +268,25 @@
                 subtensor = subtensor,
                 wallet = wallet,
                 hotkey_ss58 = hotkey_ss58,
                 amount = staking_balance,
                 wait_for_inclusion = wait_for_inclusion,
                 wait_for_finalization = wait_for_finalization,
             )
-
+        
             if staking_response: # If we successfully staked.
                 # We only wait here if we expect finalization.
+
+                if idx < len(hotkey_ss58s) - 1:
+                    # Wait for tx rate limit.
+                    tx_rate_limit_blocks = subtensor.tx_rate_limit()
+                    if tx_rate_limit_blocks > 0:
+                        bittensor.__console__.print(":hourglass: [yellow]Waiting for tx rate limit: [white]{}[/white] blocks[/yellow]".format(tx_rate_limit_blocks))
+                        sleep( tx_rate_limit_blocks * 12 ) # 12 seconds per block
+
                 if not wait_for_finalization and not wait_for_inclusion:
                     bittensor.__console__.print(":white_heavy_check_mark: [green]Sent[/green]")
                     old_balance -= staking_balance
                     successful_stakes += 1
                     if staking_all:
                         # If staked all, no need to continue
                         break
@@ -352,15 +361,14 @@
             If the hotkey is not a delegate.
         NotRegisteredError:
             If the hotkey is not registered in any subnets.
 
     """
     # Decrypt keys,
     wallet.coldkey
-    wallet.hotkey
     
     hotkey_owner = subtensor.get_hotkey_owner( hotkey_ss58 )
     own_hotkey = (wallet.coldkeypub.ss58_address == hotkey_owner)
     if not own_hotkey:
         # We are delegating.
         # Verify that the hotkey is a delegate.
         if not subtensor.is_hotkey_delegate( hotkey_ss58 = hotkey_ss58 ):
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,14 @@
                 call_module='Balances',
                 call_function='transfer',
                 call_params={
                     'dest': dest, 
                     'value': transfer_balance.rao
                 }
             )
-
             extrinsic = substrate.create_signed_extrinsic( call = call, keypair = wallet.coldkey )
             response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
             # We only wait here if we expect finalization.
             if not wait_for_finalization and not wait_for_inclusion:
                 bittensor.__console__.print(":white_heavy_check_mark: [green]Sent[/green]")
                 return True
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 from rich.prompt import Confirm
+from time import sleep
 from typing import List, Dict, Union, Optional
 from bittensor.utils.balance import Balance
 from ..errors import * 
 
 def __do_remove_stake_single(
     subtensor: 'bittensor.Subtensor',
     wallet: 'bittensor.wallet',
@@ -241,15 +242,15 @@
         old_balance = subtensor.get_balance( wallet.coldkeypub.ss58_address )
 
         for hotkey_ss58 in hotkey_ss58s:
             old_stake = subtensor.get_stake_for_coldkey_and_hotkey( coldkey_ss58 = wallet.coldkeypub.ss58_address, hotkey_ss58 = hotkey_ss58 ) # Get stake on hotkey.
             old_stakes.append(old_stake) # None if not registered.
 
     successful_unstakes = 0
-    for hotkey_ss58, amount, old_stake in zip(hotkey_ss58s, amounts, old_stakes):
+    for idx, (hotkey_ss58, amount, old_stake) in enumerate(zip(hotkey_ss58s, amounts, old_stakes)):
         # Covert to bittensor.Balance
         if amount == None:
             # Unstake it all.
             unstaking_balance = old_stake
         elif not isinstance(amount, bittensor.Balance ):
             unstaking_balance = bittensor.Balance.from_tao( amount )
         else:
@@ -275,14 +276,22 @@
                     amount = unstaking_balance,
                     wait_for_inclusion = wait_for_inclusion,
                     wait_for_finalization = wait_for_finalization,
                 )
 
             if staking_response: # If we successfully unstaked.
                 # We only wait here if we expect finalization.
+
+                if idx < len(hotkey_ss58s) - 1:
+                    # Wait for tx rate limit.
+                    tx_rate_limit_blocks = subtensor.tx_rate_limit()
+                    if tx_rate_limit_blocks > 0:
+                        bittensor.__console__.print(":hourglass: [yellow]Waiting for tx rate limit: [white]{}[/white] blocks[/yellow]".format(tx_rate_limit_blocks))
+                        sleep( tx_rate_limit_blocks * 12 ) # 12 seconds per block
+
                 if not wait_for_finalization and not wait_for_inclusion:
                     bittensor.__console__.print(":white_heavy_check_mark: [green]Sent[/green]")
                     successful_unstakes += 1
                     continue
 
                 bittensor.__console__.print(":white_heavy_check_mark: [green]Finalized[/green]")
                 with bittensor.__console__.status(":satellite: Checking Balance on: [white]{}[/white] ...".format(subtensor.network)):
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/subtensor_impl.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/subtensor_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from retry import retry
 from typing import List, Dict, Union, Optional, Tuple
 from substrateinterface import SubstrateInterface
 from bittensor.utils.balance import Balance
 from bittensor.utils import U16_NORMALIZED_FLOAT, U64_MAX, RAOPERTAO, U16_MAX
 
 # Local imports.
-from .chain_data import NeuronInfo, AxonInfo, DelegateInfo, PrometheusInfo, SubnetInfo, NeuronInfoLite
+from .chain_data import NeuronInfo, axon_info, DelegateInfo, PrometheusInfo, SubnetInfo, NeuronInfoLite
 from .errors import *
 from .extrinsics.staking import add_stake_extrinsic, add_stake_multiple_extrinsic
 from .extrinsics.unstaking import unstake_extrinsic, unstake_multiple_extrinsic
 from .extrinsics.serving import serve_extrinsic, serve_axon_extrinsic
 from .extrinsics.registration import register_extrinsic, burned_register_extrinsic
 from .extrinsics.transfer import transfer_extrinsic
 from .extrinsics.set_weights import set_weights_extrinsic
@@ -274,21 +274,22 @@
         wait_for_finalization = True,
         prompt: bool = False,
     ) -> bool:
         return serve_extrinsic( self, wallet, ip, port, protocol, netuid , placeholder1, placeholder2, wait_for_inclusion, wait_for_finalization)
 
     def serve_axon (
         self,
+        netuid: int, 
         axon: 'bittensor.Axon',
         use_upnpc: bool = False,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False,
     ) -> bool:
-        return serve_axon_extrinsic( self, axon, use_upnpc, wait_for_inclusion, wait_for_finalization)
+        return serve_axon_extrinsic( self, netuid, axon, use_upnpc, wait_for_inclusion, wait_for_finalization)
 
     def serve_prometheus (
         self,
         wallet: 'bittensor.wallet',
         port: int,
         netuid: int,
         wait_for_inclusion: bool = False,
@@ -404,115 +405,115 @@
       
     #####################################
     #### Hyper parameter calls. ####
     #####################################
 
     """ Returns network Rho hyper parameter """
     def rho (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor( "Rho", block, [netuid] ).value
 
     """ Returns network Kappa hyper parameter """
     def kappa (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return U16_NORMALIZED_FLOAT( self.query_subtensor( "Kappa", block, [netuid] ).value )
 
     """ Returns network Difficulty hyper parameter """
     def difficulty (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor( "Difficulty", block, [netuid] ).value
     
     """ Returns network Burn hyper parameter """
     def burn (self, netuid: int, block: Optional[int] = None ) -> Optional[bittensor.Balance]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return bittensor.Balance.from_rao( self.query_subtensor( "Burn", block, [netuid] ).value )
 
     """ Returns network ImmunityPeriod hyper parameter """
     def immunity_period (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("ImmunityPeriod", block, [netuid] ).value
 
     """ Returns network ValidatorBatchSize hyper parameter """
     def validator_batch_size (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("ValidatorBatchSize", block, [netuid] ).value
 
     """ Returns network ValidatorPruneLen hyper parameter """
     def validator_prune_len (self, netuid: int, block: Optional[int] = None ) -> int:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("ValidatorPruneLen", block, [netuid] ).value
 
     """ Returns network ValidatorLogitsDivergence hyper parameter """
     def validator_logits_divergence (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return U16_NORMALIZED_FLOAT(self.query_subtensor("ValidatorLogitsDivergence", block, [netuid]).value)
 
     """ Returns network ValidatorSequenceLength hyper parameter """
     def validator_sequence_length (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("ValidatorSequenceLength", block, [netuid] ).value
 
     """ Returns network ValidatorEpochsPerReset hyper parameter """
     def validator_epochs_per_reset (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("ValidatorEpochsPerReset", block, [netuid] ).value
 
     """ Returns network ValidatorEpochLen hyper parameter """
     def validator_epoch_length (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("ValidatorEpochLen", block, [netuid] ).value
 
     """ Returns network ValidatorEpochLen hyper parameter """
     def validator_exclude_quantile (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return U16_NORMALIZED_FLOAT( self.query_subtensor("ValidatorExcludeQuantile", block, [netuid] ).value )
 
     """ Returns network MaxAllowedValidators hyper parameter """
     def max_allowed_validators(self, netuid: int, block: Optional[int] = None) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor( 'MaxAllowedValidators', block, [netuid] ).value
         
     """ Returns network MinAllowedWeights hyper parameter """
     def min_allowed_weights (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor("MinAllowedWeights", block, [netuid] ).value
 
     """ Returns network MaxWeightsLimit hyper parameter """
     def max_weight_limit (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return U16_NORMALIZED_FLOAT( self.query_subtensor('MaxWeightsLimit', block, [netuid] ).value )
 
     """ Returns network ScalingLawPower hyper parameter """
     def scaling_law_power (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor('ScalingLawPower', block, [netuid] ).value / 100.
 
     """ Returns network SynergyScalingLawPower hyper parameter """
     def synergy_scaling_law_power (self, netuid: int, block: Optional[int] = None ) -> Optional[float]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor('SynergyScalingLawPower', block, [netuid] ).value / 100.
 
     """ Returns network SubnetworkN hyper parameter """
     def subnetwork_n (self, netuid: int, block: Optional[int] = None ) -> int:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor('SubnetworkN', block, [netuid] ).value
 
     """ Returns network MaxAllowedUids hyper parameter """
     def max_n (self, netuid: int, block: Optional[int] = None ) -> Optional[int]:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor('MaxAllowedUids', block, [netuid] ).value
 
     """ Returns network BlocksSinceLastStep hyper parameter """
     def blocks_since_epoch (self, netuid: int, block: Optional[int] = None) -> int:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor('BlocksSinceLastStep', block, [netuid] ).value
 
     """ Returns network Tempo hyper parameter """
     def tempo (self, netuid: int, block: Optional[int] = None) -> int:
-        if not self.subnet_exists( netuid ): return None
+        if not self.subnet_exists( netuid, block ): return None
         return self.query_subtensor('Tempo', block, [netuid] ).value
 
     ##########################
     #### Account functions ###
     ##########################
 
     """ Returns the total stake held on a hotkey including delegative """
@@ -539,31 +540,31 @@
     def get_hotkey_owner( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[str]:
         if self.does_hotkey_exist( hotkey_ss58, block ):
             return self.query_subtensor( 'Owner', block, [hotkey_ss58 ] ).value
         else:
             return None
 
     """ Returns the axon information for this hotkey account """
-    def get_axon_info( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[AxonInfo]:
+    def get_axon_info( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[axon_info]:
         result = self.query_subtensor( 'Axons', block, [hotkey_ss58 ] )        
         if result != None:
-            return AxonInfo(
+            return axon_info(
                 ip = bittensor.utils.networking.ip_from_int( result.value.ip ),
                 ip_type = result.value.ip_type,
                 port = result.value.port,
                 protocol = result.value.protocol,
                 version = result.value.version,
                 placeholder1 = result.value.placeholder1,
                 placeholder2 = result.value.placeholder2,
             )
         else:
             return None
 
     """ Returns the prometheus information for this hotkey account """
-    def get_prometheus_info( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[AxonInfo]:
+    def get_prometheus_info( self, hotkey_ss58: str, block: Optional[int] = None ) -> Optional[axon_info]:
         result = self.query_subtensor( 'Prometheus', block, [hotkey_ss58 ] )        
         if result != None:
             return PrometheusInfo (
                 ip = bittensor.utils.networking.ip_from_int( result.value.ip ),
                 ip_type = result.value.ip_type,
                 port = result.value.port,
                 version = result.value.version,
@@ -589,14 +590,17 @@
         return bittensor.Balance.from_rao( self.query_subtensor( 'TotalIssuance', block ).value )
 
     def total_stake (self,block: Optional[int] = None ) -> 'bittensor.Balance':
         return bittensor.Balance.from_rao( self.query_subtensor( "TotalStake", block ).value )
 
     def serving_rate_limit (self, block: Optional[int] = None ) -> Optional[int]:
         return self.query_subtensor( "ServingRateLimit", block ).value
+    
+    def tx_rate_limit (self, block: Optional[int] = None ) -> Optional[int]:
+        return self.query_subtensor( "TxRateLimit", block ).value
 
     #####################################
     #### Network Parameters ####
     #####################################
 
     def subnet_exists( self, netuid: int, block: Optional[int] = None ) -> bool:
         return self.query_subtensor( 'NetworksAdded', block, [netuid] ).value  
@@ -934,53 +938,26 @@
         result = json_body['result']
 
         if result in (None, []):
             return []
         
         return NeuronInfoLite.list_from_vec_u8( result )
 
-    def metagraph( self, netuid: int, block: Optional[int] = None, lite: bool = True ) -> 'bittensor.Metagraph':
+    def metagraph( self, netuid: int, lite: bool = True ) -> 'bittensor.Metagraph':
         r""" Returns the metagraph for the subnet.
         Args:
             netuid ( int ):
                 The network uid of the subnet to query.
-            block (Optional[int]):
-                The block to create the metagraph for.
-                Defaults to latest.
             lite (bool, default=True):
                 If true, returns a metagraph using the lite sync (no weights, no bonds)
         Returns:
             metagraph ( `bittensor.Metagraph` ):
                 The metagraph for the subnet at the block.
-        """
-        status: Optional['rich.console.Status'] = None
-        if bittensor.__use_console__:
-            status = bittensor.__console__.status("Synchronizing Metagraph...", spinner="earth")
-            status.start()
-        
-        # Get neurons.
-        if lite:
-            neurons = self.neurons_lite( netuid = netuid, block = block )
-        else:
-            neurons = self.neurons( netuid = netuid, block = block )
-        
-        # Get subnet info.
-        subnet_info: Optional[bittensor.SubnetInfo] = self.get_subnet_info( netuid = netuid, block = block )
-        if subnet_info == None:
-            status.stop() if status else ...
-            raise ValueError('Could not find subnet info for netuid: {}'.format(netuid))
-
-        status.stop() if status else ...
-
-        # Create metagraph.
-        block_number = self.block
-        
-        metagraph = bittensor.metagraph.from_neurons( network = self.network, netuid = netuid, info = subnet_info, neurons = neurons, block = block_number )
-        print("Metagraph subtensor: ", self.network)
-        return metagraph
+        """        
+        return bittensor.metagraph( network = self.network, netuid = netuid, lite = lite )
 
     ################
     #### Transfer ##
     ################
 
 
     
@@ -1006,15 +983,15 @@
                         module='System',
                         storage_function='Account',
                         params=[address],
                         block_hash = None if block == None else substrate.get_block_hash( block )
                     )
             result = make_substrate_call_with_retry()
         except scalecodec.exceptions.RemainingScaleBytesNotEmptyException:
-            logger.critical("Your wallet it legacy formatted, you need to run btcli stake --ammount 0 to reformat it." )
+            bittensor.logging.error( "Your wallet it legacy formatted, you need to run btcli stake --ammount 0 to reformat it." )
             return Balance(1000)
         return Balance( result.value['data']['free'] )
 
     def get_current_block(self) -> int:
         r""" Returns the current block number on the chain.
         Returns:
             block_number (int):
```

### Comparing `bittensor-4.0.0/bittensor/_subtensor/subtensor_mock.py` & `bittensor-4.1.0rc1/bittensor/_subtensor/subtensor_mock.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,17 +69,18 @@
     """
 
     @classmethod
     def mock(cls):
 
         if not cls.global_mock_process_is_running():
             # Remove any old chain db
-            if os.path.exists(bittensor.__mock_chain_db__):
-                os.system(f'rm -rf {bittensor.__mock_chain_db__}')
-            _owned_mock_subtensor_process = cls.create_global_mock_process()
+            if os.path.exists(f'{bittensor.__mock_chain_db__}_{os.getpid()}'):
+                # Name mock chain db using pid to avoid conflicts while multiple processes are running.
+                os.system(f'rm -rf {bittensor.__mock_chain_db__}_{os.getpid()}')
+            _owned_mock_subtensor_process = cls.create_global_mock_process(os.getpid())
         else:
             _owned_mock_subtensor_process = None
             print ('Mock subtensor already running.')
 
         endpoint = bittensor.__mock_entrypoint__
         port = int(endpoint.split(':')[1])
         substrate = SubstrateInterface(
@@ -97,63 +98,69 @@
             # Is mocked, optionally has owned process for ref counting.
             _is_mocked = True,
             _owned_mock_subtensor_process = _owned_mock_subtensor_process
         )
         return subtensor
 
     @classmethod
-    def global_mock_process_is_running(cle) -> bool:
-        r""" If subtensor is running a mock process this kills the mock.
+    def global_mock_process_is_running(cls) -> bool:
+        r""" Check if the global mocked subtensor process is running under a process with the same name as this one.
         """
+        this_process = psutil.Process(os.getpid())
         for p in psutil.process_iter():
-            if p.name() == GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME and p.parent().pid == os.getpid() and p.status() != psutil.STATUS_ZOMBIE and p.status() != psutil.STATUS_DEAD:
-                print(f"Found process with name {p.name()}, parent {p.parent().pid} status {p.status()} and pid {p.pid}")
-                return True
+            if p.name() == GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME and p.status() != psutil.STATUS_ZOMBIE and p.status() != psutil.STATUS_DEAD:
+                if p.parent().name == this_process.name:
+                    print(f"Found process with name {p.name()}, parent {p.parent().pid} status {p.status()} and pid {p.pid}")
+                    return True
         return False
 
     @classmethod
     def kill_global_mock_process(self):
         r""" Kills the global mocked subtensor process even if not owned.
         """
         for p in psutil.process_iter():
             if p.name() == GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME and p.parent().pid == os.getpid() :
                 p.terminate()
                 p.kill()
         time.sleep(2) # Buffer to ensure the processes actually die
 
     @classmethod
-    def create_global_mock_process(self):
+    def create_global_mock_process(self, pid: int) -> 'subprocess.Popen[bytes]':
         r""" Creates a global mocked subtensor process running in the backgroun with name GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME.
         """
         try:
             operating_system = "OSX" if platform == "darwin" else "Linux"
-            path = "./tests/mock_subtensor/bin/{}/{}".format(operating_system, GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME)
+            path_root = "./tests/mock_subtensor"
+            path = "{}/bin/{}/{}".format(path_root, operating_system, GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME)
+            path_to_spec = "{}/specs/local_raw.json".format(path_root)
             
             ws_port = int(bittensor.__mock_entrypoint__.split(':')[1])
             print(f'MockSub ws_port: {ws_port}')
             
-            command_args = [ path ] + f'--chain dev --base-path {bittensor.__mock_chain_db__} --execution native --ws-max-connections 1000 --no-mdns --rpc-cors all'.split(' ') + \
+            command_args = [ path ] + f'--chain {path_to_spec} --base-path {bittensor.__mock_chain_db__}_{pid} --execution native --ws-max-connections 1000 --no-mdns --rpc-cors all'.split(' ') + \
                 f'--port {int(bittensor.get_random_unused_port())} --rpc-port {int(bittensor.get_random_unused_port())} --ws-port {ws_port}'.split(' ') + \
                 '--validator --alice'.split(' ')
             
             print ('Starting subtensor process with command: {}'.format(command_args))
             
             _mock_subtensor_process = subprocess.Popen(
                 command_args,
                 close_fds=True, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE )
             
             # Wait for the process to start. Check for errors.
             try:
                 # Timeout is okay.
-                error_code = _mock_subtensor_process.wait(timeout=3)
+                error_code = _mock_subtensor_process.wait(timeout=12)
             except subprocess.TimeoutExpired:
                 error_code = None
             
             if error_code is not None:
-                raise RuntimeError( 'Failed to start mocked subtensor process: {}'.format(error_code) )
+                # Get the error message.
+                error_message = _mock_subtensor_process.stderr.read().decode('utf-8')
+                raise RuntimeError( 'Failed to start mocked subtensor process: {}'.format(error_code), error_message )
 
             print ('Starting subtensor process with pid {} and name {}'.format(_mock_subtensor_process.pid, GLOBAL_SUBTENSOR_MOCK_PROCESS_NAME))
 
             errored: bool = True
             while errored:
                 errored = False
                 try:
@@ -260,15 +267,42 @@
 
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
             
-    def sudo_set_difficulty(self, netuid: int, difficulty: int) -> Tuple[bool, Optional[str]]:
+    def sudo_set_tx_rate_limit(self, netuid: int, tx_rate_limit: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
+        r""" Sets the tx rate limit of the subnet in the mock chain using the sudo key.
+        """
+        with self.substrate as substrate:
+            call = substrate.compose_call(
+                    call_module='SubtensorModule',
+                    call_function='sudo_set_tx_rate_limit',
+                    call_params = {
+                        'netuid': netuid,
+                        'tx_rate_limit': tx_rate_limit
+                    }
+                )
+
+            wrapped_call = self.wrap_sudo(call)
+
+            extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
+            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
+
+            if not wait_for_finalization:
+                return True, None
+            
+            response.process_events()
+            if response.is_success:
+                return True, None
+            else:
+                return False, response.error_message
+        
+    def sudo_set_difficulty(self, netuid: int, difficulty: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Sets the difficulty of the mock chain using the sudo key.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_set_difficulty',
                     call_params = {
@@ -276,23 +310,80 @@
                         'difficulty': difficulty
                     }
                 )
 
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
-            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = True, wait_for_finalization = True )
+            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
+
+            if not wait_for_finalization:
+                return True, None
+            
+            response.process_events()
+            if response.is_success:
+                return True, None
+            else:
+                return False, response.error_message
+            
+    def sudo_set_max_difficulty(self, netuid: int, max_difficulty: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
+        r""" Sets the max difficulty of the mock chain using the sudo key.
+        """
+        with self.substrate as substrate:
+            call = substrate.compose_call(
+                    call_module='SubtensorModule',
+                    call_function='sudo_set_max_difficulty',
+                    call_params = {
+                        'netuid': netuid,
+                        'max_difficulty': max_difficulty
+                    }
+                )
+
+            wrapped_call = self.wrap_sudo(call)
+
+            extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
+            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
+
+            if not wait_for_finalization:
+                return True, None
+            
+            response.process_events()
+            if response.is_success:
+                return True, None
+            else:
+                return False, response.error_message
+
+    def sudo_set_min_difficulty(self, netuid: int, min_difficulty: int, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
+        r""" Sets the min difficulty of the mock chain using the sudo key.
+        """
+        with self.substrate as substrate:
+            call = substrate.compose_call(
+                    call_module='SubtensorModule',
+                    call_function='sudo_set_min_difficulty',
+                    call_params = {
+                        'netuid': netuid,
+                        'min_difficulty': min_difficulty
+                    }
+                )
+
+            wrapped_call = self.wrap_sudo(call)
+
+            extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
+            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
+            if not wait_for_finalization:
+                return True, None
+            
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
 
-    def sudo_add_network(self, netuid: int, tempo: int = 0, modality: int = 0) -> Tuple[bool, Optional[str]]:
+    def sudo_add_network(self, netuid: int, tempo: int = 0, modality: int = 0, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Adds a network to the mock chain using the sudo key.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_add_network',
                     call_params = {
@@ -301,23 +392,26 @@
                         'modality': modality
                     }
                 )
 
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
-            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = True, wait_for_finalization = True )
+            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
+            if not wait_for_finalization:
+                return True, None
+            
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
             
-    def sudo_register(self, netuid: int, hotkey: str, coldkey: str, stake: int = 0, balance: int = 0) -> Tuple[bool, Optional[str]]:
+    def sudo_register(self, netuid: int, hotkey: str, coldkey: str, stake: int = 0, balance: int = 0, wait_for_inclusion: bool = True, wait_for_finalization: bool = True ) -> Tuple[bool, Optional[str]]:
         r""" Registers a neuron to the subnet using sudo.
         """
         with self.substrate as substrate:
             call = substrate.compose_call(
                     call_module='SubtensorModule',
                     call_function='sudo_register',
                     call_params = {
@@ -328,14 +422,17 @@
                         'balance': balance
                     }
                 )
 
             wrapped_call = self.wrap_sudo(call)
 
             extrinsic = substrate.create_signed_extrinsic( call = wrapped_call, keypair = self.sudo_keypair )
-            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = True, wait_for_finalization = True )
+            response = substrate.submit_extrinsic( extrinsic, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization )
 
+            if not wait_for_finalization:
+                return True, None
+            
             response.process_events()
             if response.is_success:
                 return True, None
             else:
                 return False, response.error_message
```

### Comparing `bittensor-4.0.0/bittensor/_threadpool/__init__.py` & `bittensor-4.1.0rc1/bittensor/_threadpool/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 .                   The maximum number of threads in thread pool
                 maxsize (default=-1, type=int)
                     The maximum number of tasks in the priority queue
         """        
         if config == None: 
             config = prioritythreadpool.config()
         config = copy.deepcopy( config )
-        config.axon.priority.max_workers = max_workers if max_workers != None else config.axon.priority.max_workers
-        config.axon.priority.maxsize = maxsize if maxsize != None else config.axon.priority.maxsize
+        config.priority.max_workers = max_workers if max_workers != None else config.priority.max_workers
+        config.priority.maxsize = maxsize if maxsize != None else config.priority.maxsize
 
         prioritythreadpool.check_config( config )
-        return priority_thread_pool_impl.PriorityThreadPoolExecutor(maxsize = config.axon.priority.maxsize, max_workers = config.axon.priority.max_workers)
+        return priority_thread_pool_impl.PriorityThreadPoolExecutor(maxsize = config.priority.maxsize, max_workers = config.priority.max_workers)
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
         try:
-            parser.add_argument('--' + prefix_str + 'axon.priority.max_workers', type = int, help='''maximum number of threads in thread pool''', default = bittensor.defaults.axon.priority.max_workers)
-            parser.add_argument('--' + prefix_str + 'axon.priority.maxsize', type=int, help='''maximum size of tasks in priority queue''', default = bittensor.defaults.axon.priority.maxsize)  
+            parser.add_argument('--' + prefix_str + 'priority.max_workers', type = int, help='''maximum number of threads in thread pool''', default = bittensor.defaults.priority.max_workers)
+            parser.add_argument('--' + prefix_str + 'priority.maxsize', type=int, help='''maximum size of tasks in priority queue''', default = bittensor.defaults.priority.maxsize)  
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
     @classmethod   
     def help(cls):
         """ Print help to stdout
@@ -71,27 +71,27 @@
         print (cls.__new__.__doc__)
         parser.print_help()
 
     @classmethod   
     def add_defaults(cls, defaults):
         """ Adds parser defaults to object from enviroment variables.
         """
-        defaults.axon = bittensor.Config()
-        defaults.axon.priority = bittensor.Config()
-        defaults.axon.priority.max_workers = os.getenv('BT_AXON_PRIORITY_MAX_WORKERS') if os.getenv('BT_AXON_PRIORITY_MAX_WORKERS') != None else 5
-        defaults.axon.priority.maxsize = os.getenv('BT_AXON_PRIORITY_MAXSIZE') if os.getenv('BT_AXON_PRIORITY_MAXSIZE') != None else 10
+        defaults.priority = bittensor.Config()
+        defaults.priority = bittensor.Config()
+        defaults.priority.max_workers = os.getenv('BT_PRIORITY_MAX_WORKERS') if os.getenv('BT_PRIORITY_MAX_WORKERS') != None else 5
+        defaults.priority.maxsize = os.getenv('BT_PRIORITY_MAXSIZE') if os.getenv('BT_PRIORITY_MAXSIZE') != None else 10
     
     @classmethod   
     def config(cls) -> 'bittensor.Config':
         """ Get config from the argument parser
             Return: bittensor.config object 
         """
         parser = argparse.ArgumentParser()
         prioritythreadpool.add_args( parser )
         return bittensor.config( parser )
     
     @classmethod   
     def check_config(cls, config: 'bittensor.Config' ):
         """ Check config for threadpool worker number and size
         """
-        assert isinstance(config.axon.priority.max_workers, int), 'axon.priority.max_workers must be a int'
-        assert isinstance(config.axon.priority.maxsize, int), 'axon.priority.maxsize must be a int'
+        assert isinstance(config.priority.max_workers, int), 'priority.max_workers must be a int'
+        assert isinstance(config.priority.maxsize, int), 'priority.maxsize must be a int'
```

### Comparing `bittensor-4.0.0/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-4.1.0rc1/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_tokenizer/__init__.py` & `bittensor-4.1.0rc1/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/_wallet/__init__.py` & `bittensor-4.1.0rc1/bittensor/_wallet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Create and init wallet that stores coldkey and hotkey
-"""
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -20,17 +18,15 @@
 import argparse
 import copy
 from distutils.util import strtobool
 import os
 
 import bittensor
 from bittensor.utils import strtobool
-
 from . import wallet_impl, wallet_mock
-from .naka_wallet_impl import Wallet as naka_wallet
 
 class wallet:
     """ Create and init wallet that stores hot and coldkey
     """
     @classmethod
     def mock(cls) -> 'bittensor.Wallet':
         return wallet( name='mock' )
```

### Comparing `bittensor-4.0.0/bittensor/_wallet/naka_wallet_impl.py` & `bittensor-4.1.0rc1/bittensor/_wallet/wallet_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION 
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import sys
 from types import SimpleNamespace
-from typing import Optional, Union
+from typing import Optional, Union, List, Tuple, Dict, overload
 
 import bittensor
 from bittensor.utils import is_valid_bittensor_address_or_public_key
 from substrateinterface import Keypair
+from substrateinterface.base import is_valid_ss58_address
 from termcolor import colored
 
 
 def display_mnemonic_msg( keypair : Keypair, key_type : str ):
     """ Displaying the mnemonic and warning message to keep mnemonic safe
     """
     mnemonic = keypair.mnemonic
@@ -76,160 +77,194 @@
 
     def __str__(self):
         return "Wallet ({}, {}, {})".format(self.name, self.hotkey_str, self.path)
     
     def __repr__(self):
         return self.__str__()
 
-    @property
-    def neuron(self) -> SimpleNamespace:
-        return self.get_neuron()
+    def neuron(self, netuid: int) -> Optional['bittensor.NeuronInfo']:
+        return self.get_neuron(netuid=netuid)
 
-    @property
-    def trust(self) -> SimpleNamespace:
-        return self.get_neuron().trust
+    def trust(self, netuid: int) -> Optional[float]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.trust
 
-    @property
-    def rank(self) -> SimpleNamespace:
-        return self.get_neuron().rank
+    def validator_trust(self, netuid: int) -> Optional[float]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.validator_trust
 
-    @property
-    def incentive(self) -> SimpleNamespace:
-        return self.get_neuron().incentive
+    def rank(self, netuid: int) -> Optional[float]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.rank
 
-    @property
-    def dividends(self) -> SimpleNamespace:
-        return self.get_neuron().dividends
+    def incentive(self, netuid: int) -> Optional[float]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.incentive
 
-    @property
-    def consensus(self) -> SimpleNamespace:
-        return self.get_neuron().consensus
+    def dividends(self, netuid: int) -> Optional[float]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.dividends
 
-    @property
-    def inflation(self) -> SimpleNamespace:
-        return self.get_neuron().inflation
+    def consensus(self, netuid: int) -> Optional[float]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.consensus
 
-    @property
-    def ip(self) -> SimpleNamespace:
-        return self.get_neuron().ip
+    def last_update(self, netuid: int) -> Optional[int]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.last_update
 
-    @property
-    def last_update(self) -> SimpleNamespace:
-        return self.get_neuron().last_update
+    def validator_permit(self, netuid: int) -> Optional[bool]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.validator_permit
 
-    @property
-    def weights(self) -> SimpleNamespace:
-        return self.get_neuron().weights
+    def weights(self, netuid: int) -> Optional[List[List[int]]]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.weights
 
-    @property
-    def bonds(self) -> SimpleNamespace:
-        return self.get_neuron().bonds
+    def bonds(self, netuid: int) -> Optional[List[List[int]]]:
+        neuron = self.get_neuron(netuid=netuid)
+        if neuron is None:
+            return None
+        return neuron.bonds
 
-    @property
-    def uid(self) -> SimpleNamespace:
-        return self.get_uid()
+    def uid(self, netuid: int) -> int:
+        return self.get_uid(netuid=netuid)
 
     @property
-    def stake(self) -> SimpleNamespace:
+    def stake(self) -> 'bittensor.Balance':
         return self.get_stake()
 
     @property
-    def balance(self) -> SimpleNamespace:
+    def balance(self) -> 'bittensor.Balance':
         return self.get_balance()
 
-    def is_registered( self, subtensor: 'bittensor.Subtensor' = None, netuid: int = None ) -> bool:
+    def is_registered( self, subtensor: Optional['bittensor.Subtensor'] = None, netuid: Optional[int] = None ) -> bool:
         """ Returns true if this wallet is registered.
             Args:
-                subtensor( 'bittensor.Subtensor' ):
+                subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
                     Determines which network we check for registration.
+                netuid ( Optional[int] ):
+                    The network uid to check for registration.
+                    Default is None, which checks any subnetwork.
             Return:
                 is_registered (bool):
                     Is the wallet registered on the chain.
         """
-        if subtensor == None: subtensor = bittensor.subtensor()
-        return subtensor.is_hotkey_registered( self.hotkey.ss58_address )
+        if subtensor == None: subtensor = bittensor.subtensor(self.config)
+        if subtensor.network == 'nakamoto':
+            neuron = subtensor.neuron_for_pubkey( ss58_hotkey = self.hotkey.ss58_address )
+            return not neuron.is_null
+        else:
+            # default to finney
+            if netuid == None:
+                return subtensor.is_hotkey_registered_any( self.hotkey.ss58_address )
+            else:
+                return subtensor.is_hotkey_registered_on_subnet( self.hotkey.ss58_address, netuid = netuid )
+        
 
-    def get_neuron ( self, subtensor: 'bittensor.Subtensor' = None ) -> Union[ SimpleNamespace, None] :
+    def get_neuron ( self, netuid: int, subtensor: Optional['bittensor.Subtensor'] = None ) -> Optional['bittensor.NeuronInfo'] :
         """ Returns this wallet's neuron information from subtensor.
             Args:
-                subtensor( 'bittensor.Subtensor' ):
+                netuid (int):
+                    The network uid of the subnet to query.
+                subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
             Return:
-                neuron (Union[ SimpleNamespace, None ]):
+                neuron (Union[ NeuronInfo, None ]):
                     neuron account on the chain or None if you are not registered.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
-        if not self.is_registered(subtensor=subtensor): 
+        if not self.is_registered(netuid = netuid, subtensor=subtensor): 
             print(colored('This wallet is not registered. Call wallet.register() before this function.','red'))
             return None
-        neuron = subtensor.neuron_for_wallet( self )
+        neuron = subtensor.neuron_for_wallet( self, netuid = netuid )
         return neuron
 
-    def get_uid ( self, subtensor: 'bittensor.Subtensor' = None, netuid: int = None ) -> int:
+    def get_uid ( self, netuid: int, subtensor: Optional['bittensor.Subtensor'] = None ) -> int:
         """ Returns this wallet's hotkey uid or -1 if the hotkey is not subscribed.
             Args:
-                subtensor( 'bittensor.Subtensor' ):
+                netuid (int):
+                    The network uid of the subnet to query.
+                subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
             Return:
                 uid (int):
                     Network uid or -1 if you are not registered.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
-        if not self.is_registered(subtensor=subtensor): 
+        if not self.is_registered(netuid = netuid, subtensor=subtensor): 
             print(colored('This wallet is not registered. Call wallet.register() before this function.','red'))
             return -1
-        neuron = self.get_neuron(subtensor = subtensor)
+        neuron = self.get_neuron(netuid = netuid, subtensor = subtensor)
         if neuron.is_null:
             return -1
         else:
             return neuron.uid
 
-    def get_stake ( self, subtensor: 'bittensor.Subtensor' = None ) -> 'bittensor.Balance':
+    def get_stake ( self, subtensor: Optional['bittensor.Subtensor'] = None ) -> 'bittensor.Balance':
         """ Returns this wallet's staking balance from passed subtensor connection.
             Args:
-                subtensor( 'bittensor.Subtensor' ):
+                subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
             Return:
                 balance (bittensor.utils.balance.Balance):
                     Stake account balance.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
-        if not self.is_registered(subtensor=subtensor): 
+        stake = subtensor.get_stake_for_coldkey_and_hotkey( hotkey_ss58 = self.hotkey.ss58_address, coldkey_ss58 = self.coldkeypub.ss58_address )
+        if not stake: # Not registered.
             print(colored('This wallet is not registered. Call wallet.register() before this function.','red'))
             return bittensor.Balance(0)
-        neuron = self.get_neuron(subtensor = subtensor)
-        if neuron.is_null:
-            return bittensor.Balance(0)
-        else:
-            return bittensor.Balance.from_tao(neuron.stake)
+        
+        return stake
 
-    def get_balance( self, subtensor: 'bittensor.Subtensor' = None ) -> 'bittensor.Balance':
+    def get_balance( self, subtensor: Optional['bittensor.Subtensor'] = None ) -> 'bittensor.Balance':
         """ Returns this wallet's coldkey balance from passed subtensor connection.
             Args:
-                subtensor( 'bittensor.Subtensor' ):
+                subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
             Return:
                 balance (bittensor.utils.balance.Balance):
                     Coldkey balance.
         """
         if subtensor == None: subtensor = bittensor.subtensor()
         return subtensor.get_balance(address = self.coldkeypub.ss58_address)
 
     def reregister(
         self,
-        subtensor: 'bittensor.Subtensor' = None,
+        netuid: int,
+        subtensor: Optional['bittensor.Subtensor'] = None,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
-        prompt: bool = False,
-        netuid: int = None, 
+        prompt: bool = False
     ) -> Optional['bittensor.Wallet']:
         """ Re-register this wallet on the chain.
             Args:
-                subtensor( 'bittensor.Subtensor' ):
+                netuid (int):
+                    The network uid of the subnet to register on.
+                subtensor( Optional['bittensor.Subtensor'] ):
                     Bittensor subtensor connection. Overrides with defaults if None.
                 wait_for_inclusion (bool):
                     if set, waits for the extrinsic to enter a block before returning true, 
                     or returns false if the extrinsic fails to enter the block within the timeout.   
                 wait_for_finalization (bool):
                     if set, waits for the extrinsic to be finalized on the chain before returning true,
                     or returns false if the extrinsic fails to be finalized within the timeout.
@@ -238,21 +273,22 @@
                 
             Return:
                 wallet (bittensor.Wallet):
                     This wallet.
         """
         if subtensor == None:
             subtensor = bittensor.subtensor()
-        if not self.is_registered(subtensor=subtensor):
+        if not self.is_registered(netuid = netuid, subtensor=subtensor):
             # Check if the wallet should reregister
             if not self.config.wallet.get('reregister'):
                 sys.exit(0)
 
             self.register(
                 subtensor = subtensor,
+                netuid = netuid,
                 prompt = prompt,
                 TPB = self.config.subtensor.register.cuda.get('TPB', None),
                 update_interval = self.config.subtensor.register.cuda.get('update_interval', None),
                 num_processes = self.config.subtensor.register.get('num_processes', None),
                 cuda = self.config.subtensor.register.cuda.get('use_cuda', bittensor.defaults.subtensor.register.cuda.use_cuda),
                 dev_id = self.config.subtensor.register.cuda.get('dev_id', None),
                 wait_for_inclusion = wait_for_inclusion,
@@ -261,31 +297,33 @@
                 log_verbose = self.config.subtensor.register.get('verbose', bittensor.defaults.subtensor.register.verbose),
             )
 
         return self
 
     def register ( 
             self, 
-            subtensor: 'bittensor.Subtensor' = None, 
+            netuid: int,
+            subtensor: Optional['bittensor.Subtensor'] = None, 
             wait_for_inclusion: bool = False,
             wait_for_finalization: bool = True,
             prompt: bool = False,
             max_allowed_attempts: int = 3,
             cuda: bool = False,
             dev_id: int = 0,
             TPB: int = 256,
             num_processes: Optional[int] = None,
             update_interval: Optional[int] = None,
             output_in_place: bool = True,
             log_verbose: bool = False,
-            netuid: int = None
         ) -> 'bittensor.Wallet':
         """ Registers the wallet to chain.
         Args:
-            subtensor( 'bittensor.Subtensor' ):
+            netuid (int):
+                The network uid of the subnet to register on.
+            subtensor( Optional['bittensor.Subtensor'] ):
                 Bittensor subtensor connection. Overrides with defaults if None.
             wait_for_inclusion (bool):
                 If set, waits for the extrinsic to enter a block before returning true, 
                 or returns false if the extrinsic fails to enter the block within the timeout.   
             wait_for_finalization (bool):
                 If set, waits for the extrinsic to be finalized on the chain before returning true,
                 or returns false if the extrinsic fails to be finalized within the timeout.
@@ -322,23 +360,24 @@
             output_in_place = output_in_place,
             cuda=cuda,
             dev_id=dev_id,
             TPB=TPB,
             num_processes=num_processes,
             update_interval=update_interval,
             log_verbose=log_verbose,
+            netuid = netuid,
         )
         
         return self
 
     def add_stake( self, 
         amount: Union[float, bittensor.Balance] = None, 
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
-        subtensor: 'bittensor.Subtensor' = None,
+        subtensor: Optional['bittensor.Subtensor'] = None,
         prompt: bool = False
     ) -> bool:
         """ Stakes tokens from this wallet's coldkey onto it's hotkey.
             Args:
                 amount_tao (float):
                     amount of tao to stake or bittensor balance object. If None, stakes all available balance.
                 wait_for_inclusion (bool):
@@ -359,15 +398,15 @@
         if subtensor == None: subtensor = bittensor.subtensor()
         return subtensor.add_stake( wallet = self, amount = amount, wait_for_inclusion = wait_for_inclusion, wait_for_finalization = wait_for_finalization, prompt=prompt )
 
     def remove_stake( self, 
         amount: Union[float, bittensor.Balance] = None, 
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
-        subtensor: 'bittensor.Subtensor' = None,
+        subtensor: Optional['bittensor.Subtensor'] = None,
         prompt: bool = False,
     ) -> bool:
         """ Removes stake from this wallet's hotkey and moves them onto it's coldkey balance.
             Args:
                 amount_tao (float):
                     amount of tao to unstake or bittensor balance object. If None, unstakes all available hotkey balance.
                 wait_for_inclusion (bool):
@@ -390,15 +429,15 @@
 
     def transfer( 
         self, 
         dest:str,
         amount: Union[float, bittensor.Balance] , 
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
-        subtensor: 'bittensor.Subtensor' = None,
+        subtensor: Optional['bittensor.Subtensor'] = None,
         prompt: bool = False,
     ) -> bool:
         """ Transfers Tao from this wallet's coldkey to the destination address.
             Args:
                 dest (`type`:str, required):
                     The destination address either encoded as a ss58 or ed255 public-key string of 
                     secondary account.
@@ -629,31 +668,14 @@
         """
         mnemonic = Keypair.generate_mnemonic( n_words)
         keypair = Keypair.create_from_mnemonic(mnemonic)
         display_mnemonic_msg( keypair, "hotkey" )
         self.set_hotkey( keypair, encrypt=use_password, overwrite = overwrite)
         return self
 
-    def regen_coldkey( self, mnemonic: Optional[Union[list, str]]=None, seed: Optional[str]=None, use_password: bool = True,  overwrite:bool = False) -> 'Wallet':
-        """ Regenerates the coldkey from passed mnemonic, encrypts it with the user's password and save the file
-            Args:
-                mnemonic: (Union[list, str], optional):
-                    Key mnemonic as list of words or string space separated words.
-                seed: (str, optional):
-                    Seed as hex string.
-                use_password (bool, optional):
-                    Is the created key password protected.
-                overwrite (bool, optional): 
-                    Will this operation overwrite the coldkey under the same path <wallet path>/<wallet name>/coldkey
-            Returns:
-                wallet (bittensor.Wallet):
-                    this object with newly created coldkey.
-        """
-        self.regenerate_coldkey(mnemonic, seed, use_password, overwrite)
-
     def regenerate_coldkeypub( self, ss58_address: Optional[str] = None, public_key: Optional[Union[str, bytes]] = None, overwrite: bool = False ) -> 'Wallet':
         """ Regenerates the coldkeypub from passed ss58_address or public_key and saves the file
                Requires either ss58_address or public_key to be passed.
             Args:
                 ss58_address: (str, optional):
                     Address as ss58 string.
                 public_key: (str | bytes, optional):
@@ -667,94 +689,187 @@
         """
         if ss58_address is None and public_key is None:
             raise ValueError("Either ss58_address or public_key must be passed")
 
         if not is_valid_bittensor_address_or_public_key( ss58_address if ss58_address is not None else public_key ):
             raise ValueError(f"Invalid {'ss58_address' if ss58_address is not None else 'public_key'}") 
 
-        keypair = Keypair(ss58_address=ss58_address, public_key=public_key, ss58_format=bittensor.__ss58_format__)
+        if ss58_address is not None:
+            ss58_format = bittensor.utils.get_ss58_format( ss58_address )
+            keypair = Keypair(ss58_address=ss58_address, public_key=public_key, ss58_format=ss58_format)
+        else:
+            keypair = Keypair(ss58_address=ss58_address, public_key=public_key, ss58_format=bittensor.__ss58_format__)
 
         # No need to encrypt the public key
         self.set_coldkeypub( keypair, overwrite = overwrite)
 
         return self
 
     # Short name for regenerate_coldkeypub
     regen_coldkeypub = regenerate_coldkeypub
 
-    def regenerate_coldkey( self, mnemonic: Optional[Union[list, str]] = None, seed: Optional[str] = None, use_password: bool = True,  overwrite:bool = False) -> 'Wallet':
-        """ Regenerates the coldkey from passed mnemonic, encrypts it with the user's password and save the file
+    @overload
+    def regenerate_coldkey(
+            self,
+            mnemonic: Optional[Union[list, str]] = None,
+            use_password: bool = True,
+            overwrite: bool = False
+        ) -> 'Wallet':
+        ...
+
+    @overload
+    def regenerate_coldkey(
+            self,
+            seed: Optional[str] = None,
+            use_password: bool = True,
+            overwrite: bool = False
+        ) -> 'Wallet':
+        ...
+
+    @overload
+    def regenerate_coldkey(
+            self,
+            json: Optional[Tuple[Union[str, Dict], str]] = None,
+            use_password: bool = True,
+            overwrite: bool = False
+        ) -> 'Wallet':
+        ...
+
+
+    def regenerate_coldkey(
+            self,
+            use_password: bool = True,
+            overwrite: bool = False,
+            **kwargs
+        ) -> 'Wallet':
+        """ Regenerates the coldkey from passed mnemonic, seed, or json encrypts it with the user's password and saves the file
             Args:
                 mnemonic: (Union[list, str], optional):
                     Key mnemonic as list of words or string space separated words.
                 seed: (str, optional):
                     Seed as hex string.
+                json: (Tuple[Union[str, Dict], str], optional):
+                    Restore from encrypted JSON backup as (json_data: Union[str, Dict], passphrase: str)
                 use_password (bool, optional):
                     Is the created key password protected.
                 overwrite (bool, optional): 
                     Will this operation overwrite the coldkey under the same path <wallet path>/<wallet name>/coldkey
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created coldkey.
+
+            Note: uses priority order: mnemonic > seed > json
         """
-        if mnemonic is None and seed is None:
-            raise ValueError("Must pass either mnemonic or seed")
+        if len(kwargs) == 0:
+            raise ValueError("Must pass either mnemonic, seed, or json")
+        
+        # Get from kwargs
+        mnemonic = kwargs.get('mnemonic', None)
+        seed = kwargs.get('seed', None)
+        json = kwargs.get('json', None)
+        
+        if mnemonic is None and seed is None and json is None:
+            raise ValueError("Must pass either mnemonic, seed, or json")
         if mnemonic is not None:
             if isinstance( mnemonic, str): mnemonic = mnemonic.split()
             if len(mnemonic) not in [12,15,18,21,24]:
                 raise ValueError("Mnemonic has invalid size. This should be 12,15,18,21 or 24 words")
-            keypair = Keypair.create_from_mnemonic(" ".join(mnemonic))   
+            keypair = Keypair.create_from_mnemonic(" ".join(mnemonic), ss58_format=bittensor.__ss58_format__ )
             display_mnemonic_msg( keypair, "coldkey" )
+        elif seed is not None:
+            keypair = Keypair.create_from_seed(seed, ss58_format=bittensor.__ss58_format__ )
         else:
-            # seed is not None
-            keypair = Keypair.create_from_seed(seed)
+            # json is not None
+            if not isinstance(json, tuple) or len(json) != 2 or not isinstance(json[0], (str, dict)) or not isinstance(json[1], str):
+                raise ValueError("json must be a tuple of (json_data: str | Dict, passphrase: str)")
+
+            json_data, passphrase = json
+            keypair = Keypair.create_from_encrypted_json( json_data, passphrase, ss58_format=bittensor.__ss58_format__ )
             
         self.set_coldkey( keypair, encrypt = use_password, overwrite = overwrite)
         self.set_coldkeypub( keypair, overwrite = overwrite)
         return self 
 
-    def regen_hotkey( self, mnemonic: Optional[Union[list, str]], seed: Optional[str] = None, use_password: bool = True, overwrite:bool = False) -> 'Wallet':
-        """ Regenerates the hotkey from passed mnemonic, encrypts it with the user's password and save the file
-            Args:
-                mnemonic: (Union[list, str], optional):
-                    Key mnemonic as list of words or string space separated words.
-                seed: (str, optional):
-                    Seed as hex string.
-                use_password (bool, optional):
-                    Is the created key password protected.
-                overwrite (bool, optional): 
-                    Will this operation overwrite the hotkey under the same path <wallet path>/<wallet name>/hotkeys/<hotkey>
-            Returns:
-                wallet (bittensor.Wallet):
-                    this object with newly created hotkey.
-        """
-        self.regenerate_hotkey(mnemonic, seed, use_password, overwrite)
+    # Short name for regenerate_coldkey
+    regen_coldkey = regenerate_coldkey
 
-    def regenerate_hotkey( self, mnemonic: Optional[Union[list, str]] = None, seed: Optional[str] = None, use_password: bool = True, overwrite:bool = False) -> 'Wallet':
+    @overload
+    def regenerate_hotkey(
+            self,
+            mnemonic: Optional[Union[list, str]] = None,
+            use_password: bool = True,
+            overwrite: bool = False
+        ) -> 'Wallet':
+        ...
+
+    @overload
+    def regenerate_hotkey(
+            self,
+            seed: Optional[str] = None,
+            use_password: bool = True,
+            overwrite: bool = False
+        ) -> 'Wallet':
+        ...
+
+    @overload
+    def regenerate_hotkey(
+            self,
+            json: Optional[Tuple[Union[str, Dict], str]] = None,
+            use_password: bool = True,
+            overwrite: bool = False
+        ) -> 'Wallet':
+        ...
+
+    def regenerate_hotkey(
+            self,
+            use_password: bool = True,
+            overwrite: bool = False,
+            **kwargs
+        ) -> 'Wallet':
         """ Regenerates the hotkey from passed mnemonic, encrypts it with the user's password and save the file
             Args:
                 mnemonic: (Union[list, str], optional):
                     Key mnemonic as list of words or string space separated words.
                 seed: (str, optional):
                     Seed as hex string.
+                json: (Tuple[Union[str, Dict], str], optional):
+                    Restore from encrypted JSON backup as (json_data: Union[str, Dict], passphrase: str)
                 use_password (bool, optional):
                     Is the created key password protected.
                 overwrite (bool, optional): 
                     Will this operation overwrite the hotkey under the same path <wallet path>/<wallet name>/hotkeys/<hotkey>
             Returns:
                 wallet (bittensor.Wallet):
                     this object with newly created hotkey.
         """
-        if mnemonic is None and seed is None:
-            raise ValueError("Must pass either mnemonic or seed")
+        if len(kwargs) == 0:
+            raise ValueError("Must pass either mnemonic, seed, or json")
+        
+        # Get from kwargs
+        mnemonic = kwargs.get('mnemonic', None)
+        seed = kwargs.get('seed', None)
+        json = kwargs.get('json', None)
+
+        if mnemonic is None and seed is None and json is None:
+            raise ValueError("Must pass either mnemonic, seed, or json")
         if mnemonic is not None:
             if isinstance( mnemonic, str): mnemonic = mnemonic.split()
             if len(mnemonic) not in [12,15,18,21,24]:
                 raise ValueError("Mnemonic has invalid size. This should be 12,15,18,21 or 24 words")
-            keypair = Keypair.create_from_mnemonic(" ".join(mnemonic))
+            keypair = Keypair.create_from_mnemonic(" ".join(mnemonic), ss58_format=bittensor.__ss58_format__ )
             display_mnemonic_msg( keypair, "hotkey" )
+        elif seed is not None:
+            keypair = Keypair.create_from_seed(seed, ss58_format=bittensor.__ss58_format__ )
         else:
-            # seed is not None
-            keypair = Keypair.create_from_seed(seed)
+            # json is not None
+            if not isinstance(json, tuple) or len(json) != 2 or not isinstance(json[0], (str, dict)) or not isinstance(json[1], str):
+                raise ValueError("json must be a tuple of (json_data: str | Dict, passphrase: str)")
+
+            json_data, passphrase = json
+            keypair = Keypair.create_from_encrypted_json( json_data, passphrase, ss58_format=bittensor.__ss58_format__ )
+
         
         self.set_hotkey( keypair, encrypt=use_password, overwrite = overwrite)
         return self 
+    
+    # Short name for regenerate_hotkey
+    regen_hotkey = regenerate_hotkey
```

### Comparing `bittensor-4.0.0/bittensor/_wallet/wallet_mock.py` & `bittensor-4.1.0rc1/bittensor/_wallet/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/utils/__init__.py` & `bittensor-4.1.0rc1/bittensor/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numbers
-from typing import Callable, Union
+from typing import Callable, Union, List, Optional, Dict
 
 import bittensor
 import pandas
 import requests
 import torch
 import scalecodec
 from substrateinterface import Keypair
 from substrateinterface.utils import ss58
-from .registration import *
+from .registration import create_pow
 
 RAOPERTAO = 1e9
 U16_MAX = 65535
 U64_MAX = 18446744073709551615
 
 def indexed_values_to_dataframe ( 
         prefix: Union[str, int],
```

### Comparing `bittensor-4.0.0/bittensor/utils/balance.py` & `bittensor-4.1.0rc1/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/utils/codes.py` & `bittensor-4.1.0rc1/bittensor/utils/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         return 'SenderUnknown'
     elif code == 22:
         return 'UnknownException'
     elif code == 23:
         return 'Unauthenticated'
     elif code == 24:
         return 'BadEndpoint'
+    elif code == 25:
+        return 'Blacklisted'
     else:
         return 'UnknownCode'
 
 def code_to_loguru_color( code: 'bittensor.proto.ReturnCode' ) -> str:
     """ Return code -> loguru color
     """
     if code == 0: 
@@ -123,14 +125,20 @@
         return 'red'
     elif code == 20:
         return 'red'
     elif code == 21:
         return 'red'
     elif code == 22:
         return 'red'
+    elif code == 23:
+        return 'red'
+    elif code == 24:
+        return 'red'
+    elif code == 25:
+        return 'magenta'
     else:
         return 'red'
 
 def code_to_synapse( code: 'bittensor.proto.Synapse.SynapseType'):
     """Return Code -> Synapse Type"""
     if code == 1:
         return 'text_last_hidden_state'
```

### Comparing `bittensor-4.0.0/bittensor/utils/networking.py` & `bittensor-4.1.0rc1/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/utils/registration.py` & `bittensor-4.1.0rc1/bittensor/utils/registratrion_old.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import backoff
 import bittensor
 import torch
 from Crypto.Hash import keccak
 from rich import console as rich_console
 from rich import status as rich_status
 
-from .register_cuda import solve_cuda
+from ._register_cuda import solve_cuda
 
 
 class CUDAException(Exception):
     """An exception raised when an error occurs in the CUDA environment."""
     pass
 
 
@@ -101,15 +101,14 @@
     difficulty: int
     seal: bytes
 
 
 class SolverBase(multiprocessing.Process):
     """
     A process that solves the registration PoW problem.
-
     Args:
         proc_num: int
             The number of the process being created.
         num_proc: int
             The total number of processes running.
         update_interval: int
             The number of nonces to try to solve before checking for a new block.
@@ -253,19 +252,19 @@
             # increase nonce by number of nonces processed
             nonce_start += self.update_interval * self.TPB 
             nonce_start = nonce_start % nonce_limit
 
 
 def solve_for_nonce_block_cuda(solver: CUDASolver, nonce_start: int, update_interval: int, block_bytes: bytes, difficulty: int, limit: int, block_number: int, dev_id: int, TPB: int) -> Optional[POWSolution]:
     """Tries to solve the POW on a CUDA device for a block of nonces (nonce_start, nonce_start + update_interval * TPB"""
-    solution, seal = solve_cuda(nonce_start,
+    solution, seal = solve_cuda(
+                    nonce_start,
                     update_interval,
                     TPB,
                     block_bytes, 
-                    block_number,
                     difficulty, 
                     limit,
                     dev_id)
 
     if (solution != -1):
         # Check if solution is valid (i.e. not -1)
         return POWSolution(solution, block_number, difficulty, seal)
@@ -374,24 +373,22 @@
     def update( self, stats: RegistrationStatistics, verbose: bool = False ) -> None:
         if self.status is not None:
             self.status.update( self.get_status_message(stats, verbose=verbose) )
         else:
             self.console.log( self.get_status_message(stats, verbose=verbose), )
 
 
-def solve_for_difficulty_fast( subtensor, wallet, netuid: int, output_in_place: bool = True, num_processes: Optional[int] = None, update_interval: Optional[int] = None,  n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
+def solve_for_difficulty_fast( subtensor, wallet, output_in_place: bool = True, num_processes: Optional[int] = None, update_interval: Optional[int] = None,  n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
     """
     Solves the POW for registration using multiprocessing.
     Args:
         subtensor
             Subtensor to connect to for block information and to submit.
         wallet:
             Wallet to use for registration.
-        netuid: int
-            The netuid of the subnet to register to.
         output_in_place: bool
             If true, prints the status in place. Otherwise, prints the status on a new line.
         num_processes: int
             Number of processes to use.
         update_interval: int
             Number of nonces to solve before updating block information.
         n_samples: int
@@ -429,16 +426,19 @@
     check_block = multiprocessing.Lock()
     
     # Start consumers
     solvers = [ Solver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit)
                 for i in range(num_processes) ]
 
     # Get first block
-    block_number, difficulty, block_hash = get_block_with_retry(subtensor = subtensor, netuid = netuid)
-
+    block_number = subtensor.get_current_block()
+    difficulty = subtensor.difficulty
+    block_hash = subtensor.substrate.get_block_hash( block_number )
+    while block_hash == None:
+        block_hash = subtensor.substrate.get_block_hash( block_number )
     block_bytes = block_hash.encode('utf-8')[2:]
     old_block_number = block_number
     # Set to current block
     update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
 
     # Set new block events for each solver to start at the initial block
     for worker in solvers:
@@ -470,28 +470,27 @@
     logger.start()
 
     solution = None
 
     hash_rates = [0] * n_samples # The last n true hash_rates
     weights = [alpha_ ** i for i in range(n_samples)] # weights decay by alpha
     
-    while not wallet.is_registered(netuid = netuid, subtensor = subtensor):
+    while not wallet.is_registered(subtensor):
         # Wait until a solver finds a solution
         try:
             solution = solution_queue.get(block=True, timeout=0.25)
             if solution is not None:
                 break
         except Empty:
             # No solution found, try again
             pass
 
         # check for new block
         old_block_number = check_for_newest_block_and_update(
             subtensor = subtensor,
-            netuid = netuid,
             old_block_number=old_block_number,
             curr_diff=curr_diff,
             curr_block=curr_block,
             curr_block_num=curr_block_num,
             curr_stats=curr_stats,
             update_curr_block=update_curr_block,
             check_block=check_block,
@@ -542,46 +541,20 @@
     return solution
 
 
 @backoff.on_exception(backoff.constant,
                             Exception,
                             interval=1,
                             max_tries=3)
-def get_block_with_retry(subtensor: 'bittensor.Subtensor', netuid: int) -> Tuple[int, int, bytes]:
-    """
-    Gets the current block number, difficulty, and block hash from the substrate node.
-
-    Args:
-        subtensor (:obj:`bittensor.Subtensor`, `required`):
-            The subtensor object to use to get the block number, difficulty, and block hash.
-
-        netuid (:obj:`int`, `required`):
-            The netuid of the network to get the block number, difficulty, and block hash from.
-        
-    Returns:
-        block_number (:obj:`int`):
-            The current block number.
-        
-        difficulty (:obj:`int`):
-            The current difficulty of the subnet.
-
-        block_hash (:obj:`bytes`):
-            The current block hash.
-
-    Raises:
-        Exception: If the block hash is None.
-        ValueError: If the difficulty is None.
-    """
+def get_block_with_retry(subtensor: 'bittensor.Subtensor') -> Tuple[int, int, bytes]:
     block_number = subtensor.get_current_block()
-    difficulty = subtensor.difficulty(netuid = netuid)
+    difficulty = subtensor.difficulty
     block_hash = subtensor.substrate.get_block_hash( block_number )
     if block_hash is None:
         raise Exception("Network error. Could not connect to substrate to get block hash")
-    if difficulty is None:
-        raise ValueError("Chain error. Difficulty is None")
     return block_number, difficulty, block_hash
 
 
 class UsingSpawnStartMethod():
     def __init__(self, force: bool = False):
         self._old_start_method = None
         self._force = force
@@ -596,32 +569,28 @@
     def __exit__(self, *args):
         # restore the old start method
         multiprocessing.set_start_method(self._old_start_method, force=True)
 
 
 def check_for_newest_block_and_update(
     subtensor: 'bittensor.Subtensor',
-    netuid: int,
     old_block_number: int,
     curr_diff: multiprocessing.Array,
     curr_block: multiprocessing.Array,
     curr_block_num: multiprocessing.Value,
     update_curr_block: Callable,
     check_block: 'multiprocessing.Lock',
     solvers: List[Solver],
     curr_stats: RegistrationStatistics
     ) -> int:
     """
     Checks for a new block and updates the current block information if a new block is found.
-
     Args:
         subtensor (:obj:`bittensor.Subtensor`, `required`):
             The subtensor object to use for getting the current block.
-        netuid (:obj:`int`, `required`):
-            The netuid to use for retrieving the difficulty.
         old_block_number (:obj:`int`, `required`):
             The old block number to check against.
         curr_diff (:obj:`multiprocessing.Array`, `required`):
             The current difficulty as a multiprocessing array.
         curr_block (:obj:`multiprocessing.Array`, `required`):
             Where the current block is stored as a multiprocessing array.
         curr_block_num (:obj:`multiprocessing.Value`, `required`):
@@ -630,24 +599,26 @@
             A function that updates the current block.
         check_block (:obj:`multiprocessing.Lock`, `required`):
             A mp lock that is used to check for a new block.
         solvers (:obj:`List[Solver]`, `required`):
             A list of solvers to update the current block for.
         curr_stats (:obj:`RegistrationStatistics`, `required`):
             The current registration statistics to update.
-
     Returns:
         (int) The current block number.
     """
     block_number = subtensor.get_current_block()
     if block_number != old_block_number:
         old_block_number = block_number
         # update block information
-        block_number, difficulty, block_hash = get_block_with_retry(subtensor = subtensor, netuid = netuid)
+        block_hash = subtensor.substrate.get_block_hash( block_number)
+        while block_hash == None:
+            block_hash = subtensor.substrate.get_block_hash( block_number)
         block_bytes = block_hash.encode('utf-8')[2:]
+        difficulty = subtensor.difficulty
 
         update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
         # Set new block events for each solver
 
         for worker in solvers:
             worker.newBlockEvent.set()
 
@@ -655,24 +626,22 @@
         curr_stats.block_number = block_number
         curr_stats.block_hash = block_hash
         curr_stats.difficulty = difficulty
 
     return old_block_number
 
 
-def solve_for_difficulty_fast_cuda( subtensor: 'bittensor.Subtensor', wallet: 'bittensor.Wallet', netuid: int, output_in_place: bool = True, update_interval: int = 50_000, TPB: int = 512, dev_id: Union[List[int], int] = 0, n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
+def solve_for_difficulty_fast_cuda( subtensor: 'bittensor.Subtensor', wallet: 'bittensor.Wallet', output_in_place: bool = True, update_interval: int = 50_000, TPB: int = 512, dev_id: Union[List[int], int] = 0, n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
     """
     Solves the registration fast using CUDA
     Args:
         subtensor: bittensor.Subtensor
             The subtensor node to grab blocks
         wallet: bittensor.Wallet
             The wallet to register
-        netuid: int
-            The netuid of the subnet to register to.
         output_in_place: bool
             If true, prints the output in place, otherwise prints to new lines
         update_interval: int
             The number of nonces to try before checking for more blocks
         TPB: int
             The number of threads per block. CUDA param that should match the GPU capability
         dev_id: Union[List[int], int]
@@ -716,16 +685,19 @@
         
         # Start workers
         solvers = [ CUDASolver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit, dev_id[i], TPB)
                     for i in range(num_processes) ]
 
 
         # Get first block
-        block_number, difficulty, block_hash = get_block_with_retry(subtensor = subtensor, netuid = netuid)
-
+        block_number = subtensor.get_current_block()
+        difficulty = subtensor.difficulty
+        block_hash = subtensor.substrate.get_block_hash( block_number )
+        while block_hash == None:
+            block_hash = subtensor.substrate.get_block_hash( block_number )
         block_bytes = block_hash.encode('utf-8')[2:]
         old_block_number = block_number
         
         # Set to current block
         update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
 
         # Set new block events for each solver to start at the initial block
@@ -756,28 +728,27 @@
         logger = RegistrationStatisticsLogger(console, output_in_place)
         logger.start()
 
         hash_rates = [0] * n_samples # The last n true hash_rates
         weights = [alpha_ ** i for i in range(n_samples)] # weights decay by alpha
 
         solution = None
-        while not wallet.is_registered(netuid = netuid, subtensor = subtensor):
+        while not wallet.is_registered(subtensor):
             # Wait until a solver finds a solution
             try:
                 solution = solution_queue.get(block=True, timeout=0.15)
                 if solution is not None:
                     break
             except Empty:
                 # No solution found, try again
                 pass
             
             # check for new block
             old_block_number = check_for_newest_block_and_update(
                 subtensor = subtensor,
-                netuid = netuid,
                 curr_diff=curr_diff,
                 curr_block=curr_block,
                 curr_block_num=curr_block_num,
                 old_block_number=old_block_number,
                 curr_stats=curr_stats,
                 update_curr_block=update_curr_block,
                 check_block=check_block,
@@ -835,67 +806,28 @@
         worker.terminate()
         worker.join()
 
 
 def create_pow(
     subtensor,
     wallet,
-    netuid: int,
     output_in_place: bool = True,
     cuda: bool = False,
     dev_id: Union[List[int], int] = 0,
     tpb: int = 256,
     num_processes: int = None,
     update_interval: int = None,
     log_verbose: bool = False
     ) -> Optional[Dict[str, Any]]:
-    """
-    Creates a proof of work for the given subtensor and wallet.
-    Args:
-        subtensor (:obj:`bittensor.subtensor.Subtensor`, `required`):
-            The subtensor to create a proof of work for.
-        wallet (:obj:`bittensor.wallet.Wallet`, `required`):
-            The wallet to create a proof of work for.
-        netuid (:obj:`int`, `required`):
-            The netuid for the subnet to create a proof of work for.
-        output_in_place (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            If true, prints the progress of the proof of work to the console
-                in-place. Meaning the progress is printed on the same lines.
-        cuda (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            If true, uses CUDA to solve the proof of work.
-        dev_id (:obj:`Union[List[int], int]`, `optional`, defaults to :obj:`0`):
-            The CUDA device id(s) to use. If cuda is true and dev_id is a list,
-                then multiple CUDA devices will be used to solve the proof of work.
-        tpb (:obj:`int`, `optional`, defaults to :obj:`256`):
-            The number of threads per block to use when solving the proof of work.
-            Should be a multiple of 32.
-        num_processes (:obj:`int`, `optional`, defaults to :obj:`None`):
-            The number of processes to use when solving the proof of work.
-            If None, then the number of processes is equal to the number of
-                CPU cores.
-        update_interval (:obj:`int`, `optional`, defaults to :obj:`None`):
-            The number of nonces to run before checking for a new block.
-        log_verbose (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            If true, prints the progress of the proof of work more verbosely.   
-    Returns:
-        :obj:`Optional[Dict[str, Any]]`: The proof of work solution or None if
-            the wallet is already registered or there is a different error.
-    
-    Raises:
-        :obj:`ValueError`: If the subnet does not exist.
-    """
-    if not subtensor.subnet_exists(netuid = netuid):
-        raise ValueError(f'Subnet {netuid} does not exist')
-
     if cuda:
-        solution: POWSolution = solve_for_difficulty_fast_cuda( subtensor, wallet, netuid = netuid, output_in_place=output_in_place, \
+        solution: POWSolution = solve_for_difficulty_fast_cuda( subtensor, wallet, output_in_place=output_in_place, \
             dev_id=dev_id, TPB=tpb, update_interval=update_interval, log_verbose=log_verbose
         )
     else:
-        solution: POWSolution = solve_for_difficulty_fast( subtensor, wallet, netuid = netuid, output_in_place=output_in_place, \
+        solution: POWSolution = solve_for_difficulty_fast( subtensor, wallet, output_in_place=output_in_place, \
             num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose
         )
 
     return None if solution is None else {
         'nonce': solution.nonce, 
         'difficulty': solution.difficulty,
         'block_number': solution.block_number,
```

### Comparing `bittensor-4.0.0/bittensor/utils/registratrion_old.py` & `bittensor-4.1.0rc1/bittensor/utils/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,102 +13,58 @@
 import backoff
 import bittensor
 import torch
 from Crypto.Hash import keccak
 from rich import console as rich_console
 from rich import status as rich_status
 
-from .register_cuda import solve_cuda
+from .formatting import get_human_readable, millify
+from ._register_cuda import solve_cuda
 
 
 class CUDAException(Exception):
     """An exception raised when an error occurs in the CUDA environment."""
     pass
 
-
-def hex_bytes_to_u8_list( hex_bytes: bytes ):
+def _hex_bytes_to_u8_list( hex_bytes: bytes ):
     hex_chunks = [int(hex_bytes[i:i+2], 16) for i in range(0, len(hex_bytes), 2)]
     return hex_chunks
 
-
-def u8_list_to_hex( values: list ):
-    total = 0
-    for val in reversed(values):
-        total = (total << 8) + val
-    return total 
-
-
-def create_seal_hash( block_hash:bytes, nonce:int ) -> bytes:
-    block_bytes = block_hash.encode('utf-8')[2:]
+def _create_seal_hash( block_and_hotkey_hash_bytes: bytes, nonce:int ) -> bytes:
     nonce_bytes = binascii.hexlify(nonce.to_bytes(8, 'little'))
-    pre_seal = nonce_bytes + block_bytes
-    seal_sh256 = hashlib.sha256( bytearray(hex_bytes_to_u8_list(pre_seal)) ).digest()
+    pre_seal = nonce_bytes + binascii.hexlify(block_and_hotkey_hash_bytes)[:64]
+    seal_sh256 = hashlib.sha256( bytearray(_hex_bytes_to_u8_list(pre_seal)) ).digest()
     kec = keccak.new(digest_bits=256)
     seal = kec.update( seal_sh256 ).digest()
     return seal
 
-
-def seal_meets_difficulty( seal:bytes, difficulty:int ):
+def _seal_meets_difficulty( seal:bytes, difficulty:int, limit: int ):
     seal_number = int.from_bytes(seal, "big")
     product = seal_number * difficulty
-    limit = int(math.pow(2,256))- 1
-    if product > limit:
-        return False
-    else:
-        return True
-    
-
-def solve_for_difficulty( block_hash, difficulty ):
-    meets = False
-    nonce = -1
-    while not meets:
-        nonce += 1 
-        seal = create_seal_hash( block_hash, nonce )
-        meets = seal_meets_difficulty( seal, difficulty )
-        if nonce > 1:
-            break
-    return nonce, seal
-
-
-def get_human_readable(num, suffix="H"):
-    for unit in ["", "K", "M", "G", "T", "P", "E", "Z"]:
-        if abs(num) < 1000.0:
-            return f"{num:3.1f}{unit}{suffix}"
-        num /= 1000.0
-    return f"{num:.1f}Y{suffix}"
-
-
-def millify(n: int):
-    millnames = ['',' K',' M',' B',' T']
-    n = float(n)
-    millidx = max(0,min(len(millnames)-1,
-                        int(math.floor(0 if n == 0 else math.log10(abs(n))/3))))
-
-    return '{:.2f}{}'.format(n / 10**(3 * millidx), millnames[millidx])
-
-
-def POWNotStale(subtensor: 'bittensor.Subtensor', pow_result: Dict) -> bool:
-    """Returns True if the POW is not stale.
-    This means the block the POW is solved for is within 3 blocks of the current block.
-    """
-    return pow_result['block_number'] >= subtensor.get_current_block() - 3
-
+    return product < limit
 
 @dataclass
 class POWSolution:
     """A solution to the registration PoW problem."""
     nonce: int
     block_number: int
     difficulty: int
     seal: bytes
 
+    def is_stale(self, subtensor: 'bittensor.Subtensor') -> bool:
+        """Returns True if the POW is stale.
+        This means the block the POW is solved for is within 3 blocks of the current block.
+        """
+        return self.block_number < subtensor.get_current_block() - 3
+
 
-class SolverBase(multiprocessing.Process):
+class _SolverBase(multiprocessing.Process):
     """
     A process that solves the registration PoW problem.
+
     Args:
         proc_num: int
             The number of the process being created.
         num_proc: int
             The total number of processes running.
         update_interval: int
             The number of nonces to try to solve before checking for a new block.
@@ -146,14 +102,15 @@
     proc_num: int
     num_proc: int
     update_interval: int
     finished_queue: multiprocessing.Queue
     solution_queue: multiprocessing.Queue
     newBlockEvent: multiprocessing.Event
     stopEvent: multiprocessing.Event
+    hotkey_bytes: bytes
     curr_block: multiprocessing.Array
     curr_block_num: multiprocessing.Value
     curr_diff: multiprocessing.Array
     check_block: multiprocessing.Lock
     limit: int
 
     def __init__(self, proc_num, num_proc, update_interval, finished_queue, solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit):
@@ -169,80 +126,90 @@
         self.curr_block_num = curr_block_num
         self.curr_diff = curr_diff
         self.check_block = check_block
         self.stopEvent = stopEvent
         self.limit = limit
 
     def run(self):
-        raise NotImplementedError("SolverBase is an abstract class")
+        raise NotImplementedError("_SolverBase is an abstract class")
+    
+    @staticmethod
+    def create_shared_memory() -> Tuple[multiprocessing.Array, multiprocessing.Value, multiprocessing.Array]:
+        """Creates shared memory for the solver processes to use.
+        """
+        curr_block = multiprocessing.Array('h', 32, lock=True) # byte array
+        curr_block_num = multiprocessing.Value('i', 0, lock=True) # int
+        curr_diff = multiprocessing.Array('Q', [0, 0], lock=True) # [high, low]
 
+        return curr_block, curr_block_num, curr_diff
 
-class Solver(SolverBase):
+
+class _Solver(_SolverBase):
     def run(self):
         block_number: int
-        block_bytes: bytes
+        block_and_hotkey_hash_bytes: bytes
         block_difficulty: int
         nonce_limit = int(math.pow(2,64)) - 1
 
         # Start at random nonce
         nonce_start = random.randint( 0, nonce_limit )
         nonce_end = nonce_start + self.update_interval
         while not self.stopEvent.is_set():
             if self.newBlockEvent.is_set():
                 with self.check_block:
                     block_number = self.curr_block_num.value
-                    block_bytes = bytes(self.curr_block)
-                    block_difficulty = registration_diff_unpack(self.curr_diff)
+                    block_and_hotkey_hash_bytes = bytes(self.curr_block)
+                    block_difficulty = _registration_diff_unpack(self.curr_diff)
 
                 self.newBlockEvent.clear()
                 
             # Do a block of nonces
-            solution = solve_for_nonce_block(self, nonce_start, nonce_end, block_bytes, block_difficulty, self.limit, block_number)
+            solution = _solve_for_nonce_block(nonce_start, nonce_end, block_and_hotkey_hash_bytes, block_difficulty, self.limit, block_number)
             if solution is not None:
                 self.solution_queue.put(solution)
 
             try:
                 # Send time
                 self.finished_queue.put_nowait(self.proc_num)
             except Full:
                 pass
                 
             nonce_start = random.randint( 0, nonce_limit )
             nonce_start = nonce_start % nonce_limit
             nonce_end = nonce_start + self.update_interval
 
 
-class CUDASolver(SolverBase):
+class _CUDASolver(_SolverBase):
     dev_id: int
     TPB: int
 
     def __init__(self, proc_num, num_proc, update_interval, finished_queue, solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit, dev_id: int, TPB: int):
         super().__init__(proc_num, num_proc, update_interval, finished_queue, solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit)
         self.dev_id = dev_id
         self.TPB = TPB
 
     def run(self):
         block_number: int = 0 # dummy value
-        block_bytes: bytes = b'0' * 32 # dummy value
+        block_and_hotkey_hash_bytes: bytes = b'0' * 32 # dummy value
         block_difficulty: int = int(math.pow(2,64)) - 1 # dummy value
         nonce_limit = int(math.pow(2,64)) - 1 # U64MAX
 
         # Start at random nonce
         nonce_start = random.randint( 0, nonce_limit )
         while not self.stopEvent.is_set():
             if self.newBlockEvent.is_set():
                 with self.check_block:
                     block_number = self.curr_block_num.value
-                    block_bytes = bytes(self.curr_block)
-                    block_difficulty = registration_diff_unpack(self.curr_diff)
+                    block_and_hotkey_hash_bytes = bytes(self.curr_block)
+                    block_difficulty = _registration_diff_unpack(self.curr_diff)
 
                 self.newBlockEvent.clear()
                 
             # Do a block of nonces
-            solution = solve_for_nonce_block_cuda(self, nonce_start, self.update_interval, block_bytes, block_difficulty, self.limit, block_number, self.dev_id, self.TPB)
+            solution = _solve_for_nonce_block_cuda(nonce_start, self.update_interval, block_and_hotkey_hash_bytes, block_difficulty, self.limit, block_number, self.dev_id, self.TPB)
             if solution is not None:
                 self.solution_queue.put(solution)
 
             try:
                 # Signal that a nonce_block was finished using queue
                 # send our proc_num
                 self.finished_queue.put(self.proc_num)
@@ -250,72 +217,77 @@
                 pass
             
             # increase nonce by number of nonces processed
             nonce_start += self.update_interval * self.TPB 
             nonce_start = nonce_start % nonce_limit
 
 
-def solve_for_nonce_block_cuda(solver: CUDASolver, nonce_start: int, update_interval: int, block_bytes: bytes, difficulty: int, limit: int, block_number: int, dev_id: int, TPB: int) -> Optional[POWSolution]:
+def _solve_for_nonce_block_cuda(nonce_start: int, update_interval: int, block_and_hotkey_hash_bytes: bytes, difficulty: int, limit: int, block_number: int, dev_id: int, TPB: int) -> Optional[POWSolution]:
     """Tries to solve the POW on a CUDA device for a block of nonces (nonce_start, nonce_start + update_interval * TPB"""
-    solution, seal = solve_cuda(nonce_start,
+    solution, seal = solve_cuda(
+                    nonce_start,
                     update_interval,
                     TPB,
-                    block_bytes, 
-                    block_number,
+                    block_and_hotkey_hash_bytes, 
                     difficulty, 
                     limit,
                     dev_id)
+    
 
     if (solution != -1):
         # Check if solution is valid (i.e. not -1)
         return POWSolution(solution, block_number, difficulty, seal)
 
     return None
 
 
-def solve_for_nonce_block(solver: Solver, nonce_start: int, nonce_end: int, block_bytes: bytes, difficulty: int, limit: int, block_number: int) -> Optional[POWSolution]:
+def _solve_for_nonce_block(nonce_start: int, nonce_end: int, block_and_hotkey_hash_bytes: bytes, difficulty: int, limit: int, block_number: int) -> Optional[POWSolution]:
     """Tries to solve the POW for a block of nonces (nonce_start, nonce_end)""" 
     for nonce in range(nonce_start, nonce_end):
         # Create seal.
-        nonce_bytes = binascii.hexlify(nonce.to_bytes(8, 'little'))
-        pre_seal = nonce_bytes + block_bytes
-        seal_sh256 = hashlib.sha256( bytearray(hex_bytes_to_u8_list(pre_seal)) ).digest()
-        kec = keccak.new(digest_bits=256)
-        seal = kec.update( seal_sh256 ).digest()
-        seal_number = int.from_bytes(seal, "big")
+        seal = _create_seal_hash(block_and_hotkey_hash_bytes, nonce)
 
         # Check if seal meets difficulty
-        product = seal_number * difficulty
-        if product < limit:
+        if _seal_meets_difficulty(seal, difficulty, limit):
             # Found a solution, save it.
             return POWSolution(nonce, block_number, difficulty, seal)
 
     return None
 
 
-def registration_diff_unpack(packed_diff: multiprocessing.Array) -> int:
+def _registration_diff_unpack(packed_diff: multiprocessing.Array) -> int:
     """Unpacks the packed two 32-bit integers into one 64-bit integer. Little endian."""
     return int(packed_diff[0] << 32 | packed_diff[1])
 
 
-def registration_diff_pack(diff: int, packed_diff: multiprocessing.Array):
+def _registration_diff_pack(diff: int, packed_diff: multiprocessing.Array):
     """Packs the difficulty into two 32-bit integers. Little endian."""
     packed_diff[0] = diff >> 32
     packed_diff[1] = diff & 0xFFFFFFFF # low 32 bits
 
 
-def update_curr_block(curr_diff: multiprocessing.Array, curr_block: multiprocessing.Array, curr_block_num: multiprocessing.Value, block_number: int, block_bytes: bytes, diff: int, lock: multiprocessing.Lock):
+def _hash_block_with_hotkey(block_bytes: bytes, hotkey_bytes: bytes) -> bytes:
+    """Hashes the block with the hotkey using Keccak-256 to get 32 bytes"""
+    kec = keccak.new(digest_bits=256)
+    kec = kec.update(bytearray(block_bytes + hotkey_bytes))
+    block_and_hotkey_hash_bytes = kec.digest()
+    return block_and_hotkey_hash_bytes
+
+
+def _update_curr_block(curr_diff: multiprocessing.Array, curr_block: multiprocessing.Array, curr_block_num: multiprocessing.Value, block_number: int, block_bytes: bytes, diff: int, hotkey_bytes: bytes, lock: multiprocessing.Lock):
     with lock:
         curr_block_num.value = block_number
-        for i in range(64):
-            curr_block[i] = block_bytes[i]
-        registration_diff_pack(diff, curr_diff)
+        # Hash the block with the hotkey
+        block_and_hotkey_hash_bytes = _hash_block_with_hotkey(block_bytes, hotkey_bytes)
+        for i in range(32):
+            curr_block[i] = block_and_hotkey_hash_bytes[i]
+        _registration_diff_pack(diff, curr_diff)
 
 
-def get_cpu_count():
+def get_cpu_count() -> int:
     try:
         return len(os.sched_getaffinity(0))
     except AttributeError:
         # OSX does not have sched_getaffinity
         return os.cpu_count()
 
 @dataclass
@@ -373,22 +345,24 @@
     def update( self, stats: RegistrationStatistics, verbose: bool = False ) -> None:
         if self.status is not None:
             self.status.update( self.get_status_message(stats, verbose=verbose) )
         else:
             self.console.log( self.get_status_message(stats, verbose=verbose), )
 
 
-def solve_for_difficulty_fast( subtensor, wallet, output_in_place: bool = True, num_processes: Optional[int] = None, update_interval: Optional[int] = None,  n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
+def _solve_for_difficulty_fast( subtensor, wallet: 'bittensor.Wallet', netuid: int, output_in_place: bool = True, num_processes: Optional[int] = None, update_interval: Optional[int] = None,  n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
     """
     Solves the POW for registration using multiprocessing.
     Args:
         subtensor
             Subtensor to connect to for block information and to submit.
         wallet:
             Wallet to use for registration.
+        netuid: int
+            The netuid of the subnet to register to.
         output_in_place: bool
             If true, prints the status in place. Otherwise, prints the status on a new line.
         num_processes: int
             Number of processes to use.
         update_interval: int
             Number of nonces to solve before updating block information.
         n_samples: int
@@ -408,41 +382,38 @@
         num_processes = min(1, get_cpu_count())
 
     if update_interval is None:
         update_interval = 50_000
         
     limit = int(math.pow(2,256)) - 1
 
-    curr_block = multiprocessing.Array('h', 64, lock=True) # byte array
-    curr_block_num = multiprocessing.Value('i', 0, lock=True) # int
-    curr_diff = multiprocessing.Array('Q', [0, 0], lock=True) # [high, low]
+    curr_block, curr_block_num, curr_diff = _Solver.create_shared_memory()
 
     # Establish communication queues
-    ## See the Solver class for more information on the queues.
+    ## See the _Solver class for more information on the queues.
     stopEvent = multiprocessing.Event()
     stopEvent.clear()
 
     solution_queue = multiprocessing.Queue()
     finished_queues = [multiprocessing.Queue() for _ in range(num_processes)]
     check_block = multiprocessing.Lock()
+
+    hotkey_bytes = wallet.hotkey.public_key
     
     # Start consumers
-    solvers = [ Solver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit)
+    solvers = [ _Solver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit)
                 for i in range(num_processes) ]
 
     # Get first block
-    block_number = subtensor.get_current_block()
-    difficulty = subtensor.difficulty
-    block_hash = subtensor.substrate.get_block_hash( block_number )
-    while block_hash == None:
-        block_hash = subtensor.substrate.get_block_hash( block_number )
-    block_bytes = block_hash.encode('utf-8')[2:]
+    block_number, difficulty, block_hash = _get_block_with_retry(subtensor = subtensor, netuid = netuid)
+
+    block_bytes = bytes.fromhex(block_hash[2:])
     old_block_number = block_number
     # Set to current block
-    update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
+    _update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, hotkey_bytes, check_block)
 
     # Set new block events for each solver to start at the initial block
     for worker in solvers:
         worker.newBlockEvent.set()
     
     for worker in solvers:
         worker.start() # start the solver processes
@@ -470,33 +441,35 @@
     logger.start()
 
     solution = None
 
     hash_rates = [0] * n_samples # The last n true hash_rates
     weights = [alpha_ ** i for i in range(n_samples)] # weights decay by alpha
     
-    while not wallet.is_registered(subtensor):
+    while not wallet.is_registered(netuid = netuid, subtensor = subtensor):
         # Wait until a solver finds a solution
         try:
             solution = solution_queue.get(block=True, timeout=0.25)
             if solution is not None:
                 break
         except Empty:
             # No solution found, try again
             pass
 
         # check for new block
-        old_block_number = check_for_newest_block_and_update(
+        old_block_number = _check_for_newest_block_and_update(
             subtensor = subtensor,
+            netuid = netuid,
+            hotkey_bytes = hotkey_bytes,
             old_block_number=old_block_number,
             curr_diff=curr_diff,
             curr_block=curr_block,
             curr_block_num=curr_block_num,
             curr_stats=curr_stats,
-            update_curr_block=update_curr_block,
+            update_curr_block=_update_curr_block,
             check_block=check_block,
             solvers=solvers
         )
                 
         num_time = 0
         for finished_queue in finished_queues:
             try:
@@ -532,33 +505,59 @@
         logger.update(curr_stats, verbose=log_verbose)
 
     # exited while, solution contains the nonce or wallet is registered
     stopEvent.set() # stop all other processes
     logger.stop()
 
     # terminate and wait for all solvers to exit
-    terminate_workers_and_wait_for_exit(solvers)
+    _terminate_workers_and_wait_for_exit(solvers)
 
     return solution
 
 
 @backoff.on_exception(backoff.constant,
                             Exception,
                             interval=1,
                             max_tries=3)
-def get_block_with_retry(subtensor: 'bittensor.Subtensor') -> Tuple[int, int, bytes]:
+def _get_block_with_retry(subtensor: 'bittensor.Subtensor', netuid: int) -> Tuple[int, int, bytes]:
+    """
+    Gets the current block number, difficulty, and block hash from the substrate node.
+
+    Args:
+        subtensor (:obj:`bittensor.Subtensor`, `required`):
+            The subtensor object to use to get the block number, difficulty, and block hash.
+
+        netuid (:obj:`int`, `required`):
+            The netuid of the network to get the block number, difficulty, and block hash from.
+        
+    Returns:
+        block_number (:obj:`int`):
+            The current block number.
+        
+        difficulty (:obj:`int`):
+            The current difficulty of the subnet.
+
+        block_hash (:obj:`bytes`):
+            The current block hash.
+
+    Raises:
+        Exception: If the block hash is None.
+        ValueError: If the difficulty is None.
+    """
     block_number = subtensor.get_current_block()
-    difficulty = subtensor.difficulty
+    difficulty = subtensor.difficulty(netuid = netuid)
     block_hash = subtensor.substrate.get_block_hash( block_number )
     if block_hash is None:
         raise Exception("Network error. Could not connect to substrate to get block hash")
+    if difficulty is None:
+        raise ValueError("Chain error. Difficulty is None")
     return block_number, difficulty, block_hash
 
 
-class UsingSpawnStartMethod():
+class _UsingSpawnStartMethod():
     def __init__(self, force: bool = False):
         self._old_start_method = None
         self._force = force
 
     def __enter__(self):
         self._old_start_method = multiprocessing.get_start_method(allow_none=True)
         if self._old_start_method == None:
@@ -567,81 +566,88 @@
         multiprocessing.set_start_method('spawn', force=self._force)
 
     def __exit__(self, *args):
         # restore the old start method
         multiprocessing.set_start_method(self._old_start_method, force=True)
 
 
-def check_for_newest_block_and_update(
-    subtensor: 'bittensor.Subtensor',
-    old_block_number: int,
-    curr_diff: multiprocessing.Array,
-    curr_block: multiprocessing.Array,
-    curr_block_num: multiprocessing.Value,
-    update_curr_block: Callable,
-    check_block: 'multiprocessing.Lock',
-    solvers: List[Solver],
-    curr_stats: RegistrationStatistics
+def _check_for_newest_block_and_update(
+        subtensor: 'bittensor.Subtensor',
+        netuid: int,
+        old_block_number: int,
+        hotkey_bytes: bytes,
+        curr_diff: multiprocessing.Array,
+        curr_block: multiprocessing.Array,
+        curr_block_num: multiprocessing.Value,
+        update_curr_block: Callable,
+        check_block: 'multiprocessing.Lock',
+        solvers: List[_Solver],
+        curr_stats: RegistrationStatistics
     ) -> int:
     """
     Checks for a new block and updates the current block information if a new block is found.
+
     Args:
         subtensor (:obj:`bittensor.Subtensor`, `required`):
             The subtensor object to use for getting the current block.
+        netuid (:obj:`int`, `required`):
+            The netuid to use for retrieving the difficulty.
         old_block_number (:obj:`int`, `required`):
             The old block number to check against.
+        hotkey_bytes (:obj:`bytes`, `required`):
+            The bytes of the hotkey's pubkey.
         curr_diff (:obj:`multiprocessing.Array`, `required`):
             The current difficulty as a multiprocessing array.
         curr_block (:obj:`multiprocessing.Array`, `required`):
             Where the current block is stored as a multiprocessing array.
         curr_block_num (:obj:`multiprocessing.Value`, `required`):
             Where the current block number is stored as a multiprocessing value.
         update_curr_block (:obj:`Callable`, `required`):
             A function that updates the current block.
         check_block (:obj:`multiprocessing.Lock`, `required`):
             A mp lock that is used to check for a new block.
-        solvers (:obj:`List[Solver]`, `required`):
+        solvers (:obj:`List[_Solver]`, `required`):
             A list of solvers to update the current block for.
         curr_stats (:obj:`RegistrationStatistics`, `required`):
             The current registration statistics to update.
+
     Returns:
         (int) The current block number.
     """
     block_number = subtensor.get_current_block()
     if block_number != old_block_number:
         old_block_number = block_number
         # update block information
-        block_hash = subtensor.substrate.get_block_hash( block_number)
-        while block_hash == None:
-            block_hash = subtensor.substrate.get_block_hash( block_number)
-        block_bytes = block_hash.encode('utf-8')[2:]
-        difficulty = subtensor.difficulty
+        block_number, difficulty, block_hash = _get_block_with_retry(subtensor = subtensor, netuid = netuid)
+        block_bytes = bytes.fromhex(block_hash[2:])
 
-        update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
+        update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, hotkey_bytes, check_block)
         # Set new block events for each solver
 
         for worker in solvers:
             worker.newBlockEvent.set()
 
         # update stats
         curr_stats.block_number = block_number
         curr_stats.block_hash = block_hash
         curr_stats.difficulty = difficulty
 
     return old_block_number
 
 
-def solve_for_difficulty_fast_cuda( subtensor: 'bittensor.Subtensor', wallet: 'bittensor.Wallet', output_in_place: bool = True, update_interval: int = 50_000, TPB: int = 512, dev_id: Union[List[int], int] = 0, n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
+def _solve_for_difficulty_fast_cuda( subtensor: 'bittensor.Subtensor', wallet: 'bittensor.Wallet', netuid: int, output_in_place: bool = True, update_interval: int = 50_000, TPB: int = 512, dev_id: Union[List[int], int] = 0, n_samples: int = 10, alpha_: float = 0.80, log_verbose: bool = False ) -> Optional[POWSolution]:
     """
     Solves the registration fast using CUDA
     Args:
         subtensor: bittensor.Subtensor
             The subtensor node to grab blocks
         wallet: bittensor.Wallet
             The wallet to register
+        netuid: int
+            The netuid of the subnet to register to.
         output_in_place: bool
             If true, prints the output in place, otherwise prints to new lines
         update_interval: int
             The number of nonces to try before checking for more blocks
         TPB: int
             The number of threads per block. CUDA param that should match the GPU capability
         dev_id: Union[List[int], int]
@@ -664,45 +670,42 @@
 
     if not torch.cuda.is_available():
         raise Exception("CUDA not available")
         
     limit = int(math.pow(2,256)) - 1
 
     # Set mp start to use spawn so CUDA doesn't complain
-    with UsingSpawnStartMethod(force=True):
-        curr_block = multiprocessing.Array('h', 64, lock=True) # byte array
-        curr_block_num = multiprocessing.Value('i', 0, lock=True) # int
-        curr_diff = multiprocessing.Array('Q', [0, 0], lock=True) # [high, low]
+    with _UsingSpawnStartMethod(force=True):
+        curr_block, curr_block_num, curr_diff = _CUDASolver.create_shared_memory()
 
         ## Create a worker per CUDA device
         num_processes = len(dev_id)
 
         # Establish communication queues
         stopEvent = multiprocessing.Event()
         stopEvent.clear()
         solution_queue = multiprocessing.Queue()
         finished_queues = [multiprocessing.Queue() for _ in range(num_processes)]
         check_block = multiprocessing.Lock()
+
+        hotkey_bytes = wallet.hotkey.public_key
         
         # Start workers
-        solvers = [ CUDASolver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit, dev_id[i], TPB)
+        solvers = [ _CUDASolver(i, num_processes, update_interval, finished_queues[i], solution_queue, stopEvent, curr_block, curr_block_num, curr_diff, check_block, limit, dev_id[i], TPB)
                     for i in range(num_processes) ]
 
 
         # Get first block
-        block_number = subtensor.get_current_block()
-        difficulty = subtensor.difficulty
-        block_hash = subtensor.substrate.get_block_hash( block_number )
-        while block_hash == None:
-            block_hash = subtensor.substrate.get_block_hash( block_number )
-        block_bytes = block_hash.encode('utf-8')[2:]
+        block_number, difficulty, block_hash = _get_block_with_retry(subtensor = subtensor, netuid = netuid)
+
+        block_bytes = bytes.fromhex(block_hash[2:])
         old_block_number = block_number
         
         # Set to current block
-        update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, check_block)
+        _update_curr_block(curr_diff, curr_block, curr_block_num, block_number, block_bytes, difficulty, hotkey_bytes, check_block)
 
         # Set new block events for each solver to start at the initial block
         for worker in solvers:
             worker.newBlockEvent.set()
         
         for worker in solvers:
             worker.start() # start the solver processes
@@ -728,33 +731,35 @@
         logger = RegistrationStatisticsLogger(console, output_in_place)
         logger.start()
 
         hash_rates = [0] * n_samples # The last n true hash_rates
         weights = [alpha_ ** i for i in range(n_samples)] # weights decay by alpha
 
         solution = None
-        while not wallet.is_registered(subtensor):
+        while not wallet.is_registered(netuid = netuid, subtensor = subtensor):
             # Wait until a solver finds a solution
             try:
                 solution = solution_queue.get(block=True, timeout=0.15)
                 if solution is not None:
                     break
             except Empty:
                 # No solution found, try again
                 pass
             
             # check for new block
-            old_block_number = check_for_newest_block_and_update(
+            old_block_number = _check_for_newest_block_and_update(
                 subtensor = subtensor,
+                netuid = netuid,
+                hotkey_bytes = hotkey_bytes,
                 curr_diff=curr_diff,
                 curr_block=curr_block,
                 curr_block_num=curr_block_num,
                 old_block_number=old_block_number,
                 curr_stats=curr_stats,
-                update_curr_block=update_curr_block,
+                update_curr_block=_update_curr_block,
                 check_block=check_block,
                 solvers=solvers
             )
                     
             num_time = 0
             # Get times for each solver
             for finished_queue in finished_queues:
@@ -792,44 +797,78 @@
         
         # exited while, found_solution contains the nonce or wallet is registered
         
         stopEvent.set() # stop all other processes
         logger.stop()
 
         # terminate and wait for all solvers to exit
-        terminate_workers_and_wait_for_exit(solvers)
+        _terminate_workers_and_wait_for_exit(solvers)
 
         return solution
 
 
-def terminate_workers_and_wait_for_exit(workers: List[multiprocessing.Process]) -> None:
+def _terminate_workers_and_wait_for_exit(workers: List[multiprocessing.Process]) -> None:
     for worker in workers:
         worker.terminate()
         worker.join()
 
 
 def create_pow(
-    subtensor,
-    wallet,
-    output_in_place: bool = True,
-    cuda: bool = False,
-    dev_id: Union[List[int], int] = 0,
-    tpb: int = 256,
-    num_processes: int = None,
-    update_interval: int = None,
-    log_verbose: bool = False
+        subtensor,
+        wallet,
+        netuid: int,
+        output_in_place: bool = True,
+        cuda: bool = False,
+        dev_id: Union[List[int], int] = 0,
+        tpb: int = 256,
+        num_processes: int = None,
+        update_interval: int = None,
+        log_verbose: bool = False
     ) -> Optional[Dict[str, Any]]:
+    """
+    Creates a proof of work for the given subtensor and wallet.
+    Args:
+        subtensor (:obj:`bittensor.subtensor.Subtensor`, `required`):
+            The subtensor to create a proof of work for.
+        wallet (:obj:`bittensor.wallet.Wallet`, `required`):
+            The wallet to create a proof of work for.
+        netuid (:obj:`int`, `required`):
+            The netuid for the subnet to create a proof of work for.
+        output_in_place (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            If true, prints the progress of the proof of work to the console
+                in-place. Meaning the progress is printed on the same lines.
+        cuda (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            If true, uses CUDA to solve the proof of work.
+        dev_id (:obj:`Union[List[int], int]`, `optional`, defaults to :obj:`0`):
+            The CUDA device id(s) to use. If cuda is true and dev_id is a list,
+                then multiple CUDA devices will be used to solve the proof of work.
+        tpb (:obj:`int`, `optional`, defaults to :obj:`256`):
+            The number of threads per block to use when solving the proof of work.
+            Should be a multiple of 32.
+        num_processes (:obj:`int`, `optional`, defaults to :obj:`None`):
+            The number of processes to use when solving the proof of work.
+            If None, then the number of processes is equal to the number of
+                CPU cores.
+        update_interval (:obj:`int`, `optional`, defaults to :obj:`None`):
+            The number of nonces to run before checking for a new block.
+        log_verbose (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            If true, prints the progress of the proof of work more verbosely.   
+    Returns:
+        :obj:`Optional[Dict[str, Any]]`: The proof of work solution or None if
+            the wallet is already registered or there is a different error.
+    
+    Raises:
+        :obj:`ValueError`: If the subnet does not exist.
+    """
+    if not subtensor.subnet_exists(netuid = netuid):
+        raise ValueError(f'Subnet {netuid} does not exist')
+
     if cuda:
-        solution: POWSolution = solve_for_difficulty_fast_cuda( subtensor, wallet, output_in_place=output_in_place, \
+        solution: Optional[POWSolution] = _solve_for_difficulty_fast_cuda( subtensor, wallet, netuid = netuid, output_in_place=output_in_place, \
             dev_id=dev_id, TPB=tpb, update_interval=update_interval, log_verbose=log_verbose
         )
     else:
-        solution: POWSolution = solve_for_difficulty_fast( subtensor, wallet, output_in_place=output_in_place, \
+        solution: Optional[POWSolution] = _solve_for_difficulty_fast( subtensor, wallet, netuid = netuid, output_in_place=output_in_place, \
             num_processes=num_processes, update_interval=update_interval, log_verbose=log_verbose
         )
 
-    return None if solution is None else {
-        'nonce': solution.nonce, 
-        'difficulty': solution.difficulty,
-        'block_number': solution.block_number, 
-        'work': binascii.hexlify(solution.seal)
-    }
+    return solution
```

### Comparing `bittensor-4.0.0/bittensor/utils/stats.py` & `bittensor-4.1.0rc1/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/utils/test_utils.py` & `bittensor-4.1.0rc1/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor/utils/tokenizer_utils.py` & `bittensor-4.1.0rc1/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.0.0/bittensor.egg-info/requires.txt` & `bittensor-4.1.0rc1/bittensor.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 ansible_vault>=2.1
 argparse==1.4.0
 backoff==2.1.0
 base58==2.0.1
 certifi==2020.11.8
 cryptography==39.0.0
 fuzzywuzzy==0.18.0
-google-api-python-client==2.6.0
+google-api-python-client==2.7.0
 grpcio-tools==1.42.0
 grpcio==1.42.0
 hypothesis==6.47.4
 idna==2.10
 jinja2==3.0
 jsonschema[format-nongpl]<=4.17.0,>=4.14.0
+langchain>=0.0.132
 loguru==0.6.0
 markupsafe==2.0.1
 miniupnpc==2.0.2
 msgpack-numpy==0.4.7.1
 msgpack==1.0.4
 munch==2.5.0
 nest_asyncio==1.5.6
@@ -38,20 +39,18 @@
 rich==12.5.1
 scalecodec==1.2.0
 sentencepiece==0.1.97
 substrate-interface==1.5.0
 termcolor==2.1.1
 torch==1.13.1
 tqdm==4.64.1
-transformers==4.20.1
-wandb<0.13.4,>=0.11.1
+transformers>=4.20.1
 wheel==0.37.1
 
 [dev]
-codecov==2.1.12
 coveralls==3.3.1
 ddt==1.6.0
 pytest-cov==4.0.0
 pytest-rerunfailures==10.2
 pytest-split==0.8.0
 pytest-xdist==3.0.2
 pytest==7.2.0
```

### Comparing `bittensor-4.0.0/setup.py` & `bittensor-4.1.0rc1/setup.py`

 * *Files identical despite different names*

