# Comparing `tmp/kapitan-0.31.1rc3.tar.gz` & `tmp/kapitan-0.32.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapitan-0.31.1rc3.tar", max compression
+gzip compressed data, was "kapitan-0.32.0rc0.tar", max compression
```

## Comparing `kapitan-0.31.1rc3.tar` & `kapitan-0.32.0rc0.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0        0        0        0 2023-03-02 12:58:11.069229 kapitan-0.31.1rc3/LICENSES/
--rw-r--r--   0        0        0     2443 2023-03-02 12:58:11.069229 kapitan-0.31.1rc3/README.md
--rwxr-xr-x   0        0        0     1088 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/__init__.py
--rw-r--r--   0        0        0      223 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/__main__.py
--rw-r--r--   0        0        0     1889 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/cached.py
--rw-r--r--   0        0        0    21712 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/cli.py
--rw-r--r--   0        0        0      719 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/defaults.py
--rw-r--r--   0        0        0      125 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/dependency_manager/__init__.py
--rw-r--r--   0        0        0    11661 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/dependency_manager/base.py
--rw-r--r--   0        0        0     1411 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/errors.py
--rw-r--r--   0        0        0      951 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/helm_cli.py
--rw-r--r--   0        0        0     1423 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/initialiser.py
--rw-r--r--   0        0        0      125 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/__init__.py
--rw-r--r--   0        0        0     7387 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/base.py
--rw-r--r--   0        0        0     1904 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/copy.py
--rw-r--r--   0        0        0     3324 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/external.py
--rw-r--r--   0        0        0     9501 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/helm.py
--rw-r--r--   0        0        0     2705 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/jinja2.py
--rw-r--r--   0        0        0     6327 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/jinja2_filters.py
--rw-r--r--   0        0        0     6065 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/jsonnet.py
--rw-r--r--   0        0        0     7938 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/kadet.py
--rw-r--r--   0        0        0     1137 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/remove.py
--rw-r--r--   0        0        0      163 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/components/my_component/my_component.jsonnet
--rw-r--r--   0        0        0      267 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/components/other_component/__init__.py
--rw-r--r--   0        0        0       62 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/inventory/classes/common.yml
--rw-r--r--   0        0        0      629 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/inventory/classes/my_component.yml
--rw-r--r--   0        0        0       75 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/inventory/targets/my_target.yml
--rw-r--r--   0        0        0      129 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/templates/docs/my_readme.md
--rw-r--r--   0        0        0      145 2023-03-02 12:58:11.093229 kapitan-0.31.1rc3/kapitan/inputs/templates/templates/scripts/my_script.sh
--rw-r--r--   0        0        0     1008 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/lib/kapitan.libjsonnet
--rw-r--r--   0        0        0     8444 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/lint.py
--rw-r--r--   0        0        0       43 2023-03-02 12:58:11.533235 kapitan-0.31.1rc3/kapitan/reclass/.git
--rw-r--r--   0        0        0       97 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/.gitignore
--rwxr-xr-x   0        0        0      526 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/.kitchen-verify.sh
--rw-r--r--   0        0        0      868 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/.kitchen.yml
--rw-r--r--   0        0        0       31 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/.pylintrc
--rw-r--r--   0        0        0     2522 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/.travis.yml
--rw-r--r--   0        0        0     9350 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/LICENSE
--rw-r--r--   0        0        0      385 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/MANIFEST.in
--rw-r--r--   0        0        0     1366 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/Makefile
--rw-r--r--   0        0        0      282 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/Pipfile
--rw-r--r--   0        0        0    17685 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/README-extensions.rst
--rw-r--r--   0        0        0     1260 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/README.rst
--rw-r--r--   0        0        0        7 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/.gitignore
--rw-r--r--   0        0        0     5580 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/Makefile
--rw-r--r--   0        0        0     8228 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/ansible.rst
--rw-r--r--   0        0        0     3593 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/changelog.rst
--rw-r--r--   0        0        0     6304 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/concepts.rst
--rw-r--r--   0        0        0     7858 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/conf.py
--rw-r--r--   0        0        0     1398 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/configfile.rst
--rw-r--r--   0        0        0      304 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/extrefs.inc
--rw-r--r--   0        0        0     2084 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/hacking.rst
--rw-r--r--   0        0        0     2250 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/index.rst
--rw-r--r--   0        0        0     3078 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/install.rst
--rw-r--r--   0        0        0     1415 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/intro.inc
--rw-r--r--   0        0        0     1473 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/manpage.rst
--rw-r--r--   0        0        0     7147 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/operations.rst
--rw-r--r--   0        0        0      518 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/puppet.rst
--rw-r--r--   0        0        0     1261 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/refs.rst
--rw-r--r--   0        0        0     8144 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/salt.rst
--rw-r--r--   0        0        0       35 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/substs.inc
--rw-r--r--   0        0        0     6233 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/todo.rst
--rw-r--r--   0        0        0     1895 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/doc/source/usage.rst
--rwxr-xr-x   0        0        0       96 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/ansible/hosts
--rw-r--r--   0        0        0       23 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/ansible/reclass-config.yml
--rw-r--r--   0        0        0      131 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/ansible/test.yml
--rw-r--r--   0        0        0     1362 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/init.yml
--rw-r--r--   0        0        0       72 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/release/jessie.yml
--rw-r--r--   0        0        0       72 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/release/lenny.yml
--rw-r--r--   0        0        0       70 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/release/sid.yml
--rw-r--r--   0        0        0       75 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/release/squeeze.yml
--rw-r--r--   0        0        0       71 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/release/wheezy.yml
--rw-r--r--   0        0        0      492 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/archived.yml
--rw-r--r--   0        0        0      351 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/include_backports.yml
--rw-r--r--   0        0        0      346 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/include_experimental.yml
--rw-r--r--   0        0        0      320 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/include_multimedia.yml
--rw-r--r--   0        0        0      545 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml
--rw-r--r--   0        0        0      148 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/oldstable.yml
--rw-r--r--   0        0        0      146 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/stable.yml
--rw-r--r--   0        0        0      146 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/testing.yml
--rw-r--r--   0        0        0      146 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/unstable.yml
--rw-r--r--   0        0        0      563 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/example.org.yml
--rw-r--r--   0        0        0      143 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/hosted@munich.yml
--rw-r--r--   0        0        0      142 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/hosted@zurich.yml
--rw-r--r--   0        0        0       26 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/mail/init.yml
--rw-r--r--   0        0        0       68 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/mail/relay.yml
--rw-r--r--   0        0        0      200 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/mail/satellite.yml
--rw-r--r--   0        0        0       55 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/mail/server.yml
--rw-r--r--   0        0        0      177 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/salt.minion.yml
--rw-r--r--   0        0        0      320 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/sudo.yml
--rw-r--r--   0        0        0       25 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/classes/webserver.yml
--rw-r--r--   0        0        0      175 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/nodes/munich/black.example.org.yml
--rw-r--r--   0        0        0      157 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/nodes/munich/yellow.example.org.yml
--rw-r--r--   0        0        0      211 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/nodes/zurich/blue.example.org.yml
--rw-r--r--   0        0        0      159 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/nodes/zurich/white.example.org.yml
--rwxr-xr-x   0        0        0       93 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/salt/reclass
--rw-r--r--   0        0        0       23 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/examples/salt/reclass-config.yml
--rw-r--r--   0        0        0     1058 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/reclass/__init__.py
--rwxr-xr-x   0        0        0      366 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/reclass/adapters/__init__.py
--rwxr-xr-x   0        0        0     4348 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/reclass/adapters/ansible.py
--rwxr-xr-x   0        0        0     5517 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/reclass/adapters/salt.py
--rw-r--r--   0        0        0     1811 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/reclass/cli.py
--rw-r--r--   0        0        0     9536 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/config.py
--rw-r--r--   0        0        0      594 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/constants.py
--rw-r--r--   0        0        0    11835 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/core.py
--rw-r--r--   0        0        0      527 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/__init__.py
--rw-r--r--   0        0        0     2407 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/applications.py
--rw-r--r--   0        0        0     2349 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/classes.py
--rw-r--r--   0        0        0     4510 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/entity.py
--rw-r--r--   0        0        0     3644 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/exports.py
--rw-r--r--   0        0        0    14190 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/parameters.py
--rw-r--r--   0        0        0      169 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/__init__.py
--rw-r--r--   0        0        0     2483 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_applications.py
--rw-r--r--   0        0        0     4054 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_classes.py
--rw-r--r--   0        0        0    15579 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_entity.py
--rw-r--r--   0        0        0     5875 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_exports.py
--rw-r--r--   0        0        0    35361 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_parameters.py
--rw-r--r--   0        0        0     1770 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/defaults.py
--rw-r--r--   0        0        0    11777 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/errors.py
--rw-r--r--   0        0        0     1086 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/output/__init__.py
--rw-r--r--   0        0        0      697 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/output/json_outputter.py
--rw-r--r--   0        0        0      971 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/output/yaml_outputter.py
--rw-r--r--   0        0        0     2966 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/settings.py
--rw-r--r--   0        0        0     1611 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/__init__.py
--rw-r--r--   0        0        0     1294 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/common.py
--rw-r--r--   0        0        0     1284 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/loader.py
--rw-r--r--   0        0        0     2294 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/memcache_proxy.py
--rw-r--r--   0        0        0     2419 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/mixed/__init__.py
--rw-r--r--   0        0        0      169 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/__init__.py
--rw-r--r--   0        0        0      725 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/test_loader.py
--rw-r--r--   0        0        0     4070 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py
--rw-r--r--   0        0        0     1254 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/test_yamldata.py
--rw-r--r--   0        0        0     4031 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yaml_fs/__init__.py
--rw-r--r--   0        0        0     2258 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yaml_fs/directory.py
--rw-r--r--   0        0        0    12803 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yaml_git/__init__.py
--rw-r--r--   0        0        0     3721 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yamldata.py
--rw-r--r--   0        0        0      169 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/__init__.py
--rw-r--r--   0        0        0       48 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/01/classes/standard.yml
--rw-r--r--   0        0        0       63 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/01/nodes/class_notfound.yml
--rw-r--r--   0        0        0       22 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/01/nodes/data_types.yml
--rw-r--r--   0        0        0       28 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/four.yml
--rw-r--r--   0        0        0       27 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/init.yml
--rw-r--r--   0        0        0      183 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/one/alpha.yml
--rw-r--r--   0        0        0       26 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/one/beta.yml
--rw-r--r--   0        0        0       22 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/three.yml
--rw-r--r--   0        0        0       26 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/two/beta.yml
--rw-r--r--   0        0        0       27 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/classes/two/gamma.yml
--rw-r--r--   0        0        0       23 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/nodes/relative.yml
--rw-r--r--   0        0        0       19 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/02/nodes/top_relative.yml
--rw-r--r--   0        0        0       57 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/classes/a.yml
--rw-r--r--   0        0        0       57 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/classes/b.yml
--rw-r--r--   0        0        0       57 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/classes/c.yml
--rw-r--r--   0        0        0       57 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/classes/d.yml
--rw-r--r--   0        0        0       17 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/nodes/alpha/one.yml
--rw-r--r--   0        0        0       17 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/nodes/alpha/two.yml
--rw-r--r--   0        0        0       17 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/nodes/beta/one.yml
--rw-r--r--   0        0        0       17 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/03/nodes/beta/two.yml
--rw-r--r--   0        0        0       23 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/04/classes/one.yml
--rw-r--r--   0        0        0       23 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/04/classes/three.yml
--rw-r--r--   0        0        0       23 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/04/classes/two.yml
--rw-r--r--   0        0        0       17 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/04/nodes/alpha/node1.yml
--rw-r--r--   0        0        0       53 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v0.yml
--rw-r--r--   0        0        0       53 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v1.yml
--rw-r--r--   0        0        0      134 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/components/common.yml
--rw-r--r--   0        0        0       43 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v0.yml
--rw-r--r--   0        0        0       43 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v1.yml
--rw-r--r--   0        0        0       75 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/versions/default_versions.yml
--rw-r--r--   0        0        0      114 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/versions/dev.yml
--rw-r--r--   0        0        0       52 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/versions/prd.yml
--rw-r--r--   0        0        0       87 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/classes/versions/stg.yml
--rw-r--r--   0        0        0      101 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/nodes/dev.yml
--rw-r--r--   0        0        0      101 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/nodes/prd.yml
--rw-r--r--   0        0        0      101 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/05/nodes/stg.yml
--rw-r--r--   0        0        0       50 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/06/classes/applications/shared.yml
--rw-r--r--   0        0        0       98 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/06/classes/environments/envA.yml
--rw-r--r--   0        0        0       67 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/06/classes/environments/envB.yml
--rw-r--r--   0        0        0      140 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/06/nodes/A_node.yml
--rw-r--r--   0        0        0      140 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/data/06/nodes/B_node.yml
--rw-r--r--   0        0        0     6811 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/test_core.py
--rw-r--r--   0        0        0      169 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/__init__.py
--rw-r--r--   0        0        0     5289 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/dictpath.py
--rw-r--r--   0        0        0      281 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/parameterdict.py
--rw-r--r--   0        0        0      281 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/parameterlist.py
--rw-r--r--   0        0        0      169 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/tests/__init__.py
--rw-r--r--   0        0        0     4504 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/tests/test_dictpath.py
--rw-r--r--   0        0        0      173 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/__init__.py
--rw-r--r--   0        0        0      848 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/compitem.py
--rw-r--r--   0        0        0      170 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/dictitem.py
--rw-r--r--   0        0        0     9225 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/invitem.py
--rw-r--r--   0        0        0     2355 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/item.py
--rw-r--r--   0        0        0      392 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/listitem.py
--rw-r--r--   0        0        0     3031 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/parser.py
--rw-r--r--   0        0        0     7207 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/parser_funcs.py
--rw-r--r--   0        0        0     1364 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/refitem.py
--rw-r--r--   0        0        0      777 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/scaitem.py
--rw-r--r--   0        0        0        0 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/__init__.py
--rw-r--r--   0        0        0     4043 2023-03-02 12:58:11.545235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_compitem.py
--rw-r--r--   0        0        0     1398 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_item.py
--rw-r--r--   0        0        0      979 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_listitem.py
--rw-r--r--   0        0        0     4512 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_parser_functions.py
--rw-r--r--   0        0        0     1727 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_refitem.py
--rw-r--r--   0        0        0     1176 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_scaitem.py
--rw-r--r--   0        0        0     4587 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_value.py
--rw-r--r--   0        0        0     2780 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/value.py
--rw-r--r--   0        0        0     6797 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/values/valuelist.py
--rw-r--r--   0        0        0      966 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/reclass/version.py
--rwxr-xr-x   0        0        0      426 2023-03-02 12:58:11.541235 kapitan-0.31.1rc3/kapitan/reclass/reclass.py
--rw-r--r--   0        0        0     1948 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/releasenotes/config.yaml
--rw-r--r--   0        0        0      109 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/releasenotes/notes/escaping-references-e76699d8ca010013.yaml
--rw-r--r--   0        0        0       32 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/requirements.txt
--rwxr-xr-x   0        0        0      502 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/run_tests.py
--rw-r--r--   0        0        0      254 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/setup.cfg
--rw-r--r--   0        0        0     1780 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/setup.py
--rw-r--r--   0        0        0      413 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/default/classes/first.yml
--rw-r--r--   0        0        0       34 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/default/classes/lab/env/dev.yml
--rw-r--r--   0        0        0      109 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/default/classes/second.yml
--rw-r--r--   0        0        0      361 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/default/classes/third.yml
--rw-r--r--   0        0        0       18 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/default/nodes/reclass.yml
--rw-r--r--   0        0        0       22 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/default/reclass-config.yml
--rw-r--r--   0        0        0       42 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/defaults.yml
--rw-r--r--   0        0        0       77 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/first.yml
--rw-r--r--   0        0        0       34 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/lab/env/dev.yml
--rw-r--r--   0        0        0       22 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/relative/init.yml
--rw-r--r--   0        0        0       63 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/relative/nested/common.yml
--rw-r--r--   0        0        0       53 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/common.yml
--rw-r--r--   0        0        0       91 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/init.yml
--rw-r--r--   0        0        0       53 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/relative/nested/dive/session.yml
--rw-r--r--   0        0        0      100 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/relative/nested/init.yml
--rw-r--r--   0        0        0      104 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/second.yml
--rw-r--r--   0        0        0      191 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/classes/third.yml
--rw-r--r--   0        0        0       19 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/nodes/reclass.yml
--rw-r--r--   0        0        0       78 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/test/model/extensions/reclass-config.yml
--rw-r--r--   0        0        0      976 2023-03-02 12:58:11.549235 kapitan-0.31.1rc3/kapitan/reclass/tox.ini
--rw-r--r--   0        0        0      125 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/__init__.py
--rw-r--r--   0        0        0    26916 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/base.py
--rw-r--r--   0        0        0     2833 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/base64.py
--rw-r--r--   0        0        0    24002 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/cmd_parser.py
--rw-r--r--   0        0        0     1453 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/env.py
--rw-r--r--   0        0        0     7277 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/functions.py
--rw-r--r--   0        0        0      125 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/__init__.py
--rw-r--r--   0        0        0     4904 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/awskms.py
--rw-r--r--   0        0        0     5867 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/azkms.py
--rw-r--r--   0        0        0     5814 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/gkms.py
--rw-r--r--   0        0        0     7299 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/gpg.py
--rw-r--r--   0        0        0     9041 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/vaultkv.py
--rw-r--r--   0        0        0    11361 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/refs/secrets/vaulttransit.py
--rw-r--r--   0        0        0        0 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/remoteinventory/__init__.py
--rw-r--r--   0        0        0     4348 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/remoteinventory/fetch.py
--rw-r--r--   0        0        0    14175 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/resources.py
--rw-r--r--   0        0        0    35389 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/targets.py
--rw-r--r--   0        0        0    21859 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/utils.py
--rw-r--r--   0        0        0      125 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/validator/__init__.py
--rw-r--r--   0        0        0      369 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/validator/base.py
--rw-r--r--   0        0        0     3805 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/validator/kubernetes_validator.py
--rw-r--r--   0        0        0      511 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/kapitan/version.py
--rw-r--r--   0        0        0     1891 2023-03-02 12:58:11.097229 kapitan-0.31.1rc3/pyproject.toml
--rw-r--r--   0        0        0    10230 1970-01-01 00:00:00.000000 kapitan-0.31.1rc3/setup.py
--rw-r--r--   0        0        0     4732 1970-01-01 00:00:00.000000 kapitan-0.31.1rc3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-02 21:01:54.811166 kapitan-0.32.0rc0/LICENSES/
+-rw-r--r--   0        0        0     2443 2023-05-02 21:01:54.811166 kapitan-0.32.0rc0/README.md
+-rwxr-xr-x   0        0        0     1088 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/__main__.py
+-rw-r--r--   0        0        0     1889 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/cached.py
+-rw-r--r--   0        0        0    21712 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/cli.py
+-rw-r--r--   0        0        0      719 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/defaults.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/dependency_manager/__init__.py
+-rw-r--r--   0        0        0    11773 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/dependency_manager/base.py
+-rw-r--r--   0        0        0     1411 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/errors.py
+-rw-r--r--   0        0        0      951 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/helm_cli.py
+-rw-r--r--   0        0        0     1423 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/initialiser.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/__init__.py
+-rw-r--r--   0        0        0     7390 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/base.py
+-rw-r--r--   0        0        0     1904 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/copy.py
+-rw-r--r--   0        0        0     3324 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/external.py
+-rw-r--r--   0        0        0     9501 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/helm.py
+-rw-r--r--   0        0        0     2705 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/jinja2.py
+-rw-r--r--   0        0        0     6327 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/jinja2_filters.py
+-rw-r--r--   0        0        0     6087 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/jsonnet.py
+-rw-r--r--   0        0        0     7966 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/kadet.py
+-rw-r--r--   0        0        0     1137 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/remove.py
+-rw-r--r--   0        0        0      163 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/components/my_component/my_component.jsonnet
+-rw-r--r--   0        0        0      267 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/components/other_component/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/classes/common.yml
+-rw-r--r--   0        0        0      629 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/classes/my_component.yml
+-rw-r--r--   0        0        0       75 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/targets/my_target.yml
+-rw-r--r--   0        0        0      129 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/templates/docs/my_readme.md
+-rw-r--r--   0        0        0      145 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/templates/scripts/my_script.sh
+-rw-r--r--   0        0        0     1008 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/lib/kapitan.libjsonnet
+-rw-r--r--   0        0        0     8444 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/lint.py
+-rw-r--r--   0        0        0       43 2023-05-02 21:01:55.343198 kapitan-0.32.0rc0/kapitan/reclass/.git
+-rw-r--r--   0        0        0       97 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.gitignore
+-rwxr-xr-x   0        0        0      526 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.kitchen-verify.sh
+-rw-r--r--   0        0        0      868 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.kitchen.yml
+-rw-r--r--   0        0        0       31 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.pylintrc
+-rw-r--r--   0        0        0     2522 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.travis.yml
+-rw-r--r--   0        0        0     9350 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/LICENSE
+-rw-r--r--   0        0        0      385 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/MANIFEST.in
+-rw-r--r--   0        0        0     1366 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/Makefile
+-rw-r--r--   0        0        0      282 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/Pipfile
+-rw-r--r--   0        0        0    17685 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/README-extensions.rst
+-rw-r--r--   0        0        0     1260 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/README.rst
+-rw-r--r--   0        0        0        7 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/.gitignore
+-rw-r--r--   0        0        0     5580 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/Makefile
+-rw-r--r--   0        0        0     8228 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/ansible.rst
+-rw-r--r--   0        0        0     3593 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/changelog.rst
+-rw-r--r--   0        0        0     6304 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/concepts.rst
+-rw-r--r--   0        0        0     7858 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/conf.py
+-rw-r--r--   0        0        0     1398 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/configfile.rst
+-rw-r--r--   0        0        0      304 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/extrefs.inc
+-rw-r--r--   0        0        0     2084 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/hacking.rst
+-rw-r--r--   0        0        0     2250 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/index.rst
+-rw-r--r--   0        0        0     3078 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/install.rst
+-rw-r--r--   0        0        0     1415 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/intro.inc
+-rw-r--r--   0        0        0     1473 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/manpage.rst
+-rw-r--r--   0        0        0     7147 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/operations.rst
+-rw-r--r--   0        0        0      518 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/puppet.rst
+-rw-r--r--   0        0        0     1261 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/refs.rst
+-rw-r--r--   0        0        0     8144 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/salt.rst
+-rw-r--r--   0        0        0       35 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/substs.inc
+-rw-r--r--   0        0        0     6233 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/todo.rst
+-rw-r--r--   0        0        0     1895 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/usage.rst
+-rwxr-xr-x   0        0        0       96 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/ansible/hosts
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/ansible/reclass-config.yml
+-rw-r--r--   0        0        0      131 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/ansible/test.yml
+-rw-r--r--   0        0        0     1362 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/init.yml
+-rw-r--r--   0        0        0       72 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/jessie.yml
+-rw-r--r--   0        0        0       72 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/lenny.yml
+-rw-r--r--   0        0        0       70 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/sid.yml
+-rw-r--r--   0        0        0       75 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/squeeze.yml
+-rw-r--r--   0        0        0       71 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/wheezy.yml
+-rw-r--r--   0        0        0      492 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/archived.yml
+-rw-r--r--   0        0        0      351 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_backports.yml
+-rw-r--r--   0        0        0      346 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_experimental.yml
+-rw-r--r--   0        0        0      320 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_multimedia.yml
+-rw-r--r--   0        0        0      545 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml
+-rw-r--r--   0        0        0      148 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/oldstable.yml
+-rw-r--r--   0        0        0      146 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/stable.yml
+-rw-r--r--   0        0        0      146 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/testing.yml
+-rw-r--r--   0        0        0      146 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/unstable.yml
+-rw-r--r--   0        0        0      563 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/example.org.yml
+-rw-r--r--   0        0        0      143 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/hosted@munich.yml
+-rw-r--r--   0        0        0      142 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/hosted@zurich.yml
+-rw-r--r--   0        0        0       26 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/init.yml
+-rw-r--r--   0        0        0       68 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/relay.yml
+-rw-r--r--   0        0        0      200 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/satellite.yml
+-rw-r--r--   0        0        0       55 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/server.yml
+-rw-r--r--   0        0        0      177 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/salt.minion.yml
+-rw-r--r--   0        0        0      320 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/sudo.yml
+-rw-r--r--   0        0        0       25 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/webserver.yml
+-rw-r--r--   0        0        0      175 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/munich/black.example.org.yml
+-rw-r--r--   0        0        0      157 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/munich/yellow.example.org.yml
+-rw-r--r--   0        0        0      211 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/zurich/blue.example.org.yml
+-rw-r--r--   0        0        0      159 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/zurich/white.example.org.yml
+-rwxr-xr-x   0        0        0       93 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/examples/salt/reclass
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/examples/salt/reclass-config.yml
+-rw-r--r--   0        0        0     1058 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/__init__.py
+-rwxr-xr-x   0        0        0      366 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/__init__.py
+-rwxr-xr-x   0        0        0     4348 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/ansible.py
+-rwxr-xr-x   0        0        0     5517 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/salt.py
+-rw-r--r--   0        0        0     1811 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/cli.py
+-rw-r--r--   0        0        0     9536 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/config.py
+-rw-r--r--   0        0        0      594 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/constants.py
+-rw-r--r--   0        0        0    11835 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/core.py
+-rw-r--r--   0        0        0      527 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/__init__.py
+-rw-r--r--   0        0        0     2407 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/applications.py
+-rw-r--r--   0        0        0     2349 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/classes.py
+-rw-r--r--   0        0        0     4510 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/entity.py
+-rw-r--r--   0        0        0     3644 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/exports.py
+-rw-r--r--   0        0        0    14190 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/parameters.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/__init__.py
+-rw-r--r--   0        0        0     2483 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_applications.py
+-rw-r--r--   0        0        0     4054 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_classes.py
+-rw-r--r--   0        0        0    15579 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_entity.py
+-rw-r--r--   0        0        0     5875 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_exports.py
+-rw-r--r--   0        0        0    35361 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_parameters.py
+-rw-r--r--   0        0        0     1770 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/defaults.py
+-rw-r--r--   0        0        0    11777 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/errors.py
+-rw-r--r--   0        0        0     1086 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/output/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/output/json_outputter.py
+-rw-r--r--   0        0        0      971 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/output/yaml_outputter.py
+-rw-r--r--   0        0        0     2966 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/settings.py
+-rw-r--r--   0        0        0     1611 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/common.py
+-rw-r--r--   0        0        0     1284 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/loader.py
+-rw-r--r--   0        0        0     2294 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/memcache_proxy.py
+-rw-r--r--   0        0        0     2419 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/mixed/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/__init__.py
+-rw-r--r--   0        0        0      725 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_loader.py
+-rw-r--r--   0        0        0     4070 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py
+-rw-r--r--   0        0        0     1254 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_yamldata.py
+-rw-r--r--   0        0        0     4031 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/__init__.py
+-rw-r--r--   0        0        0     2258 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/directory.py
+-rw-r--r--   0        0        0    12803 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_git/__init__.py
+-rw-r--r--   0        0        0     3721 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yamldata.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/01/classes/standard.yml
+-rw-r--r--   0        0        0       63 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/01/nodes/class_notfound.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/01/nodes/data_types.yml
+-rw-r--r--   0        0        0       28 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/four.yml
+-rw-r--r--   0        0        0       27 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/init.yml
+-rw-r--r--   0        0        0      183 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/one/alpha.yml
+-rw-r--r--   0        0        0       26 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/one/beta.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/three.yml
+-rw-r--r--   0        0        0       26 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/two/beta.yml
+-rw-r--r--   0        0        0       27 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/two/gamma.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/nodes/relative.yml
+-rw-r--r--   0        0        0       19 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/nodes/top_relative.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/a.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/b.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/c.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/d.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/alpha/one.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/alpha/two.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/beta/one.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/beta/two.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/classes/one.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/classes/three.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/classes/two.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/nodes/alpha/node1.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v0.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v1.yml
+-rw-r--r--   0        0        0      134 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/common.yml
+-rw-r--r--   0        0        0       43 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v0.yml
+-rw-r--r--   0        0        0       43 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v1.yml
+-rw-r--r--   0        0        0       75 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/default_versions.yml
+-rw-r--r--   0        0        0      114 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/dev.yml
+-rw-r--r--   0        0        0       52 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/prd.yml
+-rw-r--r--   0        0        0       87 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/stg.yml
+-rw-r--r--   0        0        0      101 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/nodes/dev.yml
+-rw-r--r--   0        0        0      101 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/nodes/prd.yml
+-rw-r--r--   0        0        0      101 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/nodes/stg.yml
+-rw-r--r--   0        0        0       50 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/classes/applications/shared.yml
+-rw-r--r--   0        0        0       98 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/classes/environments/envA.yml
+-rw-r--r--   0        0        0       67 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/classes/environments/envB.yml
+-rw-r--r--   0        0        0      140 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/nodes/A_node.yml
+-rw-r--r--   0        0        0      140 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/nodes/B_node.yml
+-rw-r--r--   0        0        0     6811 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/test_core.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/dictpath.py
+-rw-r--r--   0        0        0      281 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/parameterdict.py
+-rw-r--r--   0        0        0      281 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/parameterlist.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/tests/__init__.py
+-rw-r--r--   0        0        0     4504 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/tests/test_dictpath.py
+-rw-r--r--   0        0        0      173 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/compitem.py
+-rw-r--r--   0        0        0      170 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/dictitem.py
+-rw-r--r--   0        0        0     9225 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/invitem.py
+-rw-r--r--   0        0        0     2355 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/item.py
+-rw-r--r--   0        0        0      392 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/listitem.py
+-rw-r--r--   0        0        0     3031 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser.py
+-rw-r--r--   0        0        0     7207 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser_funcs.py
+-rw-r--r--   0        0        0     1364 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/refitem.py
+-rw-r--r--   0        0        0      777 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/scaitem.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/__init__.py
+-rw-r--r--   0        0        0     4043 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_compitem.py
+-rw-r--r--   0        0        0     1398 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_item.py
+-rw-r--r--   0        0        0      979 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_listitem.py
+-rw-r--r--   0        0        0     4512 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_parser_functions.py
+-rw-r--r--   0        0        0     1727 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_refitem.py
+-rw-r--r--   0        0        0     1176 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_scaitem.py
+-rw-r--r--   0        0        0     4587 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_value.py
+-rw-r--r--   0        0        0     2780 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/value.py
+-rw-r--r--   0        0        0     6797 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/valuelist.py
+-rw-r--r--   0        0        0      966 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/version.py
+-rwxr-xr-x   0        0        0      426 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass.py
+-rw-r--r--   0        0        0     1948 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/releasenotes/config.yaml
+-rw-r--r--   0        0        0      109 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/releasenotes/notes/escaping-references-e76699d8ca010013.yaml
+-rw-r--r--   0        0        0       32 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/requirements.txt
+-rwxr-xr-x   0        0        0      502 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/run_tests.py
+-rw-r--r--   0        0        0      254 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/setup.cfg
+-rw-r--r--   0        0        0     1780 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/setup.py
+-rw-r--r--   0        0        0      413 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/first.yml
+-rw-r--r--   0        0        0       34 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/lab/env/dev.yml
+-rw-r--r--   0        0        0      109 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/second.yml
+-rw-r--r--   0        0        0      361 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/third.yml
+-rw-r--r--   0        0        0       18 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/nodes/reclass.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/reclass-config.yml
+-rw-r--r--   0        0        0       42 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/defaults.yml
+-rw-r--r--   0        0        0       77 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/first.yml
+-rw-r--r--   0        0        0       34 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/lab/env/dev.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/init.yml
+-rw-r--r--   0        0        0       63 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/common.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/common.yml
+-rw-r--r--   0        0        0       91 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/init.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/dive/session.yml
+-rw-r--r--   0        0        0      100 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/init.yml
+-rw-r--r--   0        0        0      104 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/second.yml
+-rw-r--r--   0        0        0      191 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/third.yml
+-rw-r--r--   0        0        0       19 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/nodes/reclass.yml
+-rw-r--r--   0        0        0       78 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/reclass-config.yml
+-rw-r--r--   0        0        0      976 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/tox.ini
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/__init__.py
+-rw-r--r--   0        0        0    26916 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/base.py
+-rw-r--r--   0        0        0     2833 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/base64.py
+-rw-r--r--   0        0        0    24002 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/cmd_parser.py
+-rw-r--r--   0        0        0     1453 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/env.py
+-rw-r--r--   0        0        0     7277 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/functions.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/__init__.py
+-rw-r--r--   0        0        0     4904 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/awskms.py
+-rw-r--r--   0        0        0     5867 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/azkms.py
+-rw-r--r--   0        0        0     5814 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/gkms.py
+-rw-r--r--   0        0        0     7299 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/gpg.py
+-rw-r--r--   0        0        0     9041 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/vaultkv.py
+-rw-r--r--   0        0        0    11361 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/vaulttransit.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/remoteinventory/__init__.py
+-rw-r--r--   0        0        0     4346 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/remoteinventory/fetch.py
+-rw-r--r--   0        0        0    14266 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/resources.py
+-rw-r--r--   0        0        0    35433 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/targets.py
+-rw-r--r--   0        0        0    21894 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/utils.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/validator/__init__.py
+-rw-r--r--   0        0        0      369 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/validator/base.py
+-rw-r--r--   0        0        0     3805 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/validator/kubernetes_validator.py
+-rw-r--r--   0        0        0      511 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/version.py
+-rw-r--r--   0        0        0     1855 2023-05-02 21:01:54.843168 kapitan-0.32.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    10231 1970-01-01 00:00:00.000000 kapitan-0.32.0rc0/setup.py
+-rw-r--r--   0        0        0     4633 1970-01-01 00:00:00.000000 kapitan-0.32.0rc0/PKG-INFO
```

### Comparing `kapitan-0.31.1rc3/README.md` & `kapitan-0.32.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/__init__.py` & `kapitan-0.32.0rc0/kapitan/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/cached.py` & `kapitan-0.32.0rc0/kapitan/cached.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/cli.py` & `kapitan-0.32.0rc0/kapitan/cli.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/defaults.py` & `kapitan-0.32.0rc0/kapitan/defaults.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/dependency_manager/base.py` & `kapitan-0.32.0rc0/kapitan/dependency_manager/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 # point to the full output path
                 full_output_path = normalise_join_path(output_path, item["output_path"])
                 logger.debug("Updated output_path from %s to %s", item["output_path"], output_path)
                 item["output_path"] = full_output_path
 
                 if full_output_path in deps_output_paths[source_uri]:
                     # if the output_path is duplicated for the same source_uri
-                    logger.warning("Skipping duplicate output path for uri %s", source_uri)
+                    logger.debug("Skipping duplicate output path for uri %s", source_uri)
                     continue
                 else:
                     deps_output_paths[source_uri].add(full_output_path)
 
                 if dependency_type == "git":
                     git_deps[source_uri].append(item)
                 elif dependency_type in ("http", "https"):
@@ -120,30 +120,31 @@
             if os.path.isdir(full_subdir):
                 copy_src_path = full_subdir
             else:
                 raise GitSubdirNotFoundError(
                     "{} {}: subdir {} not found in repo".format(item_type, source, sub_dir)
                 )
         if force:
-            copy_tree(copy_src_path, output_path)
+            copied = copy_tree(copy_src_path, output_path, verbose=0)
         else:
-            safe_copy_tree(copy_src_path, output_path)
-        logger.info("%s %s: saved to %s", item_type, source, output_path)
+            copied = safe_copy_tree(copy_src_path, output_path)
+        if copied:
+            logger.info("%s %s: saved to %s", item_type, source, output_path)
 
 
 def fetch_git_source(source, save_dir, item_type):
     """clones a git repository at source and saves into save_dir"""
 
     if os.path.exists(save_dir):
         rmtree(save_dir)
         logger.debug("Removed %s", save_dir)
-    logger.info("%s %s: fetching now", item_type, source)
+    logger.debug("%s %s: fetching now", item_type, source)
     try:
         Repo.clone_from(source, save_dir)
-        logger.info("%s %s: successfully fetched", item_type, source)
+        logger.debug("%s %s: successfully fetched", item_type, source)
         logger.debug("Git clone cached to %s", save_dir)
     except GitCommandError as e:
         logger.error(e)
         raise GitFetchingError("{} {}: fetching unsuccessful\n{}".format(item_type, source, e.stderr))
 
 
 def fetch_http_dependency(dep_mapping, save_dir, force, item_type="Dependency"):
@@ -190,26 +191,26 @@
             parent_dir = os.path.dirname(output_path)
             if parent_dir != "":
                 os.makedirs(parent_dir, exist_ok=True)
             if force:
                 copyfile(cached_source_path, output_path)
             else:
                 safe_copy_file(cached_source_path, output_path)
-            logger.info("%s %s: saved to %s", item_type, source, output_path)
+            logger.debug("%s %s: saved to %s", item_type, source, output_path)
 
 
 def fetch_http_source(source, save_path, item_type):
     """downloads a http[s] file from source and saves into save_path(which is a file)"""
 
     if os.path.exists(save_path):
         os.remove(save_path)
         logger.debug("Removed %s", save_path)
-    logger.info("%s %s: fetching now", item_type, source)
+    logger.debug("%s %s: fetching now", item_type, source)
     content, content_type = make_request(source)
-    logger.info("%s %s: successfully fetched", item_type, source)
+    logger.debug("%s %s: successfully fetched", item_type, source)
     if content is not None:
         with open(save_path, "wb") as f:
             f.write(content)
         logger.debug("Cached to %s", save_path)
         return content_type
     logger.warning("%s %s: failed to fetch", item_type, source)
     return None
@@ -233,23 +234,26 @@
 
     for dep in deps:
         output_path = dep["output_path"]
 
         parent_dir = os.path.dirname(output_path)
         if parent_dir != "":
             os.makedirs(parent_dir, exist_ok=True)
+
         if force:
-            copy_tree(cached_repo_path, output_path)
+            copied = copy_tree(cached_repo_path, output_path, verbose=0)
         else:
-            safe_copy_tree(cached_repo_path, output_path)
-        logger.info("Dependency %s: saved to %s", source.chart_name, output_path)
+            copied = safe_copy_tree(cached_repo_path, output_path)
+
+        if copied:
+            logger.info("Dependency %s: saved to %s", source.chart_name, output_path)
 
 
 def fetch_helm_archive(helm_path, repo, chart_name, version, save_path):
-    logger.info("Dependency helm chart %s and version %s: fetching now", chart_name, version or "latest")
+    logger.debug("Dependency helm chart %s and version %s: fetching now", chart_name, version or "latest")
     # Fetch archive and untar it into parent dir
     save_dir = os.path.dirname(save_path)
     args = ["pull", "--destination", save_dir, "--untar"]
 
     if version:
         args.append("--version")
         args.append(version)
@@ -264,16 +268,16 @@
     response = helm_cli(helm_path, args)
     if response != "":
         logger.warning("Dependency helm chart %s and version %s: %s", chart_name, version, response)
         raise HelmFetchingError(response)
     else:
         # rename chart to requested name
         os.rename(os.path.join(save_dir, chart_name), save_path)
-        logger.info("Dependency helm chart %s and version %s: successfully fetched", chart_name, version)
-        logger.info("Dependency helm chart %s and version %s: saved to %s", chart_name, version, save_path)
+        logger.debug("Dependency helm chart %s and version %s: successfully fetched", chart_name, version)
+        logger.debug("Dependency helm chart %s and version %s: saved to %s", chart_name, version, save_path)
 
 
 def exists_in_cache(item_path):
     dep_cache_path = os.path.dirname(item_path)
     if not os.path.exists(dep_cache_path):
         return False
     return os.path.basename(item_path) in os.listdir(dep_cache_path)
```

### Comparing `kapitan-0.31.1rc3/kapitan/errors.py` & `kapitan-0.32.0rc0/kapitan/errors.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/helm_cli.py` & `kapitan-0.32.0rc0/kapitan/helm_cli.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/initialiser.py` & `kapitan-0.32.0rc0/kapitan/initialiser.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/base.py` & `kapitan-0.32.0rc0/kapitan/inputs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,29 +60,29 @@
         """
         Compile validated input_path in comp_obj
         kwargs are passed into compile_file()
         """
         target_name = ext_vars["target"]
         output_path = comp_obj["output_path"]
         output_type = comp_obj.get("output_type", self.default_output_type())
-        prune_input = comp_obj.get("prune", kwargs.get("prune", False))
+        prune_output = comp_obj.get("prune", kwargs.get("prune", False))
 
         logger.debug("Compiling %s", input_path)
         try:
             if kwargs.get("compose_node_name", False):
                 _compile_path = os.path.join(self.compile_path, target_name.replace(".", "/"), output_path)
             else:
                 _compile_path = os.path.join(self.compile_path, target_name, output_path)
             self.compile_file(
                 input_path,
                 _compile_path,
                 ext_vars,
                 output=output_type,
                 target_name=target_name,
-                prune_input=prune_input,
+                prune_output=prune_output,
                 **kwargs,
             )
         except KapitanError as e:
             raise CompileError("{}\nCompile error: failed to compile target: {}".format(e, target_name))
 
     def make_compile_dirs(self, target_name, output_path, **kwargs):
         """make compile dirs, skips if dirs exist"""
```

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/copy.py` & `kapitan-0.32.0rc0/kapitan/inputs/copy.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/external.py` & `kapitan-0.32.0rc0/kapitan/inputs/external.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/helm.py` & `kapitan-0.32.0rc0/kapitan/inputs/helm.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/jinja2.py` & `kapitan-0.32.0rc0/kapitan/inputs/jinja2.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/jinja2_filters.py` & `kapitan-0.32.0rc0/kapitan/inputs/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/jsonnet.py` & `kapitan-0.32.0rc0/kapitan/inputs/jsonnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     def compile_file(self, file_path, compile_path, ext_vars, **kwargs):
         """
         Write file_path (jsonnet evaluated) items as files to compile_path.
         ext_vars will be passed as parameters to jsonnet_file()
         kwargs:
             output: default 'yaml', accepts 'json'
-            prune: default False, accepts True
+            prune_output: default False, accepts True
             reveal: default False, set to reveal refs on compile
             target_name: default None, set to current target being compiled
             indent: default 2
         """
 
         def _search_imports(cwd, imp):
             return search_imports(cwd, imp, self.search_paths)
@@ -93,20 +93,20 @@
                 import_callback=_search_imports,
                 native_callbacks=resource_callbacks(self.search_paths),
                 ext_vars=ext_vars,
             )
         output_obj = json.loads(json_output)
 
         output = kwargs.get("output", "yaml")
-        prune = kwargs.get("prune_input", False)
+        prune_output = kwargs.get("prune_output", False)
         reveal = kwargs.get("reveal", False)
         target_name = kwargs.get("target_name", None)
         indent = kwargs.get("indent", 2)
 
-        if prune:
+        if prune_output:
             output_obj = prune_empty(output_obj)
             logger.debug("Pruned output for: %s", file_path)
 
         if not isinstance(output_obj, dict):
             tmp_output_obj = output_obj
             # assume that the output filename is the
             # same as the input jsonnet filename
```

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/kadet.py` & `kapitan-0.32.0rc0/kapitan/inputs/kadet.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,21 +88,21 @@
 
     def compile_file(self, file_path, compile_path, ext_vars, **kwargs):
         """
         Write file_path (kadet evaluated) items as files to compile_path.
         ext_vars is not used in Kadet
         kwargs:
             output: default 'yaml', accepts 'json'
-            prune: default False
+            prune_output: default False
             reveal: default False, set to reveal refs on compile
             target_name: default None, set to current target being compiled
             indent: default 2
         """
         output = kwargs.get("output", "yaml")
-        prune = kwargs.get("prune", False)
+        prune_output = kwargs.get("prune_output", False)
         reveal = kwargs.get("reveal", False)
         target_name = kwargs.get("target_name", None)
         # inventory_path = kwargs.get("inventory_path", None)
         indent = kwargs.get("indent", 2)
 
         current_target.set(target_name)
         search_paths.set(self.search_paths)
@@ -131,15 +131,15 @@
                 output_obj = kadet_module.main()
         except Exception:
             # Log traceback and exception as is
             logger.exception("")
             raise CompileError(f"Could not load Kadet module: {spec.name[16:]}")
 
         output_obj = _to_dict(output_obj)
-        if prune:
+        if prune_output:
             output_obj = prune_empty(output_obj)
 
         # Return None if output_obj has no output
         if not output_obj:
             return None
 
         for item_key, item_value in output_obj.items():
```

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/remove.py` & `kapitan-0.32.0rc0/kapitan/inputs/remove.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/inputs/templates/inventory/classes/my_component.yml` & `kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/classes/my_component.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/lib/kapitan.libjsonnet` & `kapitan-0.32.0rc0/kapitan/lib/kapitan.libjsonnet`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/lint.py` & `kapitan-0.32.0rc0/kapitan/lint.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/.kitchen-verify.sh` & `kapitan-0.32.0rc0/kapitan/reclass/.kitchen-verify.sh`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/.kitchen.yml` & `kapitan-0.32.0rc0/kapitan/reclass/.kitchen.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/.travis.yml` & `kapitan-0.32.0rc0/kapitan/reclass/.travis.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/LICENSE` & `kapitan-0.32.0rc0/kapitan/reclass/LICENSE`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/Makefile` & `kapitan-0.32.0rc0/kapitan/reclass/Makefile`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/README-extensions.rst` & `kapitan-0.32.0rc0/kapitan/reclass/README-extensions.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/README.rst` & `kapitan-0.32.0rc0/kapitan/reclass/README.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/Makefile` & `kapitan-0.32.0rc0/kapitan/reclass/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/ansible.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/ansible.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/changelog.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/concepts.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/concepts.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/conf.py` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/configfile.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/configfile.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/hacking.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/hacking.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/index.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/install.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/intro.inc` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/intro.inc`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/manpage.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/manpage.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/operations.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/operations.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/puppet.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/puppet.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/refs.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/refs.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/salt.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/salt.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/todo.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/todo.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/doc/source/usage.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/init.yml` & `kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/init.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml` & `kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/examples/classes/example.org.yml` & `kapitan-0.32.0rc0/kapitan/reclass/examples/classes/example.org.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/adapters/ansible.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/ansible.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/adapters/salt.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/salt.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/cli.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/cli.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/config.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/config.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/constants.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/constants.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/core.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/core.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/applications.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/applications.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/classes.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/entity.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/entity.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/exports.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/exports.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/parameters.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/parameters.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_applications.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_classes.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_entity.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_exports.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/datatypes/tests/test_parameters.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/defaults.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/defaults.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/errors.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/errors.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/output/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/output/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/output/json_outputter.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/output/json_outputter.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/output/yaml_outputter.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/output/yaml_outputter.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/settings.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/settings.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/common.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/common.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/loader.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/loader.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/memcache_proxy.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/memcache_proxy.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/mixed/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/test_loader.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/tests/test_yamldata.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_yamldata.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yaml_fs/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yaml_fs/directory.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/directory.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yaml_git/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_git/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/storage/yamldata.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yamldata.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/tests/test_core.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/dictpath.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/dictpath.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/utils/tests/test_dictpath.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/tests/test_dictpath.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/compitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/compitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/invitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/invitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/item.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/item.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/parser.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/parser_funcs.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser_funcs.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/refitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/refitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/scaitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/scaitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_compitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_compitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_item.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_listitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_listitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_parser_functions.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_parser_functions.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_refitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_refitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_scaitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_scaitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/tests/test_value.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/value.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/value.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/values/valuelist.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/valuelist.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/reclass/version.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/version.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/releasenotes/config.yaml` & `kapitan-0.32.0rc0/kapitan/reclass/releasenotes/config.yaml`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/setup.py` & `kapitan-0.32.0rc0/kapitan/reclass/setup.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/reclass/tox.ini` & `kapitan-0.32.0rc0/kapitan/reclass/tox.ini`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/base.py` & `kapitan-0.32.0rc0/kapitan/refs/base.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/base64.py` & `kapitan-0.32.0rc0/kapitan/refs/base64.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/cmd_parser.py` & `kapitan-0.32.0rc0/kapitan/refs/cmd_parser.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/env.py` & `kapitan-0.32.0rc0/kapitan/refs/env.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/functions.py` & `kapitan-0.32.0rc0/kapitan/refs/functions.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/secrets/awskms.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/awskms.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/secrets/azkms.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/azkms.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/secrets/gkms.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/gkms.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/secrets/gpg.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/gpg.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/secrets/vaultkv.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/vaultkv.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/refs/secrets/vaulttransit.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/vaulttransit.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/kapitan/remoteinventory/fetch.py` & `kapitan-0.32.0rc0/kapitan/remoteinventory/fetch.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 # ./inventory by default
                 output_path = normalise_join_path(inventory_path, inv["output_path"])
                 logger.debug("Updated output_path from %s to %s", inv["output_path"], output_path)
                 inv["output_path"] = output_path
 
                 if output_path in inv_output_path[source_uri]:
                     # if the output_path is duplicated for the same source_uri
-                    logger.warning("Skipping duplicate output path for uri %s", source_uri)
+                    logger.debug("Skipping duplicate output path for uri %s", source_uri)
                     continue
                 else:
                     inv_output_path[source_uri].add(output_path)
 
                 if inv_type == "git":
                     git_inventories[source_uri].append(inv)
                 elif inv_type in ("http", "https"):
```

### Comparing `kapitan-0.31.1rc3/kapitan/resources.py` & `kapitan-0.32.0rc0/kapitan/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # SPDX-FileCopyrightText: 2020 The Kapitan Authors <kapitan-admins@googlegroups.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 "kapitan resources"
 
 import base64
-import errno
 import gzip
 import io
 import json
 import logging
 import os
 import sys
 from functools import partial
@@ -311,54 +310,60 @@
     (same output as running ./reclass.py -b inv_base_uri/ --inventory)
     Will attempt to read reclass config from 'reclass-config.yml' otherwise
     it will failback to the default config.
     Returns a reclass style dictionary
 
     Does not throw errors if a class is not found while --fetch flag is enabled
     """
+    # if inventory is already cached theres nothing to do
+    if cached.inv:
+        return cached.inv
+
+    # set default values initially
+    reclass_config = reclass_config_defaults = {
+        "storage_type": "yaml_fs",
+        "inventory_base_uri": inventory_path,
+        "nodes_uri": "targets",
+        "classes_uri": "classes",
+        "compose_node_name": False,
+        "allow_none_override": True,
+        "ignore_class_notfound": ignore_class_notfound,  # false by default
+    }
+
+    # get reclass config from file 'inventory/reclass-config.yml'
+    cfg_file = os.path.join(inventory_path, "reclass-config.yml")
+    if os.path.isfile(cfg_file):
+        with open(cfg_file, "r") as fp:
+            config = yaml.load(fp.read(), Loader=YamlLoader)
+            logger.debug("Using reclass inventory config at: {}".format(cfg_file))
+        if config:
+            # set attributes, take default values if not present
+            for key, value in config.items():
+                reclass_config[key] = value
+        else:
+            logger.debug("{}: Empty config file. Using reclass inventory config defaults".format(cfg_file))
+    else:
+        logger.debug("Inventory reclass: No config file found. Using reclass inventory config defaults")
 
-    if not cached.inv:
-        reclass_config = {
-            "storage_type": "yaml_fs",
-            "inventory_base_uri": inventory_path,
-            "nodes_uri": os.path.join(inventory_path, "targets"),
-            "classes_uri": os.path.join(inventory_path, "classes"),
-            "compose_node_name": False,
-            "allow_none_override": True,
-            "ignore_class_notfound": ignore_class_notfound,
-        }
-
-        try:
-            cfg_file = os.path.join(inventory_path, "reclass-config.yml")
-            with open(cfg_file) as reclass_cfg:
-                reclass_config = yaml.load(reclass_cfg, Loader=YamlLoader)
-                # normalise relative nodes_uri and classes_uri paths
-                for uri in ("nodes_uri", "classes_uri"):
-                    uri_val = reclass_config.get(uri)
-                    uri_path = os.path.join(inventory_path, uri_val)
-                    normalised_path = os.path.normpath(uri_path)
-                    reclass_config.update({uri: normalised_path})
-                logger.debug("Using reclass inventory config at: %s", cfg_file)
-        except IOError as ex:
-            # If file does not exist, ignore
-            if ex.errno == errno.ENOENT:
-                logger.debug("Using reclass inventory config defaults")
-
-        try:
-            storage = reclass.get_storage(
-                reclass_config["storage_type"],
-                reclass_config["nodes_uri"],
-                reclass_config["classes_uri"],
-                reclass_config["compose_node_name"],
-            )
-            class_mappings = reclass_config.get("class_mappings")  # this defaults to None (disabled)
-            _reclass = reclass.core.Core(storage, class_mappings, reclass.settings.Settings(reclass_config))
-
-            cached.inv = _reclass.inventory()
-        except ReclassException as e:
-            if isinstance(e, NotFoundError):
-                logger.error("Inventory reclass error: inventory not found")
-            else:
-                logger.error("Inventory reclass error: %s", e.message)
-            raise InventoryError(e.message)
+    # normalise relative nodes_uri and classes_uri paths
+    for uri in ("nodes_uri", "classes_uri"):
+        reclass_config[uri] = os.path.normpath(os.path.join(inventory_path, reclass_config[uri]))
+
+    try:
+        storage = reclass.get_storage(
+            reclass_config["storage_type"],
+            reclass_config["nodes_uri"],
+            reclass_config["classes_uri"],
+            reclass_config["compose_node_name"],
+        )
+        class_mappings = reclass_config.get("class_mappings")  # this defaults to None (disabled)
+        _reclass = reclass.core.Core(storage, class_mappings, reclass.settings.Settings(reclass_config))
+
+        cached.inv = _reclass.inventory()
+    except ReclassException as e:
+        if isinstance(e, NotFoundError):
+            logger.error("Inventory reclass error: inventory not found")
+        else:
+            logger.error("Inventory reclass error: %s", e.message)
+        raise InventoryError(e.message)
 
     return cached.inv
```

### Comparing `kapitan-0.31.1rc3/kapitan/targets.py` & `kapitan-0.32.0rc0/kapitan/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,18 @@
         # so p is only not None when raising an exception
         [p.get() for p in pool.imap_unordered(worker, target_objs) if p]
 
         os.makedirs(compile_path, exist_ok=True)
 
         # if '-t' is set on compile or only a few changed, only override selected targets
         if updated_targets:
-            for target in updated_targets:
-                compile_path_target = os.path.join(compile_path, target)
-                temp_path_target = os.path.join(temp_compile_path, target)
+            for target in target_objs:
+                path = target["target_full_path"]
+                compile_path_target = os.path.join(compile_path, path)
+                temp_path_target = os.path.join(temp_compile_path, path)
 
                 os.makedirs(compile_path_target, exist_ok=True)
 
                 shutil.rmtree(compile_path_target)
                 shutil.copytree(temp_path_target, compile_path_target)
                 logger.debug("Copied %s into %s", temp_path_target, compile_path_target)
         # otherwise override all targets
@@ -400,15 +401,15 @@
             inv_target = inv["nodes"][target_name]
             target_obj = inv_target["parameters"]["kapitan"]
             # check if parameters.kapitan is empty
             if not target_obj:
                 raise InventoryError(
                     "InventoryError: {}: parameters.kapitan has no assignment".format(target_name)
                 )
-            target_obj["target_full_path"] = inv_target["__reclass__"]["node"].replace("./", "")
+            target_obj["target_full_path"] = inv_target["parameters"]["_reclass_"]["name"]["path"]
             require_compile = not ignore_class_notfound
             valid_target_obj(target_obj, require_compile)
             validate_matching_target_name(target_name, target_obj, inventory_path)
             logger.debug("load_target_inventory: found valid kapitan target %s", target_name)
             target_objs.append(target_obj)
         except KeyError:
             logger.debug("load_target_inventory: target %s has no kapitan compile obj", target_name)
```

### Comparing `kapitan-0.31.1rc3/kapitan/utils.py` & `kapitan-0.32.0rc0/kapitan/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
     if os.path.isdir(dst):
         dir = dst
         dst = os.path.join(dst, os.path.basename(src))
     else:
         dir = os.path.dirname(dst)
 
     if os.path.isfile(dst):
-        logger.warning("Not updating %s (file already exists)", dst)
+        logger.debug("Not updating %s (file already exists)", dst)
         return (dst, 0)
     _copy_file_contents(src, dst)
     logger.debug("Copied %s to %s", src, dir)
     return (dst, 1)
 
 
 def safe_copy_tree(src, dst):
@@ -623,11 +623,12 @@
         if name.startswith("."):
             logger.debug("Not copying %s", src_name)
             continue
         if os.path.isdir(src_name):
             outputs.extend(safe_copy_tree(src_name, dst_name))
 
         else:
-            safe_copy_file(src_name, dst_name)
-            outputs.append(dst_name)
+            _, value = safe_copy_file(src_name, dst_name)
+            if value:
+                outputs.append(dst_name)
 
     return outputs
```

### Comparing `kapitan-0.31.1rc3/kapitan/validator/kubernetes_validator.py` & `kapitan-0.32.0rc0/kapitan/validator/kubernetes_validator.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.31.1rc3/pyproject.toml` & `kapitan-0.32.0rc0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -16,37 +16,36 @@
 readme = "README.md"
 keywords = ["jsonnet", "kubernetes", "reclass", "jinja"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 license = "Apache-2.0"
-version = "0.31.1rc3"
+version = "0.32.0rc0"
 packages = [
     { include = "kapitan" },
     { include = "kapitan/reclass" },
 ]
 
 [tool.poetry.scripts]
 kapitan = 'kapitan.cli:main'
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 addict = "^2.4.0"
 azure-keyvault-keys = "^4.7.0"
 boto3 = "^1.18.17"
-cryptography = "^3.4.7"
+cryptography = ">=3.4.7,<40.0.0"
 gitpython = "^3.1.30"
 google-api-python-client = "^2.15.0"
 hvac = "^0.11.0"
 jinja2 = "^3.0.1"
 jsonnet = "^0.18.0"
 jsonschema = "^4.17.3"
 kadet = "^0.2.2"
```

### Comparing `kapitan-0.31.1rc3/setup.py` & `kapitan-0.32.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 install_requires = \
 ['addict>=2.4.0,<3.0.0',
  'azure-identity>=1.12.0,<2.0.0',
  'azure-keyvault-keys>=4.7.0,<5.0.0',
  'boto3>=1.18.17,<2.0.0',
  'certifi',
- 'cryptography>=3.4.7,<4.0.0',
+ 'cryptography>=3.4.7,<40.0.0',
  'gitdb>=4.0.10,<5.0.0',
  'gitpython>=3.1.30,<4.0.0',
  'google-api-python-client>=2.15.0,<3.0.0',
  'hvac>=0.11.0,<0.12.0',
  'jinja2>=3.0.1,<4.0.0',
  'jsonnet>=0.18.0,<0.19.0',
  'jsonschema>=4.17.3,<5.0.0',
@@ -169,25 +169,25 @@
 {'gojsonnet': ['gojsonnet>=0.17.0,<0.18.0'], 'test': ['docker>=5.0.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['kapitan = kapitan.cli:main']}
 
 setup_kwargs = {
     'name': 'kapitan',
-    'version': '0.31.1rc3',
+    'version': '0.32.0rc0',
     'description': 'Generic templated configuration management for Kubernetes, Terraform and other things',
     'long_description': '# Kapitan: advanced configuration management tool\n\n![Unit Tests](https://github.com/kapicorp/kapitan/actions/workflows/test.yml/badge.svg)\n![Python Version](https://img.shields.io/pypi/pyversions/kapitan)\n![Downloads](https://img.shields.io/pypi/dm/kapitan)\n![Docker Pulls](https://img.shields.io/docker/pulls/kapicorp/kapitan)\n[![Docker](https://github.com/kapicorp/kapitan/workflows/Docker%20Build%20and%20Push/badge.svg)](https://github.com/kapicorp/kapitan/actions?query=workflow%3A%22Docker+Build+and+Push%22)\n[![Releases](https://img.shields.io/github/release/kapicorp/kapitan.svg)](https://github.com/kapicorp/kapitan/releases)\n[![Docker Image Size](https://img.shields.io/docker/image-size/kapicorp/kapitan/latest.svg)](https://hub.docker.com/r/kapicorp/kapitan)\n\n<img src="docs/images/kapitan_logo.png" width="25">\n\n\n**`Kapitan`** aims to be your *one-stop tool* to help you manage the ever growing complexity of your configurations.\n\nJoin the community [`#kapitan`](https://kubernetes.slack.com/archives/C981W2HD3)\n\n## [**Official site**](https://kapitan.dev) <https://kapitan.dev>\n\n\n## [**Quick Start**](https://kapitan.dev/kapitan_overview/#quickstart)\n\n## Install Kapitan\n\n### Docker (recommended)\n\n```shell\ndocker run -t --rm -v $(pwd):/src:delegated kapicorp/kapitan -h\n```\n\nOn Linux you can add `-u $(id -u)` to `docker run` to preserve file permissions.\n\n### Pip\n\nKapitan needs Python 3.7.\n\n#### Install Python 3.7\n\n* Linux: `sudo apt-get update && sudo apt-get install -y python3.7-dev python3-pip python3-yaml git`\n* Mac: `brew install python3 libyaml git libmagic`\n\n#### Install Kapitan\n\nUser (`$HOME/.local/lib/python3.7/bin` on Linux or `$HOME/Library/Python/3.7/bin` on macOS):\n\n```shell\npip3 install --user --upgrade kapitan\n```\n\nSystem-wide (not recommended):\n\n```shell\nsudo pip3 install --upgrade kapitan\n```\n\n## Build Kapitan\n\n### Docker\n\nTo build a docker image for the architecture of your machine, run `docker build . -t you-kapitan-image`, and to build for a specific platform, add `--platform linux/arm64`.\n\nTo build a multi-platform image (as the CI does), follow [the docker multi-platform documentation](https://docs.docker.com/build/building/multi-platform/).\n\n## Related projects\n\n* [Tesoro](https://github.com/kapicorp/tesoro) - Kubernetes Admission Controller for Kapitan Secrets\n* [Kapitan Reference](https://github.com/kapicorp/kapitan-reference) - our reference repository to get started with Kapitan\n',
     'author': 'Ricardo Amaro',
     'author_email': 'ramaro@kapicorp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kapicorp/kapitan',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `kapitan-0.31.1rc3/PKG-INFO` & `kapitan-0.32.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: kapitan
-Version: 0.31.1rc3
+Version: 0.32.0rc0
 Summary: Generic templated configuration management for Kubernetes, Terraform and other things
 Home-page: https://github.com/kapicorp/kapitan
 License: Apache-2.0
 Keywords: jsonnet,kubernetes,reclass,jinja
 Author: Ricardo Amaro
 Author-email: ramaro@kapicorp.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: gojsonnet
 Provides-Extra: test
 Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-keyvault-keys (>=4.7.0,<5.0.0)
 Requires-Dist: boto3 (>=1.18.17,<2.0.0)
 Requires-Dist: certifi
-Requires-Dist: cryptography (>=3.4.7,<4.0.0)
+Requires-Dist: cryptography (>=3.4.7,<40.0.0)
 Requires-Dist: docker (>=5.0.0,<6.0.0) ; extra == "test"
 Requires-Dist: gitdb (>=4.0.10,<5.0.0)
 Requires-Dist: gitpython (>=3.1.30,<4.0.0)
 Requires-Dist: gojsonnet (>=0.17.0,<0.18.0) ; extra == "gojsonnet"
 Requires-Dist: google-api-python-client (>=2.15.0,<3.0.0)
 Requires-Dist: hvac (>=0.11.0,<0.12.0)
 Requires-Dist: jinja2 (>=3.0.1,<4.0.0)
```

