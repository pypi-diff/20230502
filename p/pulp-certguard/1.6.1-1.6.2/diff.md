# Comparing `tmp/pulp-certguard-1.6.1.tar.gz` & `tmp/pulp-certguard-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-certguard-1.6.1.tar", last modified: Thu Mar 23 13:32:42 2023, max compression
+gzip compressed data, was "pulp-certguard-1.6.2.tar", last modified: Tue May  2 19:25:14 2023, max compression
```

## Comparing `pulp-certguard-1.6.1.tar` & `pulp-certguard-1.6.2.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.736586 pulp-certguard-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-03-23 13:32:40.000000 pulp-certguard-1.6.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-23 13:32:42.736586 pulp-certguard-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.720586 pulp-certguard-1.6.1/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.724586 pulp-certguard-1.6.1/contrib/yum/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/contrib/yum/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/contrib/yum/README
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/contrib/yum/certguard.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/contrib/yum/certguard.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard/app/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-23 13:32:41.000000 pulp-certguard-1.6.1/pulp_certguard/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/test_rhsm_certguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/test_x509_certguard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.724586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.732586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.736586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/genall.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/genca.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/genclient.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.736586 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.736586 pulp-certguard-1.6.1/pulp_certguard/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pulp_certguard/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:32:42.728586 pulp-certguard-1.6.1/pulp_certguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-23 13:32:42.000000 pulp-certguard-1.6.1/pulp_certguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-03-23 13:32:42.000000 pulp-certguard-1.6.1/pulp_certguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 13:32:42.000000 pulp-certguard-1.6.1/pulp_certguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-23 13:32:42.000000 pulp-certguard-1.6.1/pulp_certguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 13:32:42.000000 pulp-certguard-1.6.1/pulp_certguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 13:32:42.000000 pulp-certguard-1.6.1/pulp_certguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 13:32:42.736586 pulp-certguard-1.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-03-23 13:32:41.000000 pulp-certguard-1.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 13:32:29.000000 pulp-certguard-1.6.1/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.638341 pulp-certguard-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-05-02 19:25:11.000000 pulp-certguard-1.6.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/ci_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.626341 pulp-certguard-1.6.2/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.626341 pulp-certguard-1.6.2/contrib/yum/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/contrib/yum/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/contrib/yum/README
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/contrib/yum/certguard.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/contrib/yum/certguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-02 19:25:13.000000 pulp-certguard-1.6.2/pulp_certguard/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/test_rhsm_certguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/test_x509_certguard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.626341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/genall.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/genca.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/genclient.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.634341 pulp-certguard-1.6.2/pulp_certguard/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pulp_certguard/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:25:14.630341 pulp-certguard-1.6.2/pulp_certguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-02 19:25:14.000000 pulp-certguard-1.6.2/pulp_certguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-02 19:25:14.000000 pulp-certguard-1.6.2/pulp_certguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:25:14.000000 pulp-certguard-1.6.2/pulp_certguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 19:25:14.000000 pulp-certguard-1.6.2/pulp_certguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:25:14.000000 pulp-certguard-1.6.2/pulp_certguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 19:25:14.000000 pulp-certguard-1.6.2/pulp_certguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:25:14.638341 pulp-certguard-1.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-05-02 19:25:13.000000 pulp-certguard-1.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 19:24:57.000000 pulp-certguard-1.6.2/unittest_requirements.txt
```

### Comparing `pulp-certguard-1.6.1/CHANGES.rst` & `pulp-certguard-1.6.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,23 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.6.2 (2023-05-02)
+==================
+
+No significant changes.
+
+
+----
+
+
 1.6.1 (2023-03-23)
 ==================
 
 No significant changes.
 
 
 ----
```

### Comparing `pulp-certguard-1.6.1/COMMITMENT` & `pulp-certguard-1.6.2/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/COPYRIGHT` & `pulp-certguard-1.6.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/LICENSE` & `pulp-certguard-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/PKG-INFO` & `pulp-certguard-1.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-certguard
-Version: 1.6.1
+Version: 1.6.2
 Summary: Certguard plugin for the Pulp Project
 Home-page: https://docs.pulpproject.org/pulp_certguard/
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: pulp-certguard
         ==============
```

### Comparing `pulp-certguard-1.6.1/README.rst` & `pulp-certguard-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/contrib/yum/certguard.py` & `pulp-certguard-1.6.2/contrib/yum/certguard.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/app/migrations/0001_initial.py` & `pulp-certguard-1.6.2/pulp_certguard/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/app/models.py` & `pulp-certguard-1.6.2/pulp_certguard/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/app/serializers.py` & `pulp-certguard-1.6.2/pulp_certguard/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/app/utils.py` & `pulp-certguard-1.6.2/pulp_certguard/app/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/app/viewsets.py` & `pulp-certguard-1.6.2/pulp_certguard/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/__init__.py` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/base.py` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/base.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/test_rhsm_certguard.py` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/test_rhsm_certguard.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/api/test_x509_certguard.py` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/api/test_x509_certguard.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.crt`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/katello-default-ca.key`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/trusted_but_expired.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/uber.cert`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/untrusted_cert.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/1514454871848760713.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v1/159442575569388840.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/4260035510644027985.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172-key.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/rhsm/v3/5527980418107729172.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/certificates/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/genca.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/thirdparty_ca/keys/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/client.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/server.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/un_urlencoded_cert.txt`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/certificates/untrusted_client.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/genca.sh` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/genca.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/genclient.sh` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/genclient.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/gensrv.sh`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/ca.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/client.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/artifacts/x509/keys/server.pem`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/constants.py` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard/tests/functional/utils.py` & `pulp-certguard-1.6.2/pulp_certguard/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/pulp_certguard.egg-info/PKG-INFO` & `pulp-certguard-1.6.2/pulp_certguard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-certguard
-Version: 1.6.1
+Version: 1.6.2
 Summary: Certguard plugin for the Pulp Project
 Home-page: https://docs.pulpproject.org/pulp_certguard/
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: pulp-certguard
         ==============
```

### Comparing `pulp-certguard-1.6.1/pulp_certguard.egg-info/SOURCES.txt` & `pulp-certguard-1.6.2/pulp_certguard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGES.rst
 COMMITMENT
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
+ci_requirements.txt
 functest_requirements.txt
 pyproject.toml
 requirements.txt
 setup.py
 test_requirements.txt
 unittest_requirements.txt
 contrib/yum/Makefile
```

### Comparing `pulp-certguard-1.6.1/pyproject.toml` & `pulp-certguard-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-certguard-1.6.1/setup.py` & `pulp-certguard-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="pulp-certguard",
-    version="1.6.1",
+    version="1.6.2",
     description="Certguard plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-list@redhat.com",
     url="https://docs.pulpproject.org/pulp_certguard/",
     python_requires=">=3.8",
```

