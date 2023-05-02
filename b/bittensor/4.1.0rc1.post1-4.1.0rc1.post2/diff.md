# Comparing `tmp/bittensor-4.1.0rc1.post1.tar.gz` & `tmp/bittensor-4.1.0rc1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-4.1.0rc1.post1.tar", last modified: Tue May  2 20:21:07 2023, max compression
+gzip compressed data, was "bittensor-4.1.0rc1.post2.tar", last modified: Tue May  2 20:38:49 2023, max compression
```

## Comparing `bittensor-4.1.0rc1.post1.tar` & `bittensor-4.1.0rc1.post2.tar`

### file list

```diff
@@ -1,102 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/
--rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4907 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3359 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bin/
--rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.1.0rc1.post1/bin/btcli
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/
--rw-rw-r--   0 root         (0) root         (0)    14544 2023-05-02 20:20:25.000000 bittensor-4.1.0rc1.post1/bittensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_axon/
--rw-rw-r--   0 root         (0) root         (0)    17744 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_axon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_cli/
--rw-rw-r--   0 root         (0) root         (0)     6688 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/cli_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/
--rw-rw-r--   0 root         (0) root         (0)      649 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    25104 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/delegates.py
--rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/inspect.py
--rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/list.py
--rw-rw-r--   0 root         (0) root         (0)     7193 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/metagraph.py
--rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/misc.py
--rw-rw-r--   0 root         (0) root         (0)    16429 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/overview.py
--rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/register.py
--rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/stake.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    11156 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/unstake.py
--rw-rw-r--   0 root         (0) root         (0)     7733 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/utils.py
--rw-rw-r--   0 root         (0) root         (0)    17664 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/wallets.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_cli/commands/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_config/
--rw-rw-r--   0 root         (0) root         (0)     6034 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5957 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_config/config_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_dataset/
--rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27097 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_dataset/dataset_impl.py
--rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_dataset/dataset_mock.py
--rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post1/bittensor/_dataset/thread_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_ipfs/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/bittensor/_ipfs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.1.0rc1.post1/bittensor/_ipfs/ipfs_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_keyfile/
--rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/bittensor/_keyfile/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_keyfile/keyfile_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_logging/
--rw-rw-r--   0 root         (0) root         (0)    13107 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_metagraph/
--rw-rw-r--   0 root         (0) root         (0)    12460 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post1/bittensor/_metagraph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_prometheus/
--rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_prometheus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_proto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/bittensor/_proto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    30214 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_proto/bittensor_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     4422 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_proto/bittensor_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor/_serializer/
--rw-rw-r--   0 root         (0) root         (0)     6078 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_serializer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10782 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_serializer/serializer_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/bittensor/_subtensor/
--rw-rw-r--   0 root         (0) root         (0)    14289 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26232 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/chain_data.py
--rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/delegation.py
--rw-rw-r--   0 root         (0) root         (0)    27011 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/log_utilities.py
--rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/prometheus.py
--rw-rw-r--   0 root         (0) root         (0)    14454 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/registration.py
--rw-rw-r--   0 root         (0) root         (0)    10152 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/serving.py
--rw-rw-r--   0 root         (0) root         (0)     6387 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/set_weights.py
--rw-rw-r--   0 root         (0) root         (0)    18492 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/staking.py
--rw-rw-r--   0 root         (0) root         (0)     7595 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    15591 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/unstaking.py
--rw-rw-r--   0 root         (0) root         (0)    45559 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/subtensor_impl.py
--rw-rw-r--   0 root         (0) root         (0)    18974 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/_subtensor/subtensor_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/bittensor/_threadpool/
--rw-rw-r--   0 root         (0) root         (0)     4517 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_threadpool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.1.0rc1.post1/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/bittensor/_tokenizer/
--rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post1/bittensor/_tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/bittensor/_wallet/
--rw-rw-r--   0 root         (0) root         (0)     7293 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/_wallet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/_wallet/wallet_impl.py
--rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/bittensor/_wallet/wallet_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/bittensor/utils/
--rw-rw-r--   0 root         (0) root         (0)     8575 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3443 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/utils/_register_cuda.py
--rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/utils/balance.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/utils/codes.py
--rw-rw-r--   0 root         (0) root         (0)      518 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/utils/formatting.py
--rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/utils/networking.py
--rw-rw-r--   0 root         (0) root         (0)    36116 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/utils/registration.py
--rw-rw-r--   0 root         (0) root         (0)    33174 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post1/bittensor/utils/registratrion_old.py
--rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/bittensor/utils/stats.py
--rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post1/bittensor/utils/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post1/bittensor/utils/tokenizer_utils.py
--rw-rw-r--   0 root         (0) root         (0)     9986 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post1/bittensor/utils/weight_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:21:07.982964 bittensor-4.1.0rc1.post1/bittensor.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4907 2023-05-02 20:21:07.000000 bittensor-4.1.0rc1.post1/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2600 2023-05-02 20:21:07.000000 bittensor-4.1.0rc1.post1/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 20:21:07.000000 bittensor-4.1.0rc1.post1/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)     1027 2023-05-02 20:21:07.000000 bittensor-4.1.0rc1.post1/bittensor.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       10 2023-05-02 20:21:07.000000 bittensor-4.1.0rc1.post1/bittensor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 20:21:07.986965 bittensor-4.1.0rc1.post1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-05-02 18:50:29.000000 bittensor-4.1.0rc1.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/
+-rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4907 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3359 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bin/
+-rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.1.0rc1.post2/bin/btcli
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/
+-rw-rw-r--   0 root         (0) root         (0)    14544 2023-05-02 20:38:21.000000 bittensor-4.1.0rc1.post2/bittensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/_axon/
+-rw-rw-r--   0 root         (0) root         (0)    17744 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_axon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/_cli/
+-rw-rw-r--   0 root         (0) root         (0)     6688 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/cli_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/
+-rw-rw-r--   0 root         (0) root         (0)      649 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    25104 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/delegates.py
+-rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/inspect.py
+-rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/list.py
+-rw-rw-r--   0 root         (0) root         (0)     7193 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/metagraph.py
+-rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    16429 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/overview.py
+-rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/register.py
+-rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/stake.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    11156 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/unstake.py
+-rw-rw-r--   0 root         (0) root         (0)     7733 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    17664 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/wallets.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_config/
+-rw-rw-r--   0 root         (0) root         (0)     6034 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5957 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_config/config_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_dataset/
+-rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27097 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_mock.py
+-rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/thread_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_dendrite/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:35:22.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10383 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/dendrite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:35:24.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7962 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/dendrite.py
+-rw-rw-r--   0 root         (0) root         (0)     5195 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/dendrite_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_ipfs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_ipfs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.1.0rc1.post2/bittensor/_ipfs/ipfs_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_keyfile/
+-rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_keyfile/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_keyfile/keyfile_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_logging/
+-rw-rw-r--   0 root         (0) root         (0)    13107 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_metagraph/
+-rw-rw-r--   0 root         (0) root         (0)    12460 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_metagraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_prometheus/
+-rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_prometheus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_proto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    30214 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     4422 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_serializer/
+-rw-rw-r--   0 root         (0) root         (0)     6078 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_serializer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10782 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_serializer/serializer_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_subtensor/
+-rw-rw-r--   0 root         (0) root         (0)    14289 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26232 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/chain_data.py
+-rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/delegation.py
+-rw-rw-r--   0 root         (0) root         (0)    27011 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-rw-r--   0 root         (0) root         (0)    14454 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    10152 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/serving.py
+-rw-rw-r--   0 root         (0) root         (0)     6387 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-rw-r--   0 root         (0) root         (0)    18492 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/staking.py
+-rw-rw-r--   0 root         (0) root         (0)     7595 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    15591 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-rw-r--   0 root         (0) root         (0)    45559 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    18974 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_synapse/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:33:22.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6777 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/synapse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:34:23.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10714 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/miner.py
+-rw-rw-r--   0 root         (0) root         (0)     5258 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/synapse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_threadpool/
+-rw-rw-r--   0 root         (0) root         (0)     4517 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_threadpool/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.1.0rc1.post2/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_tokenizer/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post2/bittensor/_tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_wallet/
+-rw-rw-r--   0 root         (0) root         (0)     7293 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_wallet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/utils/
+-rw-rw-r--   0 root         (0) root         (0)     8575 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3443 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/_register_cuda.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/balance.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/utils/codes.py
+-rw-rw-r--   0 root         (0) root         (0)      518 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/formatting.py
+-rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/networking.py
+-rw-rw-r--   0 root         (0) root         (0)    36116 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    33174 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/registratrion_old.py
+-rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/stats.py
+-rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/tokenizer_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     9986 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/utils/weight_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4907 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3005 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)     1027 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       10 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-05-02 18:50:29.000000 bittensor-4.1.0rc1.post2/setup.py
```

### Comparing `bittensor-4.1.0rc1.post1/LICENSE` & `bittensor-4.1.0rc1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/PKG-INFO` & `bittensor-4.1.0rc1.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 4.1.0rc1.post1
+Version: 4.1.0rc1.post2
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Description: <div align="center">
```

### Comparing `bittensor-4.1.0rc1.post1/README.md` & `bittensor-4.1.0rc1.post2/README.md`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bin/btcli` & `bittensor-4.1.0rc1.post2/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from langchain.llms.base import LLM
 from typing import Optional, List, Mapping, Any, Tuple
 
 import nest_asyncio
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = '4.1.0-rc1-1'
+__version__ = '4.1.0-rc1-2'
 version_split = __version__.split("-")[0].split(".")
 __version_as_int__ = (100 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
 __new_signature_version__ = 360
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
```

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_axon/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_axon/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/cli_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/delegates.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/inspect.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/list.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/metagraph.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/misc.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/overview.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/overview.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/register.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/stake.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/transfer.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/unstake.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/utils.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/wallets.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_cli/commands/weights.py` & `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_config/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_config/config_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_config/config_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_dataset/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_dataset/dataset_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_dataset/dataset_mock.py` & `bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_dataset/thread_queue.py` & `bittensor-4.1.0rc1.post2/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_ipfs/ipfs_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_keyfile/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_keyfile/keyfile_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_logging/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_metagraph/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_metagraph/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_prometheus/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_proto/bittensor_pb2.py` & `bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_serializer/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_serializer/serializer_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_serializer/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/chain_data.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/errors.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/log_utilities.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/subtensor_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_subtensor/subtensor_mock.py` & `bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_threadpool/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_threadpool/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_tokenizer/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_wallet/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/_wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_wallet/wallet_impl.py` & `bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/_wallet/wallet_mock.py` & `bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/__init__.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/_register_cuda.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/balance.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/codes.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/formatting.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/networking.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/registration.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/registratrion_old.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/registratrion_old.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/stats.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/test_utils.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/tokenizer_utils.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor/utils/weight_utils.py` & `bittensor-4.1.0rc1.post2/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/bittensor.egg-info/PKG-INFO` & `bittensor-4.1.0rc1.post2/bittensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 4.1.0rc1.post1
+Version: 4.1.0rc1.post2
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Description: <div align="center">
```

### Comparing `bittensor-4.1.0rc1.post1/bittensor.egg-info/requires.txt` & `bittensor-4.1.0rc1.post2/bittensor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post1/setup.py` & `bittensor-4.1.0rc1.post2/setup.py`

 * *Files identical despite different names*

