# Comparing `tmp/acc_provision-5.2.3.6rc4.tar.gz` & `tmp/acc_provision-5.2.3.6rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acc_provision-5.2.3.6rc4.tar", last modified: Wed Mar 29 20:28:28 2023, max compression
+gzip compressed data, was "dist/acc_provision-5.2.3.6rc5.tar", last modified: Mon Apr  3 17:09:17 2023, max compression
```

## Comparing `acc_provision-5.2.3.6rc4.tar` & `acc_provision-5.2.3.6rc5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     1358 2023-03-29 20:27:48.000000 acc_provision-5.2.3.6rc4/setup.py
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/rpm/
--rwxrwxr-x   0 noiro     (1000) noiro     (1000)      532 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/rpm/build-rpm.sh
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     1589 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/rpm/acc-provision.spec.in
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     3336 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/acc_retrieve_cert.py
--rwxrwxr-x   0 noiro     (1000) noiro     (1000)    11287 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/kafka_cert.py
--rwxrwxr-x   0 noiro     (1000) noiro     (1000)    82006 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/acc_provision.py
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     1944 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/fake_apic.py
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      390 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-operators-configmap.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     5936 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-operators.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     6399 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/provision-config.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)    12150 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/acc-provision-configmap.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     6048 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster-1-3-17.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     5806 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster-1-3-13.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     1855 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/calicoctl.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      231 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-operators-cr.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2159 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/custom-resources-aci-calico.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      750 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/calico-bgp-config.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)   319083 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/tigera-operator.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/__init__.py
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     3038 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/99-worker-kubelet-node-port.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     1238 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-operators-crd.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2247 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aks-provision-config.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)    93040 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-containers.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     4208 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     3038 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/calico-provision-config.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      104 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/calico-node.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      387 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/calico-bgp-peer.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2304 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/99-master-kubelet-node-ip.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      496 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/apic.json
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      297 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/cluster-network-03-config.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     6921 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster-1-3-18.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2162 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/99-worker-kubelet-node-ip.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     5820 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/acc-provision-crd.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2789 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/templates/overlay-provision-config.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/__init__.py
--rwxrwxr-x   0 noiro     (1000) noiro     (1000)    28944 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/cloud_provision.py
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2176 2023-03-29 20:27:48.000000 acc_provision-5.2.3.6rc4/acc_provision/versions.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       92 2023-03-29 20:27:48.000000 acc_provision-5.2.3.6rc4/acc_provision/RELEASE-VERSION
--rw-rw-r--   0 noiro     (1000) noiro     (1000)   521709 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/apic_provision.py
--rw-rw-r--   0 noiro     (1000) noiro     (1000)   123497 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/flavors.yaml
--rw-rw-r--   0 noiro     (1000) noiro     (1000)    35341 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/acc_provision/test_main.py
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/debian/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      306 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/changelog.in
--rwxrwxr-x   0 noiro     (1000) noiro     (1000)      533 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/rules
--rw-r--r--   0 noiro     (1000) noiro     (1000)      384 2023-03-29 20:28:02.000000 acc_provision-5.2.3.6rc4/debian/acc-provision.prerm.debhelper
--rw-r--r--   0 noiro     (1000) noiro     (1000)      187 2023-03-29 20:28:04.000000 acc_provision-5.2.3.6rc4/debian/acc-provision.substvars
--rw-r--r--   0 noiro     (1000) noiro     (1000)      112 2023-03-29 20:28:18.000000 acc_provision-5.2.3.6rc4/debian/files
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      781 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/control
--rw-rw-r--   0 noiro     (1000) noiro     (1000)        2 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/compat
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       15 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/dirs
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      900 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/copyright
--rw-r--r--   0 noiro     (1000) noiro     (1000)      383 2023-03-29 20:28:17.000000 acc_provision-5.2.3.6rc4/debian/acc-provision.debhelper.log
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       24 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/install
--rwxrwxr-x   0 noiro     (1000) noiro     (1000)      733 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/build-deb.sh
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       62 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/.gitignore
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/debian/source/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       13 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/debian/source/format
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      298 2023-03-29 20:27:54.000000 acc_provision-5.2.3.6rc4/debian/changelog
--rw-r--r--   0 noiro     (1000) noiro     (1000)      148 2023-03-29 20:28:02.000000 acc_provision-5.2.3.6rc4/debian/acc-provision.postinst.debhelper
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      241 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/MANIFEST.in
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      846 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/README.md
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      392 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/PKG-INFO
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/gitversion/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     1648 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/gitversion/gitversion.py
--rw-rw-r--   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:27:05.000000 acc_provision-5.2.3.6rc4/gitversion/__init__.py
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/
--rw-rw-r--   0 noiro     (1000) noiro     (1000)     2423 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/SOURCES.txt
--rw-rw-r--   0 noiro     (1000) noiro     (1000)        1 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/dependency_links.txt
--rw-rw-r--   0 noiro     (1000) noiro     (1000)        1 2023-03-29 20:27:48.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/not-zip-safe
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       25 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/top_level.txt
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      392 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/PKG-INFO
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       50 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/requires.txt
--rw-rw-r--   0 noiro     (1000) noiro     (1000)      125 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/acc_provision.egg-info/entry_points.txt
--rw-rw-r--   0 noiro     (1000) noiro     (1000)       38 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/setup.cfg
-drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-03-29 20:28:28.000000 acc_provision-5.2.3.6rc4/bin/
--rwxrwxr-x   0 noiro     (1000) noiro     (1000) 34021376 2023-03-29 20:27:47.000000 acc_provision-5.2.3.6rc4/bin/acikubectl
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     1358 2023-04-03 17:08:35.000000 acc_provision-5.2.3.6rc5/setup.py
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/rpm/
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000)      532 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/rpm/build-rpm.sh
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     1589 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/rpm/acc-provision.spec.in
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     3336 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/acc_retrieve_cert.py
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000)    11287 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/kafka_cert.py
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000)    82006 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/acc_provision.py
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     1944 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/fake_apic.py
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      390 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-operators-configmap.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     5936 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-operators.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     6399 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/provision-config.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)    12150 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/acc-provision-configmap.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     6048 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster-1-3-17.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     5806 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster-1-3-13.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     1855 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/calicoctl.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      231 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-operators-cr.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2159 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/custom-resources-aci-calico.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      750 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/calico-bgp-config.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)   319083 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/tigera-operator.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/__init__.py
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     3038 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/99-worker-kubelet-node-port.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     1238 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-operators-crd.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2247 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aks-provision-config.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)    93257 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-containers.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     4208 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     3038 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/calico-provision-config.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      104 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/calico-node.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      387 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/calico-bgp-peer.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2304 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/99-master-kubelet-node-ip.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      496 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/apic.json
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      297 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/cluster-network-03-config.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     6921 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster-1-3-18.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2162 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/99-worker-kubelet-node-ip.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     5820 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/acc-provision-crd.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2789 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/templates/overlay-provision-config.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/__init__.py
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000)    28944 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/cloud_provision.py
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2176 2023-04-03 17:08:35.000000 acc_provision-5.2.3.6rc5/acc_provision/versions.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       92 2023-04-03 17:08:36.000000 acc_provision-5.2.3.6rc5/acc_provision/RELEASE-VERSION
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)   521709 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/apic_provision.py
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)   123497 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/flavors.yaml
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)    35341 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/acc_provision/test_main.py
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/debian/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      306 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/changelog.in
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000)      533 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/rules
+-rw-r--r--   0 noiro     (1000) noiro     (1000)      384 2023-04-03 17:08:50.000000 acc_provision-5.2.3.6rc5/debian/acc-provision.prerm.debhelper
+-rw-r--r--   0 noiro     (1000) noiro     (1000)      187 2023-04-03 17:08:52.000000 acc_provision-5.2.3.6rc5/debian/acc-provision.substvars
+-rw-r--r--   0 noiro     (1000) noiro     (1000)      112 2023-04-03 17:09:06.000000 acc_provision-5.2.3.6rc5/debian/files
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      781 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/control
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)        2 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/compat
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       15 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/dirs
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      900 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/copyright
+-rw-r--r--   0 noiro     (1000) noiro     (1000)      383 2023-04-03 17:09:06.000000 acc_provision-5.2.3.6rc5/debian/acc-provision.debhelper.log
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       24 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/install
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000)      733 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/build-deb.sh
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       62 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/.gitignore
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/debian/source/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       13 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/debian/source/format
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      298 2023-04-03 17:08:42.000000 acc_provision-5.2.3.6rc5/debian/changelog
+-rw-r--r--   0 noiro     (1000) noiro     (1000)      148 2023-04-03 17:08:50.000000 acc_provision-5.2.3.6rc5/debian/acc-provision.postinst.debhelper
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      241 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/MANIFEST.in
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      846 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/README.md
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      392 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/PKG-INFO
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/gitversion/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     1648 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/gitversion/gitversion.py
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:07:51.000000 acc_provision-5.2.3.6rc5/gitversion/__init__.py
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)     2423 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/SOURCES.txt
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)        1 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/dependency_links.txt
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)        1 2023-04-03 17:08:36.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/not-zip-safe
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       25 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/top_level.txt
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      392 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/PKG-INFO
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       50 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/requires.txt
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)      125 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/acc_provision.egg-info/entry_points.txt
+-rw-rw-r--   0 noiro     (1000) noiro     (1000)       38 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/setup.cfg
+drwxrwxr-x   0 noiro     (1000) noiro     (1000)        0 2023-04-03 17:09:17.000000 acc_provision-5.2.3.6rc5/bin/
+-rwxrwxr-x   0 noiro     (1000) noiro     (1000) 34021376 2023-04-03 17:08:35.000000 acc_provision-5.2.3.6rc5/bin/acikubectl
```

### Comparing `acc_provision-5.2.3.6rc4/setup.py` & `acc_provision-5.2.3.6rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         except SyntaxError:
             return 'latin-1', []
 
     tokenize.detect_encoding = detect_encoding
 
 setup(
     name='acc_provision',
-    version='5.2.3.6.rc4',
+    version='5.2.3.6.rc5',
     description='Tool to provision ACI for ACI Containers Controller  Build info: ' + get_git_version(),
     author="Cisco Systems, Inc.",
     author_email="apicapi@noironetworks.com",
     url='http://github.com/noironetworks/acc-provision/',
     license="http://www.apache.org/licenses/LICENSE-2.0",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `acc_provision-5.2.3.6rc4/rpm/build-rpm.sh` & `acc_provision-5.2.3.6rc5/rpm/build-rpm.sh`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/rpm/acc-provision.spec.in` & `acc_provision-5.2.3.6rc5/rpm/acc-provision.spec.in`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/acc_retrieve_cert.py` & `acc_provision-5.2.3.6rc5/acc_provision/acc_retrieve_cert.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/kafka_cert.py` & `acc_provision-5.2.3.6rc5/acc_provision/kafka_cert.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/acc_provision.py` & `acc_provision-5.2.3.6rc5/acc_provision/acc_provision.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/fake_apic.py` & `acc_provision-5.2.3.6rc5/acc_provision/fake_apic.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-operators.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-operators.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/provision-config.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/provision-config.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/acc-provision-configmap.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/acc-provision-configmap.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster-1-3-17.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster-1-3-17.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster-1-3-13.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster-1-3-13.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/calicoctl.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/calicoctl.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/custom-resources-aci-calico.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/custom-resources-aci-calico.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/calico-bgp-config.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/calico-bgp-config.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/tigera-operator.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/tigera-operator.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/99-worker-kubelet-node-port.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/99-worker-kubelet-node-port.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-operators-crd.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-operators-crd.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aks-provision-config.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aks-provision-config.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-containers.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-containers.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1540,14 +1540,17 @@
             "asyncjson": { "enabled" : {{ config.kube_config.opflex_agent_opflex_asyncjson_enabled|json }} }
           {% if not config.aci_config.client_ssl %}
             ,"ssl": { "mode": "disabled" }
           {% endif %}
           {% if config.kube_config.run_gbp_container %}
             ,"statistics" : { "mode" : "off" }
           {% endif %}
+          {% if config.kube_config.opflex_agent_policy_retry_delay_timer %}
+            ,"timers" : { "policy-retry-delay" : {{ config.kube_config.opflex_agent_policy_retry_delay_timer|json }} }
+          {% endif %}
         },
         "ovs": {
             "asyncjson": { "enabled" : {{ config.kube_config.opflex_agent_ovs_asyncjson_enabled|json }} }
         },
         "prometheus": {
             "enabled": "false"
         }
```

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/calico-provision-config.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/calico-provision-config.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/99-master-kubelet-node-ip.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/99-master-kubelet-node-ip.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/aci-network-provider-cluster-1-3-18.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/aci-network-provider-cluster-1-3-18.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/99-worker-kubelet-node-ip.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/99-worker-kubelet-node-ip.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/acc-provision-crd.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/acc-provision-crd.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/templates/overlay-provision-config.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/templates/overlay-provision-config.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/cloud_provision.py` & `acc_provision-5.2.3.6rc5/acc_provision/cloud_provision.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/versions.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/versions.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     aci_containers_operator_version: 5.1.1.0.1ae238a
     cnideploy_version: 5.1.1.0.1ae238a
     openvswitch_version: 5.1.1.0.1ae238a
     opflex_agent_version: 5.1.1.0.1ae238a
     opflex_server_version: 5.1.1.0.1ae238a
     gbp_version: 5.1.1.0.1ae238a
   5.2:
-    acc_provision_operator_version: 5.2.3.6.1d150da.032823.280
-    aci_containers_controller_version: 5.2.3.6.1d150da.032823.280
-    aci_containers_host_version: 5.2.3.6.1d150da.032823.280
-    aci_containers_operator_version: 5.2.3.6.1d150da.032823.280
-    cnideploy_version: 5.2.3.6.1d150da.032823.280
-    openvswitch_version: 5.2.3.6.1d150da.032823.280
-    opflex_agent_version: 5.2.3.6.1d150da.032823.265
-    opflex_server_version: 5.2.3.6.1d150da.032823.265
-    gbp_version: 5.2.3.6.1d150da.032823.280
+    acc_provision_operator_version: 5.2.3.6.1d150da.040223.285
+    aci_containers_controller_version: 5.2.3.6.1d150da.040223.285
+    aci_containers_host_version: 5.2.3.6.1d150da.040223.285
+    aci_containers_operator_version: 5.2.3.6.1d150da.040223.285
+    cnideploy_version: 5.2.3.6.1d150da.040223.285
+    openvswitch_version: 5.2.3.6.1d150da.040223.285
+    opflex_agent_version: 5.2.3.6.1d150da.040223.270
+    opflex_server_version: 5.2.3.6.1d150da.040223.270
+    gbp_version: 5.2.3.6.1d150da.040223.285
```

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/apic_provision.py` & `acc_provision-5.2.3.6rc5/acc_provision/apic_provision.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/flavors.yaml` & `acc_provision-5.2.3.6rc5/acc_provision/flavors.yaml`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision/test_main.py` & `acc_provision-5.2.3.6rc5/acc_provision/test_main.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/debian/rules` & `acc_provision-5.2.3.6rc5/debian/rules`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/debian/control` & `acc_provision-5.2.3.6rc5/debian/control`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/debian/copyright` & `acc_provision-5.2.3.6rc5/debian/copyright`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/debian/build-deb.sh` & `acc_provision-5.2.3.6rc5/debian/build-deb.sh`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/README.md` & `acc_provision-5.2.3.6rc5/README.md`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/gitversion/gitversion.py` & `acc_provision-5.2.3.6rc5/gitversion/gitversion.py`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/acc_provision.egg-info/SOURCES.txt` & `acc_provision-5.2.3.6rc5/acc_provision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acc_provision-5.2.3.6rc4/bin/acikubectl` & `acc_provision-5.2.3.6rc5/bin/acikubectl`

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.go.buildid
   Owner                Data size 	Description
-  Go                   0x00000053	GO BUILDID	   description data: 70 71 4a 42 31 39 36 72 58 74 47 73 73 56 57 46 48 6c 65 34 2f 57 4e 6b 39 55 65 34 68 36 67 4a 45 72 58 44 76 4c 4a 76 49 2f 50 4e 4e 42 42 37 72 6c 73 65 5f 45 69 4e 79 5a 44 70 54 4e 2f 6a 57 6c 65 73 2d 77 4e 47 35 53 59 37 50 53 76 4a 38 38 4f 
+  Go                   0x00000053	GO BUILDID	   description data: 6d 6b 74 36 73 45 4b 42 5a 32 65 2d 31 61 53 4a 61 74 6e 63 2f 57 4e 6b 39 55 65 34 68 36 67 4a 45 72 58 44 76 4c 4a 76 49 2f 50 4e 4e 42 42 37 72 6c 73 65 5f 45 69 4e 79 5a 44 70 54 4e 2f 6a 57 6c 65 73 2d 77 4e 47 35 53 59 37 50 53 76 4a 38 38 4f
```

#### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-pqJB196rXtGssVWFHle4/WNk9Ue4h6gJErXDvLJvI/PNNBB7rlse_EiNyZDpTN/jWles-wNG5SY7PSvJ88O
+mkt6sEKBZ2e-1aSJatnc/WNk9Ue4h6gJErXDvLJvI/PNNBB7rlse_EiNyZDpTN/jWles-wNG5SY7PSvJ88O
 UUUUUUUUH!
 33333333H!
 t*H9HPt$
 debugCal
 debugCal
 debugCalH9
 debugCalH9
```

