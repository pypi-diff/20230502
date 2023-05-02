# Comparing `tmp/IPFS-Toolkit-0.5.6.tar.gz` & `tmp/IPFS-Toolkit-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPFS-Toolkit-0.5.6.tar", last modified: Sun Apr 30 17:50:39 2023, max compression
+gzip compressed data, was "IPFS-Toolkit-0.5.7.tar", last modified: Tue May  2 10:39:00 2023, max compression
```

## Comparing `IPFS-Toolkit-0.5.6.tar` & `IPFS-Toolkit-0.5.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/IPFS_API.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/IPFS_DataTransmission.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/IPFS_LNS.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.546781 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1357 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/requires.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      105 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/PKG-INFO
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    19575 2023-04-30 14:11:24.000000 IPFS-Toolkit-0.5.6/ipfs_api.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.6/ipfs_cli.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.6/ipfs_datatransmission.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfs_lns.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.546781 IPFS-Toolkit-0.5.6/ipfshttpclient2/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/__init__.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/__init__.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/base.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bitswap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/block.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bootstrap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/config.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dag.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dht.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/files.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/key.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/miscellaneous.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/name.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/object.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/p2p.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pin.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pubsub.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/repo.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7484 2023-04-30 14:02:37.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/swarm.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/unstable.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/encoding.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/exceptions.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/filescanner.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http_common.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http_httpx.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http_requests.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/multipart.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/requests_wrapper.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/utils.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/version.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/setup.cfg
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1499 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/setup.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/tests/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3128 2023-04-30 17:44:05.000000 IPFS-Toolkit-0.5.6/tests/test_peers.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-30 17:45:34.000000 IPFS-Toolkit-0.5.6/tests/test_with_docker.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-30 17:46:18.000000 IPFS-Toolkit-0.5.6/tests/test_without_docker.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 10:39:00.401085 IPFS-Toolkit-0.5.7/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/IPFS_API.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/IPFS_DataTransmission.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/IPFS_LNS.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 10:39:00.397086 IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12580 2023-05-02 10:39:00.000000 IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1357 2023-05-02 10:39:00.000000 IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-05-02 10:39:00.000000 IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-05-02 10:39:00.000000 IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/requires.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      105 2023-05-02 10:39:00.000000 IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-05-02 10:39:00.401085 IPFS-Toolkit-0.5.7/PKG-INFO
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    19979 2023-05-02 09:44:19.000000 IPFS-Toolkit-0.5.7/ipfs_api.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.7/ipfs_cli.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.7/ipfs_datatransmission.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfs_lns.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 10:39:00.397086 IPFS-Toolkit-0.5.7/ipfshttpclient2/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/__init__.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 10:39:00.397086 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/__init__.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/base.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/bitswap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/block.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/bootstrap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/config.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/dag.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/dht.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/files.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/key.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/miscellaneous.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/name.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/object.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/p2p.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/pin.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/pubsub.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/repo.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7484 2023-04-30 17:51:07.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/swarm.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/client/unstable.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/encoding.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/exceptions.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/filescanner.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/http.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/http_common.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/http_httpx.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/http_requests.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/multipart.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/requests_wrapper.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/utils.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/ipfshttpclient2/version.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.7/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-02 10:39:00.401085 IPFS-Toolkit-0.5.7/setup.cfg
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1499 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.7/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 10:39:00.401085 IPFS-Toolkit-0.5.7/tests/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5311 2023-05-02 10:33:24.000000 IPFS-Toolkit-0.5.7/tests/test_peers.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-30 17:45:34.000000 IPFS-Toolkit-0.5.7/tests/test_with_docker.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-30 17:46:18.000000 IPFS-Toolkit-0.5.7/tests/test_without_docker.py
```

### Comparing `IPFS-Toolkit-0.5.6/IPFS_API.py` & `IPFS-Toolkit-0.5.7/IPFS_API.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/IPFS_DataTransmission.py` & `IPFS-Toolkit-0.5.7/IPFS_DataTransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/IPFS_LNS.py` & `IPFS-Toolkit-0.5.7/IPFS_LNS.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/PKG-INFO` & `IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.6
+Version: 0.5.7
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/SOURCES.txt` & `IPFS-Toolkit-0.5.7/IPFS_Toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/PKG-INFO` & `IPFS-Toolkit-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.6
+Version: 0.5.7
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IPFS-Toolkit-0.5.6/ipfs_api.py` & `IPFS-Toolkit-0.5.7/ipfs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,26 @@
         response = http_client.dht.findpeer(peer_id)
         if(len(response.get("Responses")[0].get("Addrs")) > 0):
             return response
     except:
         return None
 
 
+def is_peer_connected(peer_id, ping_count=1):
+    """Tests the connection to the given IPFS peer.
+    Args:
+        peer_id (str): the IPFS ID of the peer to test
+        count (int): (optional, default 1) the number of pings to send
+    Returns:
+        bool: whether or not the peer is connected
+    """
+    responses = http_client.ping(peer_id, count=ping_count)
+    return responses[-1]['Success']
+
+
 def find_providers(cid):
     """Lookup/find out which IPFS nodes provide the file with the given CID
     (including onesself).
     E.g. to check if this computer hosts a file with a certain CID:
     def DoWeHaveFile(cid:str):
         ipfs_api.my_id() in ipfs_api.find_providers(cid)
     Args:
```

### Comparing `IPFS-Toolkit-0.5.6/ipfs_cli.py` & `IPFS-Toolkit-0.5.7/ipfs_cli.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfs_datatransmission.py` & `IPFS-Toolkit-0.5.7/ipfs_datatransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfs_lns.py` & `IPFS-Toolkit-0.5.7/ipfs_lns.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/__init__.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/__init__.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/base.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/base.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bitswap.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/bitswap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/block.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/block.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bootstrap.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/bootstrap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/config.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/config.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dag.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/dag.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dht.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/dht.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/files.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/files.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/key.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/key.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/miscellaneous.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/name.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/name.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/object.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/object.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/p2p.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/p2p.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pin.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/pin.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pubsub.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/pubsub.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/repo.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/repo.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/swarm.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/swarm.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/unstable.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/client/unstable.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/encoding.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/encoding.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/exceptions.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/exceptions.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/filescanner.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/filescanner.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/http.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/http.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/http_common.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/http_common.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/http_httpx.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/http_httpx.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/http_requests.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/http_requests.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/multipart.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/multipart.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/requests_wrapper.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/utils.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/utils.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/ipfshttpclient2/version.py` & `IPFS-Toolkit-0.5.7/ipfshttpclient2/version.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/setup.py` & `IPFS-Toolkit-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/tests/test_with_docker.py` & `IPFS-Toolkit-0.5.7/tests/test_with_docker.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.6/tests/test_without_docker.py` & `IPFS-Toolkit-0.5.7/tests/test_without_docker.py`

 * *Files identical despite different names*

