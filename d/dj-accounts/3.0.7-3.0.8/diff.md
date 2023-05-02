# Comparing `tmp/dj-accounts-3.0.7.tar.gz` & `tmp/dj-accounts-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-accounts-3.0.7.tar", last modified: Sun Dec 18 21:13:14 2022, max compression
+gzip compressed data, was "dj-accounts-3.0.8.tar", last modified: Tue May  2 19:57:22 2023, max compression
```

## Comparing `dj-accounts-3.0.7.tar` & `dj-accounts-3.0.8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.077648 dj-accounts-3.0.7/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1145 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/LICENSE
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      100 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/MANIFEST.in
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1545 2022-12-18 21:13:14.077648 dj-accounts-3.0.7/PKG-INFO
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      628 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/README.md
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.629639 dj-accounts-3.0.7/accounts_pkg/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/accounts_pkg/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       79 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/accounts_pkg/api_urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/accounts_pkg/asgi.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4139 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/accounts_pkg/settings-multi-auth.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4119 2022-11-14 21:52:13.000000 dj-accounts-3.0.7/accounts_pkg/settings.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      378 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/accounts_pkg/urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/accounts_pkg/wsgi.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.861644 dj-accounts-3.0.7/dj_accounts/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      153 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/apps.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      838 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/backends.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8484 2022-10-15 02:16:36.000000 dj-accounts-3.0.7/dj_accounts/forms.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4755 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/serializers.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.261632 dj-accounts-3.0.7/dj_accounts/templates/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.933645 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      335 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/auth_base.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      573 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/confirm_email_template.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      200 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/email_verification_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      949 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/login.html
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.933645 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.957646 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1108 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      710 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      840 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/first_name.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      797 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/gender.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      809 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/last_name.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      634 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      655 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/password.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/password1.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/password2.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      668 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/phone.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      236 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      735 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/username.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1052 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/login-tabs.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      938 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/login_with_email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      940 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/login_with_phone.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/logo.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      383 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/social_login.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      954 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_confirm.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      659 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_done.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      615 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      555 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      132 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_subject.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/phone_verification_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       34 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/profile.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      553 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/profile_base.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      449 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/register.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1679 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/sidebar.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      304 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/update_email_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      313 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/update_phone_number_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      339 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/update_user_data_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      813 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/update_user_password_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/verify_phone.html
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.073648 dj-accounts-3.0.7/dj_accounts/tests/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      163 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/apps.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      718 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/factories.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.073648 dj-accounts-3.0.7/dj_accounts/tests/migrations/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3188 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/migrations/0001_initial.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/migrations/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      456 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/mocks.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2927 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/models.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2843 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_backends.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    20397 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_forms.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8251 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_serializers.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      550 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_tokens.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3918 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1425 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_verify_phone.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    24255 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_view_api.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    29865 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/tests/test_views.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.073648 dj-accounts-3.0.7/dj_accounts/urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/__init__.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.073648 dj-accounts-3.0.7/dj_accounts/urls/api_urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/api_urls/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1317 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/api_urls/urls_auth_api.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      386 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/api_urls/urls_profile_api.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.073648 dj-accounts-3.0.7/dj_accounts/urls/site_urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/site_urls/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2334 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/site_urls/urls_auth.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      352 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/urls/site_urls/urls_profile.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1120 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/utils.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      911 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/dj_accounts/verify_phone.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8724 2022-11-14 22:10:01.000000 dj-accounts-3.0.7/dj_accounts/views.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    10759 2022-12-18 21:10:53.000000 dj-accounts-3.0.7/dj_accounts/views_api.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:13.865644 dj-accounts-3.0.7/dj_accounts.egg-info/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1545 2022-12-18 21:13:10.000000 dj-accounts-3.0.7/dj_accounts.egg-info/PKG-INFO
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3716 2022-12-18 21:13:12.000000 dj-accounts-3.0.7/dj_accounts.egg-info/SOURCES.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        1 2022-12-18 21:13:10.000000 dj-accounts-3.0.7/dj_accounts.egg-info/dependency_links.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       25 2022-12-18 21:13:11.000000 dj-accounts-3.0.7/dj_accounts.egg-info/top_level.txt
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2022-12-18 21:13:14.077648 dj-accounts-3.0.7/docs/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/docs/APIAuth.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/docs/APIProfile.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1371 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/docs/PhoneVerificationService.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/docs/Profile.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/docs/SessionAuth.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3630 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/docs/index.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      108 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/pyproject.toml
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      906 2022-12-18 21:13:14.077648 dj-accounts-3.0.7/setup.cfg
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       38 2022-10-14 11:08:00.000000 dj-accounts-3.0.7/setup.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.831144 dj-accounts-3.0.8/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1145 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/LICENSE
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      100 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/MANIFEST.in
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1902 2023-05-02 19:57:22.835145 dj-accounts-3.0.8/PKG-INFO
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      628 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/README.md
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.403144 dj-accounts-3.0.8/accounts_pkg/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/accounts_pkg/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       79 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/api_urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/accounts_pkg/asgi.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4139 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/settings-multi-auth.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4119 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/settings.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      378 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/accounts_pkg/wsgi.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.435145 dj-accounts-3.0.8/dj_accounts/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/dj_accounts/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      153 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/apps.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      838 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/backends.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8485 2023-05-02 17:05:25.000000 dj-accounts-3.0.8/dj_accounts/forms.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4695 2023-05-02 17:11:11.000000 dj-accounts-3.0.8/dj_accounts/serializers.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.307144 dj-accounts-3.0.8/dj_accounts/templates/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.599145 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      335 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/auth_base.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      573 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/confirm_email_template.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      202 2023-05-02 17:52:57.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/email_verification_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      948 2023-05-02 17:54:18.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/login.html
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.603145 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.663144 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1108 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      710 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      840 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/first_name.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      797 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/gender.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      809 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/last_name.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      634 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      655 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password1.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password2.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      668 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/phone.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      236 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      735 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/username.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1052 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login-tabs.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      938 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      940 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_phone.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/logo.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      383 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/social_login.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      954 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_confirm.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      659 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_done.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      615 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      555 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      132 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_subject.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/phone_verification_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       34 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/profile.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      553 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/profile_base.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      449 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/register.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1652 2023-05-02 18:00:25.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/sidebar.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      304 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_email_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      313 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_phone_number_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      339 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_user_data_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      813 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_user_password_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/verify_phone.html
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/tests/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      163 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/apps.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      718 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/factories.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/tests/migrations/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3188 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/migrations/0001_initial.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/migrations/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      456 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/mocks.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2927 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/models.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2843 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_backends.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    20397 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_forms.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8201 2023-05-02 19:50:05.000000 dj-accounts-3.0.8/dj_accounts/tests/test_serializers.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      550 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_tokens.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3918 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1425 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_verify_phone.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    24255 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_view_api.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    29865 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_views.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/__init__.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/urls/api_urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/api_urls/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1317 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/api_urls/urls_auth_api.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      386 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/api_urls/urls_profile_api.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.707145 dj-accounts-3.0.8/dj_accounts/urls/site_urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/site_urls/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2334 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/site_urls/urls_auth.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      352 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/site_urls/urls_profile.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1120 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/utils.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      911 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/verify_phone.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8724 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/views.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    10759 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/views_api.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.435145 dj-accounts-3.0.8/dj_accounts.egg-info/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1902 2023-05-02 19:57:20.000000 dj-accounts-3.0.8/dj_accounts.egg-info/PKG-INFO
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3716 2023-05-02 19:57:21.000000 dj-accounts-3.0.8/dj_accounts.egg-info/SOURCES.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        1 2023-05-02 19:57:20.000000 dj-accounts-3.0.8/dj_accounts.egg-info/dependency_links.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       25 2023-05-02 19:57:20.000000 dj-accounts-3.0.8/dj_accounts.egg-info/top_level.txt
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.795144 dj-accounts-3.0.8/docs/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/APIAuth.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/APIProfile.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1371 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/PhoneVerificationService.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/Profile.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/SessionAuth.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3630 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/docs/index.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      108 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/pyproject.toml
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      906 2023-05-02 19:57:22.835145 dj-accounts-3.0.8/setup.cfg
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       38 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/setup.py
```

### Comparing `dj-accounts-3.0.7/LICENSE` & `dj-accounts-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/PKG-INFO` & `dj-accounts-3.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,62 @@
 Metadata-Version: 2.1
 Name: dj-accounts
-Version: 3.0.7
+Version: 3.0.8
 Summary: this application is for handling all auth operations
 Home-page: https://github.com/fritill-team/django-accounts
 Author: fritill
 Author-email: dev@fritill.com
 License: MIT
+Description: ## Installation
+        
+        ```cd
+        pip install dj-accounts
+        ```
+        
+        ## Configuration
+        
+        ```python
+        INSTALLED_APPS = [
+            ...,
+        
+            'dj_accounts',
+        ]
+        ```
+        
+        ### in your settings.py
+        
+        ```python
+        
+        # for custom register form
+        REGISTER_FORM = 'users.form.RegisterForm'
+        
+        
+        
+        # django restFramework settings
+        REST_FRAMEWORK = {
+            'DEFAULT_AUTHENTICATION_CLASSES': [
+                'rest_framework_simplejwt.authentication.JWTAuthentication',
+            ],
+        
+        }
+        ```
+        
+        
+        
+        ### in your settings.py
+        ```python
+        # django restFramework settings
+        REST_FRAMEWORK = {
+            'DEFAULT_AUTHENTICATION_CLASSES': [
+                'rest_framework_simplejwt.authentication.JWTAuthentication',
+            ],
+        
+        }
+        
+        ```
 Keywords: django translation custom
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -17,57 +64,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Installation
-
-```cd
-pip install dj-accounts
-```
-
-## Configuration
-
-```python
-INSTALLED_APPS = [
-    ...,
-
-    'dj_accounts',
-]
-```
-
-### in your settings.py
-
-```python
-
-# for custom register form
-REGISTER_FORM = 'users.form.RegisterForm'
-
-
-
-# django restFramework settings
-REST_FRAMEWORK = {
-    'DEFAULT_AUTHENTICATION_CLASSES': [
-        'rest_framework_simplejwt.authentication.JWTAuthentication',
-    ],
-
-}
-```
-
-
-
-### in your settings.py
-```python
-# django restFramework settings
-REST_FRAMEWORK = {
-    'DEFAULT_AUTHENTICATION_CLASSES': [
-        'rest_framework_simplejwt.authentication.JWTAuthentication',
-    ],
-
-}
-
-```
-
```

### Comparing `dj-accounts-3.0.7/README.md` & `dj-accounts-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/accounts_pkg/settings-multi-auth.py` & `dj-accounts-3.0.8/accounts_pkg/settings-multi-auth.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/accounts_pkg/settings.py` & `dj-accounts-3.0.8/accounts_pkg/settings.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/backends.py` & `dj-accounts-3.0.8/dj_accounts/backends.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/forms.py` & `dj-accounts-3.0.8/dj_accounts/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     class Meta:
         model = UserModel
         fields = ('first_name', 'last_name')
 
     def clean_first_name(self):
         first_name = self.cleaned_data.get('first_name', None)
         if not first_name:
-            raise ValidationError(_("Please Enter the new first"), code="required")
+            raise ValidationError(_("Please Enter the first name"), code="required")
 
         return first_name
 
     def clean_last_name(self):
         last_name = self.cleaned_data.get('last_name')
         if not last_name:
             raise ValidationError("Please Enter the last name", code="required")
```

### Comparing `dj-accounts-3.0.7/dj_accounts/serializers.py` & `dj-accounts-3.0.8/dj_accounts/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def get_authentication_form(self):
         if getattr(settings, 'MULTIPLE_AUTHENTICATION_ACTIVE', False):
             return MultipleLoginForm
         return getattr(settings, 'LOGIN_FORM', AuthenticationForm)
 
 
 class LogoutSerializer(serializers.Serializer):
-    refresh = serializers.CharField(required=True, help_text=_("Required, please provide your refresh token"))
+    refresh = serializers.CharField(required=True)
 
     def save(self, **kwargs):
         try:
             RefreshToken(self.validated_data['refresh']).blacklist()
         except TokenError:
             raise ValidationError({"refresh": _('Invalid token.')})
```

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/confirm_email_template.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/confirm_email_template.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/login.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/login.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {% block page_title %}
 {% translate "Login" %}
 {% endblock %}
 
 {% block content %}
 <div class="card">
   <div class="card-body login-card-body">
-    <p class="login-box-msg">{% translate 'Sign in to start your session' %}</p>
+    <p class="login-box-msg">{% translate 'Log in to start your session' %}</p>
 
     {% include 'dj_accounts/partials/login-tabs.html' %}
 
     {% include 'dj_accounts/partials/social_login.html' %}
 
     <p class="mb-1">
       <a href="{% url "password_reset" %}">{% translate 'I forgot my password' %}</a>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'dj_accounts/auth_base.html' %} {% load static i18n %} {% block
 styles %}
  {% endblock %} {% block page_title %} {% translate "Login" %} {% endblock %}
 {% block content %}
-{% translate 'Sign in to start your session' %}
+{% translate 'Log in to start your session' %}
 {% include 'dj_accounts/partials/login-tabs.html' %} {% include 'dj_accounts/
 partials/social_login.html' %}
  %}">{% translate 'I forgot my password' %}
 {%_translate_'Register_a_new_membership'_%}
 {% endblock %}
```

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/email.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/first_name.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/first_name.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/gender.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/gender.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/last_name.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/last_name.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/password.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/password1.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password1.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/password2.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password2.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/phone.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/phone.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/fields/username.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/username.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/login-tabs.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login-tabs.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/login_with_email.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/partials/login_with_phone.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_phone.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_confirm.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_done.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_email.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/password_reset_form.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/profile_base.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/profile_base.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/sidebar.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/sidebar.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% load static %}
 <!-- Main Sidebar Container -->
 <aside class="main-sidebar sidebar-dark-primary elevation-4">
   <!-- Brand Logo -->
   <a href="{% url " site:main:home" %}" class="brand-link">
   <img assets src="{% static "/img/AdminLTELogo.png" %}" alt="AdminLTE Logo" class="brand-image img-circle elevation-3"
   style="opacity: .8">
-  <span class="brand-text font-weight-light">{% translate 'Quran API' %}</span>
+  <span class="brand-text font-weight-light"></span>
   </a>
 
   <!-- Sidebar -->
   <div class="sidebar" data-list='{{ user_sidebar|jsonify }}'>
     <!-- Sidebar user panel (optional) -->
     {% if request.user.is_authenticated %}
     <div class="user-panel mt-3 pb-3 d-flex">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load jsonify %} {% load i18n %} {% load static %}
  %}" class="brand-link">
 mg/AdminLTELogo.png" %}" alt="AdminLTE Logo" class="brand-image img-circle
-elevation-3" style="opacity: .8"> {% translate 'Quran API' %}
+elevation-3" style="opacity: .8">
 
  {% if request.user.is_authenticated %}
 [User Image]
 Alexander_Pierce
 {% endif %}
 [Unknown INPUT type]
```

### Comparing `dj-accounts-3.0.7/dj_accounts/templates/dj_accounts/update_user_password_form.html` & `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_user_password_form.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/factories.py` & `dj-accounts-3.0.8/dj_accounts/tests/factories.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/migrations/0001_initial.py` & `dj-accounts-3.0.8/dj_accounts/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/models.py` & `dj-accounts-3.0.8/dj_accounts/tests/models.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_backends.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_forms.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_serializers.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def setUp(self):
         self.serializer = LogoutSerializer(data={'refresh': 'test'})
 
     def test_it_has_refresh_field(self):
         self.assertIn('refresh', self.serializer.fields)
 
     def test_refresh_field_help_text(self):
-        self.assertEquals(self.serializer.fields['refresh'].help_text, _("Required, please provide your refresh token"))
+        self.assertEquals(self.serializer.fields['refresh'].help_text)
 
     def test_refresh_field_is_instance_of_char_field(self):
         self.assertIsInstance(self.serializer.fields['refresh'], serializers.CharField)
 
     def test_refresh_field_is_required(self):
         self.assertTrue(self.serializer.fields['refresh'].required)
```

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_tokens.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_urls.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_verify_phone.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_verify_phone.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_view_api.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_view_api.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/tests/test_views.py` & `dj-accounts-3.0.8/dj_accounts/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/urls/api_urls/urls_auth_api.py` & `dj-accounts-3.0.8/dj_accounts/urls/api_urls/urls_auth_api.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/urls/site_urls/urls_auth.py` & `dj-accounts-3.0.8/dj_accounts/urls/site_urls/urls_auth.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/utils.py` & `dj-accounts-3.0.8/dj_accounts/utils.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/verify_phone.py` & `dj-accounts-3.0.8/dj_accounts/verify_phone.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/views.py` & `dj-accounts-3.0.8/dj_accounts/views.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts/views_api.py` & `dj-accounts-3.0.8/dj_accounts/views_api.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/dj_accounts.egg-info/PKG-INFO` & `dj-accounts-3.0.8/dj_accounts.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,62 @@
 Metadata-Version: 2.1
 Name: dj-accounts
-Version: 3.0.7
+Version: 3.0.8
 Summary: this application is for handling all auth operations
 Home-page: https://github.com/fritill-team/django-accounts
 Author: fritill
 Author-email: dev@fritill.com
 License: MIT
+Description: ## Installation
+        
+        ```cd
+        pip install dj-accounts
+        ```
+        
+        ## Configuration
+        
+        ```python
+        INSTALLED_APPS = [
+            ...,
+        
+            'dj_accounts',
+        ]
+        ```
+        
+        ### in your settings.py
+        
+        ```python
+        
+        # for custom register form
+        REGISTER_FORM = 'users.form.RegisterForm'
+        
+        
+        
+        # django restFramework settings
+        REST_FRAMEWORK = {
+            'DEFAULT_AUTHENTICATION_CLASSES': [
+                'rest_framework_simplejwt.authentication.JWTAuthentication',
+            ],
+        
+        }
+        ```
+        
+        
+        
+        ### in your settings.py
+        ```python
+        # django restFramework settings
+        REST_FRAMEWORK = {
+            'DEFAULT_AUTHENTICATION_CLASSES': [
+                'rest_framework_simplejwt.authentication.JWTAuthentication',
+            ],
+        
+        }
+        
+        ```
 Keywords: django translation custom
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -17,57 +64,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Installation
-
-```cd
-pip install dj-accounts
-```
-
-## Configuration
-
-```python
-INSTALLED_APPS = [
-    ...,
-
-    'dj_accounts',
-]
-```
-
-### in your settings.py
-
-```python
-
-# for custom register form
-REGISTER_FORM = 'users.form.RegisterForm'
-
-
-
-# django restFramework settings
-REST_FRAMEWORK = {
-    'DEFAULT_AUTHENTICATION_CLASSES': [
-        'rest_framework_simplejwt.authentication.JWTAuthentication',
-    ],
-
-}
-```
-
-
-
-### in your settings.py
-```python
-# django restFramework settings
-REST_FRAMEWORK = {
-    'DEFAULT_AUTHENTICATION_CLASSES': [
-        'rest_framework_simplejwt.authentication.JWTAuthentication',
-    ],
-
-}
-
-```
-
```

### Comparing `dj-accounts-3.0.7/dj_accounts.egg-info/SOURCES.txt` & `dj-accounts-3.0.8/dj_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/docs/PhoneVerificationService.md` & `dj-accounts-3.0.8/docs/PhoneVerificationService.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/docs/index.md` & `dj-accounts-3.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.7/setup.cfg` & `dj-accounts-3.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-accounts
-version = 3.0.7
+version = 3.0.8
 author = fritill
 author_email = dev@fritill.com
 description = this application is for handling all auth operations
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritill-team/django-accounts
 license = MIT
```

