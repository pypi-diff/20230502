# Comparing `tmp/core_website_app-2.2.0.tar.gz` & `tmp/core_website_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/core_website_app-2.2.0.tar", last modified: Thu Feb 23 20:34:59 2023, max compression
+gzip compressed data, was "core_website_app-2.3.0.tar", last modified: Tue May  2 19:48:37 2023, max compression
```

## Comparing `core_website_app-2.2.0.tar` & `core_website_app-2.3.0.tar`

### file list

```diff
@@ -1,181 +1,182 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2023-02-23 20:34:52.000000 core_website_app-2.2.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2023-02-23 20:34:59.000000 core_website_app-2.2.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-02-23 20:34:52.000000 core_website_app-2.2.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3597 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/admin.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/commons/enums.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      208 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       24 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/account_request/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/account_request/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2212 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/contact_message/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      938 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/contact_message/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/help/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/help/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      780 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/help/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/privacy_policy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/privacy_policy/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/privacy_policy/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/rules_of_behavior/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/rules_of_behavior/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/rules_of_behavior/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/components/terms_of_use/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/terms_of_use/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/components/terms_of_use/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2449 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/rest/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2934 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/account_request/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1553 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/account_request/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/account_request/tests.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5445 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/account_request/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/rest/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      457 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/contact_message/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/contact_message/tests.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5620 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/contact_message/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1870 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/css/messages.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/messages.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/messages.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4034 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/user_requests.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      273 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/user_requests.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-02-23 20:34:52.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/user/css/list.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/static/core_website_app/user/js/user_account_req.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/account_requests/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/account_requests/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1913 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1471 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/email/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      422 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/email/contact_message_for_admin.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      385 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/email/request_account_approved.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/email/request_account_denied.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/email/request_account_for_admin.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      331 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/email/request_account_for_user.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/help.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/confirm_delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/read.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/user_requests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/user_requests/accept.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/user_requests/deny.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/modals/user_requests/error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/privacy_policy.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/rules_of_behavior.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/terms_of_use.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/user_requests.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      933 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/contact.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/footer_menu.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3418 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/help.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      330 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/privacy-policy.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      239 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/request_error.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1179 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/request_new_account.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      436 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/rules_of_behavior.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/templates/core_website_app/user/terms-of-use.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      341 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/utils/custom_context_processors.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4935 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1997 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/core_website_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7550 2023-02-23 20:34:53.000000 core_website_app-2.2.0/core_website_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:57.000000 core_website_app-2.2.0/core_website_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2023-02-23 20:34:56.000000 core_website_app-2.2.0/core_website_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6048 2023-02-23 20:34:56.000000 core_website_app-2.2.0/core_website_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-02-23 20:34:56.000000 core_website_app-2.2.0/core_website_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-02-23 20:34:56.000000 core_website_app-2.2.0/core_website_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2023-02-23 20:34:56.000000 core_website_app-2.2.0/core_website_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-02-23 20:34:54.000000 core_website_app-2.2.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-02-23 20:34:54.000000 core_website_app-2.2.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-02-23 20:34:54.000000 core_website_app-2.2.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-02-23 20:34:59.000000 core_website_app-2.2.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2023-02-23 20:34:54.000000 core_website_app-2.2.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:58.000000 core_website_app-2.2.0/tests/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/commons/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8580 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/account_request/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/contact_message/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5239 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/contact_message/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/help/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/help/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1443 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/help/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/privacy_policy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/privacy_policy/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1676 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/privacy_policy/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/rules_of_behavior/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/rules_of_behavior/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1787 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/rules_of_behavior/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/terms_of_use/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/terms_of_use/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/terms_of_use/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3566 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/components/web_page/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/rest/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/rest/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8169 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/rest/account_request/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/rest/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/rest/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7339 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/rest/contact_message/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2229 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:59.000000 core_website_app-2.2.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-02-23 20:34:54.000000 core_website_app-2.2.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.676342 core_website_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:48:25.000000 core_website_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2023-05-02 19:48:25.000000 core_website_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2023-05-02 19:48:37.671443 core_website_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-05-02 19:48:25.000000 core_website_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.676558 core_website_app-2.3.0/core_website_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3597 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/admin.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.840772 core_website_app-2.3.0/core_website_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/commons/enums.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      208 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.853822 core_website_app-2.3.0/core_website_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       24 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.894073 core_website_app-2.3.0/core_website_app/components/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/account_request/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/account_request/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.934782 core_website_app-2.3.0/core_website_app/components/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2212 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/contact_message/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      938 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/contact_message/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.001684 core_website_app-2.3.0/core_website_app/components/help/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/help/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      780 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/help/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.032751 core_website_app-2.3.0/core_website_app/components/privacy_policy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/privacy_policy/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/privacy_policy/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.071099 core_website_app-2.3.0/core_website_app/components/rules_of_behavior/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/rules_of_behavior/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/rules_of_behavior/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.094996 core_website_app-2.3.0/core_website_app/components/terms_of_use/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/terms_of_use/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/components/terms_of_use/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2449 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.122471 core_website_app-2.3.0/core_website_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.152957 core_website_app-2.3.0/core_website_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.243821 core_website_app-2.3.0/core_website_app/rest/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2934 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/account_request/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1553 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/account_request/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/account_request/tests.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5445 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/account_request/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.327566 core_website_app-2.3.0/core_website_app/rest/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      457 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/contact_message/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/contact_message/tests.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5620 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/contact_message/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1870 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.226688 core_website_app-2.3.0/core_website_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.244810 core_website_app-2.3.0/core_website_app/static/core_website_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.238654 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.357010 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/css/messages.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.423132 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/messages.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/messages.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4034 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/user_requests.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      273 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/user_requests.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.253918 core_website_app-2.3.0/core_website_app/static/core_website_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.458563 core_website_app-2.3.0/core_website_app/static/core_website_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/user/css/list.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.476836 core_website_app-2.3.0/core_website_app/static/core_website_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/static/core_website_app/user/js/user_account_req.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.265496 core_website_app-2.3.0/core_website_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.335985 core_website_app-2.3.0/core_website_app/templates/core_website_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.571540 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.589113 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/account_requests/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.606476 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/account_requests/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1913 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1471 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.622450 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.638862 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.727298 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/email/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      422 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/email/contact_message_for_admin.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      385 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/email/request_account_approved.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/email/request_account_denied.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/email/request_account_for_admin.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      331 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/email/request_account_for_user.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/help.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.331223 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.774975 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/confirm_delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/read.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.829634 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/user_requests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/user_requests/accept.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/user_requests/deny.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/modals/user_requests/error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/privacy_policy.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/rules_of_behavior.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/terms_of_use.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/user_requests.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:36.957113 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      933 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/contact.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/footer_menu.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3418 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/help.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      330 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/privacy-policy.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      239 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/request_error.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1179 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/request_new_account.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      436 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/rules_of_behavior.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/templates/core_website_app/user/terms-of-use.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.003997 core_website_app-2.3.0/core_website_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      341 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/utils/custom_context_processors.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.023716 core_website_app-2.3.0/core_website_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.063437 core_website_app-2.3.0/core_website_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4935 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1997 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.130291 core_website_app-2.3.0/core_website_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7550 2023-05-02 19:48:25.000000 core_website_app-2.3.0/core_website_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:35.779786 core_website_app-2.3.0/core_website_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2023-05-02 19:48:34.000000 core_website_app-2.3.0/core_website_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6059 2023-05-02 19:48:35.000000 core_website_app-2.3.0/core_website_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:48:34.000000 core_website_app-2.3.0/core_website_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-05-02 19:48:34.000000 core_website_app-2.3.0/core_website_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2023-05-02 19:48:34.000000 core_website_app-2.3.0/core_website_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:48:30.000000 core_website_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-05-02 19:48:30.000000 core_website_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:48:30.000000 core_website_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:48:37.697004 core_website_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2023-05-02 19:48:30.000000 core_website_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.165497 core_website_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:30.000000 core_website_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.180508 core_website_app-2.3.0/tests/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:30.000000 core_website_app-2.3.0/tests/commons/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.198509 core_website_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:30.000000 core_website_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.262492 core_website_app-2.3.0/tests/components/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:30.000000 core_website_app-2.3.0/tests/components/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8580 2023-05-02 19:48:30.000000 core_website_app-2.3.0/tests/components/account_request/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.319978 core_website_app-2.3.0/tests/components/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/contact_message/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5239 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/contact_message/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.351917 core_website_app-2.3.0/tests/components/help/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/help/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1443 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/help/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.379968 core_website_app-2.3.0/tests/components/privacy_policy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/privacy_policy/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1676 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/privacy_policy/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.408757 core_website_app-2.3.0/tests/components/rules_of_behavior/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/rules_of_behavior/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1787 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/rules_of_behavior/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.448483 core_website_app-2.3.0/tests/components/terms_of_use/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/terms_of_use/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/terms_of_use/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.477349 core_website_app-2.3.0/tests/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3566 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/components/web_page/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.490796 core_website_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.526915 core_website_app-2.3.0/tests/rest/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/rest/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8169 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/rest/account_request/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.559444 core_website_app-2.3.0/tests/rest/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/rest/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7339 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/rest/contact_message/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.574393 core_website_app-2.3.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2229 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.593753 core_website_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.613371 core_website_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:32.000000 core_website_app-2.3.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.634989 core_website_app-2.3.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:33.000000 core_website_app-2.3.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:37.653925 core_website_app-2.3.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:33.000000 core_website_app-2.3.0/tests/views/user/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `core_website_app-2.2.0/PKG-INFO` & `core_website_app-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_website_app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Basic web functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_website_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ================
         Core Website App
```

### Comparing `core_website_app-2.2.0/README.rst` & `core_website_app-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/__init__.py` & `core_website_app-2.3.0/core_website_app/__init__.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/admin.py` & `core_website_app-2.3.0/core_website_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/account_request/api.py` & `core_website_app-2.3.0/core_website_app/components/account_request/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/account_request/models.py` & `core_website_app-2.3.0/core_website_app/components/account_request/models.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/contact_message/api.py` & `core_website_app-2.3.0/core_website_app/components/contact_message/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/contact_message/models.py` & `core_website_app-2.3.0/core_website_app/components/contact_message/models.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/help/api.py` & `core_website_app-2.3.0/core_website_app/components/help/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/privacy_policy/api.py` & `core_website_app-2.3.0/core_website_app/components/privacy_policy/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/rules_of_behavior/api.py` & `core_website_app-2.3.0/core_website_app/components/rules_of_behavior/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/components/terms_of_use/api.py` & `core_website_app-2.3.0/core_website_app/components/terms_of_use/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/menus.py` & `core_website_app-2.3.0/core_website_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/migrations/0001_initial.py` & `core_website_app-2.3.0/core_website_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/rest/account_request/abstract_views.py` & `core_website_app-2.3.0/core_website_app/rest/account_request/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/rest/account_request/serializers.py` & `core_website_app-2.3.0/core_website_app/rest/account_request/serializers.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/rest/account_request/views.py` & `core_website_app-2.3.0/core_website_app/rest/account_request/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/rest/contact_message/views.py` & `core_website_app-2.3.0/core_website_app/rest/contact_message/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/rest/urls.py` & `core_website_app-2.3.0/core_website_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/settings.py` & `core_website_app-2.3.0/core_website_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/messages.js` & `core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/messages.js`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/static/core_website_app/admin/js/user_requests.js` & `core_website_app-2.3.0/core_website_app/static/core_website_app/admin/js/user_requests.js`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/user/contact.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/user/contact.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/user/help.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/user/help.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/templates/core_website_app/user/request_new_account.html` & `core_website_app-2.3.0/core_website_app/templates/core_website_app/user/request_new_account.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/urls.py` & `core_website_app-2.3.0/core_website_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/views/admin/ajax.py` & `core_website_app-2.3.0/core_website_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/views/admin/views.py` & `core_website_app-2.3.0/core_website_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/views/user/forms.py` & `core_website_app-2.3.0/core_website_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app/views/user/views.py` & `core_website_app-2.3.0/core_website_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/core_website_app.egg-info/PKG-INFO` & `core_website_app-2.3.0/core_website_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-website-app
-Version: 2.2.0
+Version: 2.3.0
 Summary: Basic web functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_website_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ================
         Core Website App
```

### Comparing `core_website_app-2.2.0/core_website_app.egg-info/SOURCES.txt` & `core_website_app-2.3.0/core_website_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_website_app/__init__.py
```

### Comparing `core_website_app-2.2.0/setup.py` & `core_website_app-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_website_app",
-    version="2.2.0",
+    version="2.3.0",
     description="Basic web functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_website_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_website_app-2.2.0/tests/components/account_request/tests_unit.py` & `core_website_app-2.3.0/tests/components/account_request/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/contact_message/tests_int.py` & `core_website_app-2.3.0/tests/components/contact_message/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/contact_message/tests_unit.py` & `core_website_app-2.3.0/tests/components/contact_message/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/help/tests_unit.py` & `core_website_app-2.3.0/tests/components/help/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/privacy_policy/tests_unit.py` & `core_website_app-2.3.0/tests/components/privacy_policy/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/rules_of_behavior/tests_unit.py` & `core_website_app-2.3.0/tests/components/rules_of_behavior/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/terms_of_use/tests_unit.py` & `core_website_app-2.3.0/tests/components/terms_of_use/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/components/web_page/tests_unit.py` & `core_website_app-2.3.0/tests/components/web_page/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/rest/account_request/tests_permission.py` & `core_website_app-2.3.0/tests/rest/account_request/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/rest/contact_message/tests_permission.py` & `core_website_app-2.3.0/tests/rest/contact_message/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.2.0/tests/test_settings.py` & `core_website_app-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

