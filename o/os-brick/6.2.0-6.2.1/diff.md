# Comparing `tmp/os-brick-6.2.0.tar.gz` & `tmp/os-brick-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-brick-6.2.0.tar", last modified: Mon Feb 13 16:55:39 2023, max compression
+gzip compressed data, was "os-brick-6.2.1.tar", last modified: Tue May  2 16:00:58 2023, max compression
```

## Comparing `os-brick-6.2.0.tar` & `os-brick-6.2.1.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:39.015097 os-brick-6.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-02-13 16:55:14.000000 os-brick-6.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-13 16:55:14.000000 os-brick-6.2.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-13 16:55:14.000000 os-brick-6.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2023-02-13 16:55:14.000000 os-brick-6.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6748 2023-02-13 16:55:38.000000 os-brick-6.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-02-13 16:55:14.000000 os-brick-6.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29781 2023-02-13 16:55:38.000000 os-brick-6.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-13 16:55:14.000000 os-brick-6.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-13 16:55:14.000000 os-brick-6.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2023-02-13 16:55:39.015097 os-brick-6.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-02-13 16:55:14.000000 os-brick-6.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2023-02-13 16:55:14.000000 os-brick-6.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.959105 os-brick-6.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.959105 os-brick-6.2.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.959105 os-brick-6.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.959105 os-brick-6.2.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.959105 os-brick-6.2.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.963104 os-brick-6.2.0/doc/source/reference/os_brick/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/reference/os_brick/exception.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/reference/os_brick/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.963104 os-brick-6.2.0/doc/source/reference/os_brick/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/reference/os_brick/initiator/connector.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/reference/os_brick/initiator/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.963104 os-brick-6.2.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2023-02-13 16:55:14.000000 os-brick-6.2.0/doc/source/user/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.951106 os-brick-6.2.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.951106 os-brick-6.2.0/etc/os-brick/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.963104 os-brick-6.2.0/etc/os-brick/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-02-13 16:55:14.000000 os-brick-6.2.0/etc/os-brick/rootwrap.d/os-brick.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-02-13 16:55:14.000000 os-brick-6.2.0/mypy-files.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.963104 os-brick-6.2.0/os_brick/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.967104 os-brick-6.2.0/os_brick/caches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/caches/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/caches/opencas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.967104 os-brick-6.2.0/os_brick/encryptors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5487 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/encryptors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/encryptors/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/encryptors/cryptsetup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8404 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/encryptors/luks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/encryptors/nop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.971103 os-brick-6.2.0/os_brick/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11636 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.975103 os-brick-6.2.0/os_brick/initiator/connectors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8025 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/base_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/base_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18094 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/fibre_channel_ppc64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/fibre_channel_s390x.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57916 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13060 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56888 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20407 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10364 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/storpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/connectors/vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/host_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/initiator_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13100 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/linuxfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/linuxrbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32119 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/linuxscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.975103 os-brick-6.2.0/os_brick/initiator/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4569 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/windows/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/windows/fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/windows/iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6727 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/windows/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/initiator/windows/smbfs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.975103 os-brick-6.2.0/os_brick/local_dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/local_dev/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34702 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/local_dev/lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.979102 os-brick-6.2.0/os_brick/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/privileged/lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/privileged/nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/privileged/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/privileged/rootwrap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/privileged/scaleio.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.979102 os-brick-6.2.0/os_brick/remotefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/remotefs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11191 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/remotefs/remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5513 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/remotefs/windows_remotefs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.979102 os-brick-6.2.0/os_brick/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.979102 os-brick-6.2.0/os_brick/tests/caches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/caches/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/caches/test_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6700 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/caches/test_opencas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.983101 os-brick-6.2.0/os_brick/tests/encryptors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/encryptors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/encryptors/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6846 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/encryptors/test_cryptsetup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11941 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/encryptors/test_luks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/encryptors/test_nop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.983101 os-brick-6.2.0/os_brick/tests/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.987101 os-brick-6.2.0/os_brick/tests/initiator/connectors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_base_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_base_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38122 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3720 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85008 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_iser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10989 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    96258 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25104 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3323 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13651 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_storpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18260 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/connectors/test_vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13407 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/test_host_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25343 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/test_linuxfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8497 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/test_linuxrbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64131 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/test_linuxscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/initiator/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.987101 os-brick-6.2.0/os_brick/tests/local_dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/local_dev/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/local_dev/fake_lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/local_dev/test_brick_lvm.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.991100 os-brick-6.2.0/os_brick/tests/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8114 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/privileged/test_nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/privileged/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9226 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/privileged/test_rootwrap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.991100 os-brick-6.2.0/os_brick/tests/remotefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/remotefs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11848 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/remotefs/test_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/remotefs/test_windows_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/test_brick.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/test_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25526 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.991100 os-brick-6.2.0/os_brick/tests/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/fake_win_conn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_base_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11642 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7736 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/tests/windows/test_smbfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14715 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-02-13 16:55:14.000000 os-brick-6.2.0/os_brick/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.967104 os-brick-6.2.0/os_brick.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10825 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-02-13 16:55:38.000000 os-brick-6.2.0/os_brick.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-02-13 16:55:14.000000 os-brick-6.2.0/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:38.955105 os-brick-6.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:39.011098 os-brick-6.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/add-luks2-support-13563cfe83aba69c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/add-vstorage-protocol-b536f4e21d764801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/add-windows-fibre-channel-030c095c149da321.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/add-windows-iscsi-15d6b1392695f978.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/add-windows-smbfs-d86edaa003130a31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/add_custom_keyring_for_rbd_connection-eccbaae9ee5f3491.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bp-lightbits-lightos-clustered-nvmetcp-connector-fd8dfd73330973e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1722432-2408dab55c903c5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1862443-e87ef38b60f9b979.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1884052-798094496dccf23c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1888675-mpath-resize-6013ce39fa2b8401.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1915678-901a6bd24ecede72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1924652-2323f905f62ef8ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1929223-powerflex-connector-certificate-validation-cf9ffc98391115d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1938870-af85c420d1a108a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1944474-55c5ebb3a37801aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-1945323-4140f5aff3558082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/bug-nvmeof-connector-support-multipath-kernels-ff6f1f27fdea2c8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/default-timeout-26c838af8b7af9fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/delay-legacy-encryption-provider-name-deprecation-c0d07be3f0d92afd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/deprecate-plain-cryptsetup-encryptor-0a279abc0b0d718c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/disconnect-multipath-cfg-changed-637abc5ecf44fb10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/encryption-a642889a82ff9207.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/lock_path-c1c58a253391b41c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/lvm-delete-error-76f2cc9d8dc91f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/multipath-improvements-596c2c6eadfba6ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/multipath-nvme-f77a53eb2717a44c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/no-systool-use-b7bc430de1033670.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvme-flush-f31ab337224e5d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvme-hostnqn-c2611dc56729183b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvme-rsd-support-d487afd77c534fa1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvmeof-disconnect-83f9aaf17f8c8988.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvmeof-hide-traceback-a968ab71352684e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/nvmeof-multiple-volumes-within-subsystem-support-05879c1c3bdf52c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/privsep-logs-9e938e5a2aee042e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/rbd-disconnect-failure-9efa6932df40271b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/rbd-non-openstack-support-28ee093d7d3a700e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/rbd-windows-support-ef6e8184842409dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/rbd_check_valid_device-2f50c0639adb8e7c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/rbd_extend_volume-5bc6adc08f662c5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/refactor_iscsi_connect-dfbb24305a954783.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/refactor_iscsi_disconnect-557f4173bc1ae4ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-aoe-7a97315a73c7b24f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-bug-1633518-workaround-75c2e26843660696.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-disco-0809537ffb8c50eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-drbd-21872230fcac1138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-hgst-daa7f07c307974d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-hyperscale-468f1b61bf4dadf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-old-constants-20021f5b30bde890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/remove-sheepdog-611257b28bc88934.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/scaleio-extend-attached-ec44d3a72395882c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/start-using-reno-23e8d5f1a30851a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:39.015097 os-brick-6.2.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:39.015097 os-brick-6.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:39.015097 os-brick-6.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-13 16:55:14.000000 os-brick-6.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-02-13 16:55:14.000000 os-brick-6.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2023-02-13 16:55:39.015097 os-brick-6.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-13 16:55:14.000000 os-brick-6.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-02-13 16:55:14.000000 os-brick-6.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:55:39.015097 os-brick-6.2.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2023-02-13 16:55:14.000000 os-brick-6.2.0/tools/fast8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6189 2023-02-13 16:55:14.000000 os-brick-6.2.0/tools/generate_connector_list.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6793 2023-02-13 16:55:14.000000 os-brick-6.2.0/tools/lintstack.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2023-02-13 16:55:14.000000 os-brick-6.2.0/tools/lintstack.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-02-13 16:55:14.000000 os-brick-6.2.0/tools/mypywrap.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-02-13 16:55:14.000000 os-brick-6.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.477865 os-brick-6.2.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-02 16:00:25.000000 os-brick-6.2.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-02 16:00:25.000000 os-brick-6.2.1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-05-02 16:00:25.000000 os-brick-6.2.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2023-05-02 16:00:25.000000 os-brick-6.2.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6748 2023-05-02 16:00:58.000000 os-brick-6.2.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-05-02 16:00:25.000000 os-brick-6.2.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29923 2023-05-02 16:00:57.000000 os-brick-6.2.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-02 16:00:25.000000 os-brick-6.2.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-02 16:00:25.000000 os-brick-6.2.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-02 16:00:58.477865 os-brick-6.2.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-05-02 16:00:25.000000 os-brick-6.2.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2023-05-02 16:00:25.000000 os-brick-6.2.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/reference/os_brick/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/exception.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/doc/source/reference/os_brick/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/initiator/connector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/initiator/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/user/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.409869 os-brick-6.2.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.409869 os-brick-6.2.1/etc/os-brick/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/etc/os-brick/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-02 16:00:25.000000 os-brick-6.2.1/etc/os-brick/rootwrap.d/os-brick.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-05-02 16:00:25.000000 os-brick-6.2.1/mypy-files.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/os_brick/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.429868 os-brick-6.2.1/os_brick/caches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/caches/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/caches/opencas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.429868 os-brick-6.2.1/os_brick/encryptors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5487 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/cryptsetup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8404 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/luks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/nop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.429868 os-brick-6.2.1/os_brick/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11636 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/initiator/connectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8025 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/base_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/base_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18094 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_ppc64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_s390x.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/gpfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57916 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13060 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56888 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20407 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10364 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/storpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/host_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/initiator_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13100 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/linuxfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/linuxrbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32119 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/linuxscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/initiator/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4569 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6727 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/smbfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/local_dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/local_dev/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34702 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/local_dev/lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/rootwrap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/scaleio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/remotefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/remotefs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11191 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/remotefs/remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5513 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/remotefs/windows_remotefs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/tests/caches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/caches/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/caches/test_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6700 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/caches/test_opencas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/tests/encryptors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6846 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_cryptsetup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11941 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_luks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_nop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.445867 os-brick-6.2.1/os_brick/tests/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/initiator/connectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38122 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3720 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_gpfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85008 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10989 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    96258 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25104 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3323 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13651 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_storpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18260 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13407 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_host_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25343 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_linuxfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8497 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_linuxrbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64131 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_linuxscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/local_dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/local_dev/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/local_dev/fake_lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/local_dev/test_brick_lvm.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8114 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/test_nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9226 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/test_rootwrap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/remotefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/remotefs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11848 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/remotefs/test_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/remotefs/test_windows_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_brick.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25526 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.453866 os-brick-6.2.1/os_brick/tests/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/fake_win_conn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_base_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11642 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7736 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_smbfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14715 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/os_brick.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10825 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-05-02 16:00:25.000000 os-brick-6.2.1/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.413869 os-brick-6.2.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.469865 os-brick-6.2.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-luks2-support-13563cfe83aba69c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-vstorage-protocol-b536f4e21d764801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-windows-fibre-channel-030c095c149da321.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-windows-iscsi-15d6b1392695f978.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-windows-smbfs-d86edaa003130a31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add_custom_keyring_for_rbd_connection-eccbaae9ee5f3491.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bp-lightbits-lightos-clustered-nvmetcp-connector-fd8dfd73330973e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1722432-2408dab55c903c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1862443-e87ef38b60f9b979.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1884052-798094496dccf23c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1888675-mpath-resize-6013ce39fa2b8401.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1915678-901a6bd24ecede72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1924652-2323f905f62ef8ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1929223-powerflex-connector-certificate-validation-cf9ffc98391115d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1938870-af85c420d1a108a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1944474-55c5ebb3a37801aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1945323-4140f5aff3558082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-nvmeof-connector-support-multipath-kernels-ff6f1f27fdea2c8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/default-timeout-26c838af8b7af9fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/delay-legacy-encryption-provider-name-deprecation-c0d07be3f0d92afd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/deprecate-plain-cryptsetup-encryptor-0a279abc0b0d718c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/disconnect-multipath-cfg-changed-637abc5ecf44fb10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/encryption-a642889a82ff9207.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/lock_path-c1c58a253391b41c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/lvm-delete-error-76f2cc9d8dc91f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/multipath-improvements-596c2c6eadfba6ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/multipath-nvme-f77a53eb2717a44c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/no-systool-use-b7bc430de1033670.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvme-flush-f31ab337224e5d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvme-hostnqn-c2611dc56729183b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvme-rsd-support-d487afd77c534fa1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-disconnect-83f9aaf17f8c8988.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-hide-traceback-a968ab71352684e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-multiple-volumes-within-subsystem-support-05879c1c3bdf52c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/privsep-logs-9e938e5a2aee042e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd-disconnect-failure-9efa6932df40271b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd-non-openstack-support-28ee093d7d3a700e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd-windows-support-ef6e8184842409dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd_check_valid_device-2f50c0639adb8e7c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd_extend_volume-5bc6adc08f662c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/refactor_iscsi_connect-dfbb24305a954783.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/refactor_iscsi_disconnect-557f4173bc1ae4ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-aoe-7a97315a73c7b24f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-bug-1633518-workaround-75c2e26843660696.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-disco-0809537ffb8c50eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-drbd-21872230fcac1138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-hgst-daa7f07c307974d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-hyperscale-468f1b61bf4dadf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-old-constants-20021f5b30bde890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-sheepdog-611257b28bc88934.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/scaleio-extend-attached-ec44d3a72395882c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/start-using-reno-23e8d5f1a30851a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.473865 os-brick-6.2.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.473865 os-brick-6.2.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.473865 os-brick-6.2.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-05-02 16:00:25.000000 os-brick-6.2.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-05-02 16:00:58.477865 os-brick-6.2.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-02 16:00:25.000000 os-brick-6.2.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-05-02 16:00:25.000000 os-brick-6.2.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.477865 os-brick-6.2.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/fast8.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6189 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/generate_connector_list.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6793 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/lintstack.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/lintstack.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/mypywrap.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-05-02 16:00:25.000000 os-brick-6.2.1/tox.ini
```

### Comparing `os-brick-6.2.0/.zuul.yaml` & `os-brick-6.2.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/AUTHORS` & `os-brick-6.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/CONTRIBUTING.rst` & `os-brick-6.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/ChangeLog` & `os-brick-6.2.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+6.2.1
+-----
+
+* Add Python 3.10 to setup.cfg metadata
+* Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
+* Update .gitreview for stable/2023.1
+
 6.2.0
 -----
 
 * Update minimum requirements in os-brick
 * Fix wrong assertion methods
 * Bump hacking to 4.1.0
 * Support separate privsep logging levels
```

### Comparing `os-brick-6.2.0/LICENSE` & `os-brick-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/PKG-INFO` & `os-brick-6.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-brick
-Version: 6.2.0
+Version: 6.2.1
 Summary: OpenStack Cinder brick library for managing local volume attaches
 Home-page: https://docs.openstack.org/os-brick/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Cinder brick library for managing local volume attaches
 Platform: UNKNOWN
@@ -15,8 +15,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

### Comparing `os-brick-6.2.0/README.rst` & `os-brick-6.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/bindep.txt` & `os-brick-6.2.1/bindep.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/doc/source/conf.py` & `os-brick-6.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/doc/source/contributor/contributing.rst` & `os-brick-6.2.1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/doc/source/reference/os_brick/exception.rst` & `os-brick-6.2.1/doc/source/reference/os_brick/exception.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/doc/source/reference/os_brick/initiator/connector.rst` & `os-brick-6.2.1/doc/source/reference/os_brick/initiator/connector.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/doc/source/user/tutorial.rst` & `os-brick-6.2.1/doc/source/user/tutorial.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/mypy-files.txt` & `os-brick-6.2.1/mypy-files.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/__init__.py` & `os-brick-6.2.1/os_brick/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/caches/__init__.py` & `os-brick-6.2.1/os_brick/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/caches/opencas.py` & `os-brick-6.2.1/os_brick/caches/opencas.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/encryptors/__init__.py` & `os-brick-6.2.1/os_brick/encryptors/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/encryptors/base.py` & `os-brick-6.2.1/os_brick/encryptors/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/encryptors/cryptsetup.py` & `os-brick-6.2.1/os_brick/encryptors/cryptsetup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/encryptors/luks.py` & `os-brick-6.2.1/os_brick/encryptors/luks.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/encryptors/nop.py` & `os-brick-6.2.1/os_brick/encryptors/nop.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/exception.py` & `os-brick-6.2.1/os_brick/exception.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/executor.py` & `os-brick-6.2.1/os_brick/executor.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/i18n.py` & `os-brick-6.2.1/os_brick/i18n.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/__init__.py` & `os-brick-6.2.1/os_brick/initiator/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connector.py` & `os-brick-6.2.1/os_brick/initiator/connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/base.py` & `os-brick-6.2.1/os_brick/initiator/connectors/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/base_iscsi.py` & `os-brick-6.2.1/os_brick/initiator/connectors/base_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/base_rbd.py` & `os-brick-6.2.1/os_brick/initiator/connectors/base_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/fake.py` & `os-brick-6.2.1/os_brick/initiator/connectors/fake.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/fibre_channel.py` & `os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/fibre_channel_ppc64.py` & `os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_ppc64.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/fibre_channel_s390x.py` & `os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_s390x.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/gpfs.py` & `os-brick-6.2.1/os_brick/initiator/connectors/gpfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/huawei.py` & `os-brick-6.2.1/os_brick/initiator/connectors/huawei.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/iscsi.py` & `os-brick-6.2.1/os_brick/initiator/connectors/iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/lightos.py` & `os-brick-6.2.1/os_brick/initiator/connectors/lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/local.py` & `os-brick-6.2.1/os_brick/initiator/connectors/local.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/nvmeof.py` & `os-brick-6.2.1/os_brick/initiator/connectors/nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/rbd.py` & `os-brick-6.2.1/os_brick/initiator/connectors/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/remotefs.py` & `os-brick-6.2.1/os_brick/initiator/connectors/remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/scaleio.py` & `os-brick-6.2.1/os_brick/initiator/connectors/scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/storpool.py` & `os-brick-6.2.1/os_brick/initiator/connectors/storpool.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/connectors/vmware.py` & `os-brick-6.2.1/os_brick/initiator/connectors/vmware.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/host_driver.py` & `os-brick-6.2.1/os_brick/initiator/host_driver.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/initiator_connector.py` & `os-brick-6.2.1/os_brick/initiator/initiator_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/linuxfc.py` & `os-brick-6.2.1/os_brick/initiator/linuxfc.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/linuxrbd.py` & `os-brick-6.2.1/os_brick/initiator/linuxrbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/linuxscsi.py` & `os-brick-6.2.1/os_brick/initiator/linuxscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/utils.py` & `os-brick-6.2.1/os_brick/initiator/utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/windows/base.py` & `os-brick-6.2.1/os_brick/initiator/windows/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/windows/fibre_channel.py` & `os-brick-6.2.1/os_brick/initiator/windows/fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/windows/iscsi.py` & `os-brick-6.2.1/os_brick/initiator/windows/iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/windows/rbd.py` & `os-brick-6.2.1/os_brick/initiator/windows/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/initiator/windows/smbfs.py` & `os-brick-6.2.1/os_brick/initiator/windows/smbfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/local_dev/lvm.py` & `os-brick-6.2.1/os_brick/local_dev/lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/opts.py` & `os-brick-6.2.1/os_brick/opts.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/privileged/__init__.py` & `os-brick-6.2.1/os_brick/privileged/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/privileged/lightos.py` & `os-brick-6.2.1/os_brick/privileged/lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/privileged/nvmeof.py` & `os-brick-6.2.1/os_brick/privileged/nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/privileged/rbd.py` & `os-brick-6.2.1/os_brick/privileged/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/privileged/rootwrap.py` & `os-brick-6.2.1/os_brick/privileged/rootwrap.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/privileged/scaleio.py` & `os-brick-6.2.1/os_brick/privileged/scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/remotefs/remotefs.py` & `os-brick-6.2.1/os_brick/remotefs/remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/remotefs/windows_remotefs.py` & `os-brick-6.2.1/os_brick/remotefs/windows_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/base.py` & `os-brick-6.2.1/os_brick/tests/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/caches/test_init.py` & `os-brick-6.2.1/os_brick/tests/caches/test_init.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/caches/test_opencas.py` & `os-brick-6.2.1/os_brick/tests/caches/test_opencas.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/encryptors/test_base.py` & `os-brick-6.2.1/os_brick/tests/encryptors/test_base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/encryptors/test_cryptsetup.py` & `os-brick-6.2.1/os_brick/tests/encryptors/test_cryptsetup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/encryptors/test_luks.py` & `os-brick-6.2.1/os_brick/tests/encryptors/test_luks.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/encryptors/test_nop.py` & `os-brick-6.2.1/os_brick/tests/encryptors/test_nop.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_base_iscsi.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_base_rbd.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_fibre_channel.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_gpfs.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_gpfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_huawei.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_huawei.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_iscsi.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_iser.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iser.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_lightos.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_local.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_nvmeof.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_rbd.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_remotefs.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_scaleio.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_storpool.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_storpool.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/connectors/test_vmware.py` & `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_vmware.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/test_connector.py` & `os-brick-6.2.1/os_brick/tests/initiator/test_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/test_host_driver.py` & `os-brick-6.2.1/os_brick/tests/initiator/test_host_driver.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/test_linuxfc.py` & `os-brick-6.2.1/os_brick/tests/initiator/test_linuxfc.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/test_linuxrbd.py` & `os-brick-6.2.1/os_brick/tests/initiator/test_linuxrbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/test_linuxscsi.py` & `os-brick-6.2.1/os_brick/tests/initiator/test_linuxscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/initiator/test_utils.py` & `os-brick-6.2.1/os_brick/tests/initiator/test_utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/local_dev/fake_lvm.py` & `os-brick-6.2.1/os_brick/tests/local_dev/fake_lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/local_dev/test_brick_lvm.py` & `os-brick-6.2.1/os_brick/tests/local_dev/test_brick_lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/privileged/test_nvmeof.py` & `os-brick-6.2.1/os_brick/tests/privileged/test_nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/privileged/test_rbd.py` & `os-brick-6.2.1/os_brick/tests/privileged/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/privileged/test_rootwrap.py` & `os-brick-6.2.1/os_brick/tests/privileged/test_rootwrap.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/remotefs/test_remotefs.py` & `os-brick-6.2.1/os_brick/tests/remotefs/test_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/remotefs/test_windows_remotefs.py` & `os-brick-6.2.1/os_brick/tests/remotefs/test_windows_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/test_brick.py` & `os-brick-6.2.1/os_brick/tests/test_brick.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/test_exception.py` & `os-brick-6.2.1/os_brick/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/test_executor.py` & `os-brick-6.2.1/os_brick/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/test_utils.py` & `os-brick-6.2.1/os_brick/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/fake_win_conn.py` & `os-brick-6.2.1/os_brick/tests/windows/fake_win_conn.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_base.py` & `os-brick-6.2.1/os_brick/tests/windows/test_base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_base_connector.py` & `os-brick-6.2.1/os_brick/tests/windows/test_base_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_factory.py` & `os-brick-6.2.1/os_brick/tests/windows/test_factory.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_fibre_channel.py` & `os-brick-6.2.1/os_brick/tests/windows/test_fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_iscsi.py` & `os-brick-6.2.1/os_brick/tests/windows/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_rbd.py` & `os-brick-6.2.1/os_brick/tests/windows/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/tests/windows/test_smbfs.py` & `os-brick-6.2.1/os_brick/tests/windows/test_smbfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/utils.py` & `os-brick-6.2.1/os_brick/utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick/version.py` & `os-brick-6.2.1/os_brick/version.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/os_brick.egg-info/PKG-INFO` & `os-brick-6.2.1/os_brick.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-brick
-Version: 6.2.0
+Version: 6.2.1
 Summary: OpenStack Cinder brick library for managing local volume attaches
 Home-page: https://docs.openstack.org/os-brick/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Cinder brick library for managing local volume attaches
 Platform: UNKNOWN
@@ -15,8 +15,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

### Comparing `os-brick-6.2.0/os_brick.egg-info/SOURCES.txt` & `os-brick-6.2.1/os_brick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/pylintrc` & `os-brick-6.2.1/pylintrc`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml` & `os-brick-6.2.1/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml` & `os-brick-6.2.1/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml` & `os-brick-6.2.1/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml` & `os-brick-6.2.1/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/notes/lock_path-c1c58a253391b41c.yaml` & `os-brick-6.2.1/releasenotes/notes/lock_path-c1c58a253391b41c.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml` & `os-brick-6.2.1/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/releasenotes/source/conf.py` & `os-brick-6.2.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/requirements.txt` & `os-brick-6.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/setup.cfg` & `os-brick-6.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [files]
 packages = 
 	os_brick
 data_files = 
 	etc/ = etc/*
```

### Comparing `os-brick-6.2.0/setup.py` & `os-brick-6.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/test-requirements.txt` & `os-brick-6.2.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/tools/generate_connector_list.py` & `os-brick-6.2.1/tools/generate_connector_list.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/tools/lintstack.py` & `os-brick-6.2.1/tools/lintstack.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/tools/lintstack.sh` & `os-brick-6.2.1/tools/lintstack.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/tools/mypywrap.sh` & `os-brick-6.2.1/tools/mypywrap.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.0/tox.ini` & `os-brick-6.2.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     VIRTUAL_ENV={envdir}
     OS_TEST_PATH=./os_brick/tests
     OS_TEST_TIMEOUT=60
     OS_STDOUT_CAPTURE=1
     OS_STDERR_CAPTURE=1
 
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 
 # By default stestr will set concurrency
 # to ncpu, to specify something else use
 # the concurrency=<n> option.
 # call example: 'tox -epy37 -- --concurrency=4'
@@ -61,15 +61,15 @@
 [testenv:bandit]
 deps = -r{toxinidir}/test-requirements.txt
 # B101: skip assert used checks, they are validly used for mypy
 commands: bandit -r os_brick -x os_brick/tests -n5 -sB101
 
 [testenv:pylint]
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/requirements.txt
        pylint==0.26.0
 commands = bash tools/lintstack.sh
 
 [testenv:venv]
 commands = {posargs}
 
@@ -83,15 +83,15 @@
     stestr run {posargs}
     coverage combine
     coverage html -d cover
     coverage xml -o cover/coverage/xml
 
 [testenv:docs]
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
   -r{toxinidir}/doc/requirements.txt
 commands =
   rm -fr doc/build doc/source/contributor/api/ .autogenerated
   sphinx-build -W -b html -d doc/build/doctrees doc/source doc/build/html
 allowlist_externals = rm
 
 [testenv:pdf-docs]
```

