# Comparing `tmp/auth0-python-4.1.1.tar.gz` & `tmp/auth0-python-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth0-python-4.1.1.tar", last modified: Thu Apr 13 13:40:41 2023, max compression
+gzip compressed data, was "auth0-python-4.2.0.tar", last modified: Tue May  2 17:27:39 2023, max compression
```

## Comparing `auth0-python-4.1.1.tar` & `auth0-python-4.2.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-04-13 13:40:41.000000 auth0-python-4.1.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-04-13 13:40:41.585198 auth0-python-4.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-04-13 13:40:41.000000 auth0-python-4.1.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.569198 auth0-python-4.1.1/auth0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/asyncify.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.573198 auth0-python-4.1.1/auth0/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6779 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2439 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2498 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/client_authentication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7777 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2268 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      958 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1137 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15148 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/authentication/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      572 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.577198 auth0-python-4.1.1/auth0/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/attack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5595 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/email_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/management/users_by_email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10884 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4919 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/rest_async.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.577198 auth0-python-4.1.1/auth0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.581198 auth0-python-4.1.1/auth0/test/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8225 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32975 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/authentication/test_users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/auth0/test/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_atack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4476 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_email_endpoints.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test/management/test_users_by_email.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/auth0/test_async/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/test_async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/test_async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6618 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/test_async/test_asyncify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 13:40:41.585198 auth0-python-4.1.1/auth0_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3750 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-04-13 13:40:41.000000 auth0-python-4.1.1/auth0_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 13:40:41.585198 auth0-python-4.1.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-04-13 13:40:41.000000 auth0-python-4.1.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.080303 auth0-python-4.2.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-05-02 17:27:38.000000 auth0-python-4.2.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-05-02 17:27:39.080303 auth0-python-4.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-05-02 17:27:38.000000 auth0-python-4.2.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.068303 auth0-python-4.2.0/auth0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2776 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/asyncify.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.068303 auth0-python-4.2.0/auth0/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6779 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2439 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2498 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/client_authentication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1073 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7777 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2268 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      958 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1137 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15298 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/authentication/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      572 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.072303 auth0-python-4.2.0/auth0/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/attack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5595 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/email_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/management/users_by_email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10884 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4919 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/rest_async.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.072303 auth0-python-4.2.0/auth0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.072303 auth0-python-4.2.0/auth0/test/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8225 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33387 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/authentication/test_users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.076303 auth0-python-4.2.0/auth0/test/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_atack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4476 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_email_endpoints.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test/management/test_users_by_email.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.080303 auth0-python-4.2.0/auth0/test_async/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/test_async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/test_async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6618 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/test_async/test_asyncify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-05-02 17:27:38.000000 auth0-python-4.2.0/auth0/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-02 17:27:39.080303 auth0-python-4.2.0/auth0_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3750 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-05-02 17:27:39.000000 auth0-python-4.2.0/auth0_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-02 17:27:39.080303 auth0-python-4.2.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-05-02 17:27:38.000000 auth0-python-4.2.0/setup.py
```

### Comparing `auth0-python-4.1.1/LICENSE` & `auth0-python-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/PKG-INFO` & `auth0-python-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.1.1
+Version: 4.2.0
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.1.1 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.2.0 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.1.1/README.md` & `auth0-python-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/asyncify.py` & `auth0-python-4.2.0/auth0/asyncify.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/async_token_verifier.py` & `auth0-python-4.2.0/auth0/authentication/async_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/base.py` & `auth0-python-4.2.0/auth0/authentication/base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/client_authentication.py` & `auth0-python-4.2.0/auth0/authentication/client_authentication.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/database.py` & `auth0-python-4.2.0/auth0/authentication/database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/delegated.py` & `auth0-python-4.2.0/auth0/authentication/delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/enterprise.py` & `auth0-python-4.2.0/auth0/authentication/enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/get_token.py` & `auth0-python-4.2.0/auth0/authentication/get_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/passwordless.py` & `auth0-python-4.2.0/auth0/authentication/passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/revoke_token.py` & `auth0-python-4.2.0/auth0/authentication/revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/social.py` & `auth0-python-4.2.0/auth0/authentication/social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/authentication/token_verifier.py` & `auth0-python-4.2.0/auth0/authentication/token_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,30 +122,14 @@
         super().__init__(algorithm)
         self._shared_secret = shared_secret
 
     def _fetch_key(self, key_id=None):
         return self._shared_secret
 
 
-class AsymmetricSignatureVerifier(SignatureVerifier):
-    """Verifier for RSA signatures, which rely on public key certificates.
-
-    Args:
-        jwks_url (str): The url where the JWK set is located.
-        algorithm (str, optional): The expected signing algorithm. Defaults to "RS256".
-    """
-
-    def __init__(self, jwks_url, algorithm="RS256"):
-        super().__init__(algorithm)
-        self._fetcher = JwksFetcher(jwks_url)
-
-    def _fetch_key(self, key_id=None):
-        return self._fetcher.get_key(key_id)
-
-
 class JwksFetcher:
     """Class that fetches and holds a JSON web key set.
     This class makes use of an in-memory cache. For it to work properly, define this instance once and re-use it.
 
     Args:
         jwks_url (str): The url where the JWK set is located.
         cache_ttl (str, optional): The lifetime of the JWK set cache in seconds. Defaults to 600 seconds.
@@ -235,14 +219,31 @@
         if not self._cache_is_fresh:
             keys = self._fetch_jwks(force=True)
             if keys and key_id in keys:
                 return keys[key_id]
         raise TokenValidationError(f'RSA Public Key with ID "{key_id}" was not found.')
 
 
+class AsymmetricSignatureVerifier(SignatureVerifier):
+    """Verifier for RSA signatures, which rely on public key certificates.
+
+    Args:
+        jwks_url (str): The url where the JWK set is located.
+        algorithm (str, optional): The expected signing algorithm. Defaults to "RS256".
+        cache_ttl (int, optional): The lifetime of the JWK set cache in seconds. Defaults to 600 seconds.
+    """
+
+    def __init__(self, jwks_url, algorithm="RS256", cache_ttl=JwksFetcher.CACHE_TTL):
+        super().__init__(algorithm)
+        self._fetcher = JwksFetcher(jwks_url, cache_ttl)
+
+    def _fetch_key(self, key_id=None):
+        return self._fetcher.get_key(key_id)
+
+
 class TokenVerifier:
     """Class that verifies ID tokens following the steps defined in the OpenID Connect spec.
     An OpenID Connect ID token is not meant to be consumed until it's verified.
 
     Args:
         signature_verifier (SignatureVerifier): The instance that knows how to verify the signature.
         issuer (str): The expected issuer claim value.
```

### Comparing `auth0-python-4.1.1/auth0/authentication/users.py` & `auth0-python-4.2.0/auth0/authentication/users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/exceptions.py` & `auth0-python-4.2.0/auth0/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/__init__.py` & `auth0-python-4.2.0/auth0/management/__init__.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/actions.py` & `auth0-python-4.2.0/auth0/management/actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/async_auth0.py` & `auth0-python-4.2.0/auth0/management/async_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/attack_protection.py` & `auth0-python-4.2.0/auth0/management/attack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/auth0.py` & `auth0-python-4.2.0/auth0/management/auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/blacklists.py` & `auth0-python-4.2.0/auth0/management/blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/branding.py` & `auth0-python-4.2.0/auth0/management/branding.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/client_credentials.py` & `auth0-python-4.2.0/auth0/management/client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/client_grants.py` & `auth0-python-4.2.0/auth0/management/client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/clients.py` & `auth0-python-4.2.0/auth0/management/clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/connections.py` & `auth0-python-4.2.0/auth0/management/connections.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/custom_domains.py` & `auth0-python-4.2.0/auth0/management/custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/device_credentials.py` & `auth0-python-4.2.0/auth0/management/device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/email_templates.py` & `auth0-python-4.2.0/auth0/management/email_templates.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/emails.py` & `auth0-python-4.2.0/auth0/management/emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/grants.py` & `auth0-python-4.2.0/auth0/management/grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/guardian.py` & `auth0-python-4.2.0/auth0/management/guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/hooks.py` & `auth0-python-4.2.0/auth0/management/hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/jobs.py` & `auth0-python-4.2.0/auth0/management/jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/log_streams.py` & `auth0-python-4.2.0/auth0/management/log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/logs.py` & `auth0-python-4.2.0/auth0/management/logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/organizations.py` & `auth0-python-4.2.0/auth0/management/organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/prompts.py` & `auth0-python-4.2.0/auth0/management/prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/resource_servers.py` & `auth0-python-4.2.0/auth0/management/resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/roles.py` & `auth0-python-4.2.0/auth0/management/roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/rules.py` & `auth0-python-4.2.0/auth0/management/rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/rules_configs.py` & `auth0-python-4.2.0/auth0/management/rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/stats.py` & `auth0-python-4.2.0/auth0/management/stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/tenants.py` & `auth0-python-4.2.0/auth0/management/tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/tickets.py` & `auth0-python-4.2.0/auth0/management/tickets.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/user_blocks.py` & `auth0-python-4.2.0/auth0/management/user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/users.py` & `auth0-python-4.2.0/auth0/management/users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/management/users_by_email.py` & `auth0-python-4.2.0/auth0/management/users_by_email.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/rest.py` & `auth0-python-4.2.0/auth0/rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/rest_async.py` & `auth0-python-4.2.0/auth0/rest_async.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_base.py` & `auth0-python-4.2.0/auth0/test/authentication/test_base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_database.py` & `auth0-python-4.2.0/auth0/test/authentication/test_database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_delegated.py` & `auth0-python-4.2.0/auth0/test/authentication/test_delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_enterprise.py` & `auth0-python-4.2.0/auth0/test/authentication/test_enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_get_token.py` & `auth0-python-4.2.0/auth0/test/authentication/test_get_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_passwordless.py` & `auth0-python-4.2.0/auth0/test/authentication/test_passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_revoke_token.py` & `auth0-python-4.2.0/auth0/test/authentication/test_revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_social.py` & `auth0-python-4.2.0/auth0/test/authentication/test_social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/authentication/test_token_verifier.py` & `auth0-python-4.2.0/auth0/test/authentication/test_token_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,22 @@
         verifier = SymmetricSignatureVerifier("some secret")
         self.assertEqual(verifier._algorithm, "HS256")
 
     def test_asymmetric_verifier_uses_rs256_alg(self):
         verifier = AsymmetricSignatureVerifier("some URL")
         self.assertEqual(verifier._algorithm, "RS256")
 
+    def test_asymmetric_verifier_uses_default_jwks_cache_ttl(self):
+        verifier = AsymmetricSignatureVerifier("some URL")
+        self.assertEqual(verifier._fetcher._cache_ttl, JwksFetcher.CACHE_TTL)
+
+    def test_asymmetric_verifier_uses_provided_jwks_cache_ttl(self):
+        verifier = AsymmetricSignatureVerifier("some URL", cache_ttl=3600)
+        self.assertEqual(verifier._fetcher._cache_ttl, 3600)
+
     def test_symmetric_verifier_fetches_key(self):
         verifier = SymmetricSignatureVerifier("some secret")
         key = verifier._fetch_key()
 
         self.assertEqual(verifier._shared_secret, "some secret")
         self.assertEqual(key, "some secret")
```

### Comparing `auth0-python-4.1.1/auth0/test/management/test_actions.py` & `auth0-python-4.2.0/auth0/test/management/test_actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_atack_protection.py` & `auth0-python-4.2.0/auth0/test/management/test_atack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_auth0.py` & `auth0-python-4.2.0/auth0/test/management/test_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_blacklists.py` & `auth0-python-4.2.0/auth0/test/management/test_blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_branding.py` & `auth0-python-4.2.0/auth0/test/management/test_branding.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_client_credentials.py` & `auth0-python-4.2.0/auth0/test/management/test_client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_client_grants.py` & `auth0-python-4.2.0/auth0/test/management/test_client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_clients.py` & `auth0-python-4.2.0/auth0/test/management/test_clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_connections.py` & `auth0-python-4.2.0/auth0/test/management/test_connections.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_custom_domains.py` & `auth0-python-4.2.0/auth0/test/management/test_custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_device_credentials.py` & `auth0-python-4.2.0/auth0/test/management/test_device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_email_endpoints.py` & `auth0-python-4.2.0/auth0/test/management/test_email_endpoints.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_emails.py` & `auth0-python-4.2.0/auth0/test/management/test_emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_grants.py` & `auth0-python-4.2.0/auth0/test/management/test_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_guardian.py` & `auth0-python-4.2.0/auth0/test/management/test_guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_hooks.py` & `auth0-python-4.2.0/auth0/test/management/test_hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_jobs.py` & `auth0-python-4.2.0/auth0/test/management/test_jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_log_streams.py` & `auth0-python-4.2.0/auth0/test/management/test_log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_logs.py` & `auth0-python-4.2.0/auth0/test/management/test_logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_organizations.py` & `auth0-python-4.2.0/auth0/test/management/test_organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_prompts.py` & `auth0-python-4.2.0/auth0/test/management/test_prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_resource_servers.py` & `auth0-python-4.2.0/auth0/test/management/test_resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_rest.py` & `auth0-python-4.2.0/auth0/test/management/test_rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_roles.py` & `auth0-python-4.2.0/auth0/test/management/test_roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_rules.py` & `auth0-python-4.2.0/auth0/test/management/test_rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_rules_configs.py` & `auth0-python-4.2.0/auth0/test/management/test_rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_stats.py` & `auth0-python-4.2.0/auth0/test/management/test_stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_tenants.py` & `auth0-python-4.2.0/auth0/test/management/test_tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_tickets.py` & `auth0-python-4.2.0/auth0/test/management/test_tickets.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_user_blocks.py` & `auth0-python-4.2.0/auth0/test/management/test_user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_users.py` & `auth0-python-4.2.0/auth0/test/management/test_users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test/management/test_users_by_email.py` & `auth0-python-4.2.0/auth0/test/management/test_users_by_email.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test_async/test_async_auth0.py` & `auth0-python-4.2.0/auth0/test_async/test_async_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test_async/test_async_token_verifier.py` & `auth0-python-4.2.0/auth0/test_async/test_async_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0/test_async/test_asyncify.py` & `auth0-python-4.2.0/auth0/test_async/test_asyncify.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/auth0_python.egg-info/PKG-INFO` & `auth0-python-4.2.0/auth0_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.1.1
+Version: 4.2.0
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.1.1 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.2.0 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.1.1/auth0_python.egg-info/SOURCES.txt` & `auth0-python-4.2.0/auth0_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auth0-python-4.1.1/setup.py` & `auth0-python-4.2.0/setup.py`

 * *Files identical despite different names*

