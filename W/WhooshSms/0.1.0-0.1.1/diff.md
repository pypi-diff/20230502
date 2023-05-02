# Comparing `tmp/WhooshSms-0.1.0.tar.gz` & `tmp/WhooshSms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WhooshSms-0.1.0.tar", last modified: Tue May  2 11:26:59 2023, max compression
+gzip compressed data, was "WhooshSms-0.1.1.tar", last modified: Tue May  2 11:32:31 2023, max compression
```

## Comparing `WhooshSms-0.1.0.tar` & `WhooshSms-0.1.1.tar`

### file list

```diff
@@ -1,851 +1,851 @@
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.083519 WhooshSms-0.1.0/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1088 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/LICENSE
--rw-r--r--   0 nikhilm    (501) staff       (20)      117 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/MANIFEST.in
--rw-r--r--   0 nikhilm    (501) staff       (20)    11744 2023-05-02 11:26:59.083615 WhooshSms-0.1.0/PKG-INFO
--rw-r--r--   0 nikhilm    (501) staff       (20)    10771 2023-05-02 11:01:10.000000 WhooshSms-0.1.0/README.md
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.987382 WhooshSms-0.1.0/WhooshSms.egg-info/
--rw-r--r--   0 nikhilm    (501) staff       (20)    11744 2023-05-02 11:26:58.000000 WhooshSms-0.1.0/WhooshSms.egg-info/PKG-INFO
--rw-r--r--   0 nikhilm    (501) staff       (20)    30370 2023-05-02 11:26:58.000000 WhooshSms-0.1.0/WhooshSms.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilm    (501) staff       (20)        1 2023-05-02 11:26:58.000000 WhooshSms-0.1.0/WhooshSms.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilm    (501) staff       (20)       77 2023-05-02 11:26:58.000000 WhooshSms-0.1.0/WhooshSms.egg-info/requires.txt
--rw-r--r--   0 nikhilm    (501) staff       (20)        7 2023-05-02 11:26:58.000000 WhooshSms-0.1.0/WhooshSms.egg-info/top_level.txt
--rw-r--r--   0 nikhilm    (501) staff       (20)      236 2023-05-02 11:26:59.084007 WhooshSms-0.1.0/setup.cfg
--rwxr-xr-x   0 nikhilm    (501) staff       (20)     1672 2023-05-02 11:25:12.000000 WhooshSms-0.1.0/setup.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.987695 WhooshSms-0.1.0/twilio/
--rw-r--r--   0 nikhilm    (501) staff       (20)       76 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.989225 WhooshSms-0.1.0/twilio/base/
--rw-r--r--   0 nikhilm    (501) staff       (20)        0 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8153 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/client_base.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2019 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/deserialize.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3011 2023-05-02 10:40:30.000000 WhooshSms-0.1.0/twilio/base/domain.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2890 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/exceptions.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      147 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/instance_context.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      148 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/instance_resource.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      144 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/list_resource.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1417 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/obsolete.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5181 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/page.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2039 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/serialize.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      280 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/base/values.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14614 2023-05-02 10:39:18.000000 WhooshSms-0.1.0/twilio/base/version.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.990121 WhooshSms-0.1.0/twilio/http/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3434 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/http/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4503 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/http/async_http_client.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3735 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/http/http_client.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2655 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/http/request.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      518 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/http/response.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4810 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/http/validation_client.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.990242 WhooshSms-0.1.0/twilio/jwt/
--rw-r--r--   0 nikhilm    (501) staff       (20)     5085 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.990474 WhooshSms-0.1.0/twilio/jwt/access_token/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2415 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/access_token/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4902 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/access_token/grants.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.990594 WhooshSms-0.1.0/twilio/jwt/client/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3982 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/client/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.990838 WhooshSms-0.1.0/twilio/jwt/taskrouter/
--rw-r--r--   0 nikhilm    (501) staff       (20)     5726 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/taskrouter/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4309 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/taskrouter/capabilities.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.990965 WhooshSms-0.1.0/twilio/jwt/validation/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3156 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/jwt/validation/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4100 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/request_validator.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.991089 WhooshSms-0.1.0/twilio/rest/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20879 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.991372 WhooshSms-0.1.0/twilio/rest/accounts/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/AccountsBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1168 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.991733 WhooshSms-0.1.0/twilio/rest/accounts/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2102 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5547 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/v1/auth_token_promotion.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.992124 WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1766 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19489 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/aws.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20007 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/public_key.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6551 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/accounts/v1/secondary_auth_token.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.992419 WhooshSms-0.1.0/twilio/rest/api/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1220 2023-05-02 10:33:52.000000 WhooshSms-0.1.0/twilio/rest/api/ApiBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8255 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.992534 WhooshSms-0.1.0/twilio/rest/api/v2010/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1805 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.994744 WhooshSms-0.1.0/twilio/rest/api/v2010/account/
--rw-r--r--   0 nikhilm    (501) staff       (20)    36206 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.995036 WhooshSms-0.1.0/twilio/rest/api/v2010/account/address/
--rw-r--r--   0 nikhilm    (501) staff       (20)    35858 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/address/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17044 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    47553 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/application.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17274 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/authorized_connect_app.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.996212 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21427 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    46239 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    46210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    45860 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    45930 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    46000 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    45930 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    45790 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3186 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/balance.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.998100 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/
--rw-r--r--   0 nikhilm    (501) staff       (20)    92392 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10658 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/event.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11932 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/feedback.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13986 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/feedback_summary.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    28363 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/notification.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23472 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/payment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38495 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/recording.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    77226 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/siprec.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    77116 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/stream.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5278 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/user_defined_message.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10898 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.998504 WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/
--rw-r--r--   0 nikhilm    (501) staff       (20)    41186 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    74737 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/participant.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    32729 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/recording.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26539 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/connect_app.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.999069 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/
--rw-r--r--   0 nikhilm    (501) staff       (20)    73374 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.999343 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20750 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18341 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    36935 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    37019 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    37103 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17989 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/key.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:58.999792 WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/
--rw-r--r--   0 nikhilm    (501) staff       (20)    53984 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5102 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/feedback.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27246 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/media.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4785 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/new_key.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4813 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/new_signing_key.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27505 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/notification.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22199 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.000086 WhooshSms-0.1.0/twilio/rest/api/v2010/account/queue/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22428 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/queue/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19131 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/queue/member.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.000373 WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/
--rw-r--r--   0 nikhilm    (501) staff       (20)    37769 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.000633 WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/add_on_result/
--rw-r--r--   0 nikhilm    (501) staff       (20)    19239 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19233 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19008 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/transcription.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26406 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/short_code.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17376 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/signing_key.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.000749 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2871 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.000996 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/credential_list/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21278 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22757 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.001408 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/
--rw-r--r--   0 nikhilm    (501) staff       (20)    45116 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.001536 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2758 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.002153 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3330 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20440 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20981 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.002515 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2473 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21048 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19893 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20164 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.002813 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21808 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26238 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4823 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/token.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18034 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/transcription.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.003097 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2220 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.004479 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/
--rw-r--r--   0 nikhilm    (501) staff       (20)    41695 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38339 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/all_time.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38247 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/daily.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38431 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/last_month.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38339 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/monthly.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38431 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/this_month.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38247 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/today.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38293 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/yearly.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    38431 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    49245 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/trigger.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7397 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/api/v2010/account/validation_request.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.004792 WhooshSms-0.1.0/twilio/rest/autopilot/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1217 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/AutopilotBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      778 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.005020 WhooshSms-0.1.0/twilio/rest/autopilot/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1680 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.006085 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/
--rw-r--r--   0 nikhilm    (501) staff       (20)    35087 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8479 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/defaults.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6698 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/dialogue.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.006369 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/field_type/
--rw-r--r--   0 nikhilm    (501) staff       (20)    23752 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22246 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22851 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/model_build.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    29877 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/query.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8288 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.007022 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/
--rw-r--r--   0 nikhilm    (501) staff       (20)    28213 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20115 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/field.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27891 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/sample.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9964 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7530 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24728 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/webhook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5222 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/autopilot/v1/restore_assistant.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.007259 WhooshSms-0.1.0/twilio/rest/bulkexports/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1231 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/BulkexportsBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      792 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.007504 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1692 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.008071 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/
--rw-r--r--   0 nikhilm    (501) staff       (20)     7083 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14521 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/day.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17005 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8224 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/job.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10811 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export_configuration.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.008355 WhooshSms-0.1.0/twilio/rest/chat/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1700 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/ChatBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      970 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.008628 WhooshSms-0.1.0/twilio/rest/chat/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1569 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27856 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/credential.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.008949 WhooshSms-0.1.0/twilio/rest/chat/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    92674 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.009621 WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/
--rw-r--r--   0 nikhilm    (501) staff       (20)    28967 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22312 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/invite.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27709 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/member.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26356 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/message.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21831 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/role.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.009934 WhooshSms-0.1.0/twilio/rest/chat/v1/service/user/
--rw-r--r--   0 nikhilm    (501) staff       (20)    26317 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/user/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    12925 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v1/service/user/user_channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.010200 WhooshSms-0.1.0/twilio/rest/chat/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1569 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27486 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/credential.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.010664 WhooshSms-0.1.0/twilio/rest/chat/v2/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    66570 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22118 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/binding.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.011422 WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/
--rw-r--r--   0 nikhilm    (501) staff       (20)    39123 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22292 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/invite.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    41109 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/member.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    37545 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/message.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    33770 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/webhook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22232 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/role.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.011843 WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/
--rw-r--r--   0 nikhilm    (501) staff       (20)    29035 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21909 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/user_binding.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27050 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/user_channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.012085 WhooshSms-0.1.0/twilio/rest/chat/v3/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1268 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v3/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11567 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/chat/v3/channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.012323 WhooshSms-0.1.0/twilio/rest/content/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1203 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/ContentBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1110 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.012860 WhooshSms-0.1.0/twilio/rest/content/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2024 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.013189 WhooshSms-0.1.0/twilio/rest/content/v1/content/
--rw-r--r--   0 nikhilm    (501) staff       (20)    16628 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/v1/content/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5839 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/v1/content/approval_fetch.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11924 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/v1/content_and_approvals.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    12123 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/content/v1/legacy_content.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.013477 WhooshSms-0.1.0/twilio/rest/conversations/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1245 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/ConversationsBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2760 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.014256 WhooshSms-0.1.0/twilio/rest/conversations/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3659 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    36854 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/address_configuration.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.014564 WhooshSms-0.1.0/twilio/rest/conversations/v1/configuration/
--rw-r--r--   0 nikhilm    (501) staff       (20)    12497 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/configuration/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11083 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/configuration/webhook.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.015019 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/
--rw-r--r--   0 nikhilm    (501) staff       (20)    42957 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.015320 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/message/
--rw-r--r--   0 nikhilm    (501) staff       (20)    34972 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/message/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18063 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    40116 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/participant.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27236 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/webhook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27935 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/credential.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18739 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/participant_conversation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20943 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/role.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.015949 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20025 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22289 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/binding.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.016405 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/
--rw-r--r--   0 nikhilm    (501) staff       (20)    16088 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24410 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/notification.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13881 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/webhook.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.016895 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/
--rw-r--r--   0 nikhilm    (501) staff       (20)    44808 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.017232 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/message/
--rw-r--r--   0 nikhilm    (501) staff       (20)    36629 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19398 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    41799 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/participant.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    28926 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/webhook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19530 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/participant_conversation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22534 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/role.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.017531 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/user/
--rw-r--r--   0 nikhilm    (501) staff       (20)    29682 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/user/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26510 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/service/user/user_conversation.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.017835 WhooshSms-0.1.0/twilio/rest/conversations/v1/user/
--rw-r--r--   0 nikhilm    (501) staff       (20)    28016 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/user/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25215 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/conversations/v1/user/user_conversation.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.018100 WhooshSms-0.1.0/twilio/rest/events/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/EventsBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1277 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.018379 WhooshSms-0.1.0/twilio/rest/events/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2133 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    15317 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/event_type.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.018625 WhooshSms-0.1.0/twilio/rest/events/v1/schema/
--rw-r--r--   0 nikhilm    (501) staff       (20)     6417 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/schema/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14920 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/schema/schema_version.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.018955 WhooshSms-0.1.0/twilio/rest/events/v1/sink/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22872 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/sink/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2768 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/sink/sink_test.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3358 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/sink/sink_validate.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.019676 WhooshSms-0.1.0/twilio/rest/events/v1/subscription/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22609 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/subscription/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20282 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/events/v1/subscription/subscribed_event.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.019982 WhooshSms-0.1.0/twilio/rest/flex_api/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1471 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/FlexApiBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6332 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.022225 WhooshSms-0.1.0/twilio/rest/flex_api/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     7374 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23338 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/assessments.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19793 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/channel.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13488 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/configuration.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    46860 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/flex_flow.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17489 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    12580 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_conversations.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26467 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_questionnaires.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20324 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25940 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19100 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_segments.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5688 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_session.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3149 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2730 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_settings_comment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5365 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_user_roles.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.022352 WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/
--rw-r--r--   0 nikhilm    (501) staff       (20)     8562 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.022761 WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20915 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13861 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19858 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20821 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v1/web_channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.023007 WhooshSms-0.1.0/twilio/rest/flex_api/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1323 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5583 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/flex_api/v2/web_channels.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.023238 WhooshSms-0.1.0/twilio/rest/frontline_api/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1240 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/frontline_api/FrontlineApiBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      410 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/frontline_api/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.023462 WhooshSms-0.1.0/twilio/rest/frontline_api/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1277 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/frontline_api/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10822 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/frontline_api/v1/user.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.023720 WhooshSms-0.1.0/twilio/rest/insights/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/InsightsBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1579 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.024053 WhooshSms-0.1.0/twilio/rest/insights/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2419 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.024608 WhooshSms-0.1.0/twilio/rest/insights/v1/call/
--rw-r--r--   0 nikhilm    (501) staff       (20)     6981 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/call/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17445 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/call/annotation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9363 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/call/call_summary.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    12166 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/call/event.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13146 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/call/metric.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    28813 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/call_summaries.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.024904 WhooshSms-0.1.0/twilio/rest/insights/v1/conference/
--rw-r--r--   0 nikhilm    (501) staff       (20)    31370 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/conference/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25248 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/conference/conference_participant.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.025147 WhooshSms-0.1.0/twilio/rest/insights/v1/room/
--rw-r--r--   0 nikhilm    (501) staff       (20)    25243 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/room/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17908 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/room/participant.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8063 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/insights/v1/setting.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.025488 WhooshSms-0.1.0/twilio/rest/ip_messaging/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1507 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/IpMessagingBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      738 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.025784 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1615 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21632 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/credential.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.026122 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    62960 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.026753 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/
--rw-r--r--   0 nikhilm    (501) staff       (20)    24064 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18541 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21725 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/member.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21818 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/message.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18855 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/role.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.027076 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/user/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21365 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11548 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.027380 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1615 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21632 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/credential.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.027852 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    45390 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17907 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/binding.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.028658 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/
--rw-r--r--   0 nikhilm    (501) staff       (20)    30568 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18541 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    29520 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/member.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    28798 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/message.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26175 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18855 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/role.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.029567 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/
--rw-r--r--   0 nikhilm    (501) staff       (20)    24051 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18192 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21476 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.030295 WhooshSms-0.1.0/twilio/rest/lookups/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1468 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/lookups/LookupsBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      432 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/lookups/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.031684 WhooshSms-0.1.0/twilio/rest/lookups/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1329 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/lookups/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13250 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/lookups/v1/phone_number.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.031936 WhooshSms-0.1.0/twilio/rest/lookups/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1329 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/lookups/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20961 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/lookups/v2/phone_number.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.032189 WhooshSms-0.1.0/twilio/rest/media/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/MediaBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1107 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.032561 WhooshSms-0.1.0/twilio/rest/media/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2030 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26533 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/v1/media_processor.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22582 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/v1/media_recording.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.032825 WhooshSms-0.1.0/twilio/rest/media/v1/player_streamer/
--rw-r--r--   0 nikhilm    (501) staff       (20)    25414 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/v1/player_streamer/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9432 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/media/v1/player_streamer/playback_grant.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.033420 WhooshSms-0.1.0/twilio/rest/messaging/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1217 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/MessagingBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3308 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.035943 WhooshSms-0.1.0/twilio/rest/messaging/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     4839 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.036607 WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/
--rw-r--r--   0 nikhilm    (501) staff       (20)    24289 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3583 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19914 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5796 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/deactivations.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10495 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/domain_certs.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10525 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/domain_config.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7773 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4360 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/external_campaign.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9216 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.037344 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    54653 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18348 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/alpha_sender.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18413 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/phone_number.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18135 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/short_code.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    33395 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/us_app_to_person.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3513 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    55732 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/tollfree_verification.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2322 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/messaging/v1/usecase.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.038208 WhooshSms-0.1.0/twilio/rest/microvisor/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1224 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/MicrovisorBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1321 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.038582 WhooshSms-0.1.0/twilio/rest/microvisor/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2211 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17838 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/account_config.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17723 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/account_secret.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.038858 WhooshSms-0.1.0/twilio/rest/microvisor/v1/app/
--rw-r--r--   0 nikhilm    (501) staff       (20)    15664 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/app/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5534 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/app/app_manifest.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.039241 WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20135 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19145 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/device_config.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19030 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/device_secret.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.039476 WhooshSms-0.1.0/twilio/rest/monitor/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1203 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/monitor/MonitorBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      658 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/monitor/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.040274 WhooshSms-0.1.0/twilio/rest/monitor/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1517 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/monitor/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22723 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/monitor/v1/alert.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25437 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/monitor/v1/event.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.040531 WhooshSms-0.1.0/twilio/rest/notify/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/NotifyBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      700 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.040815 WhooshSms-0.1.0/twilio/rest/notify/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1581 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27961 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/v1/credential.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.041222 WhooshSms-0.1.0/twilio/rest/notify/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    47060 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/v1/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    30272 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/v1/service/binding.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25490 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/notify/v1/service/notification.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.041459 WhooshSms-0.1.0/twilio/rest/numbers/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1468 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/NumbersBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      491 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.041576 WhooshSms-0.1.0/twilio/rest/numbers/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1414 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.042336 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3690 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.043012 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
--rw-r--r--   0 nikhilm    (501) staff       (20)    47502 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13880 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16186 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17833 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5665 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20500 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14140 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18536 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22407 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14788 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.043284 WhooshSms-0.1.0/twilio/rest/oauth/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/OauthBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1578 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.044098 WhooshSms-0.1.0/twilio/rest/oauth/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2434 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4598 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/v1/device_code.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4115 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/v1/oauth.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7059 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/v1/openid_discovery.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6329 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/v1/token.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4714 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/oauth/v1/user_info.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.044340 WhooshSms-0.1.0/twilio/rest/preview/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3081 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/PreviewBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3528 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.045708 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1329 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.046652 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22442 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24118 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22163 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26656 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/device.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22726 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/key.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.046954 WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1892 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.047293 WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/authorization_document/
--rw-r--r--   0 nikhilm    (501) staff       (20)    32009 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24829 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    48143 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.047452 WhooshSms-0.1.0/twilio/rest/preview/marketplace/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1775 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/marketplace/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.047748 WhooshSms-0.1.0/twilio/rest/preview/marketplace/available_add_on/
--rw-r--r--   0 nikhilm    (501) staff       (20)    15067 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16163 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.048041 WhooshSms-0.1.0/twilio/rest/preview/marketplace/installed_add_on/
--rw-r--r--   0 nikhilm    (501) staff       (20)    23293 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18542 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.048190 WhooshSms-0.1.0/twilio/rest/preview/sync/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1293 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.048350 WhooshSms-0.1.0/twilio/rest/preview/sync/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22270 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.048678 WhooshSms-0.1.0/twilio/rest/preview/sync/service/document/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20547 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/document/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21455 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/document/document_permission.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.049123 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/
--rw-r--r--   0 nikhilm    (501) staff       (20)    18339 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24174 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21397 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.049589 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/
--rw-r--r--   0 nikhilm    (501) staff       (20)    18217 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24063 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21250 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.049734 WhooshSms-0.1.0/twilio/rest/preview/understand/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1343 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.050713 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/
--rw-r--r--   0 nikhilm    (501) staff       (20)    35382 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8318 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8510 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5976 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/dialogue.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.050982 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/field_type/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22348 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20410 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21062 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/model_build.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26433 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/query.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7799 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/style_sheet.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.051764 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/
--rw-r--r--   0 nikhilm    (501) staff       (20)    26813 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19110 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/field.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24937 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/sample.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8816 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/task_actions.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6871 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.052188 WhooshSms-0.1.0/twilio/rest/preview/wireless/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1849 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/wireless/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18911 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/wireless/command.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21681 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/wireless/rate_plan.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.052512 WhooshSms-0.1.0/twilio/rest/preview/wireless/sim/
--rw-r--r--   0 nikhilm    (501) staff       (20)    28867 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/wireless/sim/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6592 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/preview/wireless/sim/usage.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.052791 WhooshSms-0.1.0/twilio/rest/pricing/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1468 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/PricingBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1569 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.052920 WhooshSms-0.1.0/twilio/rest/pricing/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1867 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.053188 WhooshSms-0.1.0/twilio/rest/pricing/v1/messaging/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1443 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/messaging/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14530 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/messaging/country.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.053457 WhooshSms-0.1.0/twilio/rest/pricing/v1/phone_number/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1455 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/phone_number/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14123 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/phone_number/country.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.053805 WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1753 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14416 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/country.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5701 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/number.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.054174 WhooshSms-0.1.0/twilio/rest/pricing/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1801 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14470 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v2/country.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8966 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v2/number.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.054557 WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1753 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14446 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/country.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9040 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/number.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.054814 WhooshSms-0.1.0/twilio/rest/proxy/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/ProxyBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      387 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.054958 WhooshSms-0.1.0/twilio/rest/proxy/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1273 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.055406 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    38044 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23754 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/phone_number.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.055720 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/
--rw-r--r--   0 nikhilm    (501) staff       (20)    27767 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21109 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/interaction.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.056028 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/participant/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22765 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23242 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21333 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/proxy/v1/service/short_code.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.056290 WhooshSms-0.1.0/twilio/rest/routes/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/routes/RoutesBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1003 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/routes/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.056798 WhooshSms-0.1.0/twilio/rest/routes/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1876 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/routes/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9727 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/routes/v2/phone_number.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8319 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/routes/v2/sip_domain.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9536 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/routes/v2/trunk.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.057041 WhooshSms-0.1.0/twilio/rest/serverless/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1224 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/ServerlessBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      417 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.057162 WhooshSms-0.1.0/twilio/rest/serverless/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1298 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.057293 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    25510 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.057591 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/asset/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20582 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/asset/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16714 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/asset/asset_version.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.057882 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/build/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20195 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/build/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6403 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/build/build_status.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.058451 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21009 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18049 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/deployment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20926 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/log.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22598 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/variable.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.058600 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20928 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.058910 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/function_version/
--rw-r--r--   0 nikhilm    (501) staff       (20)    18093 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7736 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.059156 WhooshSms-0.1.0/twilio/rest/studio/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1459 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/StudioBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      694 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.059262 WhooshSms-0.1.0/twilio/rest/studio/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1248 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.059372 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/
--rw-r--r--   0 nikhilm    (501) staff       (20)    16404 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.059607 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21366 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6720 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.059851 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/step/
--rw-r--r--   0 nikhilm    (501) staff       (20)    17219 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7395 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.060115 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/
--rw-r--r--   0 nikhilm    (501) staff       (20)    27270 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6877 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_context.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.060364 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_step/
--rw-r--r--   0 nikhilm    (501) staff       (20)    17888 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7716 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.060592 WhooshSms-0.1.0/twilio/rest/studio/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1572 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.060950 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/
--rw-r--r--   0 nikhilm    (501) staff       (20)    23658 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.061222 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/
--rw-r--r--   0 nikhilm    (501) staff       (20)    27154 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6877 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_context.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.061467 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_step/
--rw-r--r--   0 nikhilm    (501) staff       (20)    17888 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7716 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16059 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/flow_revision.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7422 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow/flow_test_user.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3892 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/studio/v2/flow_validate.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.061686 WhooshSms-0.1.0/twilio/rest/supersim/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/SupersimBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2908 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.062697 WhooshSms-0.1.0/twilio/rest/supersim/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3800 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23623 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/esim_profile.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    35226 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/fleet.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26640 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/ip_command.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17582 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/network.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.062963 WhooshSms-0.1.0/twilio/rest/supersim/v1/network_access_profile/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20071 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19359 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14206 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/settings_update.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.063736 WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/
--rw-r--r--   0 nikhilm    (501) staff       (20)    28732 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    12030 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/billing_period.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10625 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23001 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/sms_command.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    26841 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/supersim/v1/usage_record.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.064075 WhooshSms-0.1.0/twilio/rest/sync/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1182 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/SyncBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      381 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.064206 WhooshSms-0.1.0/twilio/rest/sync/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1268 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.064340 WhooshSms-0.1.0/twilio/rest/sync/v1/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    36623 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.064640 WhooshSms-0.1.0/twilio/rest/sync/v1/service/document/
--rw-r--r--   0 nikhilm    (501) staff       (20)    25373 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/document/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21822 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/document/document_permission.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.065094 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/
--rw-r--r--   0 nikhilm    (501) staff       (20)    25198 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    36671 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21826 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.065535 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/
--rw-r--r--   0 nikhilm    (501) staff       (20)    24886 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    37230 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21754 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.065833 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_stream/
--rw-r--r--   0 nikhilm    (501) staff       (20)    22899 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     4315 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.066116 WhooshSms-0.1.0/twilio/rest/taskrouter/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1224 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/TaskrouterBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      431 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.066247 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1318 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.067370 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/
--rw-r--r--   0 nikhilm    (501) staff       (20)    44452 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25986 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/activity.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    32776 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/event.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.067685 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task/
--rw-r--r--   0 nikhilm    (501) staff       (20)    51478 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    79751 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23470 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.068503 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/
--rw-r--r--   0 nikhilm    (501) staff       (20)    39230 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18318 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10983 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13380 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21315 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.069534 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/
--rw-r--r--   0 nikhilm    (501) staff       (20)    43462 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    77533 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22091 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11730 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13241 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7884 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13545 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.070104 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/
--rw-r--r--   0 nikhilm    (501) staff       (20)    34579 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19228 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9689 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14701 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18165 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     9027 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13564 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.070349 WhooshSms-0.1.0/twilio/rest/trunking/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/TrunkingBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)      391 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.070477 WhooshSms-0.1.0/twilio/rest/trunking/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1268 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.071334 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/
--rw-r--r--   0 nikhilm    (501) staff       (20)    39976 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18350 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/credential_list.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18720 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27739 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/origination_url.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22459 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/phone_number.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8181 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/recording.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.071626 WhooshSms-0.1.0/twilio/rest/trusthub/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/TrusthubBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2483 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.072445 WhooshSms-0.1.0/twilio/rest/trusthub/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3431 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.073020 WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/
--rw-r--r--   0 nikhilm    (501) staff       (20)    30761 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23437 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19934 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18436 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20560 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/end_user.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14103 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/end_user_type.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13542 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/policies.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22191 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/supporting_document.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14729 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/supporting_document_type.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.073672 WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/
--rw-r--r--   0 nikhilm    (501) staff       (20)    30206 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23131 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19505 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    18057 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.074090 WhooshSms-0.1.0/twilio/rest/verify/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/VerifyBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2056 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.074879 WhooshSms-0.1.0/twilio/rest/verify/v2/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2992 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5695 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/form.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8036 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/safelist.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.075755 WhooshSms-0.1.0/twilio/rest/verify/v2/service/
--rw-r--r--   0 nikhilm    (501) staff       (20)    55315 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    10267 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/access_token.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.076206 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20668 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.076480 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/challenge/
--rw-r--r--   0 nikhilm    (501) staff       (20)    34458 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6557 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    29593 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/factor.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16164 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/new_factor.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    23201 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/messaging_configuration.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.076757 WhooshSms-0.1.0/twilio/rest/verify/v2/service/rate_limit/
--rw-r--r--   0 nikhilm    (501) staff       (20)    21507 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    22242 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    21417 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/verification.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     8363 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/verification_check.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    25389 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/service/webhook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11731 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/template.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    29432 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/verification_attempt.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13009 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/verify/v2/verification_attempts_summary.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.076993 WhooshSms-0.1.0/twilio/rest/video/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/VideoBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2050 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.077730 WhooshSms-0.1.0/twilio/rest/video/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2971 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    34977 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/composition.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    54707 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/composition_hook.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14079 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/composition_settings.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27313 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/recording.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    13910 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/recording_settings.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.078147 WhooshSms-0.1.0/twilio/rest/video/v1/room/
--rw-r--r--   0 nikhilm    (501) staff       (20)    38074 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.078767 WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/
--rw-r--r--   0 nikhilm    (501) staff       (20)    28698 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     7905 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/anonymize.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16887 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/published_track.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6391 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17079 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/subscribed_track.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     5087 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/recording_rules.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    24746 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/video/v1/room/room_recording.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.079543 WhooshSms-0.1.0/twilio/rest/voice/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/VoiceBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2099 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.080375 WhooshSms-0.1.0/twilio/rest/voice/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3035 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3316 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/archived_call.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    37359 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/byoc_trunk.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.080686 WhooshSms-0.1.0/twilio/rest/voice/v1/connection_policy/
--rw-r--r--   0 nikhilm    (501) staff       (20)    20484 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/connection_policy/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    29170 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.081143 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2327 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     3837 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.081439 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/country/
--rw-r--r--   0 nikhilm    (501) staff       (20)    26486 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    11128 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     6995 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/settings.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    20413 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/ip_record.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    19429 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/voice/v1/source_ip_mapping.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.081712 WhooshSms-0.1.0/twilio/rest/wireless/
--rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/WirelessBase.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1261 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/__init__.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.082307 WhooshSms-0.1.0/twilio/rest/wireless/v1/
--rw-r--r--   0 nikhilm    (501) staff       (20)     2135 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    27361 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/command.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    29604 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/rate_plan.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.082753 WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/
--rw-r--r--   0 nikhilm    (501) staff       (20)    46125 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    14307 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/data_session.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    17463 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/usage_record.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    16059 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/rest/wireless/v1/usage_record.py
-drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:26:59.083335 WhooshSms-0.1.0/twilio/twiml/
--rw-r--r--   0 nikhilm    (501) staff       (20)     3471 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/twiml/__init__.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     1435 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/twiml/fax_response.py
--rw-r--r--   0 nikhilm    (501) staff       (20)     2935 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/twiml/messaging_response.py
--rw-r--r--   0 nikhilm    (501) staff       (20)    82958 2023-04-25 16:20:34.000000 WhooshSms-0.1.0/twilio/twiml/voice_response.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.538961 WhooshSms-0.1.1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1088 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/LICENSE
+-rw-r--r--   0 nikhilm    (501) staff       (20)      117 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/MANIFEST.in
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10032 2023-05-02 11:32:31.539035 WhooshSms-0.1.1/PKG-INFO
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9059 2023-05-02 11:31:44.000000 WhooshSms-0.1.1/README.md
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.439014 WhooshSms-0.1.1/WhooshSms.egg-info/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10032 2023-05-02 11:32:31.000000 WhooshSms-0.1.1/WhooshSms.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilm    (501) staff       (20)    30370 2023-05-02 11:32:31.000000 WhooshSms-0.1.1/WhooshSms.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilm    (501) staff       (20)        1 2023-05-02 11:32:31.000000 WhooshSms-0.1.1/WhooshSms.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilm    (501) staff       (20)       77 2023-05-02 11:32:31.000000 WhooshSms-0.1.1/WhooshSms.egg-info/requires.txt
+-rw-r--r--   0 nikhilm    (501) staff       (20)        7 2023-05-02 11:32:31.000000 WhooshSms-0.1.1/WhooshSms.egg-info/top_level.txt
+-rw-r--r--   0 nikhilm    (501) staff       (20)      236 2023-05-02 11:32:31.539299 WhooshSms-0.1.1/setup.cfg
+-rwxr-xr-x   0 nikhilm    (501) staff       (20)     1672 2023-05-02 11:32:26.000000 WhooshSms-0.1.1/setup.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.439324 WhooshSms-0.1.1/twilio/
+-rw-r--r--   0 nikhilm    (501) staff       (20)       76 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.442232 WhooshSms-0.1.1/twilio/base/
+-rw-r--r--   0 nikhilm    (501) staff       (20)        0 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8153 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/client_base.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2019 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/deserialize.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3011 2023-05-02 10:40:30.000000 WhooshSms-0.1.1/twilio/base/domain.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2890 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/exceptions.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      147 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/instance_context.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      148 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/instance_resource.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      144 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/list_resource.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1417 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/obsolete.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5181 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/page.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2039 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/serialize.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      280 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/base/values.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14614 2023-05-02 10:39:18.000000 WhooshSms-0.1.1/twilio/base/version.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.443260 WhooshSms-0.1.1/twilio/http/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3434 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/http/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4503 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/http/async_http_client.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3735 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/http/http_client.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2655 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/http/request.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      518 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/http/response.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4810 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/http/validation_client.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.443437 WhooshSms-0.1.1/twilio/jwt/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5085 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.443777 WhooshSms-0.1.1/twilio/jwt/access_token/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2415 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/access_token/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4902 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/access_token/grants.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.443950 WhooshSms-0.1.1/twilio/jwt/client/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3982 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/client/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.444279 WhooshSms-0.1.1/twilio/jwt/taskrouter/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5726 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/taskrouter/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4309 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/taskrouter/capabilities.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.444457 WhooshSms-0.1.1/twilio/jwt/validation/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3156 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/jwt/validation/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4100 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/request_validator.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.444637 WhooshSms-0.1.1/twilio/rest/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20879 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.444983 WhooshSms-0.1.1/twilio/rest/accounts/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/AccountsBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1168 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.445474 WhooshSms-0.1.1/twilio/rest/accounts/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2102 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5547 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/v1/auth_token_promotion.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.445914 WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1766 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19489 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/aws.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20007 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/public_key.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6551 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/accounts/v1/secondary_auth_token.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.446312 WhooshSms-0.1.1/twilio/rest/api/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1220 2023-05-02 10:33:52.000000 WhooshSms-0.1.1/twilio/rest/api/ApiBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8255 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.446497 WhooshSms-0.1.1/twilio/rest/api/v2010/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1805 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.449411 WhooshSms-0.1.1/twilio/rest/api/v2010/account/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    36206 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.449765 WhooshSms-0.1.1/twilio/rest/api/v2010/account/address/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    35858 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/address/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17044 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/address/dependent_phone_number.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    47553 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/application.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17274 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/authorized_connect_app.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.451045 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21427 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    46239 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/local.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    46210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    45860 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    45930 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/national.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    46000 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    45930 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    45790 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3186 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/balance.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.452794 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    92392 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10658 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/event.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11932 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/feedback.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13986 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/feedback_summary.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28363 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/notification.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23472 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/payment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38495 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/recording.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    77226 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/siprec.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    77116 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/stream.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5278 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/user_defined_message.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10898 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.453354 WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    41186 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    74737 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/participant.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    32729 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/recording.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26539 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/connect_app.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.454069 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    73374 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.454526 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20750 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18341 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    36935 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/local.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    37019 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    37103 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17989 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/key.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.455056 WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    53984 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5102 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/feedback.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27246 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/media.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4785 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/new_key.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4813 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/new_signing_key.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27505 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/notification.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22199 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/outgoing_caller_id.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.455334 WhooshSms-0.1.1/twilio/rest/api/v2010/account/queue/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22428 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/queue/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19131 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/queue/member.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.455608 WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    37769 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.455890 WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/add_on_result/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19239 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19233 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19008 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/transcription.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26406 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/short_code.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17376 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/signing_key.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.456056 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2871 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.456380 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/credential_list/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21278 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22757 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/credential_list/credential.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.456883 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    45116 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.457036 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2758 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.457635 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3330 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20440 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20981 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.457964 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2473 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21048 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19893 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20164 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.458285 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21808 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26238 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4823 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/token.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18034 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/transcription.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.458903 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2220 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.460469 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    41695 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38339 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/all_time.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38247 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/daily.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38431 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/last_month.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38339 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/monthly.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38431 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/this_month.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38247 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/today.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38293 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/yearly.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38431 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/yesterday.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    49245 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/trigger.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7397 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/api/v2010/account/validation_request.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.460799 WhooshSms-0.1.1/twilio/rest/autopilot/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1217 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/AutopilotBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      778 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.461095 WhooshSms-0.1.1/twilio/rest/autopilot/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1680 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.462645 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    35087 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8479 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/defaults.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6698 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/dialogue.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.463097 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/field_type/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23752 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22246 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22851 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/model_build.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29877 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/query.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8288 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/style_sheet.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.464040 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28213 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20115 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/field.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27891 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/sample.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9964 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/task_actions.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7530 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24728 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/webhook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5222 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/autopilot/v1/restore_assistant.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.464332 WhooshSms-0.1.1/twilio/rest/bulkexports/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1231 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/BulkexportsBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      792 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.464922 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1692 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.465622 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7083 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14521 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/day.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17005 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/export_custom_job.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8224 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/job.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10811 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export_configuration.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.465966 WhooshSms-0.1.1/twilio/rest/chat/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1700 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/ChatBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      970 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.466298 WhooshSms-0.1.1/twilio/rest/chat/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1569 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27856 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/credential.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.466699 WhooshSms-0.1.1/twilio/rest/chat/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    92674 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.467519 WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28967 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22312 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/invite.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27709 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/member.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26356 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/message.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21831 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/role.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.467853 WhooshSms-0.1.1/twilio/rest/chat/v1/service/user/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26317 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/user/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    12925 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v1/service/user/user_channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.468144 WhooshSms-0.1.1/twilio/rest/chat/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1569 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27486 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/credential.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.468607 WhooshSms-0.1.1/twilio/rest/chat/v2/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    66570 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22118 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/binding.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.469330 WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    39123 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22292 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/invite.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    41109 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/member.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    37545 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/message.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    33770 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/webhook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22232 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/role.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.469730 WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29035 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21909 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/user_binding.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27050 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/user_channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.469986 WhooshSms-0.1.1/twilio/rest/chat/v3/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1268 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v3/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11567 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/chat/v3/channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.470290 WhooshSms-0.1.1/twilio/rest/content/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1203 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/ContentBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1110 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.470665 WhooshSms-0.1.1/twilio/rest/content/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2024 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.470957 WhooshSms-0.1.1/twilio/rest/content/v1/content/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16628 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/v1/content/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5839 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/v1/content/approval_fetch.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11924 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/v1/content_and_approvals.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    12123 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/content/v1/legacy_content.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.471262 WhooshSms-0.1.1/twilio/rest/conversations/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1245 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/ConversationsBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2760 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.472073 WhooshSms-0.1.1/twilio/rest/conversations/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3659 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    36854 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/address_configuration.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.472406 WhooshSms-0.1.1/twilio/rest/conversations/v1/configuration/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    12497 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/configuration/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11083 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/configuration/webhook.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.472911 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    42957 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.473257 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/message/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    34972 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/message/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18063 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    40116 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/participant.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27236 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/webhook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27935 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/credential.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18739 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/participant_conversation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20943 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/role.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.473899 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20025 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22289 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/binding.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.474362 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16088 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24410 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/notification.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13881 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/webhook.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.474880 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    44808 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.475224 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/message/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    36629 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/message/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19398 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    41799 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/participant.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28926 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/webhook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19530 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/participant_conversation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22534 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/role.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.475569 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/user/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29682 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/user/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26510 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/service/user/user_conversation.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.475927 WhooshSms-0.1.1/twilio/rest/conversations/v1/user/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28016 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/user/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25215 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/conversations/v1/user/user_conversation.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.476222 WhooshSms-0.1.1/twilio/rest/events/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/EventsBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1277 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.476484 WhooshSms-0.1.1/twilio/rest/events/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2133 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    15317 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/event_type.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.476763 WhooshSms-0.1.1/twilio/rest/events/v1/schema/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6417 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/schema/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14920 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/schema/schema_version.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.477206 WhooshSms-0.1.1/twilio/rest/events/v1/sink/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22872 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/sink/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2768 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/sink/sink_test.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3358 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/sink/sink_validate.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.477492 WhooshSms-0.1.1/twilio/rest/events/v1/subscription/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22609 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/subscription/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20282 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/events/v1/subscription/subscribed_event.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.477812 WhooshSms-0.1.1/twilio/rest/flex_api/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1471 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/FlexApiBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6332 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.480172 WhooshSms-0.1.1/twilio/rest/flex_api/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7374 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23338 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/assessments.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19793 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/channel.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13488 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/configuration.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    46860 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/flex_flow.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17489 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_assessments_comment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    12580 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_conversations.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26467 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_questionnaires.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20324 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_questionnaires_category.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25940 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_questionnaires_question.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19100 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_segments.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5688 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_session.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3149 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2730 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_settings_comment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5365 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_user_roles.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.480336 WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8562 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.480833 WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20915 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13861 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19858 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20821 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v1/web_channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.481169 WhooshSms-0.1.1/twilio/rest/flex_api/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1323 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5583 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/flex_api/v2/web_channels.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.481473 WhooshSms-0.1.1/twilio/rest/frontline_api/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1240 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/frontline_api/FrontlineApiBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      410 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/frontline_api/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.481742 WhooshSms-0.1.1/twilio/rest/frontline_api/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1277 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/frontline_api/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10822 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/frontline_api/v1/user.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.482000 WhooshSms-0.1.1/twilio/rest/insights/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/InsightsBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1579 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.482449 WhooshSms-0.1.1/twilio/rest/insights/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2419 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.483207 WhooshSms-0.1.1/twilio/rest/insights/v1/call/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6981 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/call/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17445 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/call/annotation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9363 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/call/call_summary.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    12166 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/call/event.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13146 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/call/metric.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28813 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/call_summaries.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.483513 WhooshSms-0.1.1/twilio/rest/insights/v1/conference/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    31370 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/conference/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25248 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/conference/conference_participant.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.483832 WhooshSms-0.1.1/twilio/rest/insights/v1/room/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25243 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/room/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17908 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/room/participant.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8063 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/insights/v1/setting.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.484139 WhooshSms-0.1.1/twilio/rest/ip_messaging/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1507 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/IpMessagingBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      738 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.484398 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1615 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21632 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/credential.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.484720 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    62960 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.485335 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24064 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18541 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/invite.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21725 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/member.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21818 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/message.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18855 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/role.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.485628 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/user/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21365 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/user/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11548 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/user/user_channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.485898 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1615 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21632 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/credential.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.486377 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    45390 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17907 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/binding.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.487603 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    30568 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18541 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/invite.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29520 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/member.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28798 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/message.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26175 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/webhook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18855 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/role.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.488102 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24051 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18192 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/user_binding.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21476 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/user_channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.488398 WhooshSms-0.1.1/twilio/rest/lookups/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1468 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/lookups/LookupsBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      432 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/lookups/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.488669 WhooshSms-0.1.1/twilio/rest/lookups/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1329 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/lookups/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13250 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/lookups/v1/phone_number.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.488934 WhooshSms-0.1.1/twilio/rest/lookups/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1329 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/lookups/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20961 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/lookups/v2/phone_number.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.489259 WhooshSms-0.1.1/twilio/rest/media/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/MediaBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1107 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.489776 WhooshSms-0.1.1/twilio/rest/media/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2030 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26533 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/v1/media_processor.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22582 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/v1/media_recording.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.490076 WhooshSms-0.1.1/twilio/rest/media/v1/player_streamer/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25414 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/v1/player_streamer/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9432 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/media/v1/player_streamer/playback_grant.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.490346 WhooshSms-0.1.1/twilio/rest/messaging/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1217 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/MessagingBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3308 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.492131 WhooshSms-0.1.1/twilio/rest/messaging/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4839 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.492711 WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24289 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3583 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19914 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5796 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/deactivations.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10495 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/domain_certs.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10525 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/domain_config.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7773 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/domain_config_messaging_service.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4360 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/external_campaign.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9216 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/linkshortening_messaging_service.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.493718 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    54653 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18348 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/alpha_sender.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18413 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/phone_number.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18135 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/short_code.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    33395 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/us_app_to_person.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3513 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    55732 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/tollfree_verification.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2322 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/messaging/v1/usecase.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.493953 WhooshSms-0.1.1/twilio/rest/microvisor/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1224 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/MicrovisorBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1321 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.494336 WhooshSms-0.1.1/twilio/rest/microvisor/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2211 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17838 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/account_config.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17723 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/account_secret.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.494634 WhooshSms-0.1.1/twilio/rest/microvisor/v1/app/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    15664 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/app/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5534 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/app/app_manifest.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.495017 WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20135 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19145 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/device_config.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19030 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/device_secret.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.495260 WhooshSms-0.1.1/twilio/rest/monitor/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1203 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/monitor/MonitorBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      658 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/monitor/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.495680 WhooshSms-0.1.1/twilio/rest/monitor/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1517 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/monitor/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22723 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/monitor/v1/alert.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25437 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/monitor/v1/event.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.495924 WhooshSms-0.1.1/twilio/rest/notify/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/NotifyBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      700 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.496153 WhooshSms-0.1.1/twilio/rest/notify/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1581 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27961 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/v1/credential.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.496562 WhooshSms-0.1.1/twilio/rest/notify/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    47060 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/v1/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    30272 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/v1/service/binding.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25490 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/notify/v1/service/notification.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.496894 WhooshSms-0.1.1/twilio/rest/numbers/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1468 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/NumbersBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      491 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.497047 WhooshSms-0.1.1/twilio/rest/numbers/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1414 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.498088 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3690 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.498763 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    47502 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13880 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16186 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17833 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5665 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20500 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14140 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18536 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22407 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14788 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.499040 WhooshSms-0.1.1/twilio/rest/oauth/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/OauthBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1578 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.499877 WhooshSms-0.1.1/twilio/rest/oauth/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2434 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4598 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/v1/device_code.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4115 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/v1/oauth.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7059 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/v1/openid_discovery.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6329 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/v1/token.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4714 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/oauth/v1/user_info.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.500153 WhooshSms-0.1.1/twilio/rest/preview/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3081 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/PreviewBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3528 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.500295 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1329 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.501063 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22442 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24118 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/certificate.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22163 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/deployment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26656 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/device.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22726 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/key.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.501362 WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1892 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.501682 WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/authorization_document/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    32009 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24829 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    48143 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/hosted_number_order.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.501836 WhooshSms-0.1.1/twilio/rest/preview/marketplace/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1775 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/marketplace/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.502109 WhooshSms-0.1.1/twilio/rest/preview/marketplace/available_add_on/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    15067 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/marketplace/available_add_on/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16163 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.502392 WhooshSms-0.1.1/twilio/rest/preview/marketplace/installed_add_on/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23293 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/marketplace/installed_add_on/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18542 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.502540 WhooshSms-0.1.1/twilio/rest/preview/sync/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1293 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.502668 WhooshSms-0.1.1/twilio/rest/preview/sync/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22270 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.502973 WhooshSms-0.1.1/twilio/rest/preview/sync/service/document/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20547 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/document/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21455 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/document/document_permission.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.503460 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18339 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24174 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21397 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.503960 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18217 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24063 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21250 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.504146 WhooshSms-0.1.1/twilio/rest/preview/understand/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1343 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.505315 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    35382 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8318 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8510 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5976 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/dialogue.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.505661 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/field_type/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22348 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/field_type/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20410 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/field_type/field_value.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21062 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/model_build.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26433 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/query.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7799 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/style_sheet.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.506543 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26813 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19110 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/field.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24937 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/sample.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8816 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/task_actions.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6871 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/task_statistics.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.507070 WhooshSms-0.1.1/twilio/rest/preview/wireless/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1849 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/wireless/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18911 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/wireless/command.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21681 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/wireless/rate_plan.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.507444 WhooshSms-0.1.1/twilio/rest/preview/wireless/sim/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28867 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/wireless/sim/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6592 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/preview/wireless/sim/usage.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.507781 WhooshSms-0.1.1/twilio/rest/pricing/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1468 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/PricingBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1569 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.507917 WhooshSms-0.1.1/twilio/rest/pricing/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1867 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.508201 WhooshSms-0.1.1/twilio/rest/pricing/v1/messaging/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1443 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/messaging/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14530 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/messaging/country.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.508473 WhooshSms-0.1.1/twilio/rest/pricing/v1/phone_number/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1455 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/phone_number/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14123 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/phone_number/country.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.508904 WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1753 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14416 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/country.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5701 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/number.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.509302 WhooshSms-0.1.1/twilio/rest/pricing/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1801 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14470 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v2/country.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8966 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v2/number.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.509702 WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1753 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14446 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/country.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9040 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/number.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.509961 WhooshSms-0.1.1/twilio/rest/proxy/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/ProxyBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      387 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.510077 WhooshSms-0.1.1/twilio/rest/proxy/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1273 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.510476 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38044 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23754 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/phone_number.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.510782 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27767 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21109 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/interaction.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.511081 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/participant/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22765 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/participant/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23242 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21333 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/proxy/v1/service/short_code.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.511345 WhooshSms-0.1.1/twilio/rest/routes/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/routes/RoutesBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1003 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/routes/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.511857 WhooshSms-0.1.1/twilio/rest/routes/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1876 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/routes/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9727 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/routes/v2/phone_number.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8319 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/routes/v2/sip_domain.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9536 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/routes/v2/trunk.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.512125 WhooshSms-0.1.1/twilio/rest/serverless/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1224 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/ServerlessBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      417 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.512267 WhooshSms-0.1.1/twilio/rest/serverless/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1298 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.512409 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25510 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.512876 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/asset/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20582 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/asset/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16714 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/asset/asset_version.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.513276 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/build/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20195 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/build/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6403 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/build/build_status.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.513992 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21009 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18049 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/deployment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20926 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/log.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22598 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/variable.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.514181 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20928 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.514539 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/function_version/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18093 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/function_version/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7736 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.514869 WhooshSms-0.1.1/twilio/rest/studio/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1459 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/StudioBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      694 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.515021 WhooshSms-0.1.1/twilio/rest/studio/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1248 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.515170 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16404 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.515524 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21366 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6720 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/engagement_context.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.516032 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/step/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17219 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/step/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7395 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/step/step_context.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.516422 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27270 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6877 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_context.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.516737 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_step/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17888 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7716 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.517028 WhooshSms-0.1.1/twilio/rest/studio/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1572 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.517453 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23658 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.517746 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27154 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6877 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_context.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.518041 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_step/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17888 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7716 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16059 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/flow_revision.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7422 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow/flow_test_user.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3892 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/studio/v2/flow_validate.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.518369 WhooshSms-0.1.1/twilio/rest/supersim/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/SupersimBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2908 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.519738 WhooshSms-0.1.1/twilio/rest/supersim/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3800 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23623 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/esim_profile.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    35226 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/fleet.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26640 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/ip_command.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17582 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/network.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.520056 WhooshSms-0.1.1/twilio/rest/supersim/v1/network_access_profile/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20071 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/network_access_profile/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19359 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14206 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/settings_update.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.520496 WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28732 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    12030 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/billing_period.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10625 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/sim_ip_address.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23001 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/sms_command.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26841 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/supersim/v1/usage_record.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.520776 WhooshSms-0.1.1/twilio/rest/sync/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1182 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/SyncBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      381 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.520922 WhooshSms-0.1.1/twilio/rest/sync/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1268 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.521058 WhooshSms-0.1.1/twilio/rest/sync/v1/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    36623 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.521374 WhooshSms-0.1.1/twilio/rest/sync/v1/service/document/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25373 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/document/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21822 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/document/document_permission.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.521818 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25198 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    36671 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21826 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.522210 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24886 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    37230 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21754 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.522471 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_stream/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22899 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_stream/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     4315 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_stream/stream_message.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.522691 WhooshSms-0.1.1/twilio/rest/taskrouter/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1224 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/TaskrouterBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      431 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.522800 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1318 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.523679 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    44452 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25986 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/activity.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    32776 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/event.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.523922 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    51478 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    79751 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task/reservation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23470 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_channel.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.524549 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    39230 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18318 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10983 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13380 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21315 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.525416 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    43462 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    77533 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22091 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11730 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13241 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7884 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13545 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.525909 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    34579 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19228 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9689 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14701 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18165 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     9027 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13564 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.526132 WhooshSms-0.1.1/twilio/rest/trunking/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/TrunkingBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)      391 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.526236 WhooshSms-0.1.1/twilio/rest/trunking/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1268 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.527283 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    39976 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18350 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/credential_list.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18720 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27739 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/origination_url.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22459 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/phone_number.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8181 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/recording.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.527551 WhooshSms-0.1.1/twilio/rest/trusthub/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/TrusthubBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2483 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.528389 WhooshSms-0.1.1/twilio/rest/trusthub/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3431 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.528975 WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    30761 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23437 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19934 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18436 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20560 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/end_user.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14103 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/end_user_type.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13542 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/policies.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22191 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/supporting_document.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14729 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/supporting_document_type.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.529565 WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    30206 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23131 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19505 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    18057 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.529819 WhooshSms-0.1.1/twilio/rest/verify/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1196 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/VerifyBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2056 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.530488 WhooshSms-0.1.1/twilio/rest/verify/v2/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2992 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5695 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/form.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8036 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/safelist.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.531338 WhooshSms-0.1.1/twilio/rest/verify/v2/service/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    55315 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    10267 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/access_token.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.531741 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20668 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.532177 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/challenge/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    34458 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/challenge/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6557 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/challenge/notification.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29593 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/factor.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16164 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/new_factor.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    23201 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/messaging_configuration.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.532519 WhooshSms-0.1.1/twilio/rest/verify/v2/service/rate_limit/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21507 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/rate_limit/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    22242 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/rate_limit/bucket.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    21417 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/verification.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     8363 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/verification_check.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    25389 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/service/webhook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11731 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/template.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29432 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/verification_attempt.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13009 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/verify/v2/verification_attempts_summary.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.532819 WhooshSms-0.1.1/twilio/rest/video/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/VideoBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2050 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.533665 WhooshSms-0.1.1/twilio/rest/video/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2971 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    34977 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/composition.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    54707 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/composition_hook.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14079 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/composition_settings.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27313 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/recording.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    13910 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/recording_settings.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.534045 WhooshSms-0.1.1/twilio/rest/video/v1/room/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    38074 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.534722 WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    28698 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     7905 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/anonymize.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16887 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/published_track.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6391 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/subscribe_rules.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17079 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/subscribed_track.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     5087 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/recording_rules.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    24746 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/video/v1/room/room_recording.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.535037 WhooshSms-0.1.1/twilio/rest/voice/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1189 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/VoiceBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2099 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.535827 WhooshSms-0.1.1/twilio/rest/voice/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3035 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3316 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/archived_call.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    37359 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/byoc_trunk.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.536167 WhooshSms-0.1.1/twilio/rest/voice/v1/connection_policy/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20484 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/connection_policy/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29170 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.536627 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2327 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3837 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.536962 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/country/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    26486 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    11128 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     6995 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/settings.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    20413 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/ip_record.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    19429 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/voice/v1/source_ip_mapping.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.537266 WhooshSms-0.1.1/twilio/rest/wireless/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1210 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/WirelessBase.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1261 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/__init__.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.537884 WhooshSms-0.1.1/twilio/rest/wireless/v1/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2135 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    27361 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/command.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    29604 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/rate_plan.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.538312 WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/
+-rw-r--r--   0 nikhilm    (501) staff       (20)    46125 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    14307 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/data_session.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    17463 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/usage_record.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    16059 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/rest/wireless/v1/usage_record.py
+drwxr-xr-x   0 nikhilm    (501) staff       (20)        0 2023-05-02 11:32:31.538797 WhooshSms-0.1.1/twilio/twiml/
+-rw-r--r--   0 nikhilm    (501) staff       (20)     3471 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/twiml/__init__.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     1435 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/twiml/fax_response.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)     2935 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/twiml/messaging_response.py
+-rw-r--r--   0 nikhilm    (501) staff       (20)    82958 2023-04-25 16:20:34.000000 WhooshSms-0.1.1/twilio/twiml/voice_response.py
```

### Comparing `WhooshSms-0.1.0/LICENSE` & `WhooshSms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/PKG-INFO` & `WhooshSms-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WhooshSms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Whoosh SMS API client
 Home-page: https://github.com/totogi/whoosh-python/
 Author: Totogi
 Author-email: help@totogi.com
 Keywords: whoosh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,20 +20,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Telephony
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whoosh-python
-
-[![Tests](https://github.com/twilio/twilio-python/actions/workflows/test-and-deploy.yml/badge.svg)](https://github.com/twilio/twilio-python/actions/workflows/test-and-deploy.yml)
-[![PyPI](https://img.shields.io/pypi/v/twilio.svg)](https://pypi.python.org/pypi/twilio)
-[![PyPI](https://img.shields.io/pypi/pyversions/twilio.svg)](https://pypi.python.org/pypi/twilio)
-[![Learn OSS Contribution in TwilioQuest](https://img.shields.io/static/v1?label=TwilioQuest&message=Learn%20to%20contribute%21&color=F22F46&labelColor=1f243c&style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAMAAAD04JH5AAAASFBMVEUAAAAZGRkcHBwjIyMoKCgAAABgYGBoaGiAgICMjIyzs7PJycnMzMzNzc3UoBfd3d3m5ubqrhfrMEDu7u739/f4vSb/3AD///9tbdyEAAAABXRSTlMAAAAAAMJrBrEAAAKoSURBVHgB7ZrRcuI6EESdyxXGYoNFvMD//+l2bSszRgyUYpFAsXOeiJGmj4NkuWx1Qeh+Ekl9DgEXOBwOx+Px5xyQhDykfgq4wG63MxxaR4ddIkg6Ul3g84vCIcjPBA5gmUMeXESrlukuoK33+33uID8TWeLAdOWsKpJYzwVMB7bOzYSGOciyUlXSn0/ABXTosJ1M1SbypZ4O4MbZuIDMU02PMbauhhHMHXbmebmALIiEbbbbbUrpF1gwE9kFfRNAJaP+FQEXCCTGyJ4ngDrjOFo3jEL5JdqjF/pueR4cCeCGgAtwmuRS6gDwaRiGvu+DMFwSBLTE3+jF8JyuV1okPZ+AC4hDFhCHyHQjdjPHUKFDlHSJkHQXMB3KpSwXNGJPcwwTdZiXlRN0gSp0zpWxNtM0beYE0nRH6QIbO7rawwXaBYz0j78gxjokDuv12gVeUuBD0MDi0OQCLvDaAho4juP1Q/jkAncXqIcCfd+7gAu4QLMACCLxpRsSuQh0igu0C9Svhi7weAGZg50L3IE3cai4IfkNZAC8dfdhsUD3CgKBVC9JE5ABAFzg4QL/taYPAAWrHdYcgfLaIgAXWJ7OV38n1LEF8tt2TH29E+QAoDoO5Ve/LtCQDmKM9kPbvCEBApK+IXzbcSJ0cIGF6e8gpcRhUDogWZ8JnaWjPXc/fNnBBUKRngiHgTUSivSzDRDgHZQOLvBQgf8rRt+VdBUUhwkU6VpJ+xcOwQUqZr+mR0kvBUgv6cB4+37hQAkXqE8PwGisGhJtN4xAHMzrsgvI7rccXqSvKh6jltGlrOHA3Xk1At3LC4QiPdX9/0ndHpGVvTjR4bZA1ypAKgVcwE5vx74ulwIugDt8e/X7JgfkucBMIAr26ndnB4UCLnDOqvteQsHlgX9N4A+c4cW3DXSPbwAAAABJRU5ErkJggg==)](https://twil.io/learn-open-source)
-
 ## Versions
 
 `whoosh-python` uses a modified version of [Semantic Versioning](https://semver.org) for all changes. [See this document](VERSIONS.md) for details.
 
 ### Supported Python Versions
 
 This library supports the following Python implementations:
@@ -46,40 +40,40 @@
 
 ## Installation
 
 Install from PyPi using [pip](https://pip.pypa.io/en/latest/), a
 package manager for Python.
 
 ```shell
-pip3 install twilio
+pip3 install WhooshSms
 ```
 
 If pip install fails on Windows, check the path length of the directory. If it is greater 260 characters then enable [Long Paths](https://docs.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation) or choose other shorter location.
 
 Don't have pip installed? Try installing it, by running this from the command
 line:
 
 ```shell
 curl https://bootstrap.pypa.io/get-pip.py | python
 ```
 
 Or, you can [download the source code
-(ZIP)](https://github.com/twilio/twilio-python/zipball/main 'twilio-python
+(ZIP)](https://github.com/totogi/whoosh-python/zipball/main 'whoosh-python
 source code') for `whoosh-python`, and then run:
 
 ```shell
 python3 setup.py install
 ```
 
 > **Info**
-> If the command line gives you an error message that says Permission Denied, try running the above commands with `sudo` (e.g., `sudo pip3 install twilio`).
+> If the command line gives you an error message that says Permission Denied, try running the above commands with `sudo` (e.g., `sudo pip3 install WhooshSms`).
 
 ### Test your installation
 
-Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Twilio account](https://console.twilio.com). The `to` phone number will be your own mobile phone.
+Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Whoosh account](https://console.whoosh.totogidemos.com). The `to` phone number will be your own mobile phone.
 
 ```python
 from twilio.rest import Client
 
 # Your Account SID and Auth Token from console.twilio.com
 account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
 auth_token  = "your_auth_token"
```

### Comparing `WhooshSms-0.1.0/README.md` & `WhooshSms-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,8 @@
 # whoosh-python
-
-[![Tests](https://github.com/twilio/twilio-python/actions/workflows/test-and-deploy.yml/badge.svg)](https://github.com/twilio/twilio-python/actions/workflows/test-and-deploy.yml)
-[![PyPI](https://img.shields.io/pypi/v/twilio.svg)](https://pypi.python.org/pypi/twilio)
-[![PyPI](https://img.shields.io/pypi/pyversions/twilio.svg)](https://pypi.python.org/pypi/twilio)
-[![Learn OSS Contribution in TwilioQuest](https://img.shields.io/static/v1?label=TwilioQuest&message=Learn%20to%20contribute%21&color=F22F46&labelColor=1f243c&style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAMAAAD04JH5AAAASFBMVEUAAAAZGRkcHBwjIyMoKCgAAABgYGBoaGiAgICMjIyzs7PJycnMzMzNzc3UoBfd3d3m5ubqrhfrMEDu7u739/f4vSb/3AD///9tbdyEAAAABXRSTlMAAAAAAMJrBrEAAAKoSURBVHgB7ZrRcuI6EESdyxXGYoNFvMD//+l2bSszRgyUYpFAsXOeiJGmj4NkuWx1Qeh+Ekl9DgEXOBwOx+Px5xyQhDykfgq4wG63MxxaR4ddIkg6Ul3g84vCIcjPBA5gmUMeXESrlukuoK33+33uID8TWeLAdOWsKpJYzwVMB7bOzYSGOciyUlXSn0/ABXTosJ1M1SbypZ4O4MbZuIDMU02PMbauhhHMHXbmebmALIiEbbbbbUrpF1gwE9kFfRNAJaP+FQEXCCTGyJ4ngDrjOFo3jEL5JdqjF/pueR4cCeCGgAtwmuRS6gDwaRiGvu+DMFwSBLTE3+jF8JyuV1okPZ+AC4hDFhCHyHQjdjPHUKFDlHSJkHQXMB3KpSwXNGJPcwwTdZiXlRN0gSp0zpWxNtM0beYE0nRH6QIbO7rawwXaBYz0j78gxjokDuv12gVeUuBD0MDi0OQCLvDaAho4juP1Q/jkAncXqIcCfd+7gAu4QLMACCLxpRsSuQh0igu0C9Svhi7weAGZg50L3IE3cai4IfkNZAC8dfdhsUD3CgKBVC9JE5ABAFzg4QL/taYPAAWrHdYcgfLaIgAXWJ7OV38n1LEF8tt2TH29E+QAoDoO5Ve/LtCQDmKM9kPbvCEBApK+IXzbcSJ0cIGF6e8gpcRhUDogWZ8JnaWjPXc/fNnBBUKRngiHgTUSivSzDRDgHZQOLvBQgf8rRt+VdBUUhwkU6VpJ+xcOwQUqZr+mR0kvBUgv6cB4+37hQAkXqE8PwGisGhJtN4xAHMzrsgvI7rccXqSvKh6jltGlrOHA3Xk1At3LC4QiPdX9/0ndHpGVvTjR4bZA1ypAKgVcwE5vx74ulwIugDt8e/X7JgfkucBMIAr26ndnB4UCLnDOqvteQsHlgX9N4A+c4cW3DXSPbwAAAABJRU5ErkJggg==)](https://twil.io/learn-open-source)
-
 ## Versions
 
 `whoosh-python` uses a modified version of [Semantic Versioning](https://semver.org) for all changes. [See this document](VERSIONS.md) for details.
 
 ### Supported Python Versions
 
 This library supports the following Python implementations:
@@ -21,40 +15,40 @@
 
 ## Installation
 
 Install from PyPi using [pip](https://pip.pypa.io/en/latest/), a
 package manager for Python.
 
 ```shell
-pip3 install twilio
+pip3 install WhooshSms
 ```
 
 If pip install fails on Windows, check the path length of the directory. If it is greater 260 characters then enable [Long Paths](https://docs.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation) or choose other shorter location.
 
 Don't have pip installed? Try installing it, by running this from the command
 line:
 
 ```shell
 curl https://bootstrap.pypa.io/get-pip.py | python
 ```
 
 Or, you can [download the source code
-(ZIP)](https://github.com/twilio/twilio-python/zipball/main 'twilio-python
+(ZIP)](https://github.com/totogi/whoosh-python/zipball/main 'whoosh-python
 source code') for `whoosh-python`, and then run:
 
 ```shell
 python3 setup.py install
 ```
 
 > **Info**
-> If the command line gives you an error message that says Permission Denied, try running the above commands with `sudo` (e.g., `sudo pip3 install twilio`).
+> If the command line gives you an error message that says Permission Denied, try running the above commands with `sudo` (e.g., `sudo pip3 install WhooshSms`).
 
 ### Test your installation
 
-Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Twilio account](https://console.twilio.com). The `to` phone number will be your own mobile phone.
+Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Whoosh account](https://console.whoosh.totogidemos.com). The `to` phone number will be your own mobile phone.
 
 ```python
 from twilio.rest import Client
 
 # Your Account SID and Auth Token from console.twilio.com
 account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
 auth_token  = "your_auth_token"
```

### Comparing `WhooshSms-0.1.0/WhooshSms.egg-info/PKG-INFO` & `WhooshSms-0.1.1/WhooshSms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WhooshSms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Whoosh SMS API client
 Home-page: https://github.com/totogi/whoosh-python/
 Author: Totogi
 Author-email: help@totogi.com
 Keywords: whoosh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,20 +20,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Telephony
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whoosh-python
-
-[![Tests](https://github.com/twilio/twilio-python/actions/workflows/test-and-deploy.yml/badge.svg)](https://github.com/twilio/twilio-python/actions/workflows/test-and-deploy.yml)
-[![PyPI](https://img.shields.io/pypi/v/twilio.svg)](https://pypi.python.org/pypi/twilio)
-[![PyPI](https://img.shields.io/pypi/pyversions/twilio.svg)](https://pypi.python.org/pypi/twilio)
-[![Learn OSS Contribution in TwilioQuest](https://img.shields.io/static/v1?label=TwilioQuest&message=Learn%20to%20contribute%21&color=F22F46&labelColor=1f243c&style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAMAAAD04JH5AAAASFBMVEUAAAAZGRkcHBwjIyMoKCgAAABgYGBoaGiAgICMjIyzs7PJycnMzMzNzc3UoBfd3d3m5ubqrhfrMEDu7u739/f4vSb/3AD///9tbdyEAAAABXRSTlMAAAAAAMJrBrEAAAKoSURBVHgB7ZrRcuI6EESdyxXGYoNFvMD//+l2bSszRgyUYpFAsXOeiJGmj4NkuWx1Qeh+Ekl9DgEXOBwOx+Px5xyQhDykfgq4wG63MxxaR4ddIkg6Ul3g84vCIcjPBA5gmUMeXESrlukuoK33+33uID8TWeLAdOWsKpJYzwVMB7bOzYSGOciyUlXSn0/ABXTosJ1M1SbypZ4O4MbZuIDMU02PMbauhhHMHXbmebmALIiEbbbbbUrpF1gwE9kFfRNAJaP+FQEXCCTGyJ4ngDrjOFo3jEL5JdqjF/pueR4cCeCGgAtwmuRS6gDwaRiGvu+DMFwSBLTE3+jF8JyuV1okPZ+AC4hDFhCHyHQjdjPHUKFDlHSJkHQXMB3KpSwXNGJPcwwTdZiXlRN0gSp0zpWxNtM0beYE0nRH6QIbO7rawwXaBYz0j78gxjokDuv12gVeUuBD0MDi0OQCLvDaAho4juP1Q/jkAncXqIcCfd+7gAu4QLMACCLxpRsSuQh0igu0C9Svhi7weAGZg50L3IE3cai4IfkNZAC8dfdhsUD3CgKBVC9JE5ABAFzg4QL/taYPAAWrHdYcgfLaIgAXWJ7OV38n1LEF8tt2TH29E+QAoDoO5Ve/LtCQDmKM9kPbvCEBApK+IXzbcSJ0cIGF6e8gpcRhUDogWZ8JnaWjPXc/fNnBBUKRngiHgTUSivSzDRDgHZQOLvBQgf8rRt+VdBUUhwkU6VpJ+xcOwQUqZr+mR0kvBUgv6cB4+37hQAkXqE8PwGisGhJtN4xAHMzrsgvI7rccXqSvKh6jltGlrOHA3Xk1At3LC4QiPdX9/0ndHpGVvTjR4bZA1ypAKgVcwE5vx74ulwIugDt8e/X7JgfkucBMIAr26ndnB4UCLnDOqvteQsHlgX9N4A+c4cW3DXSPbwAAAABJRU5ErkJggg==)](https://twil.io/learn-open-source)
-
 ## Versions
 
 `whoosh-python` uses a modified version of [Semantic Versioning](https://semver.org) for all changes. [See this document](VERSIONS.md) for details.
 
 ### Supported Python Versions
 
 This library supports the following Python implementations:
@@ -46,40 +40,40 @@
 
 ## Installation
 
 Install from PyPi using [pip](https://pip.pypa.io/en/latest/), a
 package manager for Python.
 
 ```shell
-pip3 install twilio
+pip3 install WhooshSms
 ```
 
 If pip install fails on Windows, check the path length of the directory. If it is greater 260 characters then enable [Long Paths](https://docs.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation) or choose other shorter location.
 
 Don't have pip installed? Try installing it, by running this from the command
 line:
 
 ```shell
 curl https://bootstrap.pypa.io/get-pip.py | python
 ```
 
 Or, you can [download the source code
-(ZIP)](https://github.com/twilio/twilio-python/zipball/main 'twilio-python
+(ZIP)](https://github.com/totogi/whoosh-python/zipball/main 'whoosh-python
 source code') for `whoosh-python`, and then run:
 
 ```shell
 python3 setup.py install
 ```
 
 > **Info**
-> If the command line gives you an error message that says Permission Denied, try running the above commands with `sudo` (e.g., `sudo pip3 install twilio`).
+> If the command line gives you an error message that says Permission Denied, try running the above commands with `sudo` (e.g., `sudo pip3 install WhooshSms`).
 
 ### Test your installation
 
-Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Twilio account](https://console.twilio.com). The `to` phone number will be your own mobile phone.
+Try sending yourself an SMS message. Save the following code sample to your computer with a text editor. Be sure to update the `account_sid`, `auth_token`, and `from_` phone number with values from your [Whoosh account](https://console.whoosh.totogidemos.com). The `to` phone number will be your own mobile phone.
 
 ```python
 from twilio.rest import Client
 
 # Your Account SID and Auth Token from console.twilio.com
 account_sid = "ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
 auth_token  = "your_auth_token"
```

### Comparing `WhooshSms-0.1.0/WhooshSms.egg-info/SOURCES.txt` & `WhooshSms-0.1.1/WhooshSms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/setup.py` & `WhooshSms-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # python setup.py install
 #
 # You need to have the setuptools module installed. Try reading the setuptools
 # documentation: http://pypi.python.org/pypi/setuptools
 
 setup(
     name="WhooshSms",
-    version="0.1.0",
+    version="0.1.1",
     description="Whoosh SMS API client",
     author="Totogi",
     author_email="help@totogi.com",
     url="https://github.com/totogi/whoosh-python/",
     keywords=["whoosh"],
     python_requires=">=3.7.0",
     install_requires=[
```

### Comparing `WhooshSms-0.1.0/twilio/base/client_base.py` & `WhooshSms-0.1.1/twilio/base/client_base.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/deserialize.py` & `WhooshSms-0.1.1/twilio/base/deserialize.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/domain.py` & `WhooshSms-0.1.1/twilio/base/domain.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/exceptions.py` & `WhooshSms-0.1.1/twilio/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/obsolete.py` & `WhooshSms-0.1.1/twilio/base/obsolete.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/page.py` & `WhooshSms-0.1.1/twilio/base/page.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/serialize.py` & `WhooshSms-0.1.1/twilio/base/serialize.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/base/version.py` & `WhooshSms-0.1.1/twilio/base/version.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/http/__init__.py` & `WhooshSms-0.1.1/twilio/http/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/http/async_http_client.py` & `WhooshSms-0.1.1/twilio/http/async_http_client.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/http/http_client.py` & `WhooshSms-0.1.1/twilio/http/http_client.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/http/request.py` & `WhooshSms-0.1.1/twilio/http/request.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/http/response.py` & `WhooshSms-0.1.1/twilio/http/response.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/http/validation_client.py` & `WhooshSms-0.1.1/twilio/http/validation_client.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/__init__.py` & `WhooshSms-0.1.1/twilio/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/access_token/__init__.py` & `WhooshSms-0.1.1/twilio/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/access_token/grants.py` & `WhooshSms-0.1.1/twilio/jwt/access_token/grants.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/client/__init__.py` & `WhooshSms-0.1.1/twilio/jwt/client/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/taskrouter/__init__.py` & `WhooshSms-0.1.1/twilio/jwt/taskrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/taskrouter/capabilities.py` & `WhooshSms-0.1.1/twilio/jwt/taskrouter/capabilities.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/jwt/validation/__init__.py` & `WhooshSms-0.1.1/twilio/jwt/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/request_validator.py` & `WhooshSms-0.1.1/twilio/request_validator.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/__init__.py` & `WhooshSms-0.1.1/twilio/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/AccountsBase.py` & `WhooshSms-0.1.1/twilio/rest/accounts/AccountsBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/__init__.py` & `WhooshSms-0.1.1/twilio/rest/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/v1/auth_token_promotion.py` & `WhooshSms-0.1.1/twilio/rest/accounts/v1/auth_token_promotion.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/__init__.py` & `WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/aws.py` & `WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/aws.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/v1/credential/public_key.py` & `WhooshSms-0.1.1/twilio/rest/accounts/v1/credential/public_key.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/accounts/v1/secondary_auth_token.py` & `WhooshSms-0.1.1/twilio/rest/accounts/v1/secondary_auth_token.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/ApiBase.py` & `WhooshSms-0.1.1/twilio/rest/api/ApiBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/address/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/address/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/address/dependent_phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/application.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/application.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/authorized_connect_app.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/authorized_connect_app.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/local.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/national.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/available_phone_number_country/voip.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/balance.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/balance.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/event.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/event.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/feedback.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/feedback.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/feedback_summary.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/feedback_summary.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/notification.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/notification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/payment.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/payment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/recording.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/recording.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/siprec.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/siprec.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/stream.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/stream.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/user_defined_message.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/user_defined_message.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/participant.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/participant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/conference/recording.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/conference/recording.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/connect_app.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/connect_app.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/local.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/key.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/key.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/feedback.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/feedback.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/message/media.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/message/media.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/new_key.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/new_key.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/new_signing_key.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/new_signing_key.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/notification.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/notification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/outgoing_caller_id.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/outgoing_caller_id.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/queue/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/queue/member.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/queue/member.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/add_on_result/payload.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/recording/transcription.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/recording/transcription.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/short_code.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/short_code.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/signing_key.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/signing_key.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/credential_list/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/credential_list/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/token.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/token.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/transcription.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/transcription.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/__init__.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/all_time.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/all_time.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/daily.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/daily.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/last_month.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/last_month.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/monthly.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/monthly.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/this_month.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/this_month.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/today.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/today.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/yearly.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/yearly.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/record/yesterday.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/record/yesterday.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/usage/trigger.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/usage/trigger.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/api/v2010/account/validation_request.py` & `WhooshSms-0.1.1/twilio/rest/api/v2010/account/validation_request.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/AutopilotBase.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/AutopilotBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/__init__.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/__init__.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/defaults.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/defaults.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/dialogue.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/model_build.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/query.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/query.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/style_sheet.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/__init__.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/field.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/sample.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/assistant/webhook.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/assistant/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/autopilot/v1/restore_assistant.py` & `WhooshSms-0.1.1/twilio/rest/autopilot/v1/restore_assistant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/BulkexportsBase.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/BulkexportsBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/__init__.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/__init__.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/day.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/day.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/export_custom_job.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/export_custom_job.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export/job.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export/job.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/bulkexports/v1/export_configuration.py` & `WhooshSms-0.1.1/twilio/rest/bulkexports/v1/export_configuration.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/ChatBase.py` & `WhooshSms-0.1.1/twilio/rest/chat/ChatBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/credential.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/invite.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/member.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/channel/message.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/role.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/user/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v1/service/user/user_channel.py` & `WhooshSms-0.1.1/twilio/rest/chat/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/credential.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/binding.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/invite.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/member.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/message.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/channel/webhook.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/role.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/user_binding.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v2/service/user/user_channel.py` & `WhooshSms-0.1.1/twilio/rest/chat/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v3/__init__.py` & `WhooshSms-0.1.1/twilio/rest/chat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/chat/v3/channel.py` & `WhooshSms-0.1.1/twilio/rest/chat/v3/channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/ContentBase.py` & `WhooshSms-0.1.1/twilio/rest/content/ContentBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/__init__.py` & `WhooshSms-0.1.1/twilio/rest/content/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/content/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/v1/content/__init__.py` & `WhooshSms-0.1.1/twilio/rest/content/v1/content/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/v1/content/approval_fetch.py` & `WhooshSms-0.1.1/twilio/rest/content/v1/content/approval_fetch.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/v1/content_and_approvals.py` & `WhooshSms-0.1.1/twilio/rest/content/v1/content_and_approvals.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/content/v1/legacy_content.py` & `WhooshSms-0.1.1/twilio/rest/content/v1/legacy_content.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/ConversationsBase.py` & `WhooshSms-0.1.1/twilio/rest/conversations/ConversationsBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/address_configuration.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/address_configuration.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/configuration/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/configuration/webhook.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/message/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/participant.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/conversation/webhook.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/credential.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/participant_conversation.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/role.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/role.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/binding.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/notification.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/notification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/configuration/webhook.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/participant.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/conversation/webhook.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/participant_conversation.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/role.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/user/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/service/user/user_conversation.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/service/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/user/__init__.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/user/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/conversations/v1/user/user_conversation.py` & `WhooshSms-0.1.1/twilio/rest/conversations/v1/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/EventsBase.py` & `WhooshSms-0.1.1/twilio/rest/events/EventsBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/__init__.py` & `WhooshSms-0.1.1/twilio/rest/events/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/event_type.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/event_type.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/schema/__init__.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/schema/schema_version.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/schema/schema_version.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/sink/__init__.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/sink/sink_test.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/sink/sink_test.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/sink/sink_validate.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/sink/sink_validate.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/subscription/__init__.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/events/v1/subscription/subscribed_event.py` & `WhooshSms-0.1.1/twilio/rest/events/v1/subscription/subscribed_event.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/FlexApiBase.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/FlexApiBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/__init__.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/assessments.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/assessments.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/channel.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/configuration.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/flex_flow.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/flex_flow.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_assessments_comment.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_assessments_comment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_conversations.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_conversations.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_questionnaires.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_questionnaires.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_questionnaires_category.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_questionnaires_question.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_segments.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_segments.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_session.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_session.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_settings_answer_sets.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_settings_comment.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_settings_comment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/insights_user_roles.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/insights_user_roles.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/__init__.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v1/web_channel.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v1/web_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/flex_api/v2/web_channels.py` & `WhooshSms-0.1.1/twilio/rest/flex_api/v2/web_channels.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/frontline_api/FrontlineApiBase.py` & `WhooshSms-0.1.1/twilio/rest/frontline_api/FrontlineApiBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/frontline_api/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/frontline_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/frontline_api/v1/user.py` & `WhooshSms-0.1.1/twilio/rest/frontline_api/v1/user.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/InsightsBase.py` & `WhooshSms-0.1.1/twilio/rest/insights/InsightsBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/__init__.py` & `WhooshSms-0.1.1/twilio/rest/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/call/__init__.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/call/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/call/annotation.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/call/annotation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/call/call_summary.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/call/call_summary.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/call/event.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/call/event.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/call/metric.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/call/metric.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/call_summaries.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/call_summaries.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/conference/__init__.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/conference/conference_participant.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/conference/conference_participant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/room/__init__.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/room/participant.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/room/participant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/insights/v1/setting.py` & `WhooshSms-0.1.1/twilio/rest/insights/v1/setting.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/IpMessagingBase.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/IpMessagingBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/credential.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/invite.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/member.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/channel/message.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/role.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/user/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/credential.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/binding.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/invite.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/member.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/message.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/role.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/__init__.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py` & `WhooshSms-0.1.1/twilio/rest/ip_messaging/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/lookups/LookupsBase.py` & `WhooshSms-0.1.1/twilio/rest/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/lookups/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/lookups/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/lookups/v1/phone_number.py` & `WhooshSms-0.1.1/twilio/rest/lookups/v1/phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/lookups/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/lookups/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/lookups/v2/phone_number.py` & `WhooshSms-0.1.1/twilio/rest/lookups/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/MediaBase.py` & `WhooshSms-0.1.1/twilio/rest/media/MediaBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/__init__.py` & `WhooshSms-0.1.1/twilio/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/media/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/v1/media_processor.py` & `WhooshSms-0.1.1/twilio/rest/media/v1/media_processor.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/v1/media_recording.py` & `WhooshSms-0.1.1/twilio/rest/media/v1/media_recording.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/v1/player_streamer/__init__.py` & `WhooshSms-0.1.1/twilio/rest/media/v1/player_streamer/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/media/v1/player_streamer/playback_grant.py` & `WhooshSms-0.1.1/twilio/rest/media/v1/player_streamer/playback_grant.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/MessagingBase.py` & `WhooshSms-0.1.1/twilio/rest/messaging/MessagingBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/__init__.py` & `WhooshSms-0.1.1/twilio/rest/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/__init__.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/brand_registration/brand_vetting.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/deactivations.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/deactivations.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/domain_certs.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/domain_certs.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/domain_config.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/domain_config.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/domain_config_messaging_service.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/domain_config_messaging_service.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/external_campaign.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/external_campaign.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/linkshortening_messaging_service.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/service/alpha_sender.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/service/alpha_sender.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/service/phone_number.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/service/short_code.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/service/us_app_to_person.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/service/us_app_to_person.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/tollfree_verification.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/tollfree_verification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/messaging/v1/usecase.py` & `WhooshSms-0.1.1/twilio/rest/messaging/v1/usecase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/MicrovisorBase.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/MicrovisorBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/__init__.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/account_config.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/account_config.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/account_secret.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/account_secret.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/app/__init__.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/app/app_manifest.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/app/app_manifest.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/__init__.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/device_config.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/device_config.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/microvisor/v1/device/device_secret.py` & `WhooshSms-0.1.1/twilio/rest/microvisor/v1/device/device_secret.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/monitor/MonitorBase.py` & `WhooshSms-0.1.1/twilio/rest/monitor/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/monitor/__init__.py` & `WhooshSms-0.1.1/twilio/rest/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/monitor/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/monitor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/monitor/v1/alert.py` & `WhooshSms-0.1.1/twilio/rest/monitor/v1/alert.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/monitor/v1/event.py` & `WhooshSms-0.1.1/twilio/rest/monitor/v1/event.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/NotifyBase.py` & `WhooshSms-0.1.1/twilio/rest/notify/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/__init__.py` & `WhooshSms-0.1.1/twilio/rest/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/notify/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/v1/credential.py` & `WhooshSms-0.1.1/twilio/rest/notify/v1/credential.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/notify/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/v1/service/binding.py` & `WhooshSms-0.1.1/twilio/rest/notify/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/notify/v1/service/notification.py` & `WhooshSms-0.1.1/twilio/rest/notify/v1/service/notification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/NumbersBase.py` & `WhooshSms-0.1.1/twilio/rest/numbers/NumbersBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/end_user.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/regulation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py` & `WhooshSms-0.1.1/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/OauthBase.py` & `WhooshSms-0.1.1/twilio/rest/oauth/OauthBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/__init__.py` & `WhooshSms-0.1.1/twilio/rest/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/oauth/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/v1/device_code.py` & `WhooshSms-0.1.1/twilio/rest/oauth/v1/device_code.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/v1/oauth.py` & `WhooshSms-0.1.1/twilio/rest/oauth/v1/oauth.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/v1/openid_discovery.py` & `WhooshSms-0.1.1/twilio/rest/oauth/v1/openid_discovery.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/v1/token.py` & `WhooshSms-0.1.1/twilio/rest/oauth/v1/token.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/oauth/v1/user_info.py` & `WhooshSms-0.1.1/twilio/rest/oauth/v1/user_info.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/PreviewBase.py` & `WhooshSms-0.1.1/twilio/rest/preview/PreviewBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/certificate.py` & `WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/certificate.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/deployment.py` & `WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/deployment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/device.py` & `WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/device.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/deployed_devices/fleet/key.py` & `WhooshSms-0.1.1/twilio/rest/preview/deployed_devices/fleet/key.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py` & `WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py` & `WhooshSms-0.1.1/twilio/rest/preview/hosted_numbers/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/marketplace/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/marketplace/available_add_on/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/marketplace/available_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py` & `WhooshSms-0.1.1/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/marketplace/installed_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py` & `WhooshSms-0.1.1/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/document/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/document/document_permission.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py` & `WhooshSms-0.1.1/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/dialogue.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/field_type/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/field_type/field_value.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/model_build.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/query.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/query.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/style_sheet.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/field.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/sample.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/task_actions.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/understand/assistant/task/task_statistics.py` & `WhooshSms-0.1.1/twilio/rest/preview/understand/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/wireless/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/wireless/command.py` & `WhooshSms-0.1.1/twilio/rest/preview/wireless/command.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/wireless/rate_plan.py` & `WhooshSms-0.1.1/twilio/rest/preview/wireless/rate_plan.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/wireless/sim/__init__.py` & `WhooshSms-0.1.1/twilio/rest/preview/wireless/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/preview/wireless/sim/usage.py` & `WhooshSms-0.1.1/twilio/rest/preview/wireless/sim/usage.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/PricingBase.py` & `WhooshSms-0.1.1/twilio/rest/pricing/PricingBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/messaging/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/messaging/country.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/messaging/country.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/phone_number/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/phone_number/country.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/phone_number/country.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/country.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/country.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v1/voice/number.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v1/voice/number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v2/country.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v2/country.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v2/number.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v2/number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/__init__.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/country.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/country.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/pricing/v2/voice/number.py` & `WhooshSms-0.1.1/twilio/rest/pricing/v2/voice/number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/ProxyBase.py` & `WhooshSms-0.1.1/twilio/rest/proxy/ProxyBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/phone_number.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/__init__.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/interaction.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/interaction.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/participant/__init__.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/session/participant/message_interaction.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/proxy/v1/service/short_code.py` & `WhooshSms-0.1.1/twilio/rest/proxy/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/routes/RoutesBase.py` & `WhooshSms-0.1.1/twilio/rest/routes/RoutesBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/routes/__init__.py` & `WhooshSms-0.1.1/twilio/rest/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/routes/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/routes/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/routes/v2/phone_number.py` & `WhooshSms-0.1.1/twilio/rest/routes/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/routes/v2/sip_domain.py` & `WhooshSms-0.1.1/twilio/rest/routes/v2/sip_domain.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/routes/v2/trunk.py` & `WhooshSms-0.1.1/twilio/rest/routes/v2/trunk.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/ServerlessBase.py` & `WhooshSms-0.1.1/twilio/rest/serverless/ServerlessBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/asset/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/asset/asset_version.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/asset/asset_version.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/build/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/build/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/build/build_status.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/build/build_status.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/deployment.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/deployment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/log.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/log.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/environment/variable.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/environment/variable.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/function_version/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py` & `WhooshSms-0.1.1/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/StudioBase.py` & `WhooshSms-0.1.1/twilio/rest/studio/StudioBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/engagement_context.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/step/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/engagement/step/step_context.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_context.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py` & `WhooshSms-0.1.1/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_context.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/flow_revision.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/flow_revision.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow/flow_test_user.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow/flow_test_user.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/studio/v2/flow_validate.py` & `WhooshSms-0.1.1/twilio/rest/studio/v2/flow_validate.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/SupersimBase.py` & `WhooshSms-0.1.1/twilio/rest/supersim/SupersimBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/__init__.py` & `WhooshSms-0.1.1/twilio/rest/supersim/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/esim_profile.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/esim_profile.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/fleet.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/fleet.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/ip_command.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/ip_command.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/network.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/network.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/network_access_profile/__init__.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/network_access_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/settings_update.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/settings_update.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/__init__.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/billing_period.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/billing_period.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/sim/sim_ip_address.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/sim/sim_ip_address.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/sms_command.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/sms_command.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/supersim/v1/usage_record.py` & `WhooshSms-0.1.1/twilio/rest/supersim/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/SyncBase.py` & `WhooshSms-0.1.1/twilio/rest/sync/SyncBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/document/__init__.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/document/document_permission.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/__init__.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/__init__.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_stream/__init__.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py` & `WhooshSms-0.1.1/twilio/rest/sync/v1/service/sync_stream/stream_message.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/TaskrouterBase.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/TaskrouterBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/__init__.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/activity.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/activity.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/event.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/event.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task/reservation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_channel.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/reservation.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py` & `WhooshSms-0.1.1/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/TrunkingBase.py` & `WhooshSms-0.1.1/twilio/rest/trunking/TrunkingBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/__init__.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/credential_list.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/credential_list.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/ip_access_control_list.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/origination_url.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/origination_url.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/phone_number.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/phone_number.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trunking/v1/trunk/recording.py` & `WhooshSms-0.1.1/twilio/rest/trunking/v1/trunk/recording.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/TrusthubBase.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/TrusthubBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/__init__.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/end_user.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/end_user.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/end_user_type.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/end_user_type.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/policies.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/policies.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/supporting_document.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/supporting_document.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/supporting_document_type.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/__init__.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py` & `WhooshSms-0.1.1/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/VerifyBase.py` & `WhooshSms-0.1.1/twilio/rest/verify/VerifyBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/__init__.py` & `WhooshSms-0.1.1/twilio/rest/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/__init__.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/form.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/form.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/safelist.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/safelist.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/__init__.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/access_token.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/access_token.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/__init__.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/challenge/notification.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/challenge/notification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/factor.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/factor.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/entity/new_factor.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/entity/new_factor.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/messaging_configuration.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/messaging_configuration.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/rate_limit/__init__.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/rate_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/rate_limit/bucket.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/rate_limit/bucket.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/verification.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/verification.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/verification_check.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/verification_check.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/service/webhook.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/service/webhook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/template.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/template.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/verification_attempt.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/verification_attempt.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/verify/v2/verification_attempts_summary.py` & `WhooshSms-0.1.1/twilio/rest/verify/v2/verification_attempts_summary.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/VideoBase.py` & `WhooshSms-0.1.1/twilio/rest/video/VideoBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/__init__.py` & `WhooshSms-0.1.1/twilio/rest/video/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/composition.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/composition.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/composition_hook.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/composition_hook.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/composition_settings.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/composition_settings.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/recording.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/recording.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/recording_settings.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/recording_settings.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/__init__.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/__init__.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/anonymize.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/anonymize.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/published_track.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/published_track.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/subscribe_rules.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/subscribe_rules.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/participant/subscribed_track.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/participant/subscribed_track.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/recording_rules.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/recording_rules.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/video/v1/room/room_recording.py` & `WhooshSms-0.1.1/twilio/rest/video/v1/room/room_recording.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/VoiceBase.py` & `WhooshSms-0.1.1/twilio/rest/voice/VoiceBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/__init__.py` & `WhooshSms-0.1.1/twilio/rest/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/archived_call.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/archived_call.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/byoc_trunk.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/byoc_trunk.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/connection_policy/__init__.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/connection_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/connection_policy/connection_policy_target.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/__init__.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/country/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/dialing_permissions/settings.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/dialing_permissions/settings.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/ip_record.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/ip_record.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/voice/v1/source_ip_mapping.py` & `WhooshSms-0.1.1/twilio/rest/voice/v1/source_ip_mapping.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/WirelessBase.py` & `WhooshSms-0.1.1/twilio/rest/wireless/WirelessBase.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/__init__.py` & `WhooshSms-0.1.1/twilio/rest/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/__init__.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/command.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/command.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/rate_plan.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/rate_plan.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/__init__.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/data_session.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/data_session.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/sim/usage_record.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/sim/usage_record.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/rest/wireless/v1/usage_record.py` & `WhooshSms-0.1.1/twilio/rest/wireless/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/twiml/__init__.py` & `WhooshSms-0.1.1/twilio/twiml/__init__.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/twiml/fax_response.py` & `WhooshSms-0.1.1/twilio/twiml/fax_response.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/twiml/messaging_response.py` & `WhooshSms-0.1.1/twilio/twiml/messaging_response.py`

 * *Files identical despite different names*

### Comparing `WhooshSms-0.1.0/twilio/twiml/voice_response.py` & `WhooshSms-0.1.1/twilio/twiml/voice_response.py`

 * *Files identical despite different names*

