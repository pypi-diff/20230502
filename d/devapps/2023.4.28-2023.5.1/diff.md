# Comparing `tmp/devapps-2023.4.28.tar.gz` & `tmp/devapps-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devapps-2023.4.28.tar", max compression
+gzip compressed data, was "devapps-2023.5.1.tar", max compression
```

## Comparing `devapps-2023.4.28.tar` & `devapps-2023.5.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.4.28/LICENSE
--rw-r--r--   0        0        0      992 2023-04-30 11:20:29.929892 devapps-2023.4.28/README.md
--rw-r--r--   0        0        0     5914 2023-04-30 11:20:08.175879 devapps-2023.4.28/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.4.28/src/ax/utils/__init__.py
--rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.4.28/src/ax/utils/ax_tree/__init__.py
--rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.4.28/src/ax/utils/ax_tree/_ax_tree.so
--rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.4.28/src/ax/utils/ax_tree/ax_tree.py
--rwxr-xr-x   0        0        0      491 2023-03-22 14:28:26.989865 devapps-2023.4.28/src/devapp/__init__.py
--rwxr-xr-x   0        0        0    19340 2023-04-29 11:40:41.300849 devapps-2023.4.28/src/devapp/app.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:28:26.990865 devapps-2023.4.28/src/devapp/app_token/__init__.py
--rwxr-xr-x   0        0        0     1201 2023-03-22 14:28:26.990865 devapps-2023.4.28/src/devapp/app_token/create_tokens.py
--rwxr-xr-x   0        0        0     2230 2023-03-22 14:28:26.990865 devapps-2023.4.28/src/devapp/app_token/read_tokens.py
--rwxr-xr-x   0        0        0      151 2023-03-22 14:28:26.990865 devapps-2023.4.28/src/devapp/app_token/verify_token
--rwxr-xr-x   0        0        0      297 2023-03-22 14:28:26.990865 devapps-2023.4.28/src/devapp/components/__init__.py
--rwxr-xr-x   0        0        0     6980 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/components/cloudfoundry.py
--rwxr-xr-x   0        0        0     5956 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/components/gitlab.py
--rwxr-xr-x   0        0        0     4828 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/components/gitlab_runner.py
--rwxr-xr-x   0        0        0      150 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/da.py
--rwxr-xr-x   0        0        0     1321 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/dev_mode.py
--rwxr-xr-x   0        0        0     1636 2023-04-30 10:26:20.741214 devapps-2023.4.28/src/devapp/gevent_patched.py
--rwxr-xr-x   0        0        0     1549 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/layer.py
--rwxr-xr-x   0        0        0      188 2023-03-22 14:28:26.991865 devapps-2023.4.28/src/devapp/lib/README.md
--rwxr-xr-x   0        0        0        0 2023-03-22 14:28:26.992865 devapps-2023.4.28/src/devapp/lib/__init__.py
--rwxr-xr-x   0        0        0   123141 2023-03-22 14:28:26.992865 devapps-2023.4.28/src/devapp/lib/sh.py
--rwxr-xr-x   0        0        0     2343 2023-03-22 14:28:26.992865 devapps-2023.4.28/src/devapp/load.py
--rwxr-xr-x   0        0        0      655 2023-03-22 14:28:26.993865 devapps-2023.4.28/src/devapp/logo
--rwxr-xr-x   0        0        0     1671 2023-03-22 14:28:26.993865 devapps-2023.4.28/src/devapp/max.py
--rw-r--r--   0        0        0     1752 2023-03-22 14:28:26.993865 devapps-2023.4.28/src/devapp/operations/resources.py
--rwxr-xr-x   0        0        0     1551 2023-03-22 14:28:26.993865 devapps-2023.4.28/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
--rwxr-xr-x   0        0        0     6445 2023-03-22 14:28:26.993865 devapps-2023.4.28/src/devapp/plugins/dev_devapp/repo_sym_links.py
--rw-r--r--   0        0        0     3090 2023-03-22 14:28:26.994865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resource_install.py
--rw-r--r--   0        0        0     4577 2023-03-22 14:28:26.994865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resource_run.py
--rw-r--r--   0        0        0     8983 2023-03-22 14:28:26.994865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resources.py.dis
--rw-r--r--   0        0        0      671 2023-03-22 14:28:26.994865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resources_list.py
--rw-r--r--   0        0        0      879 2023-03-22 14:28:26.994865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
--rwxr-xr-x   0        0        0     8688 2023-03-22 14:28:26.995865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/container_build.py
--rwxr-xr-x   0        0        0    10257 2023-03-22 14:28:26.995865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/container_pull.py
--rwxr-xr-x   0        0        0    28013 2023-03-22 14:28:26.995865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/fs_build.py
--rwxr-xr-x   0        0        0    13318 2023-03-22 14:28:26.995865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
--rwxr-xr-x   0        0        0     9232 2023-03-22 14:28:26.996865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
--rwxr-xr-x   0        0        0    12668 2023-03-22 14:28:26.996865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
--rwxr-xr-x   0        0        0     8750 2023-03-22 14:28:26.996865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/kubectl/__init__.py
--rwxr-xr-x   0        0        0     2975 2023-03-22 14:28:26.996865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/life_cycle.py
--rw-r--r--   0        0        0     1573 2023-03-22 14:28:26.996865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/log_view.py
--rwxr-xr-x   0        0        0    11484 2023-03-22 14:28:26.996865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/project/__init__.py
--rw-r--r--   0        0        0     9960 2023-03-22 14:28:26.997865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
--rw-r--r--   0        0        0     4994 2023-03-22 14:28:26.997865 devapps-2023.4.28/src/devapp/plugins/ops_devapp/run.py
--rwxr-xr-x   0        0        0    28235 2023-03-22 14:28:26.997865 devapps-2023.4.28/src/devapp/run.py
--rwxr-xr-x   0        0        0    25984 2023-03-22 14:28:26.997865 devapps-2023.4.28/src/devapp/spec/build.py
--rwxr-xr-x   0        0        0     2929 2023-03-22 14:28:26.997865 devapps-2023.4.28/src/devapp/spec/find_paths_in_fs_components.py
--rwxr-xr-x   0        0        0    16176 2023-03-22 14:28:26.998865 devapps-2023.4.28/src/devapp/spec/fs_components.py
--rwxr-xr-x   0        0        0     1715 2023-03-22 14:28:26.998865 devapps-2023.4.28/src/devapp/spec/links.py
--rwxr-xr-x   0        0        0     2481 2023-03-22 14:28:26.998865 devapps-2023.4.28/src/devapp/spec/os_tools.py
--rwxr-xr-x   0        0        0     7913 2023-03-22 14:28:26.998865 devapps-2023.4.28/src/devapp/spec/templ.py
--rwxr-xr-x   0        0        0     1600 2023-03-22 14:28:26.998865 devapps-2023.4.28/src/devapp/spec/templates/unit
--rwxr-xr-x   0        0        0     7586 2023-03-22 14:28:26.998865 devapps-2023.4.28/src/devapp/spec/tools.py
--rwxr-xr-x   0        0        0    30671 2023-03-22 14:28:26.999865 devapps-2023.4.28/src/devapp/t
--rw-r--r--   0        0        0     3559 2023-03-22 14:28:26.999865 devapps-2023.4.28/src/devapp/testing/auto_docs.py
--rw-r--r--   0        0        0      443 2023-03-22 14:28:26.999865 devapps-2023.4.28/src/devapp/tests/test_unit_devapp.py
--rwxr-xr-x   0        0        0    13808 2023-03-22 14:28:26.999865 devapps-2023.4.28/src/devapp/third/rpl
--rwxr-xr-x   0        0        0    49708 2023-03-22 14:28:27.000865 devapps-2023.4.28/src/devapp/tools/__init__.py
--rw-r--r--   0        0        0     4025 2023-03-22 14:28:27.000865 devapps-2023.4.28/src/devapp/tools/flag.py
--rw-r--r--   0        0        0      731 2023-03-22 14:28:27.000865 devapps-2023.4.28/src/devapp/tools/http.py
--rw-r--r--   0        0        0    35701 2023-03-22 14:28:27.000865 devapps-2023.4.28/src/devapp/tools/infra/__init__.py
--rw-r--r--   0        0        0    16618 2023-03-22 14:28:27.001865 devapps-2023.4.28/src/devapp/tools/infra/actions.py
--rw-r--r--   0        0        0     3089 2023-03-22 14:28:27.001865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/000:functions.sh
--rwxr-xr-x   0        0        0      375 2023-03-22 14:28:27.001865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
--rwxr-xr-x   0        0        0     1521 2023-03-22 14:28:27.001865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
--rwxr-xr-x   0        0        0      448 2023-03-22 14:28:27.002865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/100:docker.sh
--rwxr-xr-x   0        0        0      324 2023-03-22 14:28:27.002865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/200:tools.sh
--rwxr-xr-x   0        0        0      760 2023-03-22 14:28:27.002865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/300:dns.sh
--rwxr-xr-x   0        0        0     4375 2023-03-22 14:28:27.002865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/500:k3s.sh
--rwxr-xr-x   0        0        0      943 2023-03-22 14:28:27.002865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/501:kind.sh
--rwxr-xr-x   0        0        0    17210 2023-03-22 14:28:27.003865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/502:k3s.sh
--rw-r--r--   0        0        0      276 2023-03-22 14:28:27.003865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/510:label_workers.sh
--rwxr-xr-x   0        0        0      661 2023-03-22 14:28:27.003865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/600:longhorn.sh
--rw-r--r--   0        0        0     1737 2023-03-22 14:28:27.003865 devapps-2023.4.28/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
--rw-r--r--   0        0        0     4339 2023-03-22 14:28:27.003865 devapps-2023.4.28/src/devapp/tools/plugin.py
--rw-r--r--   0        0        0    25735 2023-03-23 18:46:53.865877 devapps-2023.4.28/src/devapp/tools/resource.py
--rw-r--r--   0        0        0     1861 2023-03-22 14:28:27.004865 devapps-2023.4.28/src/devapp/tools/times.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:28:27.004865 devapps-2023.4.28/src/devapp/utils/__init__.py
--rwxr-xr-x   0        0        0    15787 2023-03-22 14:28:27.004865 devapps-2023.4.28/src/devapp/utils/os_.py
--rwxr-xr-x   0        0        0     1871 2023-03-22 14:28:27.004865 devapps-2023.4.28/src/devapp/utils/py_source_env.py
--rwxr-xr-x   0        0        0     9335 2023-03-22 14:28:27.004865 devapps-2023.4.28/src/devapp/utils/rx_tools.py
--rwxr-xr-x   0        0        0    11529 2023-03-22 14:28:27.004865 devapps-2023.4.28/src/devapp/utils/vault.py
--rwxr-xr-x   0        0        0     1671 2023-03-22 14:28:27.005865 devapps-2023.4.28/src/devapp/utils/watch_dog.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.4.28/src/mdvl/__init__.py
--rwxr-xr-x   0        0        0    20381 2023-03-22 14:30:25.734938 devapps-2023.4.28/src/mdvl/mdvl.py
--rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.4.28/src/mdvl/tools.py
--rwxr-xr-x   0        0        0      519 2023-03-22 14:30:25.735939 devapps-2023.4.28/src/structlogging/__init__.py
--rwxr-xr-x   0        0        0     1559 2023-03-22 14:30:25.735939 devapps-2023.4.28/src/structlogging/adapters.py
--rwxr-xr-x   0        0        0       88 2023-03-22 14:30:25.735939 devapps-2023.4.28/src/structlogging/common.py
--rwxr-xr-x   0        0        0     5503 2023-03-22 14:30:25.735939 devapps-2023.4.28/src/structlogging/config.py
--rwxr-xr-x   0        0        0     1618 2023-03-22 14:30:25.735939 devapps-2023.4.28/src/structlogging/formatters.py
--rwxr-xr-x   0        0        0     2640 2023-03-22 14:30:25.736939 devapps-2023.4.28/src/structlogging/processors.py
--rwxr-xr-x   0        0        0     5472 2023-03-22 14:30:25.736939 devapps-2023.4.28/src/structlogging/renderers.py
--rwxr-xr-x   0        0        0    11172 2023-04-30 08:25:53.603088 devapps-2023.4.28/src/structlogging/sl.py
--rw-r--r--   0        0        0     4022 2023-03-22 14:30:25.736939 devapps-2023.4.28/src/structlogging/stacktrace.py
--rwxr-xr-x   0        0        0     1355 2023-03-22 14:30:25.736939 devapps-2023.4.28/src/structlogging/tests/test_structlogging.py
--rwxr-xr-x   0        0        0      886 2023-03-22 14:30:25.736939 devapps-2023.4.28/src/theming/__init__.py
--rwxr-xr-x   0        0        0    14552 2023-03-22 14:30:25.737939 devapps-2023.4.28/src/theming/absl_color_help.py
--rwxr-xr-x   0        0        0     4345 2023-03-22 14:30:25.737939 devapps-2023.4.28/src/theming/ansi2html.py
--rwxr-xr-x   0        0        0    11888 2023-03-22 14:30:25.737939 devapps-2023.4.28/src/theming/ansi2html.sh
--rwxr-xr-x   0        0        0     3030 2023-03-22 14:30:25.737939 devapps-2023.4.28/src/theming/ansistrm.py
--rwxr-xr-x   0        0        0    10066 2023-03-22 14:30:25.737939 devapps-2023.4.28/src/theming/ax_xml.py
--rwxr-xr-x   0        0        0    10495 2023-03-22 14:30:25.738939 devapps-2023.4.28/src/theming/camel_snake.py
--rwxr-xr-x   0        0        0     7517 2023-03-22 14:30:25.738939 devapps-2023.4.28/src/theming/charting.py
--rwxr-xr-x   0        0        0     3392 2023-03-22 14:30:25.738939 devapps-2023.4.28/src/theming/colorhilite.py
--rwxr-xr-x   0        0        0     1113 2023-03-22 14:30:25.738939 devapps-2023.4.28/src/theming/filesize/README.txt
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.738939 devapps-2023.4.28/src/theming/filesize/__init__.py
--rwxr-xr-x   0        0        0     2549 2023-03-22 14:30:25.738939 devapps-2023.4.28/src/theming/filesize/filesize.py
--rwxr-xr-x   0        0        0     3756 2023-03-22 14:30:25.739939 devapps-2023.4.28/src/theming/formatters.py
--rw-r--r--   0        0        0     3807 2023-03-22 14:30:25.739939 devapps-2023.4.28/src/theming/formatting/markdown.py
--rw-r--r--   0        0        0     1241 2023-03-22 14:30:25.739939 devapps-2023.4.28/src/theming/formatting/viz_sequence.py
--rwxr-xr-x   0        0        0     3410 2023-03-22 14:30:25.739939 devapps-2023.4.28/src/theming/html_tools.py
--rwxr-xr-x   0        0        0    11409 2023-03-22 14:30:25.739939 devapps-2023.4.28/src/theming/inflect.py
--rwxr-xr-x   0        0        0      460 2023-03-22 14:30:25.739939 devapps-2023.4.28/src/theming/msgs.py
--rwxr-xr-x   0        0        0     9864 2023-03-22 14:30:25.740939 devapps-2023.4.28/src/theming/pretty_print.py
--rwxr-xr-x   0        0        0    55699 2023-03-22 14:30:25.740939 devapps-2023.4.28/src/theming/tablepretty.py
--rwxr-xr-x   0        0        0    13998 2023-03-22 14:30:25.740939 devapps-2023.4.28/src/theming/term.py
--rwxr-xr-x   0        0        0     1468 2023-03-22 14:30:25.740939 devapps-2023.4.28/src/theming/term_struct_hilite.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.740939 devapps-2023.4.28/src/theming/test
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.741938 devapps-2023.4.28/src/theming/tests/__init__.py
--rwxr-xr-x   0        0        0     9454 2023-03-22 14:30:25.741938 devapps-2023.4.28/src/theming/tests/test_text_formatting.py
--rwxr-xr-x   0        0        0     1063 2023-03-22 14:30:25.741938 devapps-2023.4.28/src/theming/tracebacks.py
--rwxr-xr-x   0        0        0     3011 2023-03-22 14:30:25.741938 devapps-2023.4.28/src/theming/unicode_chars.py
--rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.4.28/src/tree_builder/__init__.py
--rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.4.28/src/tree_builder/arch/__init__.py.bak
--rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.4.28/src/tree_builder/arch/links.py.bak
--rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.4.28/src/tree_builder/arch/o.py
--rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/arch/old
--rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/arch/olinit
--rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/arch/oo
--rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/arch/py2.py
--rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/arch/render.py.bak
--rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/chrome_reload.sh
--rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.4.28/src/tree_builder/delivery2.py
--rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.4.28/src/tree_builder/links.py
--rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.4.28/src/tree_builder/py3.py
--rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.4.28/src/tree_builder/render.py
--rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.4.28/src/tree_builder/version.py
--rw-r--r--   0        0        0     3038 2023-04-30 11:20:36.643986 devapps-2023.4.28/setup.py
--rw-r--r--   0        0        0     1805 2023-04-30 11:20:36.644773 devapps-2023.4.28/PKG-INFO
+-rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.5.1/LICENSE
+-rw-r--r--   0        0        0      992 2023-05-02 12:46:04.185957 devapps-2023.5.1/README.md
+-rw-r--r--   0        0        0     5914 2023-05-02 12:45:48.609953 devapps-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.5.1/src/ax/utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.5.1/src/ax/utils/ax_tree/__init__.py
+-rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.5.1/src/ax/utils/ax_tree/_ax_tree.so
+-rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.5.1/src/ax/utils/ax_tree/ax_tree.py
+-rwxr-xr-x   0        0        0      491 2023-03-22 14:28:26.989865 devapps-2023.5.1/src/devapp/__init__.py
+-rwxr-xr-x   0        0        0    19220 2023-05-02 12:43:21.727927 devapps-2023.5.1/src/devapp/app.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/__init__.py
+-rwxr-xr-x   0        0        0     1201 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/create_tokens.py
+-rwxr-xr-x   0        0        0     2230 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/read_tokens.py
+-rwxr-xr-x   0        0        0      151 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/verify_token
+-rwxr-xr-x   0        0        0      297 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/components/__init__.py
+-rwxr-xr-x   0        0        0     6980 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/components/cloudfoundry.py
+-rwxr-xr-x   0        0        0     5956 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/components/gitlab.py
+-rwxr-xr-x   0        0        0     4828 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/components/gitlab_runner.py
+-rwxr-xr-x   0        0        0      150 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/da.py
+-rwxr-xr-x   0        0        0     1321 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/dev_mode.py
+-rwxr-xr-x   0        0        0     1636 2023-04-30 10:26:20.741214 devapps-2023.5.1/src/devapp/gevent_patched.py
+-rwxr-xr-x   0        0        0     1549 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/layer.py
+-rwxr-xr-x   0        0        0      188 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/lib/README.md
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:28:26.992865 devapps-2023.5.1/src/devapp/lib/__init__.py
+-rwxr-xr-x   0        0        0   123141 2023-03-22 14:28:26.992865 devapps-2023.5.1/src/devapp/lib/sh.py
+-rwxr-xr-x   0        0        0     2343 2023-03-22 14:28:26.992865 devapps-2023.5.1/src/devapp/load.py
+-rwxr-xr-x   0        0        0      655 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/logo
+-rwxr-xr-x   0        0        0     1671 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/max.py
+-rw-r--r--   0        0        0     1752 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/operations/resources.py
+-rwxr-xr-x   0        0        0     1551 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     6445 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/plugins/dev_devapp/repo_sym_links.py
+-rw-r--r--   0        0        0     3090 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_install.py
+-rw-r--r--   0        0        0     4577 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_run.py
+-rw-r--r--   0        0        0     8983 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources.py.dis
+-rw-r--r--   0        0        0      671 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources_list.py
+-rw-r--r--   0        0        0      879 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
+-rwxr-xr-x   0        0        0     8688 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_build.py
+-rwxr-xr-x   0        0        0    10257 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_pull.py
+-rwxr-xr-x   0        0        0    28013 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/fs_build.py
+-rwxr-xr-x   0        0        0    13318 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
+-rwxr-xr-x   0        0        0     9232 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
+-rwxr-xr-x   0        0        0    12668 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
+-rwxr-xr-x   0        0        0     8750 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/kubectl/__init__.py
+-rwxr-xr-x   0        0        0     2975 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/life_cycle.py
+-rw-r--r--   0        0        0     1573 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/log_view.py
+-rwxr-xr-x   0        0        0    11484 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/__init__.py
+-rw-r--r--   0        0        0     9960 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
+-rw-r--r--   0        0        0     4994 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/run.py
+-rwxr-xr-x   0        0        0    28235 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/run.py
+-rwxr-xr-x   0        0        0    25984 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/spec/build.py
+-rwxr-xr-x   0        0        0     2929 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/spec/find_paths_in_fs_components.py
+-rwxr-xr-x   0        0        0    16176 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/fs_components.py
+-rwxr-xr-x   0        0        0     1715 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/links.py
+-rwxr-xr-x   0        0        0     2481 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/os_tools.py
+-rwxr-xr-x   0        0        0     7913 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/templ.py
+-rwxr-xr-x   0        0        0     1600 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/templates/unit
+-rwxr-xr-x   0        0        0     7586 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/tools.py
+-rwxr-xr-x   0        0        0    30671 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/t
+-rw-r--r--   0        0        0     3559 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/testing/auto_docs.py
+-rw-r--r--   0        0        0      443 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/tests/test_unit_devapp.py
+-rwxr-xr-x   0        0        0    13808 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/third/rpl
+-rwxr-xr-x   0        0        0    50010 2023-05-02 12:16:52.557397 devapps-2023.5.1/src/devapp/tools/__init__.py
+-rw-r--r--   0        0        0     4025 2023-03-22 14:28:27.000865 devapps-2023.5.1/src/devapp/tools/flag.py
+-rw-r--r--   0        0        0      731 2023-03-22 14:28:27.000865 devapps-2023.5.1/src/devapp/tools/http.py
+-rw-r--r--   0        0        0    35701 2023-03-22 14:28:27.000865 devapps-2023.5.1/src/devapp/tools/infra/__init__.py
+-rw-r--r--   0        0        0    16618 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/actions.py
+-rw-r--r--   0        0        0     3089 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/000:functions.sh
+-rwxr-xr-x   0        0        0      375 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
+-rwxr-xr-x   0        0        0     1521 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
+-rwxr-xr-x   0        0        0      448 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/100:docker.sh
+-rwxr-xr-x   0        0        0      324 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/200:tools.sh
+-rwxr-xr-x   0        0        0      760 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/300:dns.sh
+-rwxr-xr-x   0        0        0     4375 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/500:k3s.sh
+-rwxr-xr-x   0        0        0      943 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/501:kind.sh
+-rwxr-xr-x   0        0        0    17210 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/502:k3s.sh
+-rw-r--r--   0        0        0      276 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/510:label_workers.sh
+-rwxr-xr-x   0        0        0      661 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/600:longhorn.sh
+-rw-r--r--   0        0        0     1737 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
+-rw-r--r--   0        0        0     4408 2023-05-02 12:43:20.050927 devapps-2023.5.1/src/devapp/tools/plugin.py
+-rw-r--r--   0        0        0    25788 2023-05-02 07:07:04.676265 devapps-2023.5.1/src/devapp/tools/resource.py
+-rw-r--r--   0        0        0     1861 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/tools/times.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/__init__.py
+-rwxr-xr-x   0        0        0    15787 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/os_.py
+-rwxr-xr-x   0        0        0     1871 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/py_source_env.py
+-rwxr-xr-x   0        0        0     9335 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/rx_tools.py
+-rwxr-xr-x   0        0        0    11529 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/vault.py
+-rwxr-xr-x   0        0        0     2107 2023-05-02 12:19:24.575457 devapps-2023.5.1/src/devapp/utils/watch_dog.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.5.1/src/mdvl/__init__.py
+-rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.5.1/src/mdvl/mdvl.py
+-rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/mdvl/tools.py
+-rwxr-xr-x   0        0        0      519 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/__init__.py
+-rwxr-xr-x   0        0        0     1559 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/adapters.py
+-rwxr-xr-x   0        0        0       88 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/common.py
+-rwxr-xr-x   0        0        0     5503 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/config.py
+-rwxr-xr-x   0        0        0     1618 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/formatters.py
+-rwxr-xr-x   0        0        0     2640 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/processors.py
+-rwxr-xr-x   0        0        0     5472 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/renderers.py
+-rwxr-xr-x   0        0        0    11172 2023-05-02 12:28:38.054778 devapps-2023.5.1/src/structlogging/sl.py
+-rw-r--r--   0        0        0     4022 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/stacktrace.py
+-rwxr-xr-x   0        0        0     1355 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/tests/test_structlogging.py
+-rwxr-xr-x   0        0        0      886 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/theming/__init__.py
+-rwxr-xr-x   0        0        0    14865 2023-05-02 11:32:09.295201 devapps-2023.5.1/src/theming/absl_color_help.py
+-rwxr-xr-x   0        0        0     4345 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ansi2html.py
+-rwxr-xr-x   0        0        0    11888 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ansi2html.sh
+-rwxr-xr-x   0        0        0     3030 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ansistrm.py
+-rwxr-xr-x   0        0        0    10066 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ax_xml.py
+-rwxr-xr-x   0        0        0    10495 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/camel_snake.py
+-rwxr-xr-x   0        0        0     7517 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/charting.py
+-rwxr-xr-x   0        0        0     3392 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/colorhilite.py
+-rwxr-xr-x   0        0        0     1113 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/filesize/README.txt
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/filesize/__init__.py
+-rwxr-xr-x   0        0        0     2549 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/filesize/filesize.py
+-rwxr-xr-x   0        0        0     3756 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/formatters.py
+-rw-r--r--   0        0        0     3807 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/formatting/markdown.py
+-rw-r--r--   0        0        0     1241 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/formatting/viz_sequence.py
+-rwxr-xr-x   0        0        0     3410 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/html_tools.py
+-rwxr-xr-x   0        0        0    11409 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/inflect.py
+-rwxr-xr-x   0        0        0      460 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/msgs.py
+-rwxr-xr-x   0        0        0     9864 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/pretty_print.py
+-rwxr-xr-x   0        0        0    55699 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/tablepretty.py
+-rwxr-xr-x   0        0        0    13998 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/term.py
+-rwxr-xr-x   0        0        0     1468 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/term_struct_hilite.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/test
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/tests/__init__.py
+-rwxr-xr-x   0        0        0     9454 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/tests/test_text_formatting.py
+-rwxr-xr-x   0        0        0     1063 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/tracebacks.py
+-rwxr-xr-x   0        0        0     3011 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/unicode_chars.py
+-rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/__init__.py
+-rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/arch/__init__.py.bak
+-rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/arch/links.py.bak
+-rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/arch/o.py
+-rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/old
+-rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/olinit
+-rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/oo
+-rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/py2.py
+-rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/render.py.bak
+-rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/chrome_reload.sh
+-rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/delivery2.py
+-rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/links.py
+-rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/py3.py
+-rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/render.py
+-rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/version.py
+-rw-r--r--   0        0        0     3037 2023-05-02 12:46:06.858805 devapps-2023.5.1/setup.py
+-rw-r--r--   0        0        0     1804 2023-05-02 12:46:06.859069 devapps-2023.5.1/PKG-INFO
```

### Comparing `devapps-2023.4.28/LICENSE` & `devapps-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/README.md` & `devapps-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/pyproject.toml` & `devapps-2023.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "devapps"
-version = "2023.04.28"
+version = "2023.05.01"
 description = "Apps - End to End."
 authors = ["Gunther Klessinger <g_kle_ss_ing_er@gmx.de>"]
 license = "BSD"
 readme = "README.md"
 repository = "https://github.com/AXGKl/devapps"
 homepage = "https://axgkl.github.io/devapps"
 keywords = []
```

### Comparing `devapps-2023.4.28/src/ax/utils/ax_tree/_ax_tree.so` & `devapps-2023.5.1/src/ax/utils/ax_tree/_ax_tree.so`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/ax/utils/ax_tree/ax_tree.py` & `devapps-2023.5.1/src/ax/utils/ax_tree/ax_tree.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/app.py` & `devapps-2023.5.1/src/devapp/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,34 +138,21 @@
         return
     db += '/bin'
 
     if db and os.path.exists(db):
         p = os.environ['PATH']
         if not db + ':' in p:
             os.environ['PATH'] = db + ':' + p
-    # e = env.get
-    # p = 'DA_DIR_'
-    # d = dict(
-    #    [
-    #        ('%s_dir' % k.split(p, 1)[1].lower(), e(k) + '/' + app_name)
-    #        for k in env
-    #        if k.startswith(p)
-    #    ]
-    # )
-    # an app (like build may allow to set --da_dir, overruling env:
-    # d['da_dir'] = getattr(FLG, 'da_dir', env.get('DA_DIR', '.'))
-    # we are used e.g. at construct/prepare.sh w/o DA:
-    # c = 'CONDA_PREFIX'
-    # breakpoint()
-    # d['pkgs_dir'] = env.get(c + '_1') or env.get(c) + '/pkgs'
-    # return d
+
+
+plugin = ['']
 
 
 def command_name():
-    return sys.argv[0].rsplit('/', 1)[-1].replace('.py', '')
+    return plugin[0] or sys.argv[0].rsplit('/', 1)[-1].replace('.py', '')
 
 
 def set_app(name, log):
     app.log = log
     set_direct_log_methods(app)  # app.info, app.debug, ...
     app.notify = partial(notify, app)
     app.sh = sh
@@ -212,14 +199,15 @@
     l.extend(['--environ_flags'])
     # FLG = flags.FLAGS
     FLG(l)  # <----------- Flag parsing
     # now reset their values from env
     tools.set_flag_vals_from_env()
     kw_log = {}
     sl.setup_logging(**kw_log)
+    breakpoint()   # FIXME BREAKPOINT
     log = sl.get_logger(name)
     set_app(name, log)
 
 
 running = [0]
 
 
@@ -402,15 +390,19 @@
 abslapp.install_exception_handler(dev_app_exc_handler())
 
 
 class Reloaded(Exception):
     pass
 
 
+reload_signal = 1
+
+
 def reload_handler(signum, frame):
+    app.warn('Reload!', signal=reload_signal)
     raise Reloaded('signal')
 
 
 # def wrap_flag_parser_with_action_detector(flags_parser):
 #     def parser(args, p=flags_parser):
 #         try:
 #             breakpoint()  # FIXME BREAKPOINT
@@ -489,35 +481,41 @@
         # TODO: simply do it with entr:
         # cat conf/reload _py3.8
         # !/usr/bin/env bash
 
         # ps wwwax |grep python |grep app | grep client | xargs kill
 
         # test if tools present:
-        d, match, rec = (FLG.dirwatch + '::').split(':')[:3]
+        d, match, rec, sig, freq = (FLG.dirwatch + ':::::').split(':')[:5]
+        if not sig:
+            sig = str(reload_signal)
         d = os.path.abspath(d)
         if not os.path.isdir(d):
-            app.die('No directory:', d=d, nfo='Use <dir>:<match>:[r]')
+            app.die('No directory:', d=d, nfo='Use <dir>:<match>[:r[:sig[:freq]]]')
         w = os.path.dirname(os.path.abspath(__file__)) + '/utils/watch_dog.py'
-        cmd = [w, ':'.join([d, str(os.getpid()), match, rec])]
+        cmd = [w, ':'.join([d, str(os.getpid()), match, rec, sig, freq])]
+        # print('pid', os.getpid())
+        app.info('watcher', cmd=' '.join(cmd))
         watcher_pid = subprocess.Popen(cmd).pid
 
     res = post = None
     while True:
         try:
             if isinstance(main, type):
                 main, post = handle_action_cls(app, action_cls=main)
             # so that everybody knows what is running. informational
             app._app_func = main
             # main = lambda: run_app(Action, flags=Flags, wrapper=cleanup)
+            if FLG.dirwatch:
+                signal.signal(reload_signal, reload_handler)
             res = wrapper(main) if wrapper else main()
             if FLG.dirwatch:
                 app.info('Keep running, dirwatch is set')
-                signal.signal(1, reload_handler)
                 while 1:
+                    # wait for receiving watchdog signal
                     time.sleep(10)
         except DieNow as ex:
             app.error(ex.msg, exc=ex, **ex.kw)
             raise
         except Reloaded as ex:
             continue
         except SystemExit as ex:
```

### Comparing `devapps-2023.4.28/src/devapp/app_token/create_tokens.py` & `devapps-2023.5.1/src/devapp/app_token/create_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/app_token/read_tokens.py` & `devapps-2023.5.1/src/devapp/app_token/read_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/components/cloudfoundry.py` & `devapps-2023.5.1/src/devapp/components/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/components/gitlab.py` & `devapps-2023.5.1/src/devapp/components/gitlab.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/components/gitlab_runner.py` & `devapps-2023.5.1/src/devapp/components/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/dev_mode.py` & `devapps-2023.5.1/src/devapp/dev_mode.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/gevent_patched.py` & `devapps-2023.5.1/src/devapp/gevent_patched.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/layer.py` & `devapps-2023.5.1/src/devapp/layer.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/lib/sh.py` & `devapps-2023.5.1/src/devapp/lib/sh.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/load.py` & `devapps-2023.5.1/src/devapp/load.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/logo` & `devapps-2023.5.1/src/devapp/logo`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/max.py` & `devapps-2023.5.1/src/devapp/max.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/operations/resources.py` & `devapps-2023.5.1/src/devapp/operations/resources.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/dev_devapp/repo_sym_links.py` & `devapps-2023.5.1/src/devapp/plugins/dev_devapp/repo_sym_links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resource_install.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_install.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resource_run.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resources.py.dis` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources.py.dis`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/resources_list.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources_list.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/arch/wait_for_port.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/wait_for_port.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/container_build.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/container_pull.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_pull.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/fs_build.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/fs_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/kubectl/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/kubectl/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/life_cycle.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/life_cycle.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/log_view.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/log_view.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/project/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/plugins/ops_devapp/run.py` & `devapps-2023.5.1/src/devapp/plugins/ops_devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/run.py` & `devapps-2023.5.1/src/devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/build.py` & `devapps-2023.5.1/src/devapp/spec/build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/find_paths_in_fs_components.py` & `devapps-2023.5.1/src/devapp/spec/find_paths_in_fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/fs_components.py` & `devapps-2023.5.1/src/devapp/spec/fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/links.py` & `devapps-2023.5.1/src/devapp/spec/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/os_tools.py` & `devapps-2023.5.1/src/devapp/spec/os_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/templ.py` & `devapps-2023.5.1/src/devapp/spec/templ.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/templates/unit` & `devapps-2023.5.1/src/devapp/spec/templates/unit`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/spec/tools.py` & `devapps-2023.5.1/src/devapp/spec/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/t` & `devapps-2023.5.1/src/devapp/t`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/testing/auto_docs.py` & `devapps-2023.5.1/src/devapp/testing/auto_docs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/third/rpl` & `devapps-2023.5.1/src/devapp/third/rpl`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/__init__.py` & `devapps-2023.5.1/src/devapp/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1648,20 +1648,31 @@
     autoshort = 'da'
     uc_dirwatch_flow = [
         'Running build app, monitoring flow.json, triggering plots on change',
         'build --plot_before --dirwatch .:flow',
     ]
 
     class dirwatch:
-        n = 'Spawning helper process, sending reload, monitoring changes in given directory. '
-        n += 'The app itself keeps running normally, with full access at stdin,out, err. '
-        n += 'You may deliver a match spec, colon seperated.\n'
+        '''Spawning helper process, sending reload, monitoring changes in given directory.
+        The app itself keeps full access at stdin, out, err, unlike using tools e.g. `entr`.
+
+        You may deliver a match spec, colon seperated.
+
+        Format: <dir>[:match[:r[:sig[:freq]]]].
+        - match: w/o * will be enclosed in *, left and right.
+        - r: recursive scan
+        - sig: 1(default) is reload, 15 is kill app
+        - freq: min frequency, default  1 (sec)
+
+        Examples:
+        myapp -dw .:.py # reloads app on every python file change
+        while true; do myapp -dw .:.py:1:15:2; done # kills app every 2 secs, scans recursively
+        '''
+        n = 'Restart or reload application on file changes'
         d = ''
-        n += 'Format: <dir>[:match[:r]]. r for recursive. match w/o * will be enclosed in *, left and right.\n'
-        n += 'Example: while true; do bin/client -dw .:.py:1; done'
         s = 'dw'
 
     class redir_stderr:
         """There are process spawners which mix the streams (emacs call-process)
         Spawns sys.exit(os.system(cmd + ' 2>%s' % FLG.redir_stderr))"""
 
         n = 'Global redirect of stderr'
```

### Comparing `devapps-2023.4.28/src/devapp/tools/flag.py` & `devapps-2023.5.1/src/devapp/tools/flag.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/http.py` & `devapps-2023.5.1/src/devapp/tools/http.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/__init__.py` & `devapps-2023.5.1/src/devapp/tools/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/actions.py` & `devapps-2023.5.1/src/devapp/tools/infra/actions.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/000:functions.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/000:functions.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/300:dns.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/300:dns.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/500:k3s.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/500:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/501:kind.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/501:kind.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/502:k3s.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/502:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/600:longhorn.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/600:longhorn.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh` & `devapps-2023.5.1/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/tools/plugin.py` & `devapps-2023.5.1/src/devapp/tools/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python
 """
 Tool to quickly build and app with plugins.
 
 Usage: See lc.py
-
 """
 import os
 import sys
 from fnmatch import fnmatch
 from importlib import import_module
 
 from devapp.tools import dir_of
 
 
 def get_docstr(app=None):
     if not app:
         app = sys.argv[0]
 
-    D = '''
+    D = """
 Usage: %(app)s ACTION [--flag[=value] ...]
 
 Available Plugins:
 <PLUGINS>
 
 Help:
     %(app)s <action> <-h|--helpfull> [match]
@@ -29,15 +28,15 @@
 Note:
     - Action shortcuts understood, e.g. action "foo_bar_baz" = fbb
     - Plugins are taken on first found basis
     - Flags also have shortcut versions (e.g. -hf for --helpfull)
 
 Example:
     %(app)s %(exmpl)s -hf log # all flags about logging
-    '''
+    """
     D = D % {'app': os.path.basename(app), 'exmpl': example[0]}
     return D
 
 
 class Plugins:
     pass
 
@@ -85,15 +84,17 @@
         usage(ec)
 
     plug = plugname = getattr(Plugins, plugin)
     if isinstance(plug, str):
         plug = import_module(plug)
 
     sys_argv_rm_minus_h_for_hf(argv, plug, plugname)
+    from devapp import app
 
+    app.plugin[0] = plugin   # for logging
     plug.main()
 
 
 def sys_argv_rm_minus_h_for_hf(argv, plug, plugname):
     h, hf = False, False
     r = []
     for a in argv:
```

### Comparing `devapps-2023.4.28/src/devapp/tools/resource.py` & `devapps-2023.5.1/src/devapp/tools/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,14 +532,15 @@
                 ]
             else:
                 cmd = [
                     'test -e "%(D)s/etc/profile.d/conda.sh" && . "%(D)s/etc/profile.d/conda.sh" || true',
                     '%(conda)s create %(yes)s -n "%(name)s"',
                     '%(conda)s activate "%(name)s"',
                 ]
+            ctx['conda'] = ctx.get('conda', 'conda')
             pth = '%(D)s/envs/%(name)s/bin/' % ctx
 
             if g(rsc, 'typ') == 'pip':
                 ctx['cmd'] = rsc.cmd
                 cmd += ['%(conda)s install -c conda-forge python; %p/pip install %%(cmd)s' % pth]
             else:
                 icmd = g(rsc, 'conda_inst', '')
```

### Comparing `devapps-2023.4.28/src/devapp/tools/times.py` & `devapps-2023.5.1/src/devapp/tools/times.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/utils/os_.py` & `devapps-2023.5.1/src/devapp/utils/os_.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/utils/py_source_env.py` & `devapps-2023.5.1/src/devapp/utils/py_source_env.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/utils/rx_tools.py` & `devapps-2023.5.1/src/devapp/utils/rx_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/devapp/utils/vault.py` & `devapps-2023.5.1/src/devapp/utils/vault.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/mdvl/mdvl.py` & `devapps-2023.5.1/src/mdvl/mdvl.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
       terminal we usually have them as full ansi escape str.
       Thats why `get_val` is present and adapts for that in the Colors cls.
     """
 
     _parms = None  # our (relevant) keys and values
 
     def setup(self, kw):
-        """ find all our key value defaults and override with env and **kw"""
+        """find all our key value defaults and override with env and **kw"""
         self._parms = []
         kv = [(k, getattr(self, k)) for k in dir(self) if not k.startswith('_')]
         self._parms = [(k, v) for k, v in kv if not hasattr(v, '__code__')]
         [setattr(self, k, self.get_val(k, v, kw)) for k, v in self._parms]
 
     def get_val(self, k, dflt, kw):
         try:
@@ -102,15 +102,15 @@
 
     def H(s, lev):
         res = getattr(s, 'H%s' % lev, s.L)
         return res
 
 
 class Facts(Cfg):
-    """ features config """
+    """features config"""
 
     debug = False
     term_width = 80
     no_print = False
     bq_mark = '┃'
     code_mark = ' '
     light_bg = False
@@ -147,15 +147,15 @@
     keywrd = l0[:2] + keywrd + p
     l1 = l1
     offs = 1 if l1 and l1[0] == ' ' else 2
     return len(l0) - len(l1[offs:].lstrip()) - (2 * len(p))
 
 
 def block_quote_status(l, g):
-    'blockquote'
+    """blockquote"""
     if not l.startswith('>'):
         return 0, l, ''
     _ = l.split(' ', 1)
     lev = len(_[0])
     g['max_bq_depth'] = max(lev, g['max_bq_depth'])
     return lev, _[1], _[0]
 
@@ -357,15 +357,17 @@
     # --------------- Leaving line/block scanning, reWork complete document now
     g[cur_colr] = C.O
     out = '\n'.join(out)
 
     # INLINE MARKUP, *, **, backticks
     # Alternating replacements, e.g. code, emph. requires a first space char:
     altern = lambda s, c, r: re.sub(
-        r'([^{c}]+){c}([^{c}]+){c}?'.format(c=c), r'\1%s\2%s' % (r, g[cur_colr]), ' ' + s,
+        r'([^{c}]+){c}([^{c}]+){c}?'.format(c=c),
+        r'\1%s\2%s' % (r, g[cur_colr]),
+        ' ' + s,
     )[
         1:
     ]  # removing space again
 
     # Star must be replaced, else the re would not work :((
     # currently no way to find single stars and not process them..
     out = out.replace('*', '\x01')
@@ -405,15 +407,15 @@
     out += C.O  # reset
     if not f.no_print:
         print(out)
     return out
 
 
 def strip_it(out, rst):
-    'clumsy way to strip at start at end, including color resets'
+    """clumsy way to strip at start at end, including color resets"""
     sc = {' ': 1, rst: len(rst), '\n': 1}
     while 1:
         m = False
         for k in sc:
             if out.startswith(k):
                 out = out[sc[k] :]
                 m = True
```

### Comparing `devapps-2023.4.28/src/mdvl/tools.py` & `devapps-2023.5.1/src/mdvl/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/__init__.py` & `devapps-2023.5.1/src/structlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/adapters.py` & `devapps-2023.5.1/src/structlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/config.py` & `devapps-2023.5.1/src/structlogging/config.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/formatters.py` & `devapps-2023.5.1/src/structlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/processors.py` & `devapps-2023.5.1/src/structlogging/processors.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/renderers.py` & `devapps-2023.5.1/src/structlogging/renderers.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/sl.py` & `devapps-2023.5.1/src/structlogging/sl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/stacktrace.py` & `devapps-2023.5.1/src/structlogging/stacktrace.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/structlogging/tests/test_structlogging.py` & `devapps-2023.5.1/src/structlogging/tests/test_structlogging.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/__init__.py` & `devapps-2023.5.1/src/theming/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/absl_color_help.py` & `devapps-2023.5.1/src/theming/absl_color_help.py`

 * *Files 5% similar despite different names*

```diff
@@ -357,14 +357,20 @@
 def color_usage(*a, main_module, full=None, **kw):
     """
     colorizes flag keys and match from --help <match>
     """
     ret = []
     d = main_module.__doc__
     if d:
+        if d.lstrip().startswith('# '):
+            from mdvl import mdvl
+
+            d = mdvl.render(
+                d, no_print=True, header_numbering=True, header_numb_level_min=2
+            )
         ret.append('\n' + d.strip() + '\n\n')
     add = lambda s, end='\n', ret=ret: ret.append(s + end)
     # catch the original output:
     hof = get_argv_val('--help_output_fmt')
     hof = hof if hof else 'terminal'
     match = get_argv_val('--helpfull', ign_val='--help_output_fmt')
     match = [match] if match else []
@@ -399,16 +405,16 @@
     # no match was given, the list is filtered at this point:
     if dmn and match == [dmn]:
         match = []
     match_hilite = ansi_col('1;32') + ' '.join(match) + ansi_col('0')
     j['match'] = '[matching %s]' % match_hilite if match else ''
 
     if match:
-        n, n1 = ('All supported', '') if full else ('Main', ' (-hf for all flags)')
-        add('%s command line flags %s%s:' % (n, j['match'], n1))
+        n = 'All supported' if full else 'Main'
+        add('%s command line flags %s:' % (n, j['match']))
     if hof != 'terminal':
         r = tabulate()
 
     w = term_widths(match)
 
     def do(fn_mod, w=w, flgs=None):
         # module headline:
@@ -427,14 +433,18 @@
         do(n)
     # when user has selected an action on CLI, show it last, again:
     if j.get('actions'):
         add(ansi_col('1;34') + '\nSelected Action')
         do('actions', flgs=j['actions'])
 
     # show main module's flags last - always:
+    if not full:
+        add(
+            '\n\x1b[36m-hf [match string]\x1b[0m: List \x1b[36;1mALL\x1b[0m (matching) flags. E.g. -hf or -hf log.'
+        )
     add('\033[0m')
     return ret
 
 
 hlp_flags = {'-h': False, '--help': False, '-hf': True, '--helpfull': True}
```

### Comparing `devapps-2023.4.28/src/theming/ansi2html.py` & `devapps-2023.5.1/src/theming/ansi2html.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/ansi2html.sh` & `devapps-2023.5.1/src/theming/ansi2html.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/ansistrm.py` & `devapps-2023.5.1/src/theming/ansistrm.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/ax_xml.py` & `devapps-2023.5.1/src/theming/ax_xml.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/camel_snake.py` & `devapps-2023.5.1/src/theming/camel_snake.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/charting.py` & `devapps-2023.5.1/src/theming/charting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/colorhilite.py` & `devapps-2023.5.1/src/theming/colorhilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/filesize/README.txt` & `devapps-2023.5.1/src/theming/filesize/README.txt`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/filesize/filesize.py` & `devapps-2023.5.1/src/theming/filesize/filesize.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/formatters.py` & `devapps-2023.5.1/src/theming/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/formatting/markdown.py` & `devapps-2023.5.1/src/theming/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/formatting/viz_sequence.py` & `devapps-2023.5.1/src/theming/formatting/viz_sequence.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/html_tools.py` & `devapps-2023.5.1/src/theming/html_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/inflect.py` & `devapps-2023.5.1/src/theming/inflect.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/pretty_print.py` & `devapps-2023.5.1/src/theming/pretty_print.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/tablepretty.py` & `devapps-2023.5.1/src/theming/tablepretty.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/term.py` & `devapps-2023.5.1/src/theming/term.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/term_struct_hilite.py` & `devapps-2023.5.1/src/theming/term_struct_hilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/tests/test_text_formatting.py` & `devapps-2023.5.1/src/theming/tests/test_text_formatting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/tracebacks.py` & `devapps-2023.5.1/src/theming/tracebacks.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/theming/unicode_chars.py` & `devapps-2023.5.1/src/theming/unicode_chars.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/__init__.py` & `devapps-2023.5.1/src/tree_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/__init__.py.bak` & `devapps-2023.5.1/src/tree_builder/arch/__init__.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/links.py.bak` & `devapps-2023.5.1/src/tree_builder/arch/links.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/o.py` & `devapps-2023.5.1/src/tree_builder/arch/o.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/old` & `devapps-2023.5.1/src/tree_builder/arch/old`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/olinit` & `devapps-2023.5.1/src/tree_builder/arch/olinit`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/oo` & `devapps-2023.5.1/src/tree_builder/arch/oo`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/arch/render.py.bak` & `devapps-2023.5.1/src/tree_builder/arch/render.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/chrome_reload.sh` & `devapps-2023.5.1/src/tree_builder/chrome_reload.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/delivery2.py` & `devapps-2023.5.1/src/tree_builder/delivery2.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/links.py` & `devapps-2023.5.1/src/tree_builder/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/src/tree_builder/render.py` & `devapps-2023.5.1/src/tree_builder/render.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.4.28/setup.py` & `devapps-2023.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                      'dev = devapp.tools.plugin:main',
                      'fui = interactive.cli:main',
                      'myapp = devapp.tools.plugin:main',
                      'ops = devapp.tools.plugin:main']}
 
 setup_kwargs = {
     'name': 'devapps',
-    'version': '2023.4.28',
+    'version': '2023.5.1',
     'description': 'Apps - End to End.',
     'long_description': '# devapps\n\n\n<!-- badges -->\n[![docs pages][docs pages_img]][docs pages] [![gh-ci][gh-ci_img]][gh-ci] [![pkg][pkg_img]][pkg] [![code_style][code_style_img]][code_style] \n\n[docs pages]: https://axgkl.github.io/devapps/\n[docs pages_img]: https://axgkl.github.io/devapps/img/badge_docs.svg\n[gh-ci]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml\n[gh-ci_img]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml/badge.svg\n[pkg]: https://pypi.com/\n[pkg_img]: https://axgkl.github.io/devapps/img/badge_pypi.svg\n[code_style]: https://pypi.org/project/axblack/\n[code_style_img]: https://axgkl.github.io/devapps/img/badge_axblack.svg\n<!-- badges -->\n\n\nEnabler repo for dev *and* ops friendly apps, in a normalized way.\n\nIncludes:\n\n- logging (structlog)\n- cli flags handling (abseil, with addons)\n- docutools (mkdocs-material)\n- project setup\n- (test) resources management, including daemons and container filesystem layers\n\nand more.\n\n\n\n\nDocumentation: https://axgkl.github.io/devapps/',
     'author': 'Gunther Klessinger',
     'author_email': 'g_kle_ss_ing_er@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://axgkl.github.io/devapps',
```

### Comparing `devapps-2023.4.28/PKG-INFO` & `devapps-2023.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devapps
-Version: 2023.4.28
+Version: 2023.5.1
 Summary: Apps - End to End.
 Home-page: https://axgkl.github.io/devapps
 License: BSD
 Author: Gunther Klessinger
 Author-email: g_kle_ss_ing_er@gmx.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

