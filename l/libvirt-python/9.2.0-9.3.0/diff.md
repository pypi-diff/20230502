# Comparing `tmp/libvirt-python-9.2.0.tar.gz` & `tmp/libvirt-python-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvirt-python-9.2.0.tar", last modified: Sat Apr  1 07:54:19 2023, max compression
+gzip compressed data, was "libvirt-python-9.3.0.tar", last modified: Tue May  2 12:18:43 2023, max compression
```

## Comparing `libvirt-python-9.2.0.tar` & `libvirt-python-9.3.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.086148 libvirt-python-9.2.0/
--rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.2.0/.ctags
--rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.2.0/.dir-locals.el
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.069481 libvirt-python-9.2.0/.github/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.079481 libvirt-python-9.2.0/.github/workflows/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.2.0/.github/workflows/lockdown.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/.gitignore
--rw-rw-r--   0 jirka      (500) jirka      (500)     2661 2022-11-01 11:36:52.000000 libvirt-python-9.2.0/.gitlab-ci.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.2.0/.mailmap
--rw-rw-r--   0 jirka      (500) jirka      (500)     3979 2023-04-01 07:54:18.000000 libvirt-python-9.2.0/AUTHORS
--rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.2.0/AUTHORS.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 jirka      (500) jirka      (500)    18092 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/COPYING
--rw-rw-r--   0 jirka      (500) jirka      (500)    26530 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/COPYING.LESSER
--rw-rw-r--   0 jirka      (500) jirka      (500)   404089 2023-04-01 07:54:18.000000 libvirt-python-9.2.0/ChangeLog
--rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/HACKING
--rw-rw-r--   0 jirka      (500) jirka      (500)     1283 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/MANIFEST
--rw-rw-r--   0 jirka      (500) jirka      (500)     1704 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/MANIFEST.in
--rw-rw-r--   0 jirka      (500) jirka      (500)      260 2016-10-04 07:42:23.000000 libvirt-python-9.2.0/Makefile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1162 2023-04-01 07:54:19.086148 libvirt-python-9.2.0/PKG-INFO
--rw-rw-r--   0 jirka      (500) jirka      (500)     1384 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/README
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.069481 libvirt-python-9.2.0/build/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.086148 libvirt-python-9.2.0/build/libvirt_python.egg-info/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2328 2023-04-01 07:54:19.000000 libvirt-python-9.2.0/build/libvirt_python.egg-info/SOURCES.txt
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.079481 libvirt-python-9.2.0/ci/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.079481 libvirt-python-9.2.0/ci/buildenv/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1407 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/centos-stream-8.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      965 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/centos-stream-9.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/debian-10.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/debian-sid.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      798 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/fedora-36.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/buildenv/fedora-37.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      850 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/fedora-rawhide.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      846 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/opensuse-leap-153.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      852 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/opensuse-tumbleweed.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/ubuntu-2004.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/buildenv/ubuntu-2204.sh
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.079481 libvirt-python-9.2.0/ci/containers/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1499 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/centos-stream-8.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/centos-stream-9.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1370 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/debian-10.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1371 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/debian-sid.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1280 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/fedora-36.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1280 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/containers/fedora-37.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1342 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/fedora-rawhide.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      905 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/opensuse-leap-153.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      919 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/opensuse-tumbleweed.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/ubuntu-2004.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.2.0/ci/containers/ubuntu-2204.Dockerfile
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.082814 libvirt-python-9.2.0/ci/gitlab/
--rw-rw-r--   0 jirka      (500) jirka      (500)     5363 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/gitlab/build-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     5757 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/gitlab/builds.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/gitlab/container-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1450 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/gitlab/containers.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      735 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/gitlab/sanity-checks.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     2447 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/gitlab.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1269 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/ci/manifest.yml
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.082814 libvirt-python-9.2.0/examples/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/README
--rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/consolecallback.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/dhcpleases.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/dominfo.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/domipaddrs.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/domrestore.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/domsave.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/domstart.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/esxlist.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    35898 2022-07-01 09:27:33.000000 libvirt-python-9.2.0/examples/event-test.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.082814 libvirt-python-9.2.0/examples/guest-vcpus/
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/guest-vcpus/guest-vcpu-daemon.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/guest-vcpus/guest-vcpu.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/nodestats.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/sparsestream.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/examples/topology.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    70037 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/generator.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-lxc-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-lxc-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.2.0/libvirt-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    31114 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-override-virConnect.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.2.0/libvirt-override-virDomain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-override-virDomainCheckpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-override-virDomainSnapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-override-virNetwork.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-override-virStoragePool.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-override-virStream.py
--rw-rw-r--   0 jirka      (500) jirka      (500)   329516 2023-03-01 10:15:08.000000 libvirt-python-9.2.0/libvirt-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.2.0/libvirt-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2749 2023-04-01 07:54:18.000000 libvirt-python-9.2.0/libvirt-python.spec
--rw-rw-r--   0 jirka      (500) jirka      (500)     2756 2022-12-01 09:59:29.000000 libvirt-python-9.2.0/libvirt-python.spec.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-qemu-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    14037 2023-03-01 10:15:08.000000 libvirt-python-9.2.0/libvirt-qemu-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.2.0/libvirt-qemu-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16182 2022-07-11 21:25:49.000000 libvirt-python-9.2.0/libvirt-utils.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/libvirt-utils.h
--rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.2.0/libvirtaio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/requirements-test.txt
--rw-rw-r--   0 jirka      (500) jirka      (500)       38 2023-04-01 07:54:19.086148 libvirt-python-9.2.0/setup.cfg
--rwxrwxr-x   0 jirka      (500) jirka      (500)    11854 2023-04-01 07:52:33.000000 libvirt-python-9.2.0/setup.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-04-01 07:54:19.086148 libvirt-python-9.2.0/tests/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.2.0/tests/eventmock.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.2.0/tests/test_aio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.2.0/tests/test_api_coverage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_conn.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_domain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_domain_checkpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_domain_snapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_interface.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_network.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_nodedev.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tests/test_storage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      114 2022-04-01 10:30:02.000000 libvirt-python-9.2.0/tox.ini
--rw-rw-r--   0 jirka      (500) jirka      (500)    10721 2023-03-01 10:15:08.000000 libvirt-python-9.2.0/typewrappers.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.2.0/typewrappers.h
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/
+-rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.3.0/.ctags
+-rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.3.0/.dir-locals.el
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.075835 libvirt-python-9.3.0/.github/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.079168 libvirt-python-9.3.0/.github/workflows/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.3.0/.github/workflows/lockdown.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/.gitignore
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2693 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/.gitlab-ci.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.3.0/.mailmap
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3979 2023-05-02 12:18:42.000000 libvirt-python-9.3.0/AUTHORS
+-rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.3.0/AUTHORS.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 jirka      (500) jirka      (500)    18092 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/COPYING
+-rw-rw-r--   0 jirka      (500) jirka      (500)    26530 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/COPYING.LESSER
+-rw-rw-r--   0 jirka      (500) jirka      (500)   405825 2023-05-02 12:18:42.000000 libvirt-python-9.3.0/ChangeLog
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/HACKING
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1283 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/MANIFEST
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1704 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/MANIFEST.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)      260 2016-10-04 07:42:23.000000 libvirt-python-9.3.0/Makefile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1162 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/PKG-INFO
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1384 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/README
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.075835 libvirt-python-9.3.0/build/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/build/libvirt_python.egg-info/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2328 2023-05-02 12:18:43.000000 libvirt-python-9.3.0/build/libvirt_python.egg-info/SOURCES.txt
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.079168 libvirt-python-9.3.0/ci/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/ci/buildenv/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1407 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/centos-stream-8.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      965 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/centos-stream-9.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/debian-10.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/debian-sid.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      798 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/fedora-36.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/ci/buildenv/fedora-37.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      850 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/fedora-rawhide.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      846 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/buildenv/opensuse-leap-154.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      852 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/opensuse-tumbleweed.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/ubuntu-2004.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/ubuntu-2204.sh
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/ci/containers/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1499 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/centos-stream-8.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/centos-stream-9.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1370 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/debian-10.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1371 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/debian-sid.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/fedora-36.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/fedora-37.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1343 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/fedora-rawhide.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/opensuse-leap-154.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      919 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/opensuse-tumbleweed.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/ubuntu-2004.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/ubuntu-2204.Dockerfile
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/ci/gitlab/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/build-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5849 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/builds.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/ci/gitlab/container-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1447 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/containers.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/sanity-checks.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1475 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/manifest.yml
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/examples/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/README
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/consolecallback.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/dhcpleases.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/dominfo.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domipaddrs.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domrestore.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domsave.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domstart.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/esxlist.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    35898 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/examples/event-test.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/examples/guest-vcpus/
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu-daemon.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/nodestats.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/sparsestream.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/topology.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    70037 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/generator.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-lxc-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-lxc-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.3.0/libvirt-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    31114 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virConnect.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/libvirt-override-virDomain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virDomainCheckpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virDomainSnapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virNetwork.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virStoragePool.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virStream.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)   329516 2023-03-01 10:15:08.000000 libvirt-python-9.3.0/libvirt-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.3.0/libvirt-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2759 2023-05-02 12:18:42.000000 libvirt-python-9.3.0/libvirt-python.spec
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2766 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/libvirt-python.spec.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-qemu-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    14037 2023-03-01 10:15:08.000000 libvirt-python-9.3.0/libvirt-qemu-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.3.0/libvirt-qemu-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16182 2022-07-11 21:25:49.000000 libvirt-python-9.3.0/libvirt-utils.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-utils.h
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/libvirtaio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/requirements-test.txt
+-rw-rw-r--   0 jirka      (500) jirka      (500)       38 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/setup.cfg
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    11863 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/setup.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/tests/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/tests/eventmock.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/tests/test_aio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.3.0/tests/test_api_coverage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_conn.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_domain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_domain_checkpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_domain_snapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_interface.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_network.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_nodedev.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_storage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      114 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tox.ini
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10721 2023-03-01 10:15:08.000000 libvirt-python-9.3.0/typewrappers.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.3.0/typewrappers.h
```

### Comparing `libvirt-python-9.2.0/.github/workflows/lockdown.yml` & `libvirt-python-9.3.0/.github/workflows/lockdown.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/.gitlab-ci.yml` & `libvirt-python-9.3.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     - cd "$SCRATCH_DIR"
     - git clone --depth 1 https://gitlab.com/libvirt/libvirt.git
     - cd libvirt
     - meson build -Ddriver_libvirtd=disabled "--prefix=$VROOT" "--libdir=$LIBDIR"
     - ninja -C build install
     - popd
     - $PYTHON setup.py build
-    - $PYTHON -m pip install .
+    - $PYTHON -m pip ${PIP_INSTALL:-install} .
     - $PYTHON setup.py test
     - $PYTHON setup.py sdist
     - if test -x /usr/bin/rpmbuild && test "$RPM" != "skip" ;
       then
           rpmbuild --clean --nodeps --define "_topdir $PWD/rpmbuild" -ta dist/libvirt-python*tar.gz ;
           mv rpmbuild/RPMS/x86_64/ libvirt-python-rpms ;
       fi
@@ -46,15 +46,15 @@
     - .gitlab_native_build_job_local_env
 
 .native_build_job:
   script:
     - export MAKEFLAGS="-j$(getconf _NPROCESSORS_ONLN)"
     - export CFLAGS="-Werror"
     - $PYTHON setup.py build
-    - $PYTHON -m pip install .
+    - $PYTHON -m pip ${PIP_INSTALL:-install} .
     - $PYTHON setup.py test
     - $PYTHON setup.py sdist
     - if test -x /usr/bin/rpmbuild && test "$RPM" != "skip" ;
       then
           rpmbuild --clean --nodeps --define "_topdir $PWD/rpmbuild" -ta dist/libvirt-python*tar.gz ;
           mv rpmbuild/RPMS/x86_64/ libvirt-python-rpms ;
       fi
```

### Comparing `libvirt-python-9.2.0/.mailmap` & `libvirt-python-9.3.0/.mailmap`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/AUTHORS` & `libvirt-python-9.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/CONTRIBUTING.rst` & `libvirt-python-9.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/COPYING` & `libvirt-python-9.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/COPYING.LESSER` & `libvirt-python-9.3.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ChangeLog` & `libvirt-python-9.3.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,61 @@
+2023-04-26 Daniel P. Berrangé  <berrange@redhat.com>
+    
+    rpm: convert license to SPDX format
+    
+    
+2023-04-19 Jiri Denemark  <jdenemar@redhat.com>
+    
+    Post-release version bump to 9.3.0
+    
+    
+2023-04-19 Daniel P. Berrangé  <berrange@redhat.com>
+    
+    setup: limit pytest to 'tests' subdir
+    The libvirt git repo contains test data that represents the
+    layout of files in sysfs, which has two subdirs that mutually
+    reference each other with symlinks.
+    
+    When pytest does test discovery it will traverse every
+    directory it finds underneath the libvirt-python checkout.
+    
+    Since we checkout libvirt as a sub-dir, pytest traverses
+    everything in libvirt git and gets stuck in an infinite
+    loop following symlinks in the libvirt test data.
+    
+    Telling pytest to only look at the 'tests' subdir avoids
+    this extra traversal.
+    
+    
+    
+2023-04-19 Daniel P. Berrangé  <berrange@redhat.com>
+    
+    ci: pass --break-system-packages on Debian Sid
+    Debian Sid python packages block users from installing packages using
+    pip unless using a venv. A venv has no benefit when we are running in
+    a throwaway container which has no need for software upgrades.
+    
+    
+    
+2023-04-19 Daniel P. Berrangé  <berrange@redhat.com>
+    
+    ci: mark bleeding edge distros as non-gating
+    Fedora Rawhide, Debian Sid and OpenSUSE Tumbleweed are all liable to
+    have sporadic failures due to being bleeding edge distros. Thus they
+    should not gate contributor changes that are otherwise correct.
+    
+    
+    
+2023-04-19 Daniel P. Berrangé  <berrange@redhat.com>
+    
+    ci: regenerated with lcitool manifest
+    This replaces OpenSUSE Leap 15.3 with 15.4
+    
+    
+    
 2023-03-01 Jiri Denemark  <jdenemar@redhat.com>
     
     Post-release version bump to 9.2.0
     
     
 2023-02-13 Michal Privoznik  <mprivozn@redhat.com>
```

### Comparing `libvirt-python-9.2.0/HACKING` & `libvirt-python-9.3.0/HACKING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/MANIFEST` & `libvirt-python-9.3.0/MANIFEST`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/MANIFEST.in` & `libvirt-python-9.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/PKG-INFO` & `libvirt-python-9.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libvirt-python
-Version: 9.2.0
+Version: 9.3.0
 Summary: The libvirt virtualization API python binding
 Home-page: http://www.libvirt.org
 Maintainer: Libvirt Maintainers
 Maintainer-email: libvir-list@redhat.com
 License: LGPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `libvirt-python-9.2.0/README` & `libvirt-python-9.3.0/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/build/libvirt_python.egg-info/SOURCES.txt` & `libvirt-python-9.3.0/build/libvirt_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,26 +46,26 @@
 ci/buildenv/centos-stream-8.sh
 ci/buildenv/centos-stream-9.sh
 ci/buildenv/debian-10.sh
 ci/buildenv/debian-sid.sh
 ci/buildenv/fedora-36.sh
 ci/buildenv/fedora-37.sh
 ci/buildenv/fedora-rawhide.sh
-ci/buildenv/opensuse-leap-153.sh
+ci/buildenv/opensuse-leap-154.sh
 ci/buildenv/opensuse-tumbleweed.sh
 ci/buildenv/ubuntu-2004.sh
 ci/buildenv/ubuntu-2204.sh
 ci/containers/centos-stream-8.Dockerfile
 ci/containers/centos-stream-9.Dockerfile
 ci/containers/debian-10.Dockerfile
 ci/containers/debian-sid.Dockerfile
 ci/containers/fedora-36.Dockerfile
 ci/containers/fedora-37.Dockerfile
 ci/containers/fedora-rawhide.Dockerfile
-ci/containers/opensuse-leap-153.Dockerfile
+ci/containers/opensuse-leap-154.Dockerfile
 ci/containers/opensuse-tumbleweed.Dockerfile
 ci/containers/ubuntu-2004.Dockerfile
 ci/containers/ubuntu-2204.Dockerfile
 ci/gitlab/build-templates.yml
 ci/gitlab/builds.yml
 ci/gitlab/container-templates.yml
 ci/gitlab/containers.yml
```

### Comparing `libvirt-python-9.2.0/ci/buildenv/centos-stream-8.sh` & `libvirt-python-9.3.0/ci/buildenv/centos-stream-8.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/centos-stream-9.sh` & `libvirt-python-9.3.0/ci/buildenv/centos-stream-9.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/debian-10.sh` & `libvirt-python-9.3.0/ci/buildenv/debian-10.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/debian-sid.sh` & `libvirt-python-9.3.0/ci/buildenv/debian-sid.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/fedora-36.sh` & `libvirt-python-9.3.0/ci/buildenv/fedora-36.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/fedora-37.sh` & `libvirt-python-9.3.0/ci/buildenv/fedora-37.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/fedora-rawhide.sh` & `libvirt-python-9.3.0/ci/buildenv/fedora-rawhide.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/opensuse-leap-153.sh` & `libvirt-python-9.3.0/ci/buildenv/opensuse-leap-154.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/opensuse-tumbleweed.sh` & `libvirt-python-9.3.0/ci/buildenv/opensuse-tumbleweed.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/ubuntu-2004.sh` & `libvirt-python-9.3.0/ci/buildenv/ubuntu-2004.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/buildenv/ubuntu-2204.sh` & `libvirt-python-9.3.0/ci/buildenv/ubuntu-2204.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/containers/centos-stream-8.Dockerfile` & `libvirt-python-9.3.0/ci/containers/centos-stream-8.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/containers/centos-stream-9.Dockerfile` & `libvirt-python-9.3.0/ci/containers/centos-stream-9.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/containers/debian-10.Dockerfile` & `libvirt-python-9.3.0/ci/containers/debian-10.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/containers/debian-sid.Dockerfile` & `libvirt-python-9.3.0/ci/containers/debian-sid.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/containers/fedora-36.Dockerfile` & `libvirt-python-9.3.0/ci/containers/fedora-36.Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 FROM registry.fedoraproject.org/fedora:36
 
 RUN dnf install -y nosync && \
-    echo -e '#!/bin/sh\n\
+    printf '#!/bin/sh\n\
 if test -d /usr/lib64\n\
 then\n\
     export LD_PRELOAD=/usr/lib64/nosync/nosync.so\n\
 else\n\
     export LD_PRELOAD=/usr/lib/nosync/nosync.so\n\
 fi\n\
-exec "$@"' > /usr/bin/nosync && \
+exec "$@"\n' > /usr/bin/nosync && \
     chmod +x /usr/bin/nosync && \
     nosync dnf update -y && \
     nosync dnf install -y \
                ca-certificates \
                ccache \
                gcc \
                git \
```

### Comparing `libvirt-python-9.2.0/ci/containers/fedora-37.Dockerfile` & `libvirt-python-9.3.0/ci/containers/fedora-37.Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 FROM registry.fedoraproject.org/fedora:37
 
 RUN dnf install -y nosync && \
-    echo -e '#!/bin/sh\n\
+    printf '#!/bin/sh\n\
 if test -d /usr/lib64\n\
 then\n\
     export LD_PRELOAD=/usr/lib64/nosync/nosync.so\n\
 else\n\
     export LD_PRELOAD=/usr/lib/nosync/nosync.so\n\
 fi\n\
-exec "$@"' > /usr/bin/nosync && \
+exec "$@"\n' > /usr/bin/nosync && \
     chmod +x /usr/bin/nosync && \
     nosync dnf update -y && \
     nosync dnf install -y \
                ca-certificates \
                ccache \
                gcc \
                git \
```

### Comparing `libvirt-python-9.2.0/ci/containers/fedora-rawhide.Dockerfile` & `libvirt-python-9.3.0/ci/containers/fedora-rawhide.Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
 FROM registry.fedoraproject.org/fedora:rawhide
 
 RUN dnf update -y --nogpgcheck fedora-gpg-keys && \
     dnf install -y nosync && \
-    echo -e '#!/bin/sh\n\
+    printf '#!/bin/sh\n\
 if test -d /usr/lib64\n\
 then\n\
     export LD_PRELOAD=/usr/lib64/nosync/nosync.so\n\
 else\n\
     export LD_PRELOAD=/usr/lib/nosync/nosync.so\n\
 fi\n\
-exec "$@"' > /usr/bin/nosync && \
+exec "$@"\n' > /usr/bin/nosync && \
     chmod +x /usr/bin/nosync && \
     nosync dnf distro-sync -y && \
     nosync dnf install -y \
                ca-certificates \
                ccache \
                gcc \
                git \
```

### Comparing `libvirt-python-9.2.0/ci/containers/opensuse-leap-153.Dockerfile` & `libvirt-python-9.3.0/ci/containers/opensuse-tumbleweed.Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM registry.opensuse.org/opensuse/leap:15.3
+FROM registry.opensuse.org/opensuse/tumbleweed:latest
 
-RUN zypper update -y && \
+RUN zypper dist-upgrade -y && \
     zypper install -y \
            ca-certificates \
            ccache \
            gcc \
            git \
            glibc-locale \
            libvirt-devel \
```

### Comparing `libvirt-python-9.2.0/ci/containers/opensuse-tumbleweed.Dockerfile` & `libvirt-python-9.3.0/ci/containers/opensuse-leap-154.Dockerfile`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM registry.opensuse.org/opensuse/tumbleweed:latest
+FROM registry.opensuse.org/opensuse/leap:15.4
 
-RUN zypper dist-upgrade -y && \
+RUN zypper update -y && \
     zypper install -y \
            ca-certificates \
            ccache \
            gcc \
            git \
            glibc-locale \
            libvirt-devel \
```

### Comparing `libvirt-python-9.2.0/ci/containers/ubuntu-2004.Dockerfile` & `libvirt-python-9.3.0/ci/containers/ubuntu-2004.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/containers/ubuntu-2204.Dockerfile` & `libvirt-python-9.3.0/ci/containers/ubuntu-2204.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/gitlab/build-templates.yml` & `libvirt-python-9.3.0/ci/gitlab/build-templates.yml`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,21 @@
     # upstream: pushes to the default branch
     - if: '$CI_PROJECT_NAMESPACE == $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH && $JOB_OPTIONAL'
       when: manual
       allow_failure: true
     - if: '$CI_PROJECT_NAMESPACE == $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH'
       when: on_success
 
+    # forks: pushes to a branch when a pipeline run in upstream env is explicitly requested
+    - if: '$CI_PROJECT_NAMESPACE != $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $RUN_PIPELINE_UPSTREAM_ENV && $JOB_OPTIONAL'
+      when: manual
+      allow_failure: true
+    - if: '$CI_PROJECT_NAMESPACE != $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $RUN_PIPELINE_UPSTREAM_ENV'
+      when: on_success
+
     # upstream: other web/api/scheduled pipelines targeting the default branch
     - if: '$CI_PROJECT_NAMESPACE == $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE =~ /(web|api|schedule)/ && $CI_COMMIT_REF_NAME == $CI_DEFAULT_BRANCH && $JOB_OPTIONAL'
       when: manual
       allow_failure: true
     - if: '$CI_PROJECT_NAMESPACE == $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE =~ /(web|api|schedule)/ && $CI_COMMIT_REF_NAME == $CI_DEFAULT_BRANCH'
       when: on_success
 
@@ -71,14 +78,19 @@
     # upstream: pushes to a non-default branch
     - if: '$CI_PROJECT_NAMESPACE == $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $CI_COMMIT_BRANCH != $CI_DEFAULT_BRANCH && $JOB_OPTIONAL'
       when: manual
       allow_failure: true
     - if: '$CI_PROJECT_NAMESPACE == $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $CI_COMMIT_BRANCH != $CI_DEFAULT_BRANCH'
       when: on_success
 
+    # forks: avoid build in local env when job requests run in upstream containers
+    - if: '$CI_PROJECT_NAMESPACE != $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $RUN_PIPELINE_UPSTREAM_ENV'
+      when: never
+
+    # forks: pushes to branches with pipeline requested
     - if: '$CI_PROJECT_NAMESPACE != $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $RUN_PIPELINE && $JOB_OPTIONAL'
       when: manual
       allow_failure: true
     - if: '$CI_PROJECT_NAMESPACE != $RUN_UPSTREAM_NAMESPACE && $CI_PIPELINE_SOURCE == "push" && $RUN_PIPELINE'
       when: on_success
 
     # upstream: other web/api/scheduled pipelines targeting non-default branches
```

### Comparing `libvirt-python-9.2.0/ci/gitlab/builds.yml` & `libvirt-python-9.3.0/ci/gitlab/builds.yml`

 * *Files 5% similar despite different names*

```diff
@@ -106,25 +106,27 @@
 
 
 x86_64-debian-sid-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
     - job: x86_64-debian-sid-container
       optional: true
-  allow_failure: false
+  allow_failure: true
   variables:
     NAME: debian-sid
+    PIP_INSTALL: install --break-system-packages
 
 x86_64-debian-sid-local-env:
   extends: .native_build_job_local_env
   needs: []
-  allow_failure: false
+  allow_failure: true
   variables:
     IMAGE: docker.io/library/debian:sid-slim
     NAME: debian-sid
+    PIP_INSTALL: install --break-system-packages
 
 
 x86_64-fedora-36-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
     - job: x86_64-fedora-36-container
       optional: true
@@ -176,61 +178,61 @@
 
 
 x86_64-fedora-rawhide-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
     - job: x86_64-fedora-rawhide-container
       optional: true
-  allow_failure: false
+  allow_failure: true
   variables:
     NAME: fedora-rawhide
 
 x86_64-fedora-rawhide-local-env:
   extends: .native_build_job_local_env
   needs: []
-  allow_failure: false
+  allow_failure: true
   variables:
     IMAGE: registry.fedoraproject.org/fedora:rawhide
     NAME: fedora-rawhide
 
 
-x86_64-opensuse-leap-153-prebuilt-env:
+x86_64-opensuse-leap-154-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
-    - job: x86_64-opensuse-leap-153-container
+    - job: x86_64-opensuse-leap-154-container
       optional: true
   allow_failure: false
   variables:
-    NAME: opensuse-leap-153
+    NAME: opensuse-leap-154
     RPM: skip
 
-x86_64-opensuse-leap-153-local-env:
+x86_64-opensuse-leap-154-local-env:
   extends: .native_build_job_local_env
   needs: []
   allow_failure: false
   variables:
-    IMAGE: registry.opensuse.org/opensuse/leap:15.3
-    NAME: opensuse-leap-153
+    IMAGE: registry.opensuse.org/opensuse/leap:15.4
+    NAME: opensuse-leap-154
     RPM: skip
 
 
 x86_64-opensuse-tumbleweed-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
     - job: x86_64-opensuse-tumbleweed-container
       optional: true
-  allow_failure: false
+  allow_failure: true
   variables:
     NAME: opensuse-tumbleweed
     RPM: skip
 
 x86_64-opensuse-tumbleweed-local-env:
   extends: .native_build_job_local_env
   needs: []
-  allow_failure: false
+  allow_failure: true
   variables:
     IMAGE: registry.opensuse.org/opensuse/tumbleweed:latest
     NAME: opensuse-tumbleweed
     RPM: skip
 
 
 x86_64-ubuntu-2004-prebuilt-env:
```

### Comparing `libvirt-python-9.2.0/ci/gitlab/container-templates.yml` & `libvirt-python-9.3.0/ci/gitlab/container-templates.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/ci/gitlab/containers.yml` & `libvirt-python-9.3.0/ci/gitlab/containers.yml`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   allow_failure: false
   variables:
     NAME: debian-10
 
 
 x86_64-debian-sid-container:
   extends: .container_job
-  allow_failure: false
+  allow_failure: true
   variables:
     NAME: debian-sid
 
 
 x86_64-fedora-36-container:
   extends: .container_job
   allow_failure: false
@@ -47,29 +47,29 @@
   allow_failure: false
   variables:
     NAME: fedora-37
 
 
 x86_64-fedora-rawhide-container:
   extends: .container_job
-  allow_failure: false
+  allow_failure: true
   variables:
     NAME: fedora-rawhide
 
 
-x86_64-opensuse-leap-153-container:
+x86_64-opensuse-leap-154-container:
   extends: .container_job
   allow_failure: false
   variables:
-    NAME: opensuse-leap-153
+    NAME: opensuse-leap-154
 
 
 x86_64-opensuse-tumbleweed-container:
   extends: .container_job
-  allow_failure: false
+  allow_failure: true
   variables:
     NAME: opensuse-tumbleweed
 
 
 x86_64-ubuntu-2004-container:
   extends: .container_job
   allow_failure: false
```

### Comparing `libvirt-python-9.2.0/ci/gitlab.yml` & `libvirt-python-9.3.0/ci/gitlab.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 #
 #  - RUN_PIPELINE - force creation of a CI pipeline when
 #    pushing to a branch in a forked repository. Official
 #    CI pipelines are triggered when merge requests are
 #    created/updated. Setting this variable to a non-empty
 #    value allows CI testing prior to opening a merge request.
 #
+#  - RUN_PIPELINE_UPSTREAM_ENV - same semantics as RUN_PIPELINE,
+#    but uses the CI environment (containers) from the upstream project
+#    rather than creating and updating a throwaway environment
+#    Should not be used if the pushed branch includes CI container
+#    changes.
+#
 #  - RUN_CONTAINER_BUILDS - CI pipelines in upstream only
 #    publish containers if CI file changes are detected.
 #    Setting this variable to a non-empty value will force
 #    re-publishing, even when no file changes are detected.
 #    Typically to use from a scheduled job once a month.
 #
 #  - RUN_UPSTREAM_NAMESPACE - the upstream namespace is
@@ -40,14 +46,15 @@
 #
 # Pipeline variables can also be set in the repository
 # pipeline config globally, or set against scheduled pipelines
 
 
 variables:
   RUN_UPSTREAM_NAMESPACE: libvirt
+  FF_SCRIPT_SECTIONS: 1
 
 
 workflow:
   rules:
     # upstream+forks: Avoid duplicate pipelines on pushes, if a MR is open
     - if: '$CI_PIPELINE_SOURCE == "push" && $CI_OPEN_MERGE_REQUESTS'
       when: never
```

### Comparing `libvirt-python-9.2.0/ci/manifest.yml` & `libvirt-python-9.3.0/ci/manifest.yml`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,20 @@
         artifacts:
           expire_in: 1 hour
           paths:
             - libvirt-python-rpms
 
   debian-10: x86_64
 
-  debian-sid: x86_64
+  debian-sid:
+    jobs:
+      - arch: x86_64
+        allow-failure: true
+        variables:
+          PIP_INSTALL: install --break-system-packages
 
   fedora-36:
     jobs:
       - arch: x86_64
         artifacts:
           expire_in: 1 hour
           paths:
@@ -54,24 +59,28 @@
     jobs:
       - arch: x86_64
         artifacts:
           expire_in: 1 hour
           paths:
             - libvirt-python-rpms
 
-  fedora-rawhide: x86_64
+  fedora-rawhide:
+    jobs:
+      - arch: x86_64
+        allow-failure: true
 
-  opensuse-leap-153:
+  opensuse-leap-154:
     jobs:
       - arch: x86_64
         variables:
           RPM: skip
 
   opensuse-tumbleweed:
     jobs:
       - arch: x86_64
+        allow-failure: true
         variables:
           RPM: skip
 
   ubuntu-2004: x86_64
 
   ubuntu-2204: x86_64
```

### Comparing `libvirt-python-9.2.0/examples/README` & `libvirt-python-9.3.0/examples/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/consolecallback.py` & `libvirt-python-9.3.0/examples/consolecallback.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/dhcpleases.py` & `libvirt-python-9.3.0/examples/dhcpleases.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/dominfo.py` & `libvirt-python-9.3.0/examples/dominfo.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/domipaddrs.py` & `libvirt-python-9.3.0/examples/domipaddrs.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/domrestore.py` & `libvirt-python-9.3.0/examples/domrestore.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/domsave.py` & `libvirt-python-9.3.0/examples/domsave.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/domstart.py` & `libvirt-python-9.3.0/examples/domstart.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/esxlist.py` & `libvirt-python-9.3.0/examples/esxlist.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/event-test.py` & `libvirt-python-9.3.0/examples/event-test.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/guest-vcpus/guest-vcpu-daemon.py` & `libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu-daemon.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/guest-vcpus/guest-vcpu.py` & `libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/nodestats.py` & `libvirt-python-9.3.0/examples/nodestats.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/sparsestream.py` & `libvirt-python-9.3.0/examples/sparsestream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/examples/topology.py` & `libvirt-python-9.3.0/examples/topology.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/generator.py` & `libvirt-python-9.3.0/generator.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-lxc-override-api.xml` & `libvirt-python-9.3.0/libvirt-lxc-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-lxc-override.c` & `libvirt-python-9.3.0/libvirt-lxc-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override-api.xml` & `libvirt-python-9.3.0/libvirt-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override-virConnect.py` & `libvirt-python-9.3.0/libvirt-override-virConnect.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override-virDomain.py` & `libvirt-python-9.3.0/libvirt-override-virDomain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override-virDomainCheckpoint.py` & `libvirt-python-9.3.0/libvirt-override-virDomainCheckpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override-virDomainSnapshot.py` & `libvirt-python-9.3.0/libvirt-override-virDomainSnapshot.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override-virStream.py` & `libvirt-python-9.3.0/libvirt-override-virStream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override.c` & `libvirt-python-9.3.0/libvirt-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-override.py` & `libvirt-python-9.3.0/libvirt-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-python.spec` & `libvirt-python-9.3.0/libvirt-python.spec`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     %define supported_platform 1
 %else
     %define supported_platform 0
 %endif
 
 Summary: The libvirt virtualization API python3 binding
 Name: libvirt-python
-Version: 9.2.0
+Version: 9.3.0
 Release: 1%{?dist}
 Source0: https://libvirt.org/sources/python/%{name}-%{version}.tar.gz
 Url: https://libvirt.org
-License: LGPLv2+
+License: LGPL-2.1-or-later
 BuildRequires: libvirt-devel == %{version}
 BuildRequires: python3-devel
 BuildRequires: python3-pytest
 BuildRequires: python3-lxml
 BuildRequires: python3-setuptools
 BuildRequires: gcc
```

### Comparing `libvirt-python-9.2.0/libvirt-python.spec.in` & `libvirt-python-9.3.0/libvirt-python.spec.in`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 Summary: The libvirt virtualization API python3 binding
 Name: libvirt-python
 Version: @PY_VERSION@
 Release: 1%{?dist}
 Source0: https://libvirt.org/sources/python/%{name}-%{version}.tar.gz
 Url: https://libvirt.org
-License: LGPLv2+
+License: LGPL-2.1-or-later
 BuildRequires: libvirt-devel == %{version}
 BuildRequires: python3-devel
 BuildRequires: python3-pytest
 BuildRequires: python3-lxml
 BuildRequires: python3-setuptools
 BuildRequires: gcc
```

### Comparing `libvirt-python-9.2.0/libvirt-qemu-override-api.xml` & `libvirt-python-9.3.0/libvirt-qemu-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-qemu-override.c` & `libvirt-python-9.3.0/libvirt-qemu-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-qemu-override.py` & `libvirt-python-9.3.0/libvirt-qemu-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-utils.c` & `libvirt-python-9.3.0/libvirt-utils.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirt-utils.h` & `libvirt-python-9.3.0/libvirt-utils.h`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/libvirtaio.py` & `libvirt-python-9.3.0/libvirtaio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/setup.py` & `libvirt-python-9.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 
         if "PYTHONPATH" in os.environ:
             os.environ["PYTHONPATH"] = self.build_platlib + ":" + os.environ["PYTHONPATH"]
         else:
             os.environ["PYTHONPATH"] = self.build_platlib
 
         pytest = self.find_pytest_path()
-        subprocess.check_call([pytest])
+        subprocess.check_call([pytest, "tests"])
 
 class my_clean(Command):
     user_options = [
         ('all', None, 'unused, compatibility with distutils')
     ]
 
     def initialize_options(self):
@@ -331,15 +331,15 @@
 ##################
 # Invoke setup() #
 ##################
 
 _c_modules, _py_modules = get_module_lists()
 
 setup(name = 'libvirt-python',
-      version = '9.2.0',
+      version = '9.3.0',
       url = 'http://www.libvirt.org',
       maintainer = 'Libvirt Maintainers',
       maintainer_email = 'libvir-list@redhat.com',
       description = 'The libvirt virtualization API python binding',
       long_description =
         '''The libvirt-python package provides a module that permits applications
 written in the Python 3.x programming language to call the interface
```

### Comparing `libvirt-python-9.2.0/tests/eventmock.py` & `libvirt-python-9.3.0/tests/eventmock.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/tests/test_aio.py` & `libvirt-python-9.3.0/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/tests/test_api_coverage.py` & `libvirt-python-9.3.0/tests/test_api_coverage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/tests/test_conn.py` & `libvirt-python-9.3.0/tests/test_conn.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/tests/test_domain.py` & `libvirt-python-9.3.0/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/tests/test_domain_checkpoint.py` & `libvirt-python-9.3.0/tests/test_domain_checkpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/tests/test_storage.py` & `libvirt-python-9.3.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/typewrappers.c` & `libvirt-python-9.3.0/typewrappers.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.2.0/typewrappers.h` & `libvirt-python-9.3.0/typewrappers.h`

 * *Files identical despite different names*

