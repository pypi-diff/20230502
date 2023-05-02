# Comparing `tmp/pop-create-idem-3.3.0.tar.gz` & `tmp/pop-create-idem-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-3.3.0.tar", last modified: Wed Apr 12 20:11:21 2023, max compression
+gzip compressed data, was "pop-create-idem-3.3.1.tar", last modified: Tue May  2 15:33:51 2023, max compression
```

## Comparing `pop-create-idem-3.3.0.tar` & `pop-create-idem-3.3.1.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8546 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     2533 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tool.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     5321 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3552 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2091 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      763 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2649 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     6081 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)    12534 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 20:11:20.000000 pop-create-idem-3.3.0/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4232 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.871142 pop-create-idem-3.3.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-02 15:33:51.871142 pop-create-idem-3.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.864141 pop-create-idem-3.3.1/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8546 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.864141 pop-create-idem-3.3.1/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.865141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.866141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.866141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.866141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.862141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.867141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.862141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.862141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.868142 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.869141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.869141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4931 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/schemas.py
+-rw-r--r--   0 root         (0) root         (0)    15090 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.869141 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.863141 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.870142 pop-create-idem-3.3.1/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:33:51.865141 pop-create-idem-3.3.1/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-02 15:33:51.000000 pop-create-idem-3.3.1/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 15:33:51.871142 pop-create-idem-3.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-02 15:33:33.000000 pop-create-idem-3.3.1/setup.py
```

### Comparing `pop-create-idem-3.3.0/LICENSE` & `pop-create-idem-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/PKG-INFO` & `pop-create-idem-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.3.0
+Version: 3.3.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.3.0/README.rst` & `pop-create-idem-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/cloudspec/__init__.py` & `pop-create-idem-3.3.1/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/cloudspec/conf.py` & `pop-create-idem-3.3.1/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/create/tool.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/init.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/function.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,23 @@
         function_data = functions.get(function_name)
         # This lets us create partial plugin
         if function_data:
             doc = hub.cloudspec.parse.function.doc(function_data)
             doc += hub.cloudspec.parse.param.sphinx_docs(function_data.params)
             doc += "\n\n    Returns:\n        Dict[str, Any]\n"
 
+            if "absent" == function_name and function_data.params:
+                # By idem's contract,
+                #   - all absent function parameters except 'name' should not be required
+                for param_name, metadata in function_data.params.items():
+                    if param_name.lower() != "name":
+                        metadata["required"] = False
+
             param_mapping = hub.cloudspec.parse.param.mappings(function_data.params)
+
             funcs[function_name] = dict(
                 function=dict(
                     name=function_name,
                     hardcoded=function_data.hardcoded,
                     doc=doc,
                     header_params=hub.cloudspec.parse.param.headers(
                         function_data.params
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/param.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,36 +100,57 @@
 
 
 def add_nested_param_to_header(member: Dict, offset: str) -> str:
     """
     Create a dataclass for a complex nested argument
     """
     ret = f'make_dataclass(\n{offset}"{member.name}",\n{offset}['
-    for param_name, param_data in member.get("params").items():
-        ret += f"\n{offset}    "
-        # TODO: Nested param name should be snaked
-        ret += f'("{param_name}", '
-        if param_data.member:
-            # Recursively add all nested complex arguments
-            ret += param_data.param_type.format(
-                add_nested_param_to_header(param_data.member, offset + "    ")
-            )
-        else:
-            ret += f"{param_data.param_type}"
-        if param_data["required"]:
-            ret += f"), "
-        else:
-            ret += f", field(default={param_data.default})), "
+    required_params = {
+        name: data for name, data in member.get("params").items() if data["required"]
+    }
+
+    for param_name, param_data in required_params.items():
+        ret += add_nested_param(param_name, param_data, offset)
+
+    unrequired_params = {
+        name: data
+        for name, data in member.get("params").items()
+        if not data["required"]
+    }
+
+    for param_name, param_data in unrequired_params.items():
+        ret += add_nested_param(param_name, param_data, offset)
+
     # Remove last ', '
     ret = ret[0:-2]
     ret += f"\n{offset}]\n{offset})"
 
     return ret
 
 
+def add_nested_param(param_name: str, param_data, offset: str):
+    ret = ""
+    ret += f"\n{offset}    "
+    # TODO: Nested param name should be snaked
+    ret += f'("{param_name}", '
+    if param_data.member:
+        # Recursively add all nested complex arguments
+        ret += param_data.param_type.format(
+            add_nested_param_to_header(param_data.member, offset + "    ")
+        )
+    else:
+        ret += f"{param_data.param_type}"
+    if param_data["required"]:
+        ret += f"), "
+    else:
+        ret += f", field(default={param_data.default})), "
+
+    return ret
+
+
 def callers(hub, parameters: CloudSpecParam) -> str:
     """
     Get a mapping of the function args to the values that will be used in the final caller
     """
     ret = []
 
     required_params = {
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 CREATE = """
-async def {{function.name}}(
-    hub,
-    ctx,
-    name: str
-    {% if function.header_params %}
-        {{function.header_params}}
-    {% endif -%},
-    **kwargs
-) -> Dict[str, Any]:
+async def {{function.name}}(hub, ctx{{function.header_params}}, name: str = None) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         Resource State:
 
@@ -26,21 +18,15 @@
         .. code-block:: bash
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 UPDATE = """
-async def {{function.name}}(
-    hub,
-    ctx,
-    name: str = None,
-    resource_id: str = None,
-    **kwargs
-) -> Dict[str, Any]:
+async def {{function.name}}(hub, ctx{{function.header_params}}, name: str = None, resource_id: str = None, **kwargs) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         Resource State:
 
@@ -56,21 +42,15 @@
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 
 DELETE = """
-async def {{function.name}}(
-    hub,
-    ctx,
-    name: str = None,
-    resource_id: str = None,
-    **kwargs
-) -> Dict[str, Any]:
+async def {{function.name}}(hub, ctx{{function.header_params}}, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         Resource State:
 
@@ -85,21 +65,15 @@
         .. code-block:: bash
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 GET = """
-async def {{function.name}}(
-    hub,
-    ctx,
-    name: str,
-    resource_id: str,
-    **kwargs
-) -> Dict[str, Any]:
+async def {{function.name}}(hub, ctx{{function.header_params}}, name: str = None, resource_id: str = None) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
 
     Examples:
 
         Unmanaged Resource State:
@@ -117,19 +91,15 @@
         .. code-block:: bash
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 LIST = """
-async def list_(
-    hub,
-    ctx,
-    **kwargs
-) -> Dict[str, Any]:
+async def list_(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         Unmanaged Resource State:
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-3.3.1/pop_create_idem/cloudspec/template/state.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 Templates for state modules
 """
 
 PRESENT_FUNCTION = """
 async def {{function.name}}(
     hub,
     ctx,
-    name: str,
-    resource_id: str= None,
+    name: str
+    {% if function.header_params %}
+        {{function.header_params}}
+    {% endif -%},
+    resource_id: str = None,
     **kwargs
 ) -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
@@ -23,15 +26,18 @@
     '''
 """
 
 ABSENT_FUNCTION = """
 async def {{function.name}}(
     hub,
     ctx,
-    name: str = None,
+    name: str
+    {% if function.header_params %}
+        {{function.header_params}}
+    {% endif -%},
     resource_id: str = None,
     **kwargs
 )  -> Dict[str, Any]:
     r'''
     **Autogenerated function**
     {{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/conf.py` & `pop-create-idem-3.3.1/pop_create_idem/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         "nargs": "+",
         "subcommands": ["openapi3", "swagger", "idem-cloud"],
         "dyne": "pop_create",
     },
 }
 CONFIG = {
     "create_plugin": {
-        "default": "auto_states",
+        "default": "state_modules",
         "dyne": "pop_create",
-        "help": "The `create` plugin to use for resource modules",
+        "help": "The `create` plugin to use for resource modules. The other options are 'auto_states', 'exec_modules'.",
     },
     "acct_plugin": {
         "default": None,
         "help": "The acct plugin to use for authentication -- default is to create a new plugin",
         "dyne": "pop_create",
     },
     "simple_service_name": {
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any
 from typing import Dict
 
 import openapi3.object_base
 import tqdm
 
-__func_alias__ = {"type_": "type"}
-
 
 def plugins(hub, ctx, api: openapi3.OpenAPI) -> Dict[str, Any]:
     ret = {}
     paths: openapi3.object_base.Map = api.paths
+
+    all_schemas = hub.pop_create.openapi3.schemas.parse(api)
+
     for name, path in tqdm.tqdm(paths.items(), desc="Parsing paths"):
         if not isinstance(path, openapi3.paths.Path):
             # Let's not fail but continue to other paths instead
             hub.log.warning(
                 f"The {name} is not an instance of Path. It will not be parsed."
             )
             continue
@@ -53,14 +54,18 @@
                 # This is the first time we have looked at this plugin
                 ret[ref] = {
                     "functions": {},
                     "doc": "",
                     "imports": [
                         "from typing import Any",
                         "from typing import Dict",
+                        "from typing import List",
+                        "from collections import OrderedDict",
+                        "from dataclasses import field",
+                        "from dataclasses import make_dataclass",
                         "import dict_tools.differ as differ",
                     ],
                 }
 
             # See if this function will be reserved CRUD operations, if so change the name
             reserved_func_name = (
                 hub.pop_create.openapi3.parse.resolve_reserved_function_name(
@@ -73,100 +78,59 @@
                 hub.pop_create.openapi3.parse.resolve_function_name(
                     name, plugin, request_type, func
                 )
                 if not reserved_func_name
                 else reserved_func_name
             )
 
-            func_data = hub.pop_create.openapi3.parse.function(func, api)
-            func_data["hardcoded"] = {
-                "method": request_type,
-                "path": name.split(" ")[0],
-                "service_name": ctx.service_name,
-                "resource_name": plugin,
-            }
-            ret[ref]["functions"][func_name] = func_data
+            try:
+                ret[ref]["functions"][
+                    func_name
+                ] = hub.pop_create.openapi3.function.parse(
+                    ctx,
+                    request_type,
+                    name,
+                    plugin,
+                    func,
+                    all_schemas,
+                )
+            except Exception as e:
+                hub.log.debug(
+                    f"Failed to parse function data for {plugin}: {request_type} '{name}': {e.__class__.__name__}: {e}"
+                )
 
     return ret
 
 
-def function(
-    hub,
-    func: openapi3.paths.Operation,
-    api: openapi3.OpenAPI,
-) -> Dict[str, Any]:
-
-    params = {}
-    for p in func.parameters:
-        # TODO: openapi3.general.Reference is unsupported at the moment
-        if isinstance(p, openapi3.paths.Parameter):
-            params[p.name] = hub.pop_create.openapi3.parse.parameter(p)
-
-    deprecated_text = "\nDEPRECATED" if func.deprecated else ""
-
-    return {
-        "doc": f"{func.summary}\n    {func.description}    {deprecated_text}".strip(),
-        "params": params,
-    }
-
-
-def parameter(hub, parameter: openapi3.paths.Parameter):
-    if parameter.in_ == "query":
-        target_type = "mapping"
-    elif parameter.in_ == "path":
-        target_type = "mapping"
-    elif parameter.in_ == "header":
-        target_type = "mapping"
-    elif parameter.in_ == "cookie":
-        target_type = "mapping"
-    else:
-        raise ValueError(f"Unknown parameter type: {parameter.in_}")
-
-    return {
-        "required": parameter.required,
-        "target_type": target_type,
-        "target": parameter.in_,
-        "param_type": hub.pop_create.openapi3.parse.type(
-            parameter.schema.type
-            if isinstance(parameter.schema, openapi3.schemas.Schema)
-            else None
-        ),
-        "doc": parameter.description or parameter.name,
-    }
-
-
-def type_(hub, param_type: str) -> str:
-    if "integer" == param_type:
-        return "int"
-    elif "boolean" == param_type:
-        return "bool"
-    elif "number" == param_type:
-        return "float"
-    elif "string" == param_type:
-        return "str"
-    elif "array" == param_type:
-        return "list"
-    else:
-        return ""
-
-
 def resolve_reserved_function_name(
     hub, name: str, plugin: str, request_type: str, func: openapi3.paths.Operation
 ):
     # Do not make deprecated API paths into CRUDs and throw them into tools/*
+    possible_resource_names = tuple(
+        [
+            # e.g. /store_order, /store-order, /store_orders, /store-orders
+            plugin,
+            plugin.replace("_", "-"),
+            f"{plugin}s",
+            f"{plugin.replace('_', '-')}s",
+        ]
+    )
     if not func.deprecated:
         # e.g. plugin: pets, path: /pets
-        if name.endswith(plugin):
+        if name.endswith(possible_resource_names):
             # list/post
             if request_type == "get":
                 return "list"
             elif request_type == "post":
                 return "create"
+            elif request_type == "put":
+                # PUT /pets
+                return "update"
         # e.g.: plugin: pets, path: /pets/{id}
-        elif name.rsplit("/", 1)[0].endswith(plugin):
+        elif name.rsplit("/", 1)[0].endswith(possible_resource_names):
             # get/list/put
             if request_type == "get":
                 return "get"
             elif request_type == "put" or request_type == "patch":
                 return "update"
             elif request_type == "delete":
                 return "delete"
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/template.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/template.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,17 +26,38 @@
     # Case: Empty results
     if not get["ret"]:
         result["comment"].append(
             f"Get '{name}' result is empty"
         )
         return result
 
+    {% if function.hardcoded.response_mappings %}
+    # Convert raw response into present format
+    raw_resource = get["ret"]
+
+    # TODO: Make sure resource_id is mapped in get response
+    resource_in_present_format = {
+        "name": name,
+        "resource_id": resource_id
+    }
+    resource_parameters = OrderedDict(
+    {{ function.hardcoded.response_mappings|pprint|indent(12,true) }}
+    )
+
+    for parameter_raw, parameter_present in resource_parameters.items():
+        if parameter_raw in raw_resource and raw_resource.get(parameter_raw):
+            resource_in_present_format[parameter_present] = raw_resource.get(parameter_raw)
+
+    result["ret"] = resource_in_present_format
+    {% else %}
     # TODO: Make sure resource_id is mapped in get response
     get["ret"]["resource_id"] = resource_id
     result["ret"] = get["ret"]
+    {% endif %}
+
     return result
 """
 
 LIST_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
     # TODO: Change function methods params if needed
@@ -51,71 +72,95 @@
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
 
     for resource in list["ret"]:
+        {% if function.hardcoded.response_mappings %}
+        # Convert raw response into present format
+        resource_in_present_format = {
+            # TODO: Make sure name, resource_id is mapped accordingly
+            "name": "name",
+            "resource_id": "resource_id"
+        }
+        resource_parameters = OrderedDict(
+        {{ function.hardcoded.response_mappings|pprint|indent(16,true) }}
+        )
+
+        for parameter_raw, parameter_present in resource_parameters.items():
+            if parameter_raw in resource and resource.get(parameter_raw):
+                resource_in_present_format[parameter_present] = resource.get(parameter_raw)
+
+        result["ret"].append(resource_in_present_format)
+        {% else %}
         # TODO: Map resource_id from response
         resource["resource_id"] = ""
         result["ret"].append(resource)
+        {% endif %}
     return result
 """
 
 CREATE_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
-    # TODO: Change function methods params if needed.
+    # TODO: Change request param mapping as necessary
+    payload = {{ function.hardcoded.request_mappings|default("{}", true) }}
+
     create = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}",
         query_params={{ parameter.mapping.query|default({}) }},
-        data={},
+        data=payload,
         headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
     result["comment"].append(f"Created {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} '{name}'",)
 
     result["ret"] = create["ret"]
+    # TODO: add "resource_id" to returned response by mapping to correct resource identifier
     return result
 """
 
 UPDATE_REQUEST_FORMAT = """
     result = dict(comment=[], ret=[], result=True)
 
-    desired_state = {"name": name, "resource_id": resource_id, **kwargs}
+    desired_state = {
+        k: v
+        for k, v in locals().items()
+        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+    }
 
-    resource_to_raw_input_mapping = OrderedDict(
-    **{{ parameter.mapping.path|default({})|pprint|indent(12,true) }}
-    )
+    # TODO: Change request param mapping as necessary
+    resource_to_raw_input_mapping = {{ function.hardcoded.request_mappings|default("{}", true) }}
 
-    parameters_to_update = {}
+    payload = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
-            parameters_to_update[resource_to_raw_input_mapping[key]] = desired_state.get(key)
+            payload[resource_to_raw_input_mapping[key]] = desired_state.get(key)
 
-    if parameters_to_update:
+    if payload:
         update = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
             ctx,
             method="{{ function.hardcoded.method }}",
             path="{{ function.hardcoded.path }}".format(
                 **{{ parameter.mapping.path|default({}) }}
             ),
             query_params={{ parameter.mapping.query|default({}) }},
-            data={},
+            data=payload,
             headers={{ parameter.mapping.header|default({}) }},
         )
 
-        if not create["result"]:
+        if not update["result"]:
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
         result["ret"] = update["ret"]
         result["comment"].append(f"Updated {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }} '{name}'",)
 
@@ -144,40 +189,64 @@
     result["comment"].append(f"Deleted '{name}'")
     return result
 """
 
 OTHER_FUNCTION_REQUEST_FORMAT = """
     result = dict(comment=[], ret=None, result=True)
 
+    # TODO: Change request param mapping as necessary
+    payload = {{ function.hardcoded.request_mappings|default("{}", true) }}
+
     ret = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
-        data={},
+        data=payload,
         headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not ret["result"]:
         result["comment"].append(ret["comment"])
         result["result"] = False
         return result
 
-    result["ret"] = ret
+    {% if function.hardcoded.response_mappings %}
+    # Convert raw response into present format
+    raw_resource = ret["ret"]
+
+    resource_in_present_format = {}
+    resource_parameters = OrderedDict(
+    {{ function.hardcoded.response_mappings|pprint|indent(12,true) }}
+    )
+
+    for parameter_raw, parameter_present in resource_parameters.items():
+        if parameter_raw in raw_resource and raw_resource.get(parameter_raw):
+            resource_in_present_format[parameter_present] = raw_resource.get(parameter_raw)
+
+    result["ret"] = resource_in_present_format
+    {% else %}
+    result["ret"] = ret["ret"]
+    {% endif %}
+
     return result
 """
 
 PRESENT_REQUEST_FORMAT = """
     result = dict(
         comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
     )
 
-    desired_state = {"name": name, "resource_id": resource_id, **kwargs}
+    desired_state = {
+        k: v
+        for k, v in locals().items()
+        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+    }
 
     if resource_id:
         # Possible parameters: **{{ parameter.mapping.kwargs|default({}) }}
         before = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.get(
             ctx,
             name=name,
             resource_id=resource_id,
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-3.3.1/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/tool/format/case.py` & `pop-create-idem-3.3.1/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-3.3.1/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem/tool/gradle.py` & `pop-create-idem-3.3.1/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.3.0/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-3.3.1/pop_create_idem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.3.0
+Version: 3.3.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.3.0/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-3.3.1/pop_create_idem.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,19 @@
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
 pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+pop_create_idem/pop_create/openapi3/function.py
 pop_create_idem/pop_create/openapi3/init.py
+pop_create_idem/pop_create/openapi3/params.py
 pop_create_idem/pop_create/openapi3/parse.py
+pop_create_idem/pop_create/openapi3/schemas.py
 pop_create_idem/pop_create/openapi3/template.py
 pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
 pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
 pop_create_idem/pop_create/rest/init.py
 pop_create_idem/pop_create/swagger/init.py
```

### Comparing `pop-create-idem-3.3.0/setup.py` & `pop-create-idem-3.3.1/setup.py`

 * *Files identical despite different names*

