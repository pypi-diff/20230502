# Comparing `tmp/iambic_core-0.3.1.tar.gz` & `tmp/iambic_core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.3.1.tar", max compression
+gzip compressed data, was "iambic_core-0.4.1.tar", max compression
```

## Comparing `iambic_core-0.3.1.tar` & `iambic_core-0.4.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11356 2023-04-21 20:14:05.441705 iambic_core-0.3.1/LICENSE.md
--rw-r--r--   0        0        0    10252 2023-04-21 20:14:05.441705 iambic_core-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/templates.py
--rw-r--r--   0        0        0     1955 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/utils.py
--rw-r--r--   0        0        0    68924 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/logger.py
--rw-r--r--   0        0        0    24862 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5244 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/parser.py
--rw-r--r--   0        0        0    46094 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/template_generation.py
--rw-r--r--   0        0        0    26626 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/lambda/app.py
--rw-r--r--   0        0        0    13644 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/main.py
--rw-r--r--   0        0        0      664 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/__init__.py
--rw-r--r--   0        0        0     2763 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     1715 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     1842 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     1888 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    13572 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    33240 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17683 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15824 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17544 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10649 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21304 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24395 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20623 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22579 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4534 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31350 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35369 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    28215 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     2973 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10183 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8455 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5066 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9282 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2687 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9405 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13563 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      137 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     1922 2023-04-21 20:14:05.481705 iambic_core-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    12575 1970-01-01 00:00:00.000000 iambic_core-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-01 22:30:16.826649 iambic_core-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0    10551 2023-05-01 22:30:16.826649 iambic_core-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/templates.py
+-rw-r--r--   0        0        0     1955 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    69560 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    24862 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5244 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    46094 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    26626 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13644 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2149 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2276 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2498 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    13572 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    33240 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17683 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15824 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17544 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10649 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21304 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24395 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20623 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22579 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4534 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31350 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35369 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    28215 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     2973 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10183 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8455 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5066 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9282 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2687 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9405 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13563 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      137 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     1922 2023-05-01 22:30:16.874637 iambic_core-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.4.1/PKG-INFO
```

### Comparing `iambic_core-0.3.1/LICENSE.md` & `iambic_core-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/README.md` & `iambic_core-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 - **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
 - **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
 - **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
+## 📣 Let's chat
+Do you want to connect with our contributors?
+
+Just click the button below and follow the instructions.
+
+[![slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)](https://communityinviter.com/apps/noqcommunity/noq)
+
 ## Getting Started
 
 Dive into IAMbic with our [quick-start guide](http://docs.iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
 ## Installing IAMbic and Supported Versions
 
 IAMbic is available on PyPI:
@@ -252,8 +259,8 @@
 
 IAMbic is licensed under the Apache-2.0 license. Commercial licenses and support are also available from Noq Software, Inc.
 
 ### Provider Plugins
 
 Provider Plugins (Such as the AWS, Okta, Azure Active Directory, and Google Workspace plugins) are licensed under Apache 2. You are free to write your own provider plugins for internal services without releasing its source code.
 
-For more information, please visit [iambic.org](https://docs.iambic.org/license).
+For more information, please visit [https://docs.iambic.org/license](https://docs.iambic.org/license).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iambic_core-0.3.1/iambic/config/dynamic_config.py` & `iambic_core-0.4.1/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/config/utils.py` & `iambic_core-0.4.1/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/config/wizard.py` & `iambic_core-0.4.1/iambic/config/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         operation_str = f"{operation.value} in"
     elif operation == Operation.DELETED:
         operation_str = f"{operation.value} from"
     else:
         raise ValueError(f"Invalid operation: {operation}")
 
     if not questionary.confirm(
-        f"To preserve these changes, {command_type} must be ran to sync your templates.\n"
+        f"To preserve these changes, {command_type} must be run to sync your templates.\n"
         "Proceed?"
     ).unsafe_ask():
         if questionary.confirm(
             f"The {provider_type} will not be {operation_str} the config and wizard will exit.\n"
             "Proceed?"
         ).unsafe_ask():
             log.info("Exiting...")
@@ -448,23 +448,32 @@
 
         with contextlib.suppress(ClientError, NoCredentialsError, FileNotFoundError):
             self.autodetected_org_settings = self.boto3_session.client(
                 "organizations"
             ).describe_organization()["Organization"]
 
     def resolve_aws_profile_defaults_from_env(self) -> str:
-        if profile_name := os.environ.get("AWS_PROFILE"):
+        if "AWS_ACCESS_KEY_ID" in os.environ:
+            # Environment variables has 1st priority
+            profile_name = "None"
+            log.info("Using AWS credentials from environment", profile=profile_name)
+        elif profile_name := os.environ.get("AWS_PROFILE"):
+            # Explicit profile has 2nd priority
             log.info("Using AWS profile from environment", profile=profile_name)
         elif profile_name := os.environ.get("AWS_DEFAULT_PROFILE"):
-            log.info("Using AWS default profile from environment", profile=profile_name)
-        elif "AWS_ACCESS_KEY_ID" in os.environ:
-            profile_name = "default"
+            # Fallback profile has 3rd priority
             log.info("Using AWS default profile from environment", profile=profile_name)
         else:
+            # User has to direct the wizard at this point since
+            # we cannot reason what credential to use.
             profile_name = "None"
+            log.info(
+                "Not able detect a standard credential provider chain",
+                profile=profile_name,
+            )
 
         return profile_name
 
     def set_aws_profile_name(
         self, question_text: str = None, allow_none: bool = False
     ) -> Union[str, None]:
         questionary_params = {}
@@ -570,17 +579,21 @@
             ):
                 self.autodetected_org_settings = self.boto3_session.client(
                     "organizations"
                 ).describe_organization()["Organization"]
             break
 
     def get_boto3_session_for_account(self, account_id: str):
+        # This need to follow standard credentials provider chain
         if account_id == self.hub_account_id:
             if not self.profile_name:
-                if profile_name := os.getenv("AWS_PROFILE"):
+                if os.getenv("AWS_ACCESS_KEY_ID"):
+                    # environment variables credentials detected
+                    self.profile_name = None
+                elif profile_name := os.getenv("AWS_PROFILE"):
                     self.profile_name = profile_name
                 else:
                     self.profile_name = self.set_aws_profile_name(
                         "Please specify the profile to use to access to the AWS Account.",
                         allow_none=False,
                     )
             return self.boto3_session, self.profile_name
@@ -776,15 +789,15 @@
                     default=False,
                 ).unsafe_ask()
             )
 
         else:
             if requires_sync:
                 if not questionary.confirm(
-                    "Adding this account will require a sync to be ran.\n"
+                    "Adding this account will require a sync to be run.\n"
                     "This is to apply any matching templates to the account if the resource does not already exist.\n"
                     "Then, the account resources will be imported into Iambic.\n"
                     "Proceed?"
                 ).unsafe_ask():
                     log.info(
                         "Unable to add the AWS account without creating the required role."
                     )
```

### Comparing `iambic_core-0.3.1/iambic/core/aio_utils/__init__.py` & `iambic_core-0.4.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/exceptions.py` & `iambic_core-0.4.1/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/git.py` & `iambic_core-0.4.1/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/iambic_enum.py` & `iambic_core-0.4.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/iambic_plugin.py` & `iambic_core-0.4.1/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/logger.py` & `iambic_core-0.4.1/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/models.py` & `iambic_core-0.4.1/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/noq_json.py` & `iambic_core-0.4.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/parser.py` & `iambic_core-0.4.1/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/template_generation.py` & `iambic_core-0.4.1/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/core/utils.py` & `iambic_core-0.4.1/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.4.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.4.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.4.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/github/templates/iambic-import.yml` & `iambic_core-0.4.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/github/utils.py` & `iambic_core-0.4.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/lambda/app.py` & `iambic_core-0.4.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/main.py` & `iambic_core-0.4.1/iambic/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/__init__.py` & `iambic_core-0.4.1/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/filters.py` & `iambic_core-0.4.1/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/models.py` & `iambic_core-0.4.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.4.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.4.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.4.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/output/text.py` & `iambic_core-0.4.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/README.md` & `iambic_core-0.4.1/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
           !If
           - IsAssumeAsArnProvided
           -
             - Effect: Allow
               Action:
                 - sts:AssumeRole
                 - sts:TagSession
+                - sts:SetSourceIdentity
               Principal:
                 AWS: !Ref AssumeAsArn
           -
             - Effect: Deny
               Action: sts:AssumeRole
               Principal:
                 Service: ec2.amazonaws.com
@@ -40,14 +41,15 @@
         - PolicyName: assume_spoke_role
           PolicyDocument:
             Version: '2012-10-17'
             Statement:
               - Effect: Allow
                 Action:
                   - sts:assumerole
+                  - sts:SetSourceIdentity
                 Resource:
                   - !Sub 'arn:aws:iam::*:role/${SpokeRoleName}*'
         - PolicyName: list_spoke_account_info
           PolicyDocument:
             Version: '2012-10-17'
             Statement:
               - Effect: Allow
```

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 AWSTemplateFormatVersion: 2010-09-09
 Description: >-
-  This template creates the IAMbic spoke role.
+  This template creates the IAMbic read-only spoke role.
 Parameters:
   SpokeRoleName:
     Type: String
   HubRoleArn:
     Type: String
 Resources:
-  IambicSpokeRole:
+  IambicSpokeRoleReadOnly:
     Type: 'AWS::IAM::Role'
     Properties:
       RoleName: !Ref SpokeRoleName
       Description: >-
         This role is used by IAMbic to perform all actions on the account.
         It is assumed by the Iambic hub role in the hub account.
         Managed via CloudFormation.
       AssumeRolePolicyDocument:
         Version: '2012-10-17'
         Statement:
           - Effect: Allow
             Action:
               - sts:AssumeRole
               - sts:TagSession
+              - sts:SetSourceIdentity
             Principal:
               AWS: !Ref HubRoleArn
       Policies:
         - PolicyName: base_permissions
           PolicyDocument:
             Version: '2012-10-17'
             Statement:
               - Effect: Allow
                 Action:
-                  - ec2:Describe*
-                  - identitystore:*
+                  - identitystore:Describe*
+                  - identitystore:Get*
+                  - identitystore:List*
                   - organizations:describe*
                   - organizations:list*
-                  - iam:*
-                  - sso:*
+                  - iam:Get*
+                  - iam:List*
+                  - sso:Describe*
+                  - sso:Get*
+                  - sso:List*
+                  - sso:Search*
                 Resource:
                   - '*'
               - Effect: Allow
                 Action:
                   - secretsmanager:CreateSecret
                   - secretsmanager:GetSecretValue
                   - secretsmanager:describesecret
                   - secretsmanager:listsecrets
                   - secretsmanager:listsecretversionids
                   - secretsmanager:PutSecretValue
                 Resource:
                   - 'arn:aws:secretsmanager:*:*:secret:iambic-config-secrets-*'
-      ManagedPolicyArns:
-        - 'arn:aws:iam::aws:policy/ReadOnlyAccess'
+              - Sid: 'SqsWriteAccessForResourceMonitoring'
+                Effect: Allow
+                Action:
+                  - sqs:ReceiveMessage
+                  - sqs:SendMessage
+                  - sqs:DeleteMessage
+                  - sqs:GetQueueUrl
+                  - sqs:GetQueueAttributes
+                Resource:
+                  - 'arn:aws:sqs:*:*:IAMbicChangeDetectionQueue'
```

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files 12% similar despite different names*

```diff
@@ -58,8 +58,28 @@
       - IAMbicEventBus
       - IAMbicChangeDetectionQueue
   IAMbicChangeDetectionQueue:
     Type: 'AWS::SQS::Queue'
     Properties:
       QueueName: IAMbicChangeDetectionQueue
       MessageRetentionPeriod: 604800
-
+  IAMbicChangeDetectionQueueSQSPolicy: 
+    Type: AWS::SQS::QueuePolicy
+    Properties: 
+      Queues: 
+        - !Ref IAMbicChangeDetectionQueue
+      PolicyDocument: 
+        Statement: 
+          - Action: 
+              - "sqs:SendMessage" 
+            Effect: "Allow"
+            Resource: !GetAtt IAMbicChangeDetectionQueue.Arn
+            Principal:  
+              Service:
+                - "events.amazonaws.com"
+            Condition:
+              ArnEquals:
+                aws:SourceArn: !GetAtt IAMbicEventRule.Arn
+    DependsOn:
+      - IAMbicEventRule
+      - IAMbicChangeDetectionQueue
+
```

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/request_handler/expire_resources.py` & `iambic_core-0.4.1/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/request_handler/git_apply.py` & `iambic_core-0.4.1/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/request_handler/git_plan.py` & `iambic_core-0.4.1/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.3.1/pyproject.toml` & `iambic_core-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.3.1"
+version = "0.4.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.3.1/PKG-INFO` & `iambic_core-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.3.1
+Version: 0.4.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -72,14 +72,21 @@
 - **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
 - **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
 - **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
+## 📣 Let's chat
+Do you want to connect with our contributors?
+
+Just click the button below and follow the instructions.
+
+[![slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)](https://communityinviter.com/apps/noqcommunity/noq)
+
 ## Getting Started
 
 Dive into IAMbic with our [quick-start guide](http://docs.iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
 ## Installing IAMbic and Supported Versions
 
 IAMbic is available on PyPI:
@@ -308,9 +315,9 @@
 
 IAMbic is licensed under the Apache-2.0 license. Commercial licenses and support are also available from Noq Software, Inc.
 
 ### Provider Plugins
 
 Provider Plugins (Such as the AWS, Okta, Azure Active Directory, and Google Workspace plugins) are licensed under Apache 2. You are free to write your own provider plugins for internal services without releasing its source code.
 
-For more information, please visit [iambic.org](https://docs.iambic.org/license).
+For more information, please visit [https://docs.iambic.org/license](https://docs.iambic.org/license).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

