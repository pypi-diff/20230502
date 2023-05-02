# Comparing `tmp/moneykit-0.0.8.tar.gz` & `tmp/moneykit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneykit-0.0.8.tar", max compression
+gzip compressed data, was "moneykit-0.0.9.tar", max compression
```

## Comparing `moneykit-0.0.8.tar` & `moneykit-0.0.9.tar`

### file list

```diff
@@ -1,391 +1,391 @@
--rw-r--r--   0        0        0    20273 2023-05-01 19:33:44.000000 moneykit-0.0.8/README.md
--rw-r--r--   0        0        0      739 2023-05-01 19:35:25.118100 moneykit-0.0.8/moneykit/__init__.py
--rw-r--r--   0        0        0    56712 2023-05-01 19:33:50.823969 moneykit-0.0.8/moneykit/api_client.py
--rw-r--r--   0        0        0      215 2023-05-01 19:33:48.062027 moneykit-0.0.8/moneykit/apis/__init__.py
--rw-r--r--   0        0        0     3789 2023-05-01 19:33:50.820886 moneykit-0.0.8/moneykit/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/apis/paths/__init__.py
--rw-r--r--   0        0        0      108 2023-05-01 19:33:40.000000 moneykit-0.0.8/moneykit/apis/paths/auth_introspect.py
--rw-r--r--   0        0        0      101 2023-05-01 19:33:40.000000 moneykit-0.0.8/moneykit/apis/paths/auth_token.py
--rw-r--r--   0        0        0      103 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/institutions.py
--rw-r--r--   0        0        0      131 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/institutions_institution_id.py
--rw-r--r--   0        0        0      146 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/institutions_institution_id_styling.py
--rw-r--r--   0        0        0      105 2023-05-01 19:33:42.000000 moneykit-0.0.8/moneykit/apis/paths/link_session.py
--rw-r--r--   0        0        0      133 2023-05-01 19:33:42.000000 moneykit-0.0.8/moneykit/apis/paths/link_session_exchange_token.py
--rw-r--r--   0        0        0      239 2023-05-01 19:33:50.823217 moneykit-0.0.8/moneykit/apis/paths/links_id.py
--rw-r--r--   0        0        0      111 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_accounts.py
--rw-r--r--   0        0        0      131 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_accounts_account_id.py
--rw-r--r--   0        0        0      126 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_accounts_numbers.py
--rw-r--r--   0        0        0      111 2023-05-01 19:33:41.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_identity.py
--rw-r--r--   0        0        0      114 2023-05-01 19:33:42.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_products.py
--rw-r--r--   0        0        0      119 2023-05-01 19:33:43.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_transactions.py
--rw-r--r--   0        0        0      128 2023-05-01 19:33:43.000000 moneykit-0.0.8/moneykit/apis/paths/links_id_transactions_sync.py
--rw-r--r--   0        0        0      111 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/apis/paths/users_id_accounts.py
--rw-r--r--   0        0        0      105 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/apis/paths/users_id_links.py
--rw-r--r--   0        0        0      119 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/apis/paths/users_id_transactions.py
--rw-r--r--   0        0        0      116 2023-05-01 19:33:40.000000 moneykit-0.0.8/moneykit/apis/paths/well_known_jwks_json.py
--rw-r--r--   0        0        0     1650 2023-05-01 19:33:50.821311 moneykit-0.0.8/moneykit/apis/tag_to_api.py
--rw-r--r--   0        0        0      575 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/apis/tags/__init__.py
--rw-r--r--   0        0        0      718 2023-05-01 19:33:50.817469 moneykit-0.0.8/moneykit/apis/tags/access_token_api.py
--rw-r--r--   0        0        0      552 2023-05-01 19:33:48.071183 moneykit-0.0.8/moneykit/apis/tags/account_numbers_api.py
--rw-r--r--   0        0        0      797 2023-05-01 19:33:50.817732 moneykit-0.0.8/moneykit/apis/tags/accounts_api.py
--rw-r--r--   0        0        0      530 2023-05-01 19:33:48.072784 moneykit-0.0.8/moneykit/apis/tags/identity_api.py
--rw-r--r--   0        0        0      743 2023-05-01 19:33:50.817991 moneykit-0.0.8/moneykit/apis/tags/institutions_api.py
--rw-r--r--   0        0        0      630 2023-05-01 19:33:48.077157 moneykit-0.0.8/moneykit/apis/tags/link_session_api.py
--rw-r--r--   0        0        0      722 2023-05-01 19:33:50.819676 moneykit-0.0.8/moneykit/apis/tags/links_api.py
--rw-r--r--   0        0        0      535 2023-05-01 19:33:48.076709 moneykit-0.0.8/moneykit/apis/tags/products_api.py
--rw-r--r--   0        0        0      743 2023-05-01 19:33:48.077894 moneykit-0.0.8/moneykit/apis/tags/transactions_api.py
--rw-r--r--   0        0        0      706 2023-05-01 19:33:48.079724 moneykit-0.0.8/moneykit/apis/tags/users_api.py
--rw-r--r--   0        0        0    18643 2023-05-01 19:33:50.817208 moneykit-0.0.8/moneykit/configuration.py
--rw-r--r--   0        0        0     4490 2023-05-01 19:33:48.100550 moneykit-0.0.8/moneykit/exceptions.py
--rw-r--r--   0        0        0      342 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/model/__init__.py
--rw-r--r--   0        0        0    11454 2023-05-01 19:33:50.840309 moneykit-0.0.8/moneykit/model/account.py
--rw-r--r--   0        0        0    11337 2023-05-01 19:33:50.826352 moneykit-0.0.8/moneykit/model/account.pyi
--rw-r--r--   0        0        0     9362 2023-05-01 19:33:50.814276 moneykit-0.0.8/moneykit/model/account_balances.py
--rw-r--r--   0        0        0     9265 2023-05-01 19:33:50.828569 moneykit-0.0.8/moneykit/model/account_balances.pyi
--rw-r--r--   0        0        0     5097 2023-05-01 19:33:50.814015 moneykit-0.0.8/moneykit/model/account_group.py
--rw-r--r--   0        0        0     5034 2023-05-01 19:33:50.815503 moneykit-0.0.8/moneykit/model/account_group.pyi
--rw-r--r--   0        0        0    12821 2023-05-01 19:33:50.822738 moneykit-0.0.8/moneykit/model/account_identity.py
--rw-r--r--   0        0        0    12684 2023-05-01 19:33:50.815975 moneykit-0.0.8/moneykit/model/account_identity.pyi
--rw-r--r--   0        0        0     7878 2023-05-01 19:33:50.841243 moneykit-0.0.8/moneykit/model/account_numbers.py
--rw-r--r--   0        0        0     7774 2023-05-01 19:33:50.827430 moneykit-0.0.8/moneykit/model/account_numbers.pyi
--rw-r--r--   0        0        0     5932 2023-05-01 19:33:50.843882 moneykit-0.0.8/moneykit/model/account_numbers_link_product.py
--rw-r--r--   0        0        0     5852 2023-05-01 19:33:50.827326 moneykit-0.0.8/moneykit/model/account_numbers_link_product.pyi
--rw-r--r--   0        0        0     3467 2023-05-01 19:33:50.830935 moneykit-0.0.8/moneykit/model/account_numbers_product_settings.py
--rw-r--r--   0        0        0     3409 2023-05-01 19:33:50.844662 moneykit-0.0.8/moneykit/model/account_numbers_product_settings.pyi
--rw-r--r--   0        0        0     2418 2023-05-01 19:33:50.827189 moneykit-0.0.8/moneykit/model/account_type.py
--rw-r--r--   0        0        0     1831 2023-05-01 19:33:50.826268 moneykit-0.0.8/moneykit/model/account_type.pyi
--rw-r--r--   0        0        0    14837 2023-05-01 19:33:50.818113 moneykit-0.0.8/moneykit/model/account_with_account_numbers.py
--rw-r--r--   0        0        0    14701 2023-05-01 19:33:50.810093 moneykit-0.0.8/moneykit/model/account_with_account_numbers.pyi
--rw-r--r--   0        0        0     5109 2023-05-01 19:33:50.814935 moneykit-0.0.8/moneykit/model/accounts_link_product.py
--rw-r--r--   0        0        0     5048 2023-05-01 19:33:50.836442 moneykit-0.0.8/moneykit/model/accounts_link_product.pyi
--rw-r--r--   0        0        0     5023 2023-05-01 19:33:50.828644 moneykit-0.0.8/moneykit/model/ach_number.py
--rw-r--r--   0        0        0     4974 2023-05-01 19:33:50.839075 moneykit-0.0.8/moneykit/model/ach_number.pyi
--rw-r--r--   0        0        0     8379 2023-05-01 19:33:50.843063 moneykit-0.0.8/moneykit/model/address.py
--rw-r--r--   0        0        0     8248 2023-05-01 19:33:50.841927 moneykit-0.0.8/moneykit/model/address.pyi
--rw-r--r--   0        0        0     5259 2023-05-01 19:33:50.830284 moneykit-0.0.8/moneykit/model/api_error_auth_expired_access_token_response.py
--rw-r--r--   0        0        0     4981 2023-05-01 19:33:50.833461 moneykit-0.0.8/moneykit/model/api_error_auth_expired_access_token_response.pyi
--rw-r--r--   0        0        0     5291 2023-05-01 19:33:50.819044 moneykit-0.0.8/moneykit/model/api_error_auth_unauthorized_response.py
--rw-r--r--   0        0        0     5030 2023-05-01 19:33:50.821244 moneykit-0.0.8/moneykit/model/api_error_auth_unauthorized_response.pyi
--rw-r--r--   0        0        0     5225 2023-05-01 19:33:50.837516 moneykit-0.0.8/moneykit/model/api_error_rate_limit_exceeded_response.py
--rw-r--r--   0        0        0     4959 2023-05-01 19:33:50.832183 moneykit-0.0.8/moneykit/model/api_error_rate_limit_exceeded_response.pyi
--rw-r--r--   0        0        0     3626 2023-05-01 19:33:50.811445 moneykit-0.0.8/moneykit/model/bacs_number.py
--rw-r--r--   0        0        0     3582 2023-05-01 19:33:50.810830 moneykit-0.0.8/moneykit/model/bacs_number.pyi
--rw-r--r--   0        0        0     5566 2023-05-01 19:33:50.844389 moneykit-0.0.8/moneykit/model/basic_account_details.py
--rw-r--r--   0        0        0     5484 2023-05-01 19:33:50.832288 moneykit-0.0.8/moneykit/model/basic_account_details.pyi
--rw-r--r--   0        0        0     1162 2023-05-01 19:33:50.831188 moneykit-0.0.8/moneykit/model/country.py
--rw-r--r--   0        0        0     1025 2023-05-01 19:33:50.844154 moneykit-0.0.8/moneykit/model/country.pyi
--rw-r--r--   0        0        0    17582 2023-05-01 19:33:50.834397 moneykit-0.0.8/moneykit/model/create_link_session_request.py
--rw-r--r--   0        0        0    17291 2023-05-01 19:33:50.813291 moneykit-0.0.8/moneykit/model/create_link_session_request.pyi
--rw-r--r--   0        0        0     2943 2023-05-01 19:33:50.836746 moneykit-0.0.8/moneykit/model/create_link_session_response.py
--rw-r--r--   0        0        0     2903 2023-05-01 19:33:50.816198 moneykit-0.0.8/moneykit/model/create_link_session_response.pyi
--rw-r--r--   0        0        0    18827 2023-05-01 19:33:50.813524 moneykit-0.0.8/moneykit/model/currency.py
--rw-r--r--   0        0        0    13878 2023-05-01 19:33:50.849503 moneykit-0.0.8/moneykit/model/currency.pyi
--rw-r--r--   0        0        0     3163 2023-05-01 19:33:50.830793 moneykit-0.0.8/moneykit/model/cursor_pagination.py
--rw-r--r--   0        0        0     3122 2023-05-01 19:33:50.845245 moneykit-0.0.8/moneykit/model/cursor_pagination.pyi
--rw-r--r--   0        0        0     3473 2023-05-01 19:33:50.828254 moneykit-0.0.8/moneykit/model/customer_app.py
--rw-r--r--   0        0        0     3415 2023-05-01 19:33:50.810491 moneykit-0.0.8/moneykit/model/customer_app.pyi
--rw-r--r--   0        0        0     4489 2023-05-01 19:33:50.830195 moneykit-0.0.8/moneykit/model/eft_number.py
--rw-r--r--   0        0        0     4427 2023-05-01 19:33:50.813050 moneykit-0.0.8/moneykit/model/eft_number.pyi
--rw-r--r--   0        0        0     3449 2023-05-01 19:33:50.814413 moneykit-0.0.8/moneykit/model/email.py
--rw-r--r--   0        0        0     3391 2023-05-01 19:33:50.809633 moneykit-0.0.8/moneykit/model/email.pyi
--rw-r--r--   0        0        0     2933 2023-05-01 19:33:50.844721 moneykit-0.0.8/moneykit/model/exchange_token_request.py
--rw-r--r--   0        0        0     2893 2023-05-01 19:33:50.838744 moneykit-0.0.8/moneykit/model/exchange_token_request.pyi
--rw-r--r--   0        0        0     6194 2023-05-01 19:33:50.817623 moneykit-0.0.8/moneykit/model/exchange_token_response.py
--rw-r--r--   0        0        0     6133 2023-05-01 19:33:50.818959 moneykit-0.0.8/moneykit/model/exchange_token_response.pyi
--rw-r--r--   0        0        0     4350 2023-05-01 19:33:50.832813 moneykit-0.0.8/moneykit/model/generate_access_token_response.py
--rw-r--r--   0        0        0     4274 2023-05-01 19:33:50.830961 moneykit-0.0.8/moneykit/model/generate_access_token_response.pyi
--rw-r--r--   0        0        0     4468 2023-05-01 19:33:50.831778 moneykit-0.0.8/moneykit/model/get_account_numbers_response.py
--rw-r--r--   0        0        0     4405 2023-05-01 19:33:50.836705 moneykit-0.0.8/moneykit/model/get_account_numbers_response.pyi
--rw-r--r--   0        0        0     6175 2023-05-01 19:33:50.837383 moneykit-0.0.8/moneykit/model/get_account_response.py
--rw-r--r--   0        0        0     6114 2023-05-01 19:33:50.815376 moneykit-0.0.8/moneykit/model/get_account_response.pyi
--rw-r--r--   0        0        0     6991 2023-05-01 19:33:50.834694 moneykit-0.0.8/moneykit/model/get_accounts_response.py
--rw-r--r--   0        0        0     6928 2023-05-01 19:33:50.828630 moneykit-0.0.8/moneykit/model/get_accounts_response.pyi
--rw-r--r--   0        0        0     7164 2023-05-01 19:33:50.827857 moneykit-0.0.8/moneykit/model/get_institutions_response.py
--rw-r--r--   0        0        0     7101 2023-05-01 19:33:50.815268 moneykit-0.0.8/moneykit/model/get_institutions_response.pyi
--rw-r--r--   0        0        0    10245 2023-05-01 19:33:50.825697 moneykit-0.0.8/moneykit/model/get_transactions_response.py
--rw-r--r--   0        0        0    10108 2023-05-01 19:33:50.820451 moneykit-0.0.8/moneykit/model/get_transactions_response.pyi
--rw-r--r--   0        0        0     3894 2023-05-01 19:33:50.833062 moneykit-0.0.8/moneykit/model/get_user_accounts_response.py
--rw-r--r--   0        0        0     3849 2023-05-01 19:33:50.811936 moneykit-0.0.8/moneykit/model/get_user_accounts_response.pyi
--rw-r--r--   0        0        0     3874 2023-05-01 19:33:50.823650 moneykit-0.0.8/moneykit/model/get_user_links_response.py
--rw-r--r--   0        0        0     3829 2023-05-01 19:33:50.827692 moneykit-0.0.8/moneykit/model/get_user_links_response.pyi
--rw-r--r--   0        0        0     7425 2023-05-01 19:33:50.815563 moneykit-0.0.8/moneykit/model/get_user_transactions_response.py
--rw-r--r--   0        0        0     7306 2023-05-01 19:33:50.829878 moneykit-0.0.8/moneykit/model/get_user_transactions_response.pyi
--rw-r--r--   0        0        0     6893 2023-05-01 19:33:50.832043 moneykit-0.0.8/moneykit/model/http_validation_error.py
--rw-r--r--   0        0        0     6594 2023-05-01 19:33:50.829800 moneykit-0.0.8/moneykit/model/http_validation_error.pyi
--rw-r--r--   0        0        0     5871 2023-05-01 19:33:50.816998 moneykit-0.0.8/moneykit/model/identity_link_product.py
--rw-r--r--   0        0        0     5791 2023-05-01 19:33:50.824241 moneykit-0.0.8/moneykit/model/identity_link_product.pyi
--rw-r--r--   0        0        0     3455 2023-05-01 19:33:50.830162 moneykit-0.0.8/moneykit/model/identity_product_settings.py
--rw-r--r--   0        0        0     3397 2023-05-01 19:33:50.824089 moneykit-0.0.8/moneykit/model/identity_product_settings.pyi
--rw-r--r--   0        0        0     4332 2023-05-01 19:33:50.820095 moneykit-0.0.8/moneykit/model/identity_response.py
--rw-r--r--   0        0        0     4269 2023-05-01 19:33:50.836187 moneykit-0.0.8/moneykit/model/identity_response.pyi
--rw-r--r--   0        0        0    10361 2023-05-01 19:33:50.817215 moneykit-0.0.8/moneykit/model/institution.py
--rw-r--r--   0        0        0    10223 2023-05-01 19:33:50.823129 moneykit-0.0.8/moneykit/model/institution.pyi
--rw-r--r--   0        0        0     5215 2023-05-01 19:33:50.835146 moneykit-0.0.8/moneykit/model/institution_error_not_found_response.py
--rw-r--r--   0        0        0     4953 2023-05-01 19:33:50.810752 moneykit-0.0.8/moneykit/model/institution_error_not_found_response.pyi
--rw-r--r--   0        0        0     9656 2023-05-01 19:33:50.826142 moneykit-0.0.8/moneykit/model/institution_styling_response.py
--rw-r--r--   0        0        0     9489 2023-05-01 19:33:50.825561 moneykit-0.0.8/moneykit/model/institution_styling_response.pyi
--rw-r--r--   0        0        0     3388 2023-05-01 19:33:50.811992 moneykit-0.0.8/moneykit/model/international_number.py
--rw-r--r--   0        0        0     3330 2023-05-01 19:33:50.838122 moneykit-0.0.8/moneykit/model/international_number.pyi
--rw-r--r--   0        0        0     8829 2023-05-01 19:33:50.814631 moneykit-0.0.8/moneykit/model/introspect_client_response.py
--rw-r--r--   0        0        0     8713 2023-05-01 19:33:50.810368 moneykit-0.0.8/moneykit/model/introspect_client_response.pyi
--rw-r--r--   0        0        0     3841 2023-05-01 19:33:50.816429 moneykit-0.0.8/moneykit/model/jwk_set.py
--rw-r--r--   0        0        0     3798 2023-05-01 19:33:50.819500 moneykit-0.0.8/moneykit/model/jwk_set.pyi
--rw-r--r--   0        0        0    16329 2023-05-01 19:33:50.829373 moneykit-0.0.8/moneykit/model/link_common.py
--rw-r--r--   0        0        0    16184 2023-05-01 19:33:50.818773 moneykit-0.0.8/moneykit/model/link_common.pyi
--rw-r--r--   0        0        0     1836 2023-05-01 19:33:50.826051 moneykit-0.0.8/moneykit/model/link_error.py
--rw-r--r--   0        0        0     1451 2023-05-01 19:33:50.840104 moneykit-0.0.8/moneykit/model/link_error.pyi
--rw-r--r--   0        0        0     5991 2023-05-01 19:33:50.835436 moneykit-0.0.8/moneykit/model/link_error_bad_state_response.py
--rw-r--r--   0        0        0     5754 2023-05-01 19:33:50.812932 moneykit-0.0.8/moneykit/model/link_error_bad_state_response.pyi
--rw-r--r--   0        0        0     5191 2023-05-01 19:33:50.823506 moneykit-0.0.8/moneykit/model/link_error_deleted_response.py
--rw-r--r--   0        0        0     4947 2023-05-01 19:33:50.809742 moneykit-0.0.8/moneykit/model/link_error_deleted_response.pyi
--rw-r--r--   0        0        0     5291 2023-05-01 19:33:50.825775 moneykit-0.0.8/moneykit/model/link_error_forbidden_action_response.py
--rw-r--r--   0        0        0     5030 2023-05-01 19:33:50.811758 moneykit-0.0.8/moneykit/model/link_error_forbidden_action_response.pyi
--rw-r--r--   0        0        0     5173 2023-05-01 19:33:50.809884 moneykit-0.0.8/moneykit/model/link_error_not_found_response.py
--rw-r--r--   0        0        0     4925 2023-05-01 19:33:50.821853 moneykit-0.0.8/moneykit/model/link_error_not_found_response.pyi
--rw-r--r--   0        0        0     5233 2023-05-01 19:33:50.834848 moneykit-0.0.8/moneykit/model/link_error_unauthorized_access_response.py
--rw-r--r--   0        0        0     4965 2023-05-01 19:33:50.831072 moneykit-0.0.8/moneykit/model/link_error_unauthorized_access_response.pyi
--rw-r--r--   0        0        0     1461 2023-05-01 19:33:50.824432 moneykit-0.0.8/moneykit/model/link_permission_scope.py
--rw-r--r--   0        0        0     1229 2023-05-01 19:33:50.830412 moneykit-0.0.8/moneykit/model/link_permission_scope.pyi
--rw-r--r--   0        0        0     3654 2023-05-01 19:33:50.834557 moneykit-0.0.8/moneykit/model/link_permissions.py
--rw-r--r--   0        0        0     3610 2023-05-01 19:33:50.824957 moneykit-0.0.8/moneykit/model/link_permissions.pyi
--rw-r--r--   0        0        0     4930 2023-05-01 19:33:50.830001 moneykit-0.0.8/moneykit/model/link_products.py
--rw-r--r--   0        0        0     4850 2023-05-01 19:33:50.816812 moneykit-0.0.8/moneykit/model/link_products.pyi
--rw-r--r--   0        0        0    20792 2023-05-01 19:33:50.832924 moneykit-0.0.8/moneykit/model/link_response.py
--rw-r--r--   0        0        0    20610 2023-05-01 19:33:50.814575 moneykit-0.0.8/moneykit/model/link_response.pyi
--rw-r--r--   0        0        0     8548 2023-05-01 19:33:50.811244 moneykit-0.0.8/moneykit/model/link_session_customer_user.py
--rw-r--r--   0        0        0     8207 2023-05-01 19:33:50.820180 moneykit-0.0.8/moneykit/model/link_session_customer_user.pyi
--rw-r--r--   0        0        0     4714 2023-05-01 19:33:50.841982 moneykit-0.0.8/moneykit/model/link_session_customer_user_email.py
--rw-r--r--   0        0        0     4391 2023-05-01 19:33:50.818322 moneykit-0.0.8/moneykit/model/link_session_customer_user_email.pyi
--rw-r--r--   0        0        0     7373 2023-05-01 19:33:50.811116 moneykit-0.0.8/moneykit/model/link_session_customer_user_phone.py
--rw-r--r--   0        0        0     7031 2023-05-01 19:33:50.810159 moneykit-0.0.8/moneykit/model/link_session_customer_user_phone.pyi
--rw-r--r--   0        0        0     5337 2023-05-01 19:33:50.826954 moneykit-0.0.8/moneykit/model/link_session_error_forbidden_config_response.py
--rw-r--r--   0        0        0     5060 2023-05-01 19:33:50.837172 moneykit-0.0.8/moneykit/model/link_session_error_forbidden_config_response.pyi
--rw-r--r--   0        0        0     5355 2023-05-01 19:33:50.833212 moneykit-0.0.8/moneykit/model/link_session_error_invalid_token_exchange.py
--rw-r--r--   0        0        0     5066 2023-05-01 19:33:50.825580 moneykit-0.0.8/moneykit/model/link_session_error_invalid_token_exchange.pyi
--rw-r--r--   0        0        0    10704 2023-05-01 19:33:50.819591 moneykit-0.0.8/moneykit/model/link_session_setting_overrides.py
--rw-r--r--   0        0        0    10536 2023-05-01 19:33:50.838610 moneykit-0.0.8/moneykit/model/link_session_setting_overrides.pyi
--rw-r--r--   0        0        0     1528 2023-05-01 19:33:50.833254 moneykit-0.0.8/moneykit/model/link_state.py
--rw-r--r--   0        0        0     1253 2023-05-01 19:33:50.831188 moneykit-0.0.8/moneykit/model/link_state.pyi
--rw-r--r--   0        0        0    11804 2023-05-01 19:33:50.842679 moneykit-0.0.8/moneykit/model/link_state_changed_webhook.py
--rw-r--r--   0        0        0    11152 2023-05-01 19:33:50.829797 moneykit-0.0.8/moneykit/model/link_state_changed_webhook.pyi
--rw-r--r--   0        0        0     1124 2023-05-01 19:33:50.825889 moneykit-0.0.8/moneykit/model/money_kit_env.py
--rw-r--r--   0        0        0      986 2023-05-01 19:33:50.830919 moneykit-0.0.8/moneykit/model/money_kit_env.pyi
--rw-r--r--   0        0        0     3586 2023-05-01 19:33:50.818564 moneykit-0.0.8/moneykit/model/money_link_features.py
--rw-r--r--   0        0        0     3542 2023-05-01 19:33:50.819728 moneykit-0.0.8/moneykit/model/money_link_features.pyi
--rw-r--r--   0        0        0     8201 2023-05-01 19:33:50.809948 moneykit-0.0.8/moneykit/model/owner.py
--rw-r--r--   0        0        0     8097 2023-05-01 19:33:50.839959 moneykit-0.0.8/moneykit/model/owner.pyi
--rw-r--r--   0        0        0     6748 2023-05-01 19:33:50.814335 moneykit-0.0.8/moneykit/model/phone_number.py
--rw-r--r--   0        0        0     6669 2023-05-01 19:33:50.819583 moneykit-0.0.8/moneykit/model/phone_number.pyi
--rw-r--r--   0        0        0     1308 2023-05-01 19:33:50.824576 moneykit-0.0.8/moneykit/model/phone_number_type.py
--rw-r--r--   0        0        0     1124 2023-05-01 19:33:50.837084 moneykit-0.0.8/moneykit/model/phone_number_type.pyi
--rw-r--r--   0        0        0     1419 2023-05-01 19:33:50.810890 moneykit-0.0.8/moneykit/model/product.py
--rw-r--r--   0        0        0     1187 2023-05-01 19:33:50.830695 moneykit-0.0.8/moneykit/model/product.pyi
--rw-r--r--   0        0        0    12687 2023-05-01 19:33:50.814279 moneykit-0.0.8/moneykit/model/products_settings.py
--rw-r--r--   0        0        0    12620 2023-05-01 19:33:50.838351 moneykit-0.0.8/moneykit/model/products_settings.pyi
--rw-r--r--   0        0        0     1427 2023-05-01 19:33:50.820156 moneykit-0.0.8/moneykit/model/provider.py
--rw-r--r--   0        0        0     1202 2023-05-01 19:33:50.820289 moneykit-0.0.8/moneykit/model/provider.pyi
--rw-r--r--   0        0        0     3578 2023-05-01 19:33:50.844499 moneykit-0.0.8/moneykit/model/refresh_products_request.py
--rw-r--r--   0        0        0     3493 2023-05-01 19:33:50.834089 moneykit-0.0.8/moneykit/model/refresh_products_request.pyi
--rw-r--r--   0        0        0     6841 2023-05-01 19:33:50.832090 moneykit-0.0.8/moneykit/model/requested_link_permission.py
--rw-r--r--   0        0        0     6762 2023-05-01 19:33:50.828780 moneykit-0.0.8/moneykit/model/requested_link_permission.pyi
--rw-r--r--   0        0        0     1029 2023-05-01 19:33:50.815681 moneykit-0.0.8/moneykit/model/supported_version.py
--rw-r--r--   0        0        0      919 2023-05-01 19:33:50.827567 moneykit-0.0.8/moneykit/model/supported_version.pyi
--rw-r--r--   0        0        0    12832 2023-05-01 19:33:50.819304 moneykit-0.0.8/moneykit/model/transaction.py
--rw-r--r--   0        0        0    12654 2023-05-01 19:33:50.821895 moneykit-0.0.8/moneykit/model/transaction.pyi
--rw-r--r--   0        0        0     6744 2023-05-01 19:33:50.825582 moneykit-0.0.8/moneykit/model/transaction_diff.py
--rw-r--r--   0        0        0     6660 2023-05-01 19:33:50.821751 moneykit-0.0.8/moneykit/model/transaction_diff.pyi
--rw-r--r--   0        0        0    12987 2023-05-01 19:33:50.822991 moneykit-0.0.8/moneykit/model/transaction_sync_response.py
--rw-r--r--   0        0        0    12887 2023-05-01 19:33:50.841550 moneykit-0.0.8/moneykit/model/transaction_sync_response.pyi
--rw-r--r--   0        0        0     1104 2023-05-01 19:33:50.835730 moneykit-0.0.8/moneykit/model/transaction_type.py
--rw-r--r--   0        0        0      978 2023-05-01 19:33:50.826867 moneykit-0.0.8/moneykit/model/transaction_type.pyi
--rw-r--r--   0        0        0     1110 2023-05-01 19:33:50.823431 moneykit-0.0.8/moneykit/model/transaction_type_filter.py
--rw-r--r--   0        0        0      984 2023-05-01 19:33:50.830077 moneykit-0.0.8/moneykit/model/transaction_type_filter.pyi
--rw-r--r--   0        0        0     5911 2023-05-01 19:33:50.831647 moneykit-0.0.8/moneykit/model/transactions_link_product.py
--rw-r--r--   0        0        0     5831 2023-05-01 19:33:50.812081 moneykit-0.0.8/moneykit/model/transactions_link_product.pyi
--rw-r--r--   0        0        0     4128 2023-05-01 19:33:50.822632 moneykit-0.0.8/moneykit/model/transactions_product_settings.py
--rw-r--r--   0        0        0     4052 2023-05-01 19:33:50.824339 moneykit-0.0.8/moneykit/model/transactions_product_settings.pyi
--rw-r--r--   0        0        0     4719 2023-05-01 19:33:50.812693 moneykit-0.0.8/moneykit/model/update_link_request.py
--rw-r--r--   0        0        0     4584 2023-05-01 19:33:50.825108 moneykit-0.0.8/moneykit/model/update_link_request.pyi
--rw-r--r--   0        0        0     4612 2023-05-01 19:33:50.820797 moneykit-0.0.8/moneykit/model/user_accounts_out.py
--rw-r--r--   0        0        0     4568 2023-05-01 19:33:50.812609 moneykit-0.0.8/moneykit/model/user_accounts_out.pyi
--rw-r--r--   0        0        0     4606 2023-05-01 19:33:50.816895 moneykit-0.0.8/moneykit/model/user_links_out.py
--rw-r--r--   0        0        0     4562 2023-05-01 19:33:50.816110 moneykit-0.0.8/moneykit/model/user_links_out.pyi
--rw-r--r--   0        0        0     4704 2023-05-01 19:33:50.810670 moneykit-0.0.8/moneykit/model/user_transactions_paged_response.py
--rw-r--r--   0        0        0     4660 2023-05-01 19:33:50.822220 moneykit-0.0.8/moneykit/model/user_transactions_paged_response.pyi
--rw-r--r--   0        0        0     9395 2023-05-01 19:33:50.821188 moneykit-0.0.8/moneykit/model/validation_error.py
--rw-r--r--   0        0        0     9315 2023-05-01 19:33:50.832954 moneykit-0.0.8/moneykit/model/validation_error.pyi
--rw-r--r--   0        0        0     6451 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/models/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-01 19:33:44.000000 moneykit-0.0.8/moneykit/paths/__init__.py
--rw-r--r--   0        0        0      306 2023-05-01 19:33:49.139360 moneykit-0.0.8/moneykit/paths/auth_introspect/__init__.py
--rw-r--r--   0        0        0    13677 2023-05-01 19:33:50.834090 moneykit-0.0.8/moneykit/paths/auth_introspect/get.py
--rw-r--r--   0        0        0    13392 2023-05-01 19:33:50.836572 moneykit-0.0.8/moneykit/paths/auth_introspect/get.pyi
--rw-r--r--   0        0        0      296 2023-05-01 19:33:49.170755 moneykit-0.0.8/moneykit/paths/auth_token/__init__.py
--rw-r--r--   0        0        0    17719 2023-05-01 19:33:50.818755 moneykit-0.0.8/moneykit/paths/auth_token/post.py
--rw-r--r--   0        0        0    17426 2023-05-01 19:33:50.814510 moneykit-0.0.8/moneykit/paths/auth_token/post.pyi
--rw-r--r--   0        0        0      300 2023-05-01 19:33:49.170937 moneykit-0.0.8/moneykit/paths/institutions/__init__.py
--rw-r--r--   0        0        0    18697 2023-05-01 19:33:50.839965 moneykit-0.0.8/moneykit/paths/institutions/get.py
--rw-r--r--   0        0        0    18300 2023-05-01 19:33:50.840807 moneykit-0.0.8/moneykit/paths/institutions/get.pyi
--rw-r--r--   0        0        0      330 2023-05-01 19:33:49.171691 moneykit-0.0.8/moneykit/paths/institutions_institution_id/__init__.py
--rw-r--r--   0        0        0    16873 2023-05-01 19:33:50.849043 moneykit-0.0.8/moneykit/paths/institutions_institution_id/get.py
--rw-r--r--   0        0        0    16522 2023-05-01 19:33:50.842156 moneykit-0.0.8/moneykit/paths/institutions_institution_id/get.pyi
--rw-r--r--   0        0        0      346 2023-05-01 19:33:49.176564 moneykit-0.0.8/moneykit/paths/institutions_institution_id_styling/__init__.py
--rw-r--r--   0        0        0    17015 2023-05-01 19:33:50.847056 moneykit-0.0.8/moneykit/paths/institutions_institution_id_styling/get.py
--rw-r--r--   0        0        0    16664 2023-05-01 19:33:50.848386 moneykit-0.0.8/moneykit/paths/institutions_institution_id_styling/get.pyi
--rw-r--r--   0        0        0      299 2023-05-01 19:33:49.248865 moneykit-0.0.8/moneykit/paths/link_session/__init__.py
--rw-r--r--   0        0        0    18397 2023-05-01 19:33:50.848919 moneykit-0.0.8/moneykit/paths/link_session/post.py
--rw-r--r--   0        0        0    18052 2023-05-01 19:33:50.846628 moneykit-0.0.8/moneykit/paths/link_session/post.pyi
--rw-r--r--   0        0        0      328 2023-05-01 19:33:49.302210 moneykit-0.0.8/moneykit/paths/link_session_exchange_token/__init__.py
--rw-r--r--   0        0        0    18303 2023-05-01 19:33:50.850692 moneykit-0.0.8/moneykit/paths/link_session_exchange_token/post.py
--rw-r--r--   0        0        0    17958 2023-05-01 19:33:50.847117 moneykit-0.0.8/moneykit/paths/link_session_exchange_token/post.pyi
--rw-r--r--   0        0        0      292 2023-05-01 19:33:49.318176 moneykit-0.0.8/moneykit/paths/links_id/__init__.py
--rw-r--r--   0        0        0    18419 2023-05-01 19:33:50.836319 moneykit-0.0.8/moneykit/paths/links_id/delete.py
--rw-r--r--   0        0        0    17972 2023-05-01 19:33:50.839754 moneykit-0.0.8/moneykit/paths/links_id/delete.pyi
--rw-r--r--   0        0        0    18631 2023-05-01 19:33:50.837516 moneykit-0.0.8/moneykit/paths/links_id/get.py
--rw-r--r--   0        0        0    18184 2023-05-01 19:33:50.839444 moneykit-0.0.8/moneykit/paths/links_id/get.pyi
--rw-r--r--   0        0        0    22888 2023-05-01 19:33:50.842507 moneykit-0.0.8/moneykit/paths/links_id/patch.py
--rw-r--r--   0        0        0    22413 2023-05-01 19:33:50.836939 moneykit-0.0.8/moneykit/paths/links_id/patch.pyi
--rw-r--r--   0        0        0      310 2023-05-01 19:33:49.413874 moneykit-0.0.8/moneykit/paths/links_id_accounts/__init__.py
--rw-r--r--   0        0        0    21397 2023-05-01 19:33:50.850244 moneykit-0.0.8/moneykit/paths/links_id_accounts/get.py
--rw-r--r--   0        0        0    20945 2023-05-01 19:33:50.844079 moneykit-0.0.8/moneykit/paths/links_id_accounts/get.pyi
--rw-r--r--   0        0        0      332 2023-05-01 19:33:49.460274 moneykit-0.0.8/moneykit/paths/links_id_accounts_account_id/__init__.py
--rw-r--r--   0        0        0    19061 2023-05-01 19:33:50.843960 moneykit-0.0.8/moneykit/paths/links_id_accounts_account_id/get.py
--rw-r--r--   0        0        0    18614 2023-05-01 19:33:50.844949 moneykit-0.0.8/moneykit/paths/links_id_accounts_account_id/get.pyi
--rw-r--r--   0        0        0      326 2023-05-01 19:33:49.513399 moneykit-0.0.8/moneykit/paths/links_id_accounts_numbers/__init__.py
--rw-r--r--   0        0        0    18809 2023-05-01 19:33:50.846366 moneykit-0.0.8/moneykit/paths/links_id_accounts_numbers/get.py
--rw-r--r--   0        0        0    18362 2023-05-01 19:33:50.846716 moneykit-0.0.8/moneykit/paths/links_id_accounts_numbers/get.pyi
--rw-r--r--   0        0        0      310 2023-05-01 19:33:49.525252 moneykit-0.0.8/moneykit/paths/links_id_identity/__init__.py
--rw-r--r--   0        0        0    21409 2023-05-01 19:33:50.838924 moneykit-0.0.8/moneykit/paths/links_id_identity/get.py
--rw-r--r--   0        0        0    20957 2023-05-01 19:33:50.841741 moneykit-0.0.8/moneykit/paths/links_id_identity/get.pyi
--rw-r--r--   0        0        0      310 2023-05-01 19:33:49.585695 moneykit-0.0.8/moneykit/paths/links_id_products/__init__.py
--rw-r--r--   0        0        0    22935 2023-05-01 19:33:50.830797 moneykit-0.0.8/moneykit/paths/links_id_products/post.py
--rw-r--r--   0        0        0    22460 2023-05-01 19:33:50.838270 moneykit-0.0.8/moneykit/paths/links_id_products/post.pyi
--rw-r--r--   0        0        0      318 2023-05-01 19:33:49.602343 moneykit-0.0.8/moneykit/paths/links_id_transactions/__init__.py
--rw-r--r--   0        0        0    23741 2023-05-01 19:33:50.847602 moneykit-0.0.8/moneykit/paths/links_id_transactions/get.py
--rw-r--r--   0        0        0    23171 2023-05-01 19:33:50.849731 moneykit-0.0.8/moneykit/paths/links_id_transactions/get.pyi
--rw-r--r--   0        0        0      328 2023-05-01 19:33:49.631645 moneykit-0.0.8/moneykit/paths/links_id_transactions_sync/__init__.py
--rw-r--r--   0        0        0    21818 2023-05-01 19:33:50.830629 moneykit-0.0.8/moneykit/paths/links_id_transactions_sync/get.py
--rw-r--r--   0        0        0    21293 2023-05-01 19:33:50.833261 moneykit-0.0.8/moneykit/paths/links_id_transactions_sync/get.pyi
--rw-r--r--   0        0        0      310 2023-05-01 19:33:49.654006 moneykit-0.0.8/moneykit/paths/users_id_accounts/__init__.py
--rw-r--r--   0        0        0    19316 2023-05-01 19:33:50.823253 moneykit-0.0.8/moneykit/paths/users_id_accounts/get.py
--rw-r--r--   0        0        0    18938 2023-05-01 19:33:50.826457 moneykit-0.0.8/moneykit/paths/users_id_accounts/get.pyi
--rw-r--r--   0        0        0      304 2023-05-01 19:33:49.686637 moneykit-0.0.8/moneykit/paths/users_id_links/__init__.py
--rw-r--r--   0        0        0    15565 2023-05-01 19:33:50.810274 moneykit-0.0.8/moneykit/paths/users_id_links/get.py
--rw-r--r--   0        0        0    15278 2023-05-01 19:33:50.812216 moneykit-0.0.8/moneykit/paths/users_id_links/get.pyi
--rw-r--r--   0        0        0      318 2023-05-01 19:33:49.801614 moneykit-0.0.8/moneykit/paths/users_id_transactions/__init__.py
--rw-r--r--   0        0        0    23515 2023-05-01 19:33:50.848352 moneykit-0.0.8/moneykit/paths/users_id_transactions/get.py
--rw-r--r--   0        0        0    23015 2023-05-01 19:33:50.849824 moneykit-0.0.8/moneykit/paths/users_id_transactions/get.pyi
--rw-r--r--   0        0        0      316 2023-05-01 19:33:49.823303 moneykit-0.0.8/moneykit/paths/well_known_jwks_json/__init__.py
--rw-r--r--   0        0        0    13631 2023-05-01 19:33:50.832544 moneykit-0.0.8/moneykit/paths/well_known_jwks_json/get.py
--rw-r--r--   0        0        0    13346 2023-05-01 19:33:50.834960 moneykit-0.0.8/moneykit/paths/well_known_jwks_json/get.pyi
--rw-r--r--   0        0        0      963 2023-05-01 19:34:30.643036 moneykit-0.0.8/moneykit/plaid_compatible/__init__.py
--rw-r--r--   0        0        0      227 2023-05-01 19:34:30.675078 moneykit-0.0.8/moneykit/plaid_compatible/api/__init__.py
--rw-r--r--   0        0        0    50030 2023-05-01 19:34:30.675797 moneykit-0.0.8/moneykit/plaid_compatible/api/plaid_api.py
--rw-r--r--   0        0        0    36839 2023-05-01 19:34:30.676696 moneykit-0.0.8/moneykit/plaid_compatible/api_client.py
--rw-r--r--   0        0        0      470 2023-05-01 19:34:30.642493 moneykit-0.0.8/moneykit/plaid_compatible/apis/__init__.py
--rw-r--r--   0        0        0    17735 2023-05-01 19:34:30.642285 moneykit-0.0.8/moneykit/plaid_compatible/configuration.py
--rw-r--r--   0        0        0     5093 2023-05-01 19:34:30.676065 moneykit-0.0.8/moneykit/plaid_compatible/exceptions.py
--rw-r--r--   0        0        0      348 2023-05-01 19:34:30.655029 moneykit-0.0.8/moneykit/plaid_compatible/model/__init__.py
--rw-r--r--   0        0        0    10890 2023-05-01 19:34:30.661531 moneykit-0.0.8/moneykit/plaid_compatible/model/account_balance.py
--rw-r--r--   0        0        0    10741 2023-05-01 19:34:30.658408 moneykit-0.0.8/moneykit/plaid_compatible/model/account_base.py
--rw-r--r--   0        0        0    11657 2023-05-01 19:34:30.652402 moneykit-0.0.8/moneykit/plaid_compatible/model/account_identity.py
--rw-r--r--   0        0        0    11414 2023-05-01 19:34:30.657685 moneykit-0.0.8/moneykit/plaid_compatible/model/account_subtype.py
--rw-r--r--   0        0        0     7191 2023-05-01 19:34:30.671877 moneykit-0.0.8/moneykit/plaid_compatible/model/account_type.py
--rw-r--r--   0        0        0     7674 2023-05-01 19:34:30.658705 moneykit-0.0.8/moneykit/plaid_compatible/model/accounts_get_request.py
--rw-r--r--   0        0        0     6636 2023-05-01 19:34:30.669392 moneykit-0.0.8/moneykit/plaid_compatible/model/accounts_get_request_options.py
--rw-r--r--   0        0        0     7447 2023-05-01 19:34:30.665506 moneykit-0.0.8/moneykit/plaid_compatible/model/accounts_get_response.py
--rw-r--r--   0        0        0     6925 2023-05-01 19:34:30.645177 moneykit-0.0.8/moneykit/plaid_compatible/model/address.py
--rw-r--r--   0        0        0     7501 2023-05-01 19:34:30.659913 moneykit-0.0.8/moneykit/plaid_compatible/model/address_data.py
--rw-r--r--   0        0        0     7793 2023-05-01 19:34:30.669692 moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_numbers.py
--rw-r--r--   0        0        0     7642 2023-05-01 19:34:30.668540 moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_request.py
--rw-r--r--   0        0        0     6715 2023-05-01 19:34:30.658037 moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_request_options.py
--rw-r--r--   0        0        0     7635 2023-05-01 19:34:30.673828 moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_response.py
--rw-r--r--   0        0        0     7265 2023-05-01 19:34:30.647357 moneykit-0.0.8/moneykit/plaid_compatible/model/counterparty_type.py
--rw-r--r--   0        0        0     6955 2023-05-01 19:34:30.669977 moneykit-0.0.8/moneykit/plaid_compatible/model/country_code.py
--rw-r--r--   0        0        0     7029 2023-05-01 19:34:30.647714 moneykit-0.0.8/moneykit/plaid_compatible/model/credit_account_subtype.py
--rw-r--r--   0        0        0     7070 2023-05-01 19:34:30.644576 moneykit-0.0.8/moneykit/plaid_compatible/model/credit_filter.py
--rw-r--r--   0        0        0     7417 2023-05-01 19:34:30.667383 moneykit-0.0.8/moneykit/plaid_compatible/model/depository_account_subtype.py
--rw-r--r--   0        0        0     7102 2023-05-01 19:34:30.668804 moneykit-0.0.8/moneykit/plaid_compatible/model/depository_filter.py
--rw-r--r--   0        0        0     6966 2023-05-01 19:34:30.663270 moneykit-0.0.8/moneykit/plaid_compatible/model/email.py
--rw-r--r--   0        0        0     6965 2023-05-01 19:34:30.674103 moneykit-0.0.8/moneykit/plaid_compatible/model/employment_source_type.py
--rw-r--r--   0        0        0     6724 2023-05-01 19:34:30.659644 moneykit-0.0.8/moneykit/plaid_compatible/model/http_validation_error.py
--rw-r--r--   0        0        0     9101 2023-05-01 19:34:30.663657 moneykit-0.0.8/moneykit/plaid_compatible/model/id_number_type.py
--rw-r--r--   0        0        0     7674 2023-05-01 19:34:30.665991 moneykit-0.0.8/moneykit/plaid_compatible/model/identity_get_request.py
--rw-r--r--   0        0        0     6723 2023-05-01 19:34:30.667098 moneykit-0.0.8/moneykit/plaid_compatible/model/identity_get_request_options.py
--rw-r--r--   0        0        0     7362 2023-05-01 19:34:30.664334 moneykit-0.0.8/moneykit/plaid_compatible/model/identity_get_response.py
--rw-r--r--   0        0        0     7111 2023-05-01 19:34:30.646772 moneykit-0.0.8/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py
--rw-r--r--   0        0        0     6981 2023-05-01 19:34:30.649429 moneykit-0.0.8/moneykit/plaid_compatible/model/income_verification_source_type.py
--rw-r--r--   0        0        0     9913 2023-05-01 19:34:30.672188 moneykit-0.0.8/moneykit/plaid_compatible/model/investment_account_subtype.py
--rw-r--r--   0        0        0     7102 2023-05-01 19:34:30.660868 moneykit-0.0.8/moneykit/plaid_compatible/model/investment_filter.py
--rw-r--r--   0        0        0    10420 2023-05-01 19:34:30.673553 moneykit-0.0.8/moneykit/plaid_compatible/model/item.py
--rw-r--r--   0        0        0     7717 2023-05-01 19:34:30.658996 moneykit-0.0.8/moneykit/plaid_compatible/model/item_error_webhook.py
--rw-r--r--   0        0        0     7265 2023-05-01 19:34:30.662927 moneykit-0.0.8/moneykit/plaid_compatible/model/item_get_request.py
--rw-r--r--   0        0        0     7287 2023-05-01 19:34:30.646422 moneykit-0.0.8/moneykit/plaid_compatible/model/item_get_response.py
--rw-r--r--   0        0        0     7331 2023-05-01 19:34:30.664009 moneykit-0.0.8/moneykit/plaid_compatible/model/item_public_token_exchange_request.py
--rw-r--r--   0        0        0     7235 2023-05-01 19:34:30.674459 moneykit-0.0.8/moneykit/plaid_compatible/model/item_public_token_exchange_response.py
--rw-r--r--   0        0        0     7271 2023-05-01 19:34:30.648363 moneykit-0.0.8/moneykit/plaid_compatible/model/item_remove_request.py
--rw-r--r--   0        0        0     6715 2023-05-01 19:34:30.670849 moneykit-0.0.8/moneykit/plaid_compatible/model/item_remove_response.py
--rw-r--r--   0        0        0     7362 2023-05-01 19:34:30.669120 moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_investments.py
--rw-r--r--   0        0        0     6852 2023-05-01 19:34:30.660581 moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_last_webhook.py
--rw-r--r--   0        0        0     7489 2023-05-01 19:34:30.667656 moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_nullable.py
--rw-r--r--   0        0        0     7366 2023-05-01 19:34:30.651005 moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_transactions.py
--rw-r--r--   0        0        0     7595 2023-05-01 19:34:30.672457 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_account_filters.py
--rw-r--r--   0        0        0     6644 2023-05-01 19:34:30.657276 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_institution_data.py
--rw-r--r--   0        0        0    21548 2023-05-01 19:34:30.671332 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request.py
--rw-r--r--   0        0        0     8258 2023-05-01 19:34:30.646141 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_auth.py
--rw-r--r--   0        0        0     6733 2023-05-01 19:34:30.652007 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py
--rw-r--r--   0        0        0     7534 2023-05-01 19:34:30.652690 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_employment.py
--rw-r--r--   0        0        0     6722 2023-05-01 19:34:30.654479 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py
--rw-r--r--   0        0        0     7661 2023-05-01 19:34:30.662192 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py
--rw-r--r--   0        0        0    10586 2023-05-01 19:34:30.670297 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py
--rw-r--r--   0        0        0     7020 2023-05-01 19:34:30.643645 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py
--rw-r--r--   0        0        0     7697 2023-05-01 19:34:30.653270 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py
--rw-r--r--   0        0        0     6937 2023-05-01 19:34:30.644238 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py
--rw-r--r--   0        0        0     6940 2023-05-01 19:34:30.661155 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_transfer.py
--rw-r--r--   0        0        0     6779 2023-05-01 19:34:30.650714 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_update.py
--rw-r--r--   0        0        0    11399 2023-05-01 19:34:30.644912 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_user.py
--rw-r--r--   0        0        0     6963 2023-05-01 19:34:30.672727 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_user_name.py
--rw-r--r--   0        0        0     8414 2023-05-01 19:34:30.650422 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py
--rw-r--r--   0        0        0     7615 2023-05-01 19:34:30.653589 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_response.py
--rw-r--r--   0        0        0     6616 2023-05-01 19:34:30.666765 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_eu_config.py
--rw-r--r--   0        0        0     6769 2023-05-01 19:34:30.673258 moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_investments.py
--rw-r--r--   0        0        0     7573 2023-05-01 19:34:30.652982 moneykit-0.0.8/moneykit/plaid_compatible/model/loan_account_subtype.py
--rw-r--r--   0        0        0     7054 2023-05-01 19:34:30.656221 moneykit-0.0.8/moneykit/plaid_compatible/model/loan_filter.py
--rw-r--r--   0        0        0     7487 2023-05-01 19:34:30.660284 moneykit-0.0.8/moneykit/plaid_compatible/model/location.py
--rw-r--r--   0        0        0     7716 2023-05-01 19:34:30.655610 moneykit-0.0.8/moneykit/plaid_compatible/model/money_link_features.py
--rw-r--r--   0        0        0     8621 2023-05-01 19:34:30.670578 moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_ach.py
--rw-r--r--   0        0        0     7019 2023-05-01 19:34:30.649725 moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_bacs.py
--rw-r--r--   0        0        0     7225 2023-05-01 19:34:30.654827 moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_eft.py
--rw-r--r--   0        0        0     7007 2023-05-01 19:34:30.659350 moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_international.py
--rw-r--r--   0        0        0     8304 2023-05-01 19:34:30.656582 moneykit-0.0.8/moneykit/plaid_compatible/model/owner.py
--rw-r--r--   0        0        0     7593 2023-05-01 19:34:30.643939 moneykit-0.0.8/moneykit/plaid_compatible/model/payment_meta.py
--rw-r--r--   0        0        0     6930 2023-05-01 19:34:30.648001 moneykit-0.0.8/moneykit/plaid_compatible/model/personal_finance_category.py
--rw-r--r--   0        0        0     6934 2023-05-01 19:34:30.653922 moneykit-0.0.8/moneykit/plaid_compatible/model/phone_number.py
--rw-r--r--   0        0        0     9494 2023-05-01 19:34:30.674826 moneykit-0.0.8/moneykit/plaid_compatible/model/plaid_error.py
--rw-r--r--   0        0        0     8113 2023-05-01 19:34:30.645496 moneykit-0.0.8/moneykit/plaid_compatible/model/plaid_error_type.py
--rw-r--r--   0        0        0     7129 2023-05-01 19:34:30.655292 moneykit-0.0.8/moneykit/plaid_compatible/model/products.py
--rw-r--r--   0        0        0     6610 2023-05-01 19:34:30.645840 moneykit-0.0.8/moneykit/plaid_compatible/model/removed_transaction.py
--rw-r--r--   0        0        0    16756 2023-05-01 19:34:30.651442 moneykit-0.0.8/moneykit/plaid_compatible/model/transaction.py
--rw-r--r--   0        0        0     7632 2023-05-01 19:34:30.655935 moneykit-0.0.8/moneykit/plaid_compatible/model/transaction_code.py
--rw-r--r--   0        0        0     7510 2023-05-01 19:34:30.649123 moneykit-0.0.8/moneykit/plaid_compatible/model/transaction_counterparty.py
--rw-r--r--   0        0        0     8236 2023-05-01 19:34:30.664723 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_get_request.py
--rw-r--r--   0        0        0     9639 2023-05-01 19:34:30.661865 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_get_request_options.py
--rw-r--r--   0        0        0     8530 2023-05-01 19:34:30.667955 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_get_response.py
--rw-r--r--   0        0        0     7289 2023-05-01 19:34:30.672996 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_refresh_request.py
--rw-r--r--   0        0        0     6733 2023-05-01 19:34:30.647071 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_refresh_response.py
--rw-r--r--   0        0        0     8397 2023-05-01 19:34:30.665082 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_sync_request.py
--rw-r--r--   0        0        0     8427 2023-05-01 19:34:30.668271 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_sync_request_options.py
--rw-r--r--   0        0        0     8900 2023-05-01 19:34:30.656974 moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_sync_response.py
--rw-r--r--   0        0        0     7916 2023-05-01 19:34:30.662555 moneykit-0.0.8/moneykit/plaid_compatible/model/user_address.py
--rw-r--r--   0        0        0     6950 2023-05-01 19:34:30.666400 moneykit-0.0.8/moneykit/plaid_compatible/model/user_id_number.py
--rw-r--r--   0        0        0     7625 2023-05-01 19:34:30.671604 moneykit-0.0.8/moneykit/plaid_compatible/model/user_stated_income_source_category.py
--rw-r--r--   0        0        0     7187 2023-05-01 19:34:30.650075 moneykit-0.0.8/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py
--rw-r--r--   0        0        0     7027 2023-05-01 19:34:30.654201 moneykit-0.0.8/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py
--rw-r--r--   0        0        0     6793 2023-05-01 19:34:30.648714 moneykit-0.0.8/moneykit/plaid_compatible/model/validation_error.py
--rw-r--r--   0        0        0     7069 2023-05-01 19:34:30.651731 moneykit-0.0.8/moneykit/plaid_compatible/model/webhook_environment_values.py
--rw-r--r--   0        0        0    74795 2023-05-01 19:34:30.641802 moneykit-0.0.8/moneykit/plaid_compatible/model_utils.py
--rw-r--r--   0        0        0     8892 2023-05-01 19:34:30.643326 moneykit-0.0.8/moneykit/plaid_compatible/models/__init__.py
--rw-r--r--   0        0        0    12537 2023-05-01 19:34:30.642813 moneykit-0.0.8/moneykit/plaid_compatible/rest.py
--rw-r--r--   0        0        0     9365 2023-05-01 19:33:50.839439 moneykit-0.0.8/moneykit/rest.py
--rw-r--r--   0        0        0    99126 2023-05-01 19:33:50.853811 moneykit-0.0.8/moneykit/schemas.py
--rw-r--r--   0        0        0      941 2023-05-01 19:35:25.117577 moneykit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    21125 1970-01-01 00:00:00.000000 moneykit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    20273 2023-05-01 19:33:44.000000 moneykit-0.0.9/README.md
+-rw-r--r--   0        0        0      739 2023-05-01 19:38:06.906311 moneykit-0.0.9/moneykit/__init__.py
+-rw-r--r--   0        0        0    56712 2023-05-01 19:33:50.823969 moneykit-0.0.9/moneykit/api_client.py
+-rw-r--r--   0        0        0      215 2023-05-01 19:33:48.062027 moneykit-0.0.9/moneykit/apis/__init__.py
+-rw-r--r--   0        0        0     3789 2023-05-01 19:33:50.820886 moneykit-0.0.9/moneykit/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/apis/paths/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-01 19:33:40.000000 moneykit-0.0.9/moneykit/apis/paths/auth_introspect.py
+-rw-r--r--   0        0        0      101 2023-05-01 19:33:40.000000 moneykit-0.0.9/moneykit/apis/paths/auth_token.py
+-rw-r--r--   0        0        0      103 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/institutions.py
+-rw-r--r--   0        0        0      131 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/institutions_institution_id.py
+-rw-r--r--   0        0        0      146 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/institutions_institution_id_styling.py
+-rw-r--r--   0        0        0      105 2023-05-01 19:33:42.000000 moneykit-0.0.9/moneykit/apis/paths/link_session.py
+-rw-r--r--   0        0        0      133 2023-05-01 19:33:42.000000 moneykit-0.0.9/moneykit/apis/paths/link_session_exchange_token.py
+-rw-r--r--   0        0        0      239 2023-05-01 19:33:50.823217 moneykit-0.0.9/moneykit/apis/paths/links_id.py
+-rw-r--r--   0        0        0      111 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_accounts.py
+-rw-r--r--   0        0        0      131 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_accounts_account_id.py
+-rw-r--r--   0        0        0      126 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_accounts_numbers.py
+-rw-r--r--   0        0        0      111 2023-05-01 19:33:41.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_identity.py
+-rw-r--r--   0        0        0      114 2023-05-01 19:33:42.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_products.py
+-rw-r--r--   0        0        0      119 2023-05-01 19:33:43.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_transactions.py
+-rw-r--r--   0        0        0      128 2023-05-01 19:33:43.000000 moneykit-0.0.9/moneykit/apis/paths/links_id_transactions_sync.py
+-rw-r--r--   0        0        0      111 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/apis/paths/users_id_accounts.py
+-rw-r--r--   0        0        0      105 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/apis/paths/users_id_links.py
+-rw-r--r--   0        0        0      119 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/apis/paths/users_id_transactions.py
+-rw-r--r--   0        0        0      116 2023-05-01 19:33:40.000000 moneykit-0.0.9/moneykit/apis/paths/well_known_jwks_json.py
+-rw-r--r--   0        0        0     1650 2023-05-01 19:33:50.821311 moneykit-0.0.9/moneykit/apis/tag_to_api.py
+-rw-r--r--   0        0        0      575 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/apis/tags/__init__.py
+-rw-r--r--   0        0        0      718 2023-05-01 19:33:50.817469 moneykit-0.0.9/moneykit/apis/tags/access_token_api.py
+-rw-r--r--   0        0        0      552 2023-05-01 19:33:48.071183 moneykit-0.0.9/moneykit/apis/tags/account_numbers_api.py
+-rw-r--r--   0        0        0      797 2023-05-01 19:33:50.817732 moneykit-0.0.9/moneykit/apis/tags/accounts_api.py
+-rw-r--r--   0        0        0      530 2023-05-01 19:33:48.072784 moneykit-0.0.9/moneykit/apis/tags/identity_api.py
+-rw-r--r--   0        0        0      743 2023-05-01 19:33:50.817991 moneykit-0.0.9/moneykit/apis/tags/institutions_api.py
+-rw-r--r--   0        0        0      630 2023-05-01 19:33:48.077157 moneykit-0.0.9/moneykit/apis/tags/link_session_api.py
+-rw-r--r--   0        0        0      722 2023-05-01 19:33:50.819676 moneykit-0.0.9/moneykit/apis/tags/links_api.py
+-rw-r--r--   0        0        0      535 2023-05-01 19:33:48.076709 moneykit-0.0.9/moneykit/apis/tags/products_api.py
+-rw-r--r--   0        0        0      743 2023-05-01 19:33:48.077894 moneykit-0.0.9/moneykit/apis/tags/transactions_api.py
+-rw-r--r--   0        0        0      706 2023-05-01 19:33:48.079724 moneykit-0.0.9/moneykit/apis/tags/users_api.py
+-rw-r--r--   0        0        0    18643 2023-05-01 19:33:50.817208 moneykit-0.0.9/moneykit/configuration.py
+-rw-r--r--   0        0        0     4490 2023-05-01 19:33:48.100550 moneykit-0.0.9/moneykit/exceptions.py
+-rw-r--r--   0        0        0      342 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/model/__init__.py
+-rw-r--r--   0        0        0    11454 2023-05-01 19:33:50.840309 moneykit-0.0.9/moneykit/model/account.py
+-rw-r--r--   0        0        0    11337 2023-05-01 19:33:50.826352 moneykit-0.0.9/moneykit/model/account.pyi
+-rw-r--r--   0        0        0     9362 2023-05-01 19:33:50.814276 moneykit-0.0.9/moneykit/model/account_balances.py
+-rw-r--r--   0        0        0     9265 2023-05-01 19:33:50.828569 moneykit-0.0.9/moneykit/model/account_balances.pyi
+-rw-r--r--   0        0        0     5097 2023-05-01 19:33:50.814015 moneykit-0.0.9/moneykit/model/account_group.py
+-rw-r--r--   0        0        0     5034 2023-05-01 19:33:50.815503 moneykit-0.0.9/moneykit/model/account_group.pyi
+-rw-r--r--   0        0        0    12821 2023-05-01 19:33:50.822738 moneykit-0.0.9/moneykit/model/account_identity.py
+-rw-r--r--   0        0        0    12684 2023-05-01 19:33:50.815975 moneykit-0.0.9/moneykit/model/account_identity.pyi
+-rw-r--r--   0        0        0     7878 2023-05-01 19:33:50.841243 moneykit-0.0.9/moneykit/model/account_numbers.py
+-rw-r--r--   0        0        0     7774 2023-05-01 19:33:50.827430 moneykit-0.0.9/moneykit/model/account_numbers.pyi
+-rw-r--r--   0        0        0     5932 2023-05-01 19:33:50.843882 moneykit-0.0.9/moneykit/model/account_numbers_link_product.py
+-rw-r--r--   0        0        0     5852 2023-05-01 19:33:50.827326 moneykit-0.0.9/moneykit/model/account_numbers_link_product.pyi
+-rw-r--r--   0        0        0     3467 2023-05-01 19:33:50.830935 moneykit-0.0.9/moneykit/model/account_numbers_product_settings.py
+-rw-r--r--   0        0        0     3409 2023-05-01 19:33:50.844662 moneykit-0.0.9/moneykit/model/account_numbers_product_settings.pyi
+-rw-r--r--   0        0        0     2418 2023-05-01 19:33:50.827189 moneykit-0.0.9/moneykit/model/account_type.py
+-rw-r--r--   0        0        0     1831 2023-05-01 19:33:50.826268 moneykit-0.0.9/moneykit/model/account_type.pyi
+-rw-r--r--   0        0        0    14837 2023-05-01 19:33:50.818113 moneykit-0.0.9/moneykit/model/account_with_account_numbers.py
+-rw-r--r--   0        0        0    14701 2023-05-01 19:33:50.810093 moneykit-0.0.9/moneykit/model/account_with_account_numbers.pyi
+-rw-r--r--   0        0        0     5109 2023-05-01 19:33:50.814935 moneykit-0.0.9/moneykit/model/accounts_link_product.py
+-rw-r--r--   0        0        0     5048 2023-05-01 19:33:50.836442 moneykit-0.0.9/moneykit/model/accounts_link_product.pyi
+-rw-r--r--   0        0        0     5023 2023-05-01 19:33:50.828644 moneykit-0.0.9/moneykit/model/ach_number.py
+-rw-r--r--   0        0        0     4974 2023-05-01 19:33:50.839075 moneykit-0.0.9/moneykit/model/ach_number.pyi
+-rw-r--r--   0        0        0     8379 2023-05-01 19:33:50.843063 moneykit-0.0.9/moneykit/model/address.py
+-rw-r--r--   0        0        0     8248 2023-05-01 19:33:50.841927 moneykit-0.0.9/moneykit/model/address.pyi
+-rw-r--r--   0        0        0     5259 2023-05-01 19:33:50.830284 moneykit-0.0.9/moneykit/model/api_error_auth_expired_access_token_response.py
+-rw-r--r--   0        0        0     4981 2023-05-01 19:33:50.833461 moneykit-0.0.9/moneykit/model/api_error_auth_expired_access_token_response.pyi
+-rw-r--r--   0        0        0     5291 2023-05-01 19:33:50.819044 moneykit-0.0.9/moneykit/model/api_error_auth_unauthorized_response.py
+-rw-r--r--   0        0        0     5030 2023-05-01 19:33:50.821244 moneykit-0.0.9/moneykit/model/api_error_auth_unauthorized_response.pyi
+-rw-r--r--   0        0        0     5225 2023-05-01 19:33:50.837516 moneykit-0.0.9/moneykit/model/api_error_rate_limit_exceeded_response.py
+-rw-r--r--   0        0        0     4959 2023-05-01 19:33:50.832183 moneykit-0.0.9/moneykit/model/api_error_rate_limit_exceeded_response.pyi
+-rw-r--r--   0        0        0     3626 2023-05-01 19:33:50.811445 moneykit-0.0.9/moneykit/model/bacs_number.py
+-rw-r--r--   0        0        0     3582 2023-05-01 19:33:50.810830 moneykit-0.0.9/moneykit/model/bacs_number.pyi
+-rw-r--r--   0        0        0     5566 2023-05-01 19:33:50.844389 moneykit-0.0.9/moneykit/model/basic_account_details.py
+-rw-r--r--   0        0        0     5484 2023-05-01 19:33:50.832288 moneykit-0.0.9/moneykit/model/basic_account_details.pyi
+-rw-r--r--   0        0        0     1162 2023-05-01 19:33:50.831188 moneykit-0.0.9/moneykit/model/country.py
+-rw-r--r--   0        0        0     1025 2023-05-01 19:33:50.844154 moneykit-0.0.9/moneykit/model/country.pyi
+-rw-r--r--   0        0        0    17582 2023-05-01 19:33:50.834397 moneykit-0.0.9/moneykit/model/create_link_session_request.py
+-rw-r--r--   0        0        0    17291 2023-05-01 19:33:50.813291 moneykit-0.0.9/moneykit/model/create_link_session_request.pyi
+-rw-r--r--   0        0        0     2943 2023-05-01 19:33:50.836746 moneykit-0.0.9/moneykit/model/create_link_session_response.py
+-rw-r--r--   0        0        0     2903 2023-05-01 19:33:50.816198 moneykit-0.0.9/moneykit/model/create_link_session_response.pyi
+-rw-r--r--   0        0        0    18827 2023-05-01 19:33:50.813524 moneykit-0.0.9/moneykit/model/currency.py
+-rw-r--r--   0        0        0    13878 2023-05-01 19:33:50.849503 moneykit-0.0.9/moneykit/model/currency.pyi
+-rw-r--r--   0        0        0     3163 2023-05-01 19:33:50.830793 moneykit-0.0.9/moneykit/model/cursor_pagination.py
+-rw-r--r--   0        0        0     3122 2023-05-01 19:33:50.845245 moneykit-0.0.9/moneykit/model/cursor_pagination.pyi
+-rw-r--r--   0        0        0     3473 2023-05-01 19:33:50.828254 moneykit-0.0.9/moneykit/model/customer_app.py
+-rw-r--r--   0        0        0     3415 2023-05-01 19:33:50.810491 moneykit-0.0.9/moneykit/model/customer_app.pyi
+-rw-r--r--   0        0        0     4489 2023-05-01 19:33:50.830195 moneykit-0.0.9/moneykit/model/eft_number.py
+-rw-r--r--   0        0        0     4427 2023-05-01 19:33:50.813050 moneykit-0.0.9/moneykit/model/eft_number.pyi
+-rw-r--r--   0        0        0     3449 2023-05-01 19:33:50.814413 moneykit-0.0.9/moneykit/model/email.py
+-rw-r--r--   0        0        0     3391 2023-05-01 19:33:50.809633 moneykit-0.0.9/moneykit/model/email.pyi
+-rw-r--r--   0        0        0     2933 2023-05-01 19:33:50.844721 moneykit-0.0.9/moneykit/model/exchange_token_request.py
+-rw-r--r--   0        0        0     2893 2023-05-01 19:33:50.838744 moneykit-0.0.9/moneykit/model/exchange_token_request.pyi
+-rw-r--r--   0        0        0     6194 2023-05-01 19:33:50.817623 moneykit-0.0.9/moneykit/model/exchange_token_response.py
+-rw-r--r--   0        0        0     6133 2023-05-01 19:33:50.818959 moneykit-0.0.9/moneykit/model/exchange_token_response.pyi
+-rw-r--r--   0        0        0     4350 2023-05-01 19:33:50.832813 moneykit-0.0.9/moneykit/model/generate_access_token_response.py
+-rw-r--r--   0        0        0     4274 2023-05-01 19:33:50.830961 moneykit-0.0.9/moneykit/model/generate_access_token_response.pyi
+-rw-r--r--   0        0        0     4468 2023-05-01 19:33:50.831778 moneykit-0.0.9/moneykit/model/get_account_numbers_response.py
+-rw-r--r--   0        0        0     4405 2023-05-01 19:33:50.836705 moneykit-0.0.9/moneykit/model/get_account_numbers_response.pyi
+-rw-r--r--   0        0        0     6175 2023-05-01 19:33:50.837383 moneykit-0.0.9/moneykit/model/get_account_response.py
+-rw-r--r--   0        0        0     6114 2023-05-01 19:33:50.815376 moneykit-0.0.9/moneykit/model/get_account_response.pyi
+-rw-r--r--   0        0        0     6991 2023-05-01 19:33:50.834694 moneykit-0.0.9/moneykit/model/get_accounts_response.py
+-rw-r--r--   0        0        0     6928 2023-05-01 19:33:50.828630 moneykit-0.0.9/moneykit/model/get_accounts_response.pyi
+-rw-r--r--   0        0        0     7164 2023-05-01 19:33:50.827857 moneykit-0.0.9/moneykit/model/get_institutions_response.py
+-rw-r--r--   0        0        0     7101 2023-05-01 19:33:50.815268 moneykit-0.0.9/moneykit/model/get_institutions_response.pyi
+-rw-r--r--   0        0        0    10245 2023-05-01 19:33:50.825697 moneykit-0.0.9/moneykit/model/get_transactions_response.py
+-rw-r--r--   0        0        0    10108 2023-05-01 19:33:50.820451 moneykit-0.0.9/moneykit/model/get_transactions_response.pyi
+-rw-r--r--   0        0        0     3894 2023-05-01 19:33:50.833062 moneykit-0.0.9/moneykit/model/get_user_accounts_response.py
+-rw-r--r--   0        0        0     3849 2023-05-01 19:33:50.811936 moneykit-0.0.9/moneykit/model/get_user_accounts_response.pyi
+-rw-r--r--   0        0        0     3874 2023-05-01 19:33:50.823650 moneykit-0.0.9/moneykit/model/get_user_links_response.py
+-rw-r--r--   0        0        0     3829 2023-05-01 19:33:50.827692 moneykit-0.0.9/moneykit/model/get_user_links_response.pyi
+-rw-r--r--   0        0        0     7425 2023-05-01 19:33:50.815563 moneykit-0.0.9/moneykit/model/get_user_transactions_response.py
+-rw-r--r--   0        0        0     7306 2023-05-01 19:33:50.829878 moneykit-0.0.9/moneykit/model/get_user_transactions_response.pyi
+-rw-r--r--   0        0        0     6893 2023-05-01 19:33:50.832043 moneykit-0.0.9/moneykit/model/http_validation_error.py
+-rw-r--r--   0        0        0     6594 2023-05-01 19:33:50.829800 moneykit-0.0.9/moneykit/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     5871 2023-05-01 19:33:50.816998 moneykit-0.0.9/moneykit/model/identity_link_product.py
+-rw-r--r--   0        0        0     5791 2023-05-01 19:33:50.824241 moneykit-0.0.9/moneykit/model/identity_link_product.pyi
+-rw-r--r--   0        0        0     3455 2023-05-01 19:33:50.830162 moneykit-0.0.9/moneykit/model/identity_product_settings.py
+-rw-r--r--   0        0        0     3397 2023-05-01 19:33:50.824089 moneykit-0.0.9/moneykit/model/identity_product_settings.pyi
+-rw-r--r--   0        0        0     4332 2023-05-01 19:33:50.820095 moneykit-0.0.9/moneykit/model/identity_response.py
+-rw-r--r--   0        0        0     4269 2023-05-01 19:33:50.836187 moneykit-0.0.9/moneykit/model/identity_response.pyi
+-rw-r--r--   0        0        0    10361 2023-05-01 19:33:50.817215 moneykit-0.0.9/moneykit/model/institution.py
+-rw-r--r--   0        0        0    10223 2023-05-01 19:33:50.823129 moneykit-0.0.9/moneykit/model/institution.pyi
+-rw-r--r--   0        0        0     5215 2023-05-01 19:33:50.835146 moneykit-0.0.9/moneykit/model/institution_error_not_found_response.py
+-rw-r--r--   0        0        0     4953 2023-05-01 19:33:50.810752 moneykit-0.0.9/moneykit/model/institution_error_not_found_response.pyi
+-rw-r--r--   0        0        0     9656 2023-05-01 19:33:50.826142 moneykit-0.0.9/moneykit/model/institution_styling_response.py
+-rw-r--r--   0        0        0     9489 2023-05-01 19:33:50.825561 moneykit-0.0.9/moneykit/model/institution_styling_response.pyi
+-rw-r--r--   0        0        0     3388 2023-05-01 19:33:50.811992 moneykit-0.0.9/moneykit/model/international_number.py
+-rw-r--r--   0        0        0     3330 2023-05-01 19:33:50.838122 moneykit-0.0.9/moneykit/model/international_number.pyi
+-rw-r--r--   0        0        0     8829 2023-05-01 19:33:50.814631 moneykit-0.0.9/moneykit/model/introspect_client_response.py
+-rw-r--r--   0        0        0     8713 2023-05-01 19:33:50.810368 moneykit-0.0.9/moneykit/model/introspect_client_response.pyi
+-rw-r--r--   0        0        0     3841 2023-05-01 19:33:50.816429 moneykit-0.0.9/moneykit/model/jwk_set.py
+-rw-r--r--   0        0        0     3798 2023-05-01 19:33:50.819500 moneykit-0.0.9/moneykit/model/jwk_set.pyi
+-rw-r--r--   0        0        0    16329 2023-05-01 19:33:50.829373 moneykit-0.0.9/moneykit/model/link_common.py
+-rw-r--r--   0        0        0    16184 2023-05-01 19:33:50.818773 moneykit-0.0.9/moneykit/model/link_common.pyi
+-rw-r--r--   0        0        0     1836 2023-05-01 19:33:50.826051 moneykit-0.0.9/moneykit/model/link_error.py
+-rw-r--r--   0        0        0     1451 2023-05-01 19:33:50.840104 moneykit-0.0.9/moneykit/model/link_error.pyi
+-rw-r--r--   0        0        0     5991 2023-05-01 19:33:50.835436 moneykit-0.0.9/moneykit/model/link_error_bad_state_response.py
+-rw-r--r--   0        0        0     5754 2023-05-01 19:33:50.812932 moneykit-0.0.9/moneykit/model/link_error_bad_state_response.pyi
+-rw-r--r--   0        0        0     5191 2023-05-01 19:33:50.823506 moneykit-0.0.9/moneykit/model/link_error_deleted_response.py
+-rw-r--r--   0        0        0     4947 2023-05-01 19:33:50.809742 moneykit-0.0.9/moneykit/model/link_error_deleted_response.pyi
+-rw-r--r--   0        0        0     5291 2023-05-01 19:33:50.825775 moneykit-0.0.9/moneykit/model/link_error_forbidden_action_response.py
+-rw-r--r--   0        0        0     5030 2023-05-01 19:33:50.811758 moneykit-0.0.9/moneykit/model/link_error_forbidden_action_response.pyi
+-rw-r--r--   0        0        0     5173 2023-05-01 19:33:50.809884 moneykit-0.0.9/moneykit/model/link_error_not_found_response.py
+-rw-r--r--   0        0        0     4925 2023-05-01 19:33:50.821853 moneykit-0.0.9/moneykit/model/link_error_not_found_response.pyi
+-rw-r--r--   0        0        0     5233 2023-05-01 19:33:50.834848 moneykit-0.0.9/moneykit/model/link_error_unauthorized_access_response.py
+-rw-r--r--   0        0        0     4965 2023-05-01 19:33:50.831072 moneykit-0.0.9/moneykit/model/link_error_unauthorized_access_response.pyi
+-rw-r--r--   0        0        0     1461 2023-05-01 19:33:50.824432 moneykit-0.0.9/moneykit/model/link_permission_scope.py
+-rw-r--r--   0        0        0     1229 2023-05-01 19:33:50.830412 moneykit-0.0.9/moneykit/model/link_permission_scope.pyi
+-rw-r--r--   0        0        0     3654 2023-05-01 19:33:50.834557 moneykit-0.0.9/moneykit/model/link_permissions.py
+-rw-r--r--   0        0        0     3610 2023-05-01 19:33:50.824957 moneykit-0.0.9/moneykit/model/link_permissions.pyi
+-rw-r--r--   0        0        0     4930 2023-05-01 19:33:50.830001 moneykit-0.0.9/moneykit/model/link_products.py
+-rw-r--r--   0        0        0     4850 2023-05-01 19:33:50.816812 moneykit-0.0.9/moneykit/model/link_products.pyi
+-rw-r--r--   0        0        0    20792 2023-05-01 19:33:50.832924 moneykit-0.0.9/moneykit/model/link_response.py
+-rw-r--r--   0        0        0    20610 2023-05-01 19:33:50.814575 moneykit-0.0.9/moneykit/model/link_response.pyi
+-rw-r--r--   0        0        0     8548 2023-05-01 19:33:50.811244 moneykit-0.0.9/moneykit/model/link_session_customer_user.py
+-rw-r--r--   0        0        0     8207 2023-05-01 19:33:50.820180 moneykit-0.0.9/moneykit/model/link_session_customer_user.pyi
+-rw-r--r--   0        0        0     4714 2023-05-01 19:33:50.841982 moneykit-0.0.9/moneykit/model/link_session_customer_user_email.py
+-rw-r--r--   0        0        0     4391 2023-05-01 19:33:50.818322 moneykit-0.0.9/moneykit/model/link_session_customer_user_email.pyi
+-rw-r--r--   0        0        0     7373 2023-05-01 19:33:50.811116 moneykit-0.0.9/moneykit/model/link_session_customer_user_phone.py
+-rw-r--r--   0        0        0     7031 2023-05-01 19:33:50.810159 moneykit-0.0.9/moneykit/model/link_session_customer_user_phone.pyi
+-rw-r--r--   0        0        0     5337 2023-05-01 19:33:50.826954 moneykit-0.0.9/moneykit/model/link_session_error_forbidden_config_response.py
+-rw-r--r--   0        0        0     5060 2023-05-01 19:33:50.837172 moneykit-0.0.9/moneykit/model/link_session_error_forbidden_config_response.pyi
+-rw-r--r--   0        0        0     5355 2023-05-01 19:33:50.833212 moneykit-0.0.9/moneykit/model/link_session_error_invalid_token_exchange.py
+-rw-r--r--   0        0        0     5066 2023-05-01 19:33:50.825580 moneykit-0.0.9/moneykit/model/link_session_error_invalid_token_exchange.pyi
+-rw-r--r--   0        0        0    10704 2023-05-01 19:33:50.819591 moneykit-0.0.9/moneykit/model/link_session_setting_overrides.py
+-rw-r--r--   0        0        0    10536 2023-05-01 19:33:50.838610 moneykit-0.0.9/moneykit/model/link_session_setting_overrides.pyi
+-rw-r--r--   0        0        0     1528 2023-05-01 19:33:50.833254 moneykit-0.0.9/moneykit/model/link_state.py
+-rw-r--r--   0        0        0     1253 2023-05-01 19:33:50.831188 moneykit-0.0.9/moneykit/model/link_state.pyi
+-rw-r--r--   0        0        0    11804 2023-05-01 19:33:50.842679 moneykit-0.0.9/moneykit/model/link_state_changed_webhook.py
+-rw-r--r--   0        0        0    11152 2023-05-01 19:33:50.829797 moneykit-0.0.9/moneykit/model/link_state_changed_webhook.pyi
+-rw-r--r--   0        0        0     1124 2023-05-01 19:33:50.825889 moneykit-0.0.9/moneykit/model/money_kit_env.py
+-rw-r--r--   0        0        0      986 2023-05-01 19:33:50.830919 moneykit-0.0.9/moneykit/model/money_kit_env.pyi
+-rw-r--r--   0        0        0     3586 2023-05-01 19:33:50.818564 moneykit-0.0.9/moneykit/model/money_link_features.py
+-rw-r--r--   0        0        0     3542 2023-05-01 19:33:50.819728 moneykit-0.0.9/moneykit/model/money_link_features.pyi
+-rw-r--r--   0        0        0     8201 2023-05-01 19:33:50.809948 moneykit-0.0.9/moneykit/model/owner.py
+-rw-r--r--   0        0        0     8097 2023-05-01 19:33:50.839959 moneykit-0.0.9/moneykit/model/owner.pyi
+-rw-r--r--   0        0        0     6748 2023-05-01 19:33:50.814335 moneykit-0.0.9/moneykit/model/phone_number.py
+-rw-r--r--   0        0        0     6669 2023-05-01 19:33:50.819583 moneykit-0.0.9/moneykit/model/phone_number.pyi
+-rw-r--r--   0        0        0     1308 2023-05-01 19:33:50.824576 moneykit-0.0.9/moneykit/model/phone_number_type.py
+-rw-r--r--   0        0        0     1124 2023-05-01 19:33:50.837084 moneykit-0.0.9/moneykit/model/phone_number_type.pyi
+-rw-r--r--   0        0        0     1419 2023-05-01 19:33:50.810890 moneykit-0.0.9/moneykit/model/product.py
+-rw-r--r--   0        0        0     1187 2023-05-01 19:33:50.830695 moneykit-0.0.9/moneykit/model/product.pyi
+-rw-r--r--   0        0        0    12687 2023-05-01 19:33:50.814279 moneykit-0.0.9/moneykit/model/products_settings.py
+-rw-r--r--   0        0        0    12620 2023-05-01 19:33:50.838351 moneykit-0.0.9/moneykit/model/products_settings.pyi
+-rw-r--r--   0        0        0     1427 2023-05-01 19:33:50.820156 moneykit-0.0.9/moneykit/model/provider.py
+-rw-r--r--   0        0        0     1202 2023-05-01 19:33:50.820289 moneykit-0.0.9/moneykit/model/provider.pyi
+-rw-r--r--   0        0        0     3578 2023-05-01 19:33:50.844499 moneykit-0.0.9/moneykit/model/refresh_products_request.py
+-rw-r--r--   0        0        0     3493 2023-05-01 19:33:50.834089 moneykit-0.0.9/moneykit/model/refresh_products_request.pyi
+-rw-r--r--   0        0        0     6841 2023-05-01 19:33:50.832090 moneykit-0.0.9/moneykit/model/requested_link_permission.py
+-rw-r--r--   0        0        0     6762 2023-05-01 19:33:50.828780 moneykit-0.0.9/moneykit/model/requested_link_permission.pyi
+-rw-r--r--   0        0        0     1029 2023-05-01 19:33:50.815681 moneykit-0.0.9/moneykit/model/supported_version.py
+-rw-r--r--   0        0        0      919 2023-05-01 19:33:50.827567 moneykit-0.0.9/moneykit/model/supported_version.pyi
+-rw-r--r--   0        0        0    12832 2023-05-01 19:33:50.819304 moneykit-0.0.9/moneykit/model/transaction.py
+-rw-r--r--   0        0        0    12654 2023-05-01 19:33:50.821895 moneykit-0.0.9/moneykit/model/transaction.pyi
+-rw-r--r--   0        0        0     6744 2023-05-01 19:33:50.825582 moneykit-0.0.9/moneykit/model/transaction_diff.py
+-rw-r--r--   0        0        0     6660 2023-05-01 19:33:50.821751 moneykit-0.0.9/moneykit/model/transaction_diff.pyi
+-rw-r--r--   0        0        0    12987 2023-05-01 19:33:50.822991 moneykit-0.0.9/moneykit/model/transaction_sync_response.py
+-rw-r--r--   0        0        0    12887 2023-05-01 19:33:50.841550 moneykit-0.0.9/moneykit/model/transaction_sync_response.pyi
+-rw-r--r--   0        0        0     1104 2023-05-01 19:33:50.835730 moneykit-0.0.9/moneykit/model/transaction_type.py
+-rw-r--r--   0        0        0      978 2023-05-01 19:33:50.826867 moneykit-0.0.9/moneykit/model/transaction_type.pyi
+-rw-r--r--   0        0        0     1110 2023-05-01 19:33:50.823431 moneykit-0.0.9/moneykit/model/transaction_type_filter.py
+-rw-r--r--   0        0        0      984 2023-05-01 19:33:50.830077 moneykit-0.0.9/moneykit/model/transaction_type_filter.pyi
+-rw-r--r--   0        0        0     5911 2023-05-01 19:33:50.831647 moneykit-0.0.9/moneykit/model/transactions_link_product.py
+-rw-r--r--   0        0        0     5831 2023-05-01 19:33:50.812081 moneykit-0.0.9/moneykit/model/transactions_link_product.pyi
+-rw-r--r--   0        0        0     4128 2023-05-01 19:33:50.822632 moneykit-0.0.9/moneykit/model/transactions_product_settings.py
+-rw-r--r--   0        0        0     4052 2023-05-01 19:33:50.824339 moneykit-0.0.9/moneykit/model/transactions_product_settings.pyi
+-rw-r--r--   0        0        0     4719 2023-05-01 19:33:50.812693 moneykit-0.0.9/moneykit/model/update_link_request.py
+-rw-r--r--   0        0        0     4584 2023-05-01 19:33:50.825108 moneykit-0.0.9/moneykit/model/update_link_request.pyi
+-rw-r--r--   0        0        0     4612 2023-05-01 19:33:50.820797 moneykit-0.0.9/moneykit/model/user_accounts_out.py
+-rw-r--r--   0        0        0     4568 2023-05-01 19:33:50.812609 moneykit-0.0.9/moneykit/model/user_accounts_out.pyi
+-rw-r--r--   0        0        0     4606 2023-05-01 19:33:50.816895 moneykit-0.0.9/moneykit/model/user_links_out.py
+-rw-r--r--   0        0        0     4562 2023-05-01 19:33:50.816110 moneykit-0.0.9/moneykit/model/user_links_out.pyi
+-rw-r--r--   0        0        0     4704 2023-05-01 19:33:50.810670 moneykit-0.0.9/moneykit/model/user_transactions_paged_response.py
+-rw-r--r--   0        0        0     4660 2023-05-01 19:33:50.822220 moneykit-0.0.9/moneykit/model/user_transactions_paged_response.pyi
+-rw-r--r--   0        0        0     9395 2023-05-01 19:33:50.821188 moneykit-0.0.9/moneykit/model/validation_error.py
+-rw-r--r--   0        0        0     9315 2023-05-01 19:33:50.832954 moneykit-0.0.9/moneykit/model/validation_error.pyi
+-rw-r--r--   0        0        0     6451 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/models/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-01 19:33:44.000000 moneykit-0.0.9/moneykit/paths/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-01 19:33:49.139360 moneykit-0.0.9/moneykit/paths/auth_introspect/__init__.py
+-rw-r--r--   0        0        0    13677 2023-05-01 19:33:50.834090 moneykit-0.0.9/moneykit/paths/auth_introspect/get.py
+-rw-r--r--   0        0        0    13392 2023-05-01 19:33:50.836572 moneykit-0.0.9/moneykit/paths/auth_introspect/get.pyi
+-rw-r--r--   0        0        0      296 2023-05-01 19:33:49.170755 moneykit-0.0.9/moneykit/paths/auth_token/__init__.py
+-rw-r--r--   0        0        0    17719 2023-05-01 19:33:50.818755 moneykit-0.0.9/moneykit/paths/auth_token/post.py
+-rw-r--r--   0        0        0    17426 2023-05-01 19:33:50.814510 moneykit-0.0.9/moneykit/paths/auth_token/post.pyi
+-rw-r--r--   0        0        0      300 2023-05-01 19:33:49.170937 moneykit-0.0.9/moneykit/paths/institutions/__init__.py
+-rw-r--r--   0        0        0    18697 2023-05-01 19:33:50.839965 moneykit-0.0.9/moneykit/paths/institutions/get.py
+-rw-r--r--   0        0        0    18300 2023-05-01 19:33:50.840807 moneykit-0.0.9/moneykit/paths/institutions/get.pyi
+-rw-r--r--   0        0        0      330 2023-05-01 19:33:49.171691 moneykit-0.0.9/moneykit/paths/institutions_institution_id/__init__.py
+-rw-r--r--   0        0        0    16873 2023-05-01 19:33:50.849043 moneykit-0.0.9/moneykit/paths/institutions_institution_id/get.py
+-rw-r--r--   0        0        0    16522 2023-05-01 19:33:50.842156 moneykit-0.0.9/moneykit/paths/institutions_institution_id/get.pyi
+-rw-r--r--   0        0        0      346 2023-05-01 19:33:49.176564 moneykit-0.0.9/moneykit/paths/institutions_institution_id_styling/__init__.py
+-rw-r--r--   0        0        0    17015 2023-05-01 19:33:50.847056 moneykit-0.0.9/moneykit/paths/institutions_institution_id_styling/get.py
+-rw-r--r--   0        0        0    16664 2023-05-01 19:33:50.848386 moneykit-0.0.9/moneykit/paths/institutions_institution_id_styling/get.pyi
+-rw-r--r--   0        0        0      299 2023-05-01 19:33:49.248865 moneykit-0.0.9/moneykit/paths/link_session/__init__.py
+-rw-r--r--   0        0        0    18397 2023-05-01 19:33:50.848919 moneykit-0.0.9/moneykit/paths/link_session/post.py
+-rw-r--r--   0        0        0    18052 2023-05-01 19:33:50.846628 moneykit-0.0.9/moneykit/paths/link_session/post.pyi
+-rw-r--r--   0        0        0      328 2023-05-01 19:33:49.302210 moneykit-0.0.9/moneykit/paths/link_session_exchange_token/__init__.py
+-rw-r--r--   0        0        0    18303 2023-05-01 19:33:50.850692 moneykit-0.0.9/moneykit/paths/link_session_exchange_token/post.py
+-rw-r--r--   0        0        0    17958 2023-05-01 19:33:50.847117 moneykit-0.0.9/moneykit/paths/link_session_exchange_token/post.pyi
+-rw-r--r--   0        0        0      292 2023-05-01 19:33:49.318176 moneykit-0.0.9/moneykit/paths/links_id/__init__.py
+-rw-r--r--   0        0        0    18419 2023-05-01 19:33:50.836319 moneykit-0.0.9/moneykit/paths/links_id/delete.py
+-rw-r--r--   0        0        0    17972 2023-05-01 19:33:50.839754 moneykit-0.0.9/moneykit/paths/links_id/delete.pyi
+-rw-r--r--   0        0        0    18631 2023-05-01 19:33:50.837516 moneykit-0.0.9/moneykit/paths/links_id/get.py
+-rw-r--r--   0        0        0    18184 2023-05-01 19:33:50.839444 moneykit-0.0.9/moneykit/paths/links_id/get.pyi
+-rw-r--r--   0        0        0    22888 2023-05-01 19:33:50.842507 moneykit-0.0.9/moneykit/paths/links_id/patch.py
+-rw-r--r--   0        0        0    22413 2023-05-01 19:33:50.836939 moneykit-0.0.9/moneykit/paths/links_id/patch.pyi
+-rw-r--r--   0        0        0      310 2023-05-01 19:33:49.413874 moneykit-0.0.9/moneykit/paths/links_id_accounts/__init__.py
+-rw-r--r--   0        0        0    21397 2023-05-01 19:33:50.850244 moneykit-0.0.9/moneykit/paths/links_id_accounts/get.py
+-rw-r--r--   0        0        0    20945 2023-05-01 19:33:50.844079 moneykit-0.0.9/moneykit/paths/links_id_accounts/get.pyi
+-rw-r--r--   0        0        0      332 2023-05-01 19:33:49.460274 moneykit-0.0.9/moneykit/paths/links_id_accounts_account_id/__init__.py
+-rw-r--r--   0        0        0    19061 2023-05-01 19:33:50.843960 moneykit-0.0.9/moneykit/paths/links_id_accounts_account_id/get.py
+-rw-r--r--   0        0        0    18614 2023-05-01 19:33:50.844949 moneykit-0.0.9/moneykit/paths/links_id_accounts_account_id/get.pyi
+-rw-r--r--   0        0        0      326 2023-05-01 19:33:49.513399 moneykit-0.0.9/moneykit/paths/links_id_accounts_numbers/__init__.py
+-rw-r--r--   0        0        0    18809 2023-05-01 19:33:50.846366 moneykit-0.0.9/moneykit/paths/links_id_accounts_numbers/get.py
+-rw-r--r--   0        0        0    18362 2023-05-01 19:33:50.846716 moneykit-0.0.9/moneykit/paths/links_id_accounts_numbers/get.pyi
+-rw-r--r--   0        0        0      310 2023-05-01 19:33:49.525252 moneykit-0.0.9/moneykit/paths/links_id_identity/__init__.py
+-rw-r--r--   0        0        0    21409 2023-05-01 19:33:50.838924 moneykit-0.0.9/moneykit/paths/links_id_identity/get.py
+-rw-r--r--   0        0        0    20957 2023-05-01 19:33:50.841741 moneykit-0.0.9/moneykit/paths/links_id_identity/get.pyi
+-rw-r--r--   0        0        0      310 2023-05-01 19:33:49.585695 moneykit-0.0.9/moneykit/paths/links_id_products/__init__.py
+-rw-r--r--   0        0        0    22935 2023-05-01 19:33:50.830797 moneykit-0.0.9/moneykit/paths/links_id_products/post.py
+-rw-r--r--   0        0        0    22460 2023-05-01 19:33:50.838270 moneykit-0.0.9/moneykit/paths/links_id_products/post.pyi
+-rw-r--r--   0        0        0      318 2023-05-01 19:33:49.602343 moneykit-0.0.9/moneykit/paths/links_id_transactions/__init__.py
+-rw-r--r--   0        0        0    23741 2023-05-01 19:33:50.847602 moneykit-0.0.9/moneykit/paths/links_id_transactions/get.py
+-rw-r--r--   0        0        0    23171 2023-05-01 19:33:50.849731 moneykit-0.0.9/moneykit/paths/links_id_transactions/get.pyi
+-rw-r--r--   0        0        0      328 2023-05-01 19:33:49.631645 moneykit-0.0.9/moneykit/paths/links_id_transactions_sync/__init__.py
+-rw-r--r--   0        0        0    21818 2023-05-01 19:33:50.830629 moneykit-0.0.9/moneykit/paths/links_id_transactions_sync/get.py
+-rw-r--r--   0        0        0    21293 2023-05-01 19:33:50.833261 moneykit-0.0.9/moneykit/paths/links_id_transactions_sync/get.pyi
+-rw-r--r--   0        0        0      310 2023-05-01 19:33:49.654006 moneykit-0.0.9/moneykit/paths/users_id_accounts/__init__.py
+-rw-r--r--   0        0        0    19316 2023-05-01 19:33:50.823253 moneykit-0.0.9/moneykit/paths/users_id_accounts/get.py
+-rw-r--r--   0        0        0    18938 2023-05-01 19:33:50.826457 moneykit-0.0.9/moneykit/paths/users_id_accounts/get.pyi
+-rw-r--r--   0        0        0      304 2023-05-01 19:33:49.686637 moneykit-0.0.9/moneykit/paths/users_id_links/__init__.py
+-rw-r--r--   0        0        0    15565 2023-05-01 19:33:50.810274 moneykit-0.0.9/moneykit/paths/users_id_links/get.py
+-rw-r--r--   0        0        0    15278 2023-05-01 19:33:50.812216 moneykit-0.0.9/moneykit/paths/users_id_links/get.pyi
+-rw-r--r--   0        0        0      318 2023-05-01 19:33:49.801614 moneykit-0.0.9/moneykit/paths/users_id_transactions/__init__.py
+-rw-r--r--   0        0        0    23515 2023-05-01 19:33:50.848352 moneykit-0.0.9/moneykit/paths/users_id_transactions/get.py
+-rw-r--r--   0        0        0    23015 2023-05-01 19:33:50.849824 moneykit-0.0.9/moneykit/paths/users_id_transactions/get.pyi
+-rw-r--r--   0        0        0      316 2023-05-01 19:33:49.823303 moneykit-0.0.9/moneykit/paths/well_known_jwks_json/__init__.py
+-rw-r--r--   0        0        0    13631 2023-05-01 19:33:50.832544 moneykit-0.0.9/moneykit/paths/well_known_jwks_json/get.py
+-rw-r--r--   0        0        0    13346 2023-05-01 19:33:50.834960 moneykit-0.0.9/moneykit/paths/well_known_jwks_json/get.pyi
+-rw-r--r--   0        0        0      963 2023-05-01 19:34:30.643036 moneykit-0.0.9/moneykit/plaid_compatible/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-01 19:34:30.675078 moneykit-0.0.9/moneykit/plaid_compatible/api/__init__.py
+-rw-r--r--   0        0        0    50030 2023-05-01 19:34:30.675797 moneykit-0.0.9/moneykit/plaid_compatible/api/plaid_api.py
+-rw-r--r--   0        0        0    36839 2023-05-01 19:34:30.676696 moneykit-0.0.9/moneykit/plaid_compatible/api_client.py
+-rw-r--r--   0        0        0      470 2023-05-01 19:34:30.642493 moneykit-0.0.9/moneykit/plaid_compatible/apis/__init__.py
+-rw-r--r--   0        0        0    17735 2023-05-01 19:34:30.642285 moneykit-0.0.9/moneykit/plaid_compatible/configuration.py
+-rw-r--r--   0        0        0     5093 2023-05-01 19:34:30.676065 moneykit-0.0.9/moneykit/plaid_compatible/exceptions.py
+-rw-r--r--   0        0        0      348 2023-05-01 19:34:30.655029 moneykit-0.0.9/moneykit/plaid_compatible/model/__init__.py
+-rw-r--r--   0        0        0    10890 2023-05-01 19:34:30.661531 moneykit-0.0.9/moneykit/plaid_compatible/model/account_balance.py
+-rw-r--r--   0        0        0    10741 2023-05-01 19:34:30.658408 moneykit-0.0.9/moneykit/plaid_compatible/model/account_base.py
+-rw-r--r--   0        0        0    11657 2023-05-01 19:34:30.652402 moneykit-0.0.9/moneykit/plaid_compatible/model/account_identity.py
+-rw-r--r--   0        0        0    11414 2023-05-01 19:34:30.657685 moneykit-0.0.9/moneykit/plaid_compatible/model/account_subtype.py
+-rw-r--r--   0        0        0     7191 2023-05-01 19:34:30.671877 moneykit-0.0.9/moneykit/plaid_compatible/model/account_type.py
+-rw-r--r--   0        0        0     7674 2023-05-01 19:34:30.658705 moneykit-0.0.9/moneykit/plaid_compatible/model/accounts_get_request.py
+-rw-r--r--   0        0        0     6636 2023-05-01 19:34:30.669392 moneykit-0.0.9/moneykit/plaid_compatible/model/accounts_get_request_options.py
+-rw-r--r--   0        0        0     7447 2023-05-01 19:34:30.665506 moneykit-0.0.9/moneykit/plaid_compatible/model/accounts_get_response.py
+-rw-r--r--   0        0        0     6925 2023-05-01 19:34:30.645177 moneykit-0.0.9/moneykit/plaid_compatible/model/address.py
+-rw-r--r--   0        0        0     7501 2023-05-01 19:34:30.659913 moneykit-0.0.9/moneykit/plaid_compatible/model/address_data.py
+-rw-r--r--   0        0        0     7793 2023-05-01 19:34:30.669692 moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_numbers.py
+-rw-r--r--   0        0        0     7642 2023-05-01 19:34:30.668540 moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_request.py
+-rw-r--r--   0        0        0     6715 2023-05-01 19:34:30.658037 moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_request_options.py
+-rw-r--r--   0        0        0     7635 2023-05-01 19:34:30.673828 moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_response.py
+-rw-r--r--   0        0        0     7265 2023-05-01 19:34:30.647357 moneykit-0.0.9/moneykit/plaid_compatible/model/counterparty_type.py
+-rw-r--r--   0        0        0     6955 2023-05-01 19:34:30.669977 moneykit-0.0.9/moneykit/plaid_compatible/model/country_code.py
+-rw-r--r--   0        0        0     7029 2023-05-01 19:34:30.647714 moneykit-0.0.9/moneykit/plaid_compatible/model/credit_account_subtype.py
+-rw-r--r--   0        0        0     7070 2023-05-01 19:34:30.644576 moneykit-0.0.9/moneykit/plaid_compatible/model/credit_filter.py
+-rw-r--r--   0        0        0     7417 2023-05-01 19:34:30.667383 moneykit-0.0.9/moneykit/plaid_compatible/model/depository_account_subtype.py
+-rw-r--r--   0        0        0     7102 2023-05-01 19:34:30.668804 moneykit-0.0.9/moneykit/plaid_compatible/model/depository_filter.py
+-rw-r--r--   0        0        0     6966 2023-05-01 19:34:30.663270 moneykit-0.0.9/moneykit/plaid_compatible/model/email.py
+-rw-r--r--   0        0        0     6965 2023-05-01 19:34:30.674103 moneykit-0.0.9/moneykit/plaid_compatible/model/employment_source_type.py
+-rw-r--r--   0        0        0     6724 2023-05-01 19:34:30.659644 moneykit-0.0.9/moneykit/plaid_compatible/model/http_validation_error.py
+-rw-r--r--   0        0        0     9101 2023-05-01 19:34:30.663657 moneykit-0.0.9/moneykit/plaid_compatible/model/id_number_type.py
+-rw-r--r--   0        0        0     7674 2023-05-01 19:34:30.665991 moneykit-0.0.9/moneykit/plaid_compatible/model/identity_get_request.py
+-rw-r--r--   0        0        0     6723 2023-05-01 19:34:30.667098 moneykit-0.0.9/moneykit/plaid_compatible/model/identity_get_request_options.py
+-rw-r--r--   0        0        0     7362 2023-05-01 19:34:30.664334 moneykit-0.0.9/moneykit/plaid_compatible/model/identity_get_response.py
+-rw-r--r--   0        0        0     7111 2023-05-01 19:34:30.646772 moneykit-0.0.9/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py
+-rw-r--r--   0        0        0     6981 2023-05-01 19:34:30.649429 moneykit-0.0.9/moneykit/plaid_compatible/model/income_verification_source_type.py
+-rw-r--r--   0        0        0     9913 2023-05-01 19:34:30.672188 moneykit-0.0.9/moneykit/plaid_compatible/model/investment_account_subtype.py
+-rw-r--r--   0        0        0     7102 2023-05-01 19:34:30.660868 moneykit-0.0.9/moneykit/plaid_compatible/model/investment_filter.py
+-rw-r--r--   0        0        0    10420 2023-05-01 19:34:30.673553 moneykit-0.0.9/moneykit/plaid_compatible/model/item.py
+-rw-r--r--   0        0        0     7717 2023-05-01 19:34:30.658996 moneykit-0.0.9/moneykit/plaid_compatible/model/item_error_webhook.py
+-rw-r--r--   0        0        0     7265 2023-05-01 19:34:30.662927 moneykit-0.0.9/moneykit/plaid_compatible/model/item_get_request.py
+-rw-r--r--   0        0        0     7287 2023-05-01 19:34:30.646422 moneykit-0.0.9/moneykit/plaid_compatible/model/item_get_response.py
+-rw-r--r--   0        0        0     7331 2023-05-01 19:34:30.664009 moneykit-0.0.9/moneykit/plaid_compatible/model/item_public_token_exchange_request.py
+-rw-r--r--   0        0        0     7235 2023-05-01 19:34:30.674459 moneykit-0.0.9/moneykit/plaid_compatible/model/item_public_token_exchange_response.py
+-rw-r--r--   0        0        0     7271 2023-05-01 19:34:30.648363 moneykit-0.0.9/moneykit/plaid_compatible/model/item_remove_request.py
+-rw-r--r--   0        0        0     6715 2023-05-01 19:34:30.670849 moneykit-0.0.9/moneykit/plaid_compatible/model/item_remove_response.py
+-rw-r--r--   0        0        0     7362 2023-05-01 19:34:30.669120 moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_investments.py
+-rw-r--r--   0        0        0     6852 2023-05-01 19:34:30.660581 moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_last_webhook.py
+-rw-r--r--   0        0        0     7489 2023-05-01 19:34:30.667656 moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_nullable.py
+-rw-r--r--   0        0        0     7366 2023-05-01 19:34:30.651005 moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_transactions.py
+-rw-r--r--   0        0        0     7595 2023-05-01 19:34:30.672457 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_account_filters.py
+-rw-r--r--   0        0        0     6644 2023-05-01 19:34:30.657276 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_institution_data.py
+-rw-r--r--   0        0        0    21548 2023-05-01 19:34:30.671332 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request.py
+-rw-r--r--   0        0        0     8258 2023-05-01 19:34:30.646141 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_auth.py
+-rw-r--r--   0        0        0     6733 2023-05-01 19:34:30.652007 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py
+-rw-r--r--   0        0        0     7534 2023-05-01 19:34:30.652690 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_employment.py
+-rw-r--r--   0        0        0     6722 2023-05-01 19:34:30.654479 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py
+-rw-r--r--   0        0        0     7661 2023-05-01 19:34:30.662192 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py
+-rw-r--r--   0        0        0    10586 2023-05-01 19:34:30.670297 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py
+-rw-r--r--   0        0        0     7020 2023-05-01 19:34:30.643645 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py
+-rw-r--r--   0        0        0     7697 2023-05-01 19:34:30.653270 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py
+-rw-r--r--   0        0        0     6937 2023-05-01 19:34:30.644238 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py
+-rw-r--r--   0        0        0     6940 2023-05-01 19:34:30.661155 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_transfer.py
+-rw-r--r--   0        0        0     6779 2023-05-01 19:34:30.650714 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_update.py
+-rw-r--r--   0        0        0    11399 2023-05-01 19:34:30.644912 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_user.py
+-rw-r--r--   0        0        0     6963 2023-05-01 19:34:30.672727 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_user_name.py
+-rw-r--r--   0        0        0     8414 2023-05-01 19:34:30.650422 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py
+-rw-r--r--   0        0        0     7615 2023-05-01 19:34:30.653589 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_response.py
+-rw-r--r--   0        0        0     6616 2023-05-01 19:34:30.666765 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_eu_config.py
+-rw-r--r--   0        0        0     6769 2023-05-01 19:34:30.673258 moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_investments.py
+-rw-r--r--   0        0        0     7573 2023-05-01 19:34:30.652982 moneykit-0.0.9/moneykit/plaid_compatible/model/loan_account_subtype.py
+-rw-r--r--   0        0        0     7054 2023-05-01 19:34:30.656221 moneykit-0.0.9/moneykit/plaid_compatible/model/loan_filter.py
+-rw-r--r--   0        0        0     7487 2023-05-01 19:34:30.660284 moneykit-0.0.9/moneykit/plaid_compatible/model/location.py
+-rw-r--r--   0        0        0     7716 2023-05-01 19:34:30.655610 moneykit-0.0.9/moneykit/plaid_compatible/model/money_link_features.py
+-rw-r--r--   0        0        0     8621 2023-05-01 19:34:30.670578 moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_ach.py
+-rw-r--r--   0        0        0     7019 2023-05-01 19:34:30.649725 moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_bacs.py
+-rw-r--r--   0        0        0     7225 2023-05-01 19:34:30.654827 moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_eft.py
+-rw-r--r--   0        0        0     7007 2023-05-01 19:34:30.659350 moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_international.py
+-rw-r--r--   0        0        0     8304 2023-05-01 19:34:30.656582 moneykit-0.0.9/moneykit/plaid_compatible/model/owner.py
+-rw-r--r--   0        0        0     7593 2023-05-01 19:34:30.643939 moneykit-0.0.9/moneykit/plaid_compatible/model/payment_meta.py
+-rw-r--r--   0        0        0     6930 2023-05-01 19:34:30.648001 moneykit-0.0.9/moneykit/plaid_compatible/model/personal_finance_category.py
+-rw-r--r--   0        0        0     6934 2023-05-01 19:34:30.653922 moneykit-0.0.9/moneykit/plaid_compatible/model/phone_number.py
+-rw-r--r--   0        0        0     9494 2023-05-01 19:34:30.674826 moneykit-0.0.9/moneykit/plaid_compatible/model/plaid_error.py
+-rw-r--r--   0        0        0     8113 2023-05-01 19:34:30.645496 moneykit-0.0.9/moneykit/plaid_compatible/model/plaid_error_type.py
+-rw-r--r--   0        0        0     7129 2023-05-01 19:34:30.655292 moneykit-0.0.9/moneykit/plaid_compatible/model/products.py
+-rw-r--r--   0        0        0     6610 2023-05-01 19:34:30.645840 moneykit-0.0.9/moneykit/plaid_compatible/model/removed_transaction.py
+-rw-r--r--   0        0        0    16756 2023-05-01 19:34:30.651442 moneykit-0.0.9/moneykit/plaid_compatible/model/transaction.py
+-rw-r--r--   0        0        0     7632 2023-05-01 19:34:30.655935 moneykit-0.0.9/moneykit/plaid_compatible/model/transaction_code.py
+-rw-r--r--   0        0        0     7510 2023-05-01 19:34:30.649123 moneykit-0.0.9/moneykit/plaid_compatible/model/transaction_counterparty.py
+-rw-r--r--   0        0        0     8236 2023-05-01 19:34:30.664723 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_get_request.py
+-rw-r--r--   0        0        0     9639 2023-05-01 19:34:30.661865 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_get_request_options.py
+-rw-r--r--   0        0        0     8530 2023-05-01 19:34:30.667955 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_get_response.py
+-rw-r--r--   0        0        0     7289 2023-05-01 19:34:30.672996 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_refresh_request.py
+-rw-r--r--   0        0        0     6733 2023-05-01 19:34:30.647071 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_refresh_response.py
+-rw-r--r--   0        0        0     8397 2023-05-01 19:34:30.665082 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_sync_request.py
+-rw-r--r--   0        0        0     8427 2023-05-01 19:34:30.668271 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_sync_request_options.py
+-rw-r--r--   0        0        0     8900 2023-05-01 19:34:30.656974 moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_sync_response.py
+-rw-r--r--   0        0        0     7916 2023-05-01 19:34:30.662555 moneykit-0.0.9/moneykit/plaid_compatible/model/user_address.py
+-rw-r--r--   0        0        0     6950 2023-05-01 19:34:30.666400 moneykit-0.0.9/moneykit/plaid_compatible/model/user_id_number.py
+-rw-r--r--   0        0        0     7625 2023-05-01 19:34:30.671604 moneykit-0.0.9/moneykit/plaid_compatible/model/user_stated_income_source_category.py
+-rw-r--r--   0        0        0     7187 2023-05-01 19:34:30.650075 moneykit-0.0.9/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py
+-rw-r--r--   0        0        0     7027 2023-05-01 19:34:30.654201 moneykit-0.0.9/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py
+-rw-r--r--   0        0        0     6793 2023-05-01 19:34:30.648714 moneykit-0.0.9/moneykit/plaid_compatible/model/validation_error.py
+-rw-r--r--   0        0        0     7069 2023-05-01 19:34:30.651731 moneykit-0.0.9/moneykit/plaid_compatible/model/webhook_environment_values.py
+-rw-r--r--   0        0        0    74795 2023-05-01 19:34:30.641802 moneykit-0.0.9/moneykit/plaid_compatible/model_utils.py
+-rw-r--r--   0        0        0     8892 2023-05-01 19:34:30.643326 moneykit-0.0.9/moneykit/plaid_compatible/models/__init__.py
+-rw-r--r--   0        0        0    12537 2023-05-01 19:34:30.642813 moneykit-0.0.9/moneykit/plaid_compatible/rest.py
+-rw-r--r--   0        0        0     9365 2023-05-01 19:33:50.839439 moneykit-0.0.9/moneykit/rest.py
+-rw-r--r--   0        0        0    99126 2023-05-01 19:33:50.853811 moneykit-0.0.9/moneykit/schemas.py
+-rw-r--r--   0        0        0      940 2023-05-01 19:38:06.905649 moneykit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    21132 1970-01-01 00:00:00.000000 moneykit-0.0.9/PKG-INFO
```

### Comparing `moneykit-0.0.8/README.md` & `moneykit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/__init__.py` & `moneykit-0.0.9/moneykit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 # import ApiClient
 from moneykit.api_client import ApiClient
 
 # import Configuration
 from moneykit.configuration import Configuration
```

### Comparing `moneykit-0.0.8/moneykit/api_client.py` & `moneykit-0.0.9/moneykit/api_client.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/path_to_api.py` & `moneykit-0.0.9/moneykit/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tag_to_api.py` & `moneykit-0.0.9/moneykit/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/__init__.py` & `moneykit-0.0.9/moneykit/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/access_token_api.py` & `moneykit-0.0.9/moneykit/apis/tags/access_token_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/account_numbers_api.py` & `moneykit-0.0.9/moneykit/apis/tags/account_numbers_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/accounts_api.py` & `moneykit-0.0.9/moneykit/apis/tags/accounts_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/identity_api.py` & `moneykit-0.0.9/moneykit/apis/tags/identity_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/institutions_api.py` & `moneykit-0.0.9/moneykit/apis/tags/institutions_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/link_session_api.py` & `moneykit-0.0.9/moneykit/apis/tags/link_session_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/links_api.py` & `moneykit-0.0.9/moneykit/apis/tags/links_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/products_api.py` & `moneykit-0.0.9/moneykit/apis/tags/products_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/transactions_api.py` & `moneykit-0.0.9/moneykit/apis/tags/transactions_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/apis/tags/users_api.py` & `moneykit-0.0.9/moneykit/apis/tags/users_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/configuration.py` & `moneykit-0.0.9/moneykit/configuration.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/exceptions.py` & `moneykit-0.0.9/moneykit/exceptions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account.py` & `moneykit-0.0.9/moneykit/model/account.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account.pyi` & `moneykit-0.0.9/moneykit/model/account.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_balances.py` & `moneykit-0.0.9/moneykit/model/account_balances.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_balances.pyi` & `moneykit-0.0.9/moneykit/model/account_balances.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_group.py` & `moneykit-0.0.9/moneykit/model/account_group.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_group.pyi` & `moneykit-0.0.9/moneykit/model/account_group.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_identity.py` & `moneykit-0.0.9/moneykit/model/account_identity.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_identity.pyi` & `moneykit-0.0.9/moneykit/model/account_identity.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_numbers.py` & `moneykit-0.0.9/moneykit/model/account_numbers.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_numbers.pyi` & `moneykit-0.0.9/moneykit/model/account_numbers.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_numbers_link_product.py` & `moneykit-0.0.9/moneykit/model/account_numbers_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_numbers_link_product.pyi` & `moneykit-0.0.9/moneykit/model/account_numbers_link_product.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_numbers_product_settings.py` & `moneykit-0.0.9/moneykit/model/account_numbers_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_numbers_product_settings.pyi` & `moneykit-0.0.9/moneykit/model/account_numbers_product_settings.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_type.py` & `moneykit-0.0.9/moneykit/model/account_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_type.pyi` & `moneykit-0.0.9/moneykit/model/account_type.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_with_account_numbers.py` & `moneykit-0.0.9/moneykit/model/account_with_account_numbers.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/account_with_account_numbers.pyi` & `moneykit-0.0.9/moneykit/model/account_with_account_numbers.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/accounts_link_product.py` & `moneykit-0.0.9/moneykit/model/accounts_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/accounts_link_product.pyi` & `moneykit-0.0.9/moneykit/model/accounts_link_product.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/ach_number.py` & `moneykit-0.0.9/moneykit/model/ach_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/ach_number.pyi` & `moneykit-0.0.9/moneykit/model/ach_number.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/address.py` & `moneykit-0.0.9/moneykit/model/address.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/address.pyi` & `moneykit-0.0.9/moneykit/model/address.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/api_error_auth_expired_access_token_response.py` & `moneykit-0.0.9/moneykit/model/api_error_auth_expired_access_token_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/api_error_auth_expired_access_token_response.pyi` & `moneykit-0.0.9/moneykit/model/api_error_auth_expired_access_token_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/api_error_auth_unauthorized_response.py` & `moneykit-0.0.9/moneykit/model/api_error_auth_unauthorized_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/api_error_auth_unauthorized_response.pyi` & `moneykit-0.0.9/moneykit/model/api_error_auth_unauthorized_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/api_error_rate_limit_exceeded_response.py` & `moneykit-0.0.9/moneykit/model/api_error_rate_limit_exceeded_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/api_error_rate_limit_exceeded_response.pyi` & `moneykit-0.0.9/moneykit/model/api_error_rate_limit_exceeded_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/bacs_number.py` & `moneykit-0.0.9/moneykit/model/bacs_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/bacs_number.pyi` & `moneykit-0.0.9/moneykit/model/bacs_number.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/basic_account_details.py` & `moneykit-0.0.9/moneykit/model/basic_account_details.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/basic_account_details.pyi` & `moneykit-0.0.9/moneykit/model/basic_account_details.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/country.py` & `moneykit-0.0.9/moneykit/model/country.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/country.pyi` & `moneykit-0.0.9/moneykit/model/country.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/create_link_session_request.py` & `moneykit-0.0.9/moneykit/model/create_link_session_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/create_link_session_request.pyi` & `moneykit-0.0.9/moneykit/model/create_link_session_request.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/create_link_session_response.py` & `moneykit-0.0.9/moneykit/model/create_link_session_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/create_link_session_response.pyi` & `moneykit-0.0.9/moneykit/model/create_link_session_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/currency.py` & `moneykit-0.0.9/moneykit/model/currency.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/currency.pyi` & `moneykit-0.0.9/moneykit/model/currency.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/cursor_pagination.py` & `moneykit-0.0.9/moneykit/model/cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/cursor_pagination.pyi` & `moneykit-0.0.9/moneykit/model/cursor_pagination.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/customer_app.py` & `moneykit-0.0.9/moneykit/model/customer_app.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/customer_app.pyi` & `moneykit-0.0.9/moneykit/model/customer_app.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/eft_number.py` & `moneykit-0.0.9/moneykit/model/eft_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/eft_number.pyi` & `moneykit-0.0.9/moneykit/model/eft_number.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/email.py` & `moneykit-0.0.9/moneykit/model/email.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/email.pyi` & `moneykit-0.0.9/moneykit/model/email.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/exchange_token_request.py` & `moneykit-0.0.9/moneykit/model/exchange_token_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/exchange_token_request.pyi` & `moneykit-0.0.9/moneykit/model/exchange_token_request.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/exchange_token_response.py` & `moneykit-0.0.9/moneykit/model/exchange_token_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/exchange_token_response.pyi` & `moneykit-0.0.9/moneykit/model/exchange_token_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/generate_access_token_response.py` & `moneykit-0.0.9/moneykit/model/generate_access_token_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/generate_access_token_response.pyi` & `moneykit-0.0.9/moneykit/model/generate_access_token_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_account_numbers_response.py` & `moneykit-0.0.9/moneykit/model/get_account_numbers_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_account_numbers_response.pyi` & `moneykit-0.0.9/moneykit/model/get_account_numbers_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_account_response.py` & `moneykit-0.0.9/moneykit/model/get_account_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_account_response.pyi` & `moneykit-0.0.9/moneykit/model/get_account_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_accounts_response.py` & `moneykit-0.0.9/moneykit/model/get_accounts_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_accounts_response.pyi` & `moneykit-0.0.9/moneykit/model/get_accounts_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_institutions_response.py` & `moneykit-0.0.9/moneykit/model/get_institutions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_institutions_response.pyi` & `moneykit-0.0.9/moneykit/model/get_institutions_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_transactions_response.py` & `moneykit-0.0.9/moneykit/model/get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_transactions_response.pyi` & `moneykit-0.0.9/moneykit/model/get_transactions_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_user_accounts_response.py` & `moneykit-0.0.9/moneykit/model/get_user_accounts_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_user_accounts_response.pyi` & `moneykit-0.0.9/moneykit/model/get_user_accounts_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_user_links_response.py` & `moneykit-0.0.9/moneykit/model/get_user_links_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_user_links_response.pyi` & `moneykit-0.0.9/moneykit/model/get_user_links_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_user_transactions_response.py` & `moneykit-0.0.9/moneykit/model/get_user_transactions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/get_user_transactions_response.pyi` & `moneykit-0.0.9/moneykit/model/get_user_transactions_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/http_validation_error.py` & `moneykit-0.0.9/moneykit/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/http_validation_error.pyi` & `moneykit-0.0.9/moneykit/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/identity_link_product.py` & `moneykit-0.0.9/moneykit/model/identity_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/identity_link_product.pyi` & `moneykit-0.0.9/moneykit/model/identity_link_product.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/identity_product_settings.py` & `moneykit-0.0.9/moneykit/model/identity_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/identity_product_settings.pyi` & `moneykit-0.0.9/moneykit/model/identity_product_settings.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/identity_response.py` & `moneykit-0.0.9/moneykit/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/identity_response.pyi` & `moneykit-0.0.9/moneykit/model/identity_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/institution.py` & `moneykit-0.0.9/moneykit/model/institution.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/institution.pyi` & `moneykit-0.0.9/moneykit/model/institution.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/institution_error_not_found_response.py` & `moneykit-0.0.9/moneykit/model/institution_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/institution_error_not_found_response.pyi` & `moneykit-0.0.9/moneykit/model/institution_error_not_found_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/institution_styling_response.py` & `moneykit-0.0.9/moneykit/model/institution_styling_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/institution_styling_response.pyi` & `moneykit-0.0.9/moneykit/model/institution_styling_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/international_number.py` & `moneykit-0.0.9/moneykit/model/international_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/international_number.pyi` & `moneykit-0.0.9/moneykit/model/international_number.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/introspect_client_response.py` & `moneykit-0.0.9/moneykit/model/introspect_client_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/introspect_client_response.pyi` & `moneykit-0.0.9/moneykit/model/introspect_client_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/jwk_set.py` & `moneykit-0.0.9/moneykit/model/jwk_set.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/jwk_set.pyi` & `moneykit-0.0.9/moneykit/model/jwk_set.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_common.py` & `moneykit-0.0.9/moneykit/model/link_common.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_common.pyi` & `moneykit-0.0.9/moneykit/model/link_common.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error.py` & `moneykit-0.0.9/moneykit/model/link_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error.pyi` & `moneykit-0.0.9/moneykit/model/link_error.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_bad_state_response.py` & `moneykit-0.0.9/moneykit/model/link_error_bad_state_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_bad_state_response.pyi` & `moneykit-0.0.9/moneykit/model/link_error_bad_state_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_deleted_response.py` & `moneykit-0.0.9/moneykit/model/link_error_deleted_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_deleted_response.pyi` & `moneykit-0.0.9/moneykit/model/link_error_deleted_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_forbidden_action_response.py` & `moneykit-0.0.9/moneykit/model/link_error_forbidden_action_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_forbidden_action_response.pyi` & `moneykit-0.0.9/moneykit/model/link_error_forbidden_action_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_not_found_response.py` & `moneykit-0.0.9/moneykit/model/link_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_not_found_response.pyi` & `moneykit-0.0.9/moneykit/model/link_error_not_found_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_unauthorized_access_response.py` & `moneykit-0.0.9/moneykit/model/link_error_unauthorized_access_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_error_unauthorized_access_response.pyi` & `moneykit-0.0.9/moneykit/model/link_error_unauthorized_access_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_permission_scope.py` & `moneykit-0.0.9/moneykit/model/link_permission_scope.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_permission_scope.pyi` & `moneykit-0.0.9/moneykit/model/link_permission_scope.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_permissions.py` & `moneykit-0.0.9/moneykit/model/link_permissions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_permissions.pyi` & `moneykit-0.0.9/moneykit/model/link_permissions.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_products.py` & `moneykit-0.0.9/moneykit/model/link_products.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_products.pyi` & `moneykit-0.0.9/moneykit/model/link_products.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_response.py` & `moneykit-0.0.9/moneykit/model/link_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_response.pyi` & `moneykit-0.0.9/moneykit/model/link_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_customer_user.py` & `moneykit-0.0.9/moneykit/model/link_session_customer_user.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_customer_user.pyi` & `moneykit-0.0.9/moneykit/model/link_session_customer_user.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_customer_user_email.py` & `moneykit-0.0.9/moneykit/model/link_session_customer_user_email.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_customer_user_email.pyi` & `moneykit-0.0.9/moneykit/model/link_session_customer_user_email.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_customer_user_phone.py` & `moneykit-0.0.9/moneykit/model/link_session_customer_user_phone.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_customer_user_phone.pyi` & `moneykit-0.0.9/moneykit/model/link_session_customer_user_phone.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_error_forbidden_config_response.py` & `moneykit-0.0.9/moneykit/model/link_session_error_forbidden_config_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_error_forbidden_config_response.pyi` & `moneykit-0.0.9/moneykit/model/link_session_error_forbidden_config_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_error_invalid_token_exchange.py` & `moneykit-0.0.9/moneykit/model/link_session_error_invalid_token_exchange.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_error_invalid_token_exchange.pyi` & `moneykit-0.0.9/moneykit/model/link_session_error_invalid_token_exchange.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_setting_overrides.py` & `moneykit-0.0.9/moneykit/model/link_session_setting_overrides.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_session_setting_overrides.pyi` & `moneykit-0.0.9/moneykit/model/link_session_setting_overrides.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_state.py` & `moneykit-0.0.9/moneykit/model/link_state.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_state.pyi` & `moneykit-0.0.9/moneykit/model/link_state.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_state_changed_webhook.py` & `moneykit-0.0.9/moneykit/model/link_state_changed_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/link_state_changed_webhook.pyi` & `moneykit-0.0.9/moneykit/model/link_state_changed_webhook.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/money_kit_env.py` & `moneykit-0.0.9/moneykit/model/money_kit_env.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/money_kit_env.pyi` & `moneykit-0.0.9/moneykit/model/money_kit_env.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/money_link_features.py` & `moneykit-0.0.9/moneykit/model/money_link_features.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/money_link_features.pyi` & `moneykit-0.0.9/moneykit/model/money_link_features.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/owner.py` & `moneykit-0.0.9/moneykit/model/owner.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/owner.pyi` & `moneykit-0.0.9/moneykit/model/owner.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/phone_number.py` & `moneykit-0.0.9/moneykit/model/phone_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/phone_number.pyi` & `moneykit-0.0.9/moneykit/model/phone_number.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/phone_number_type.py` & `moneykit-0.0.9/moneykit/model/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/phone_number_type.pyi` & `moneykit-0.0.9/moneykit/model/phone_number_type.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/product.py` & `moneykit-0.0.9/moneykit/model/product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/product.pyi` & `moneykit-0.0.9/moneykit/model/product.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/products_settings.py` & `moneykit-0.0.9/moneykit/model/products_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/products_settings.pyi` & `moneykit-0.0.9/moneykit/model/products_settings.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/provider.py` & `moneykit-0.0.9/moneykit/model/provider.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/provider.pyi` & `moneykit-0.0.9/moneykit/model/provider.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/refresh_products_request.py` & `moneykit-0.0.9/moneykit/model/refresh_products_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/refresh_products_request.pyi` & `moneykit-0.0.9/moneykit/model/refresh_products_request.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/requested_link_permission.py` & `moneykit-0.0.9/moneykit/model/requested_link_permission.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/requested_link_permission.pyi` & `moneykit-0.0.9/moneykit/model/requested_link_permission.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/supported_version.py` & `moneykit-0.0.9/moneykit/model/supported_version.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/supported_version.pyi` & `moneykit-0.0.9/moneykit/model/supported_version.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction.py` & `moneykit-0.0.9/moneykit/model/transaction.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction.pyi` & `moneykit-0.0.9/moneykit/model/transaction.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_diff.py` & `moneykit-0.0.9/moneykit/model/transaction_diff.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_diff.pyi` & `moneykit-0.0.9/moneykit/model/transaction_diff.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_sync_response.py` & `moneykit-0.0.9/moneykit/model/transaction_sync_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_sync_response.pyi` & `moneykit-0.0.9/moneykit/model/transaction_sync_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_type.py` & `moneykit-0.0.9/moneykit/model/transaction_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_type.pyi` & `moneykit-0.0.9/moneykit/model/transaction_type.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_type_filter.py` & `moneykit-0.0.9/moneykit/model/transaction_type_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transaction_type_filter.pyi` & `moneykit-0.0.9/moneykit/model/transaction_type_filter.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transactions_link_product.py` & `moneykit-0.0.9/moneykit/model/transactions_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transactions_link_product.pyi` & `moneykit-0.0.9/moneykit/model/transactions_link_product.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transactions_product_settings.py` & `moneykit-0.0.9/moneykit/model/transactions_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/transactions_product_settings.pyi` & `moneykit-0.0.9/moneykit/model/transactions_product_settings.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/update_link_request.py` & `moneykit-0.0.9/moneykit/model/update_link_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/update_link_request.pyi` & `moneykit-0.0.9/moneykit/model/update_link_request.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/user_accounts_out.py` & `moneykit-0.0.9/moneykit/model/user_accounts_out.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/user_accounts_out.pyi` & `moneykit-0.0.9/moneykit/model/user_accounts_out.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/user_links_out.py` & `moneykit-0.0.9/moneykit/model/user_links_out.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/user_links_out.pyi` & `moneykit-0.0.9/moneykit/model/user_links_out.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/user_transactions_paged_response.py` & `moneykit-0.0.9/moneykit/model/user_transactions_paged_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/user_transactions_paged_response.pyi` & `moneykit-0.0.9/moneykit/model/user_transactions_paged_response.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/validation_error.py` & `moneykit-0.0.9/moneykit/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/model/validation_error.pyi` & `moneykit-0.0.9/moneykit/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/models/__init__.py` & `moneykit-0.0.9/moneykit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/__init__.py` & `moneykit-0.0.9/moneykit/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/auth_introspect/get.py` & `moneykit-0.0.9/moneykit/paths/auth_introspect/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/auth_introspect/get.pyi` & `moneykit-0.0.9/moneykit/paths/auth_introspect/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/auth_token/post.py` & `moneykit-0.0.9/moneykit/paths/auth_token/post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/auth_token/post.pyi` & `moneykit-0.0.9/moneykit/paths/auth_token/post.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/institutions/get.py` & `moneykit-0.0.9/moneykit/paths/institutions/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/institutions/get.pyi` & `moneykit-0.0.9/moneykit/paths/institutions/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/institutions_institution_id/get.py` & `moneykit-0.0.9/moneykit/paths/institutions_institution_id/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/institutions_institution_id/get.pyi` & `moneykit-0.0.9/moneykit/paths/institutions_institution_id/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/institutions_institution_id_styling/get.py` & `moneykit-0.0.9/moneykit/paths/institutions_institution_id_styling/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/institutions_institution_id_styling/get.pyi` & `moneykit-0.0.9/moneykit/paths/institutions_institution_id_styling/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/link_session/post.py` & `moneykit-0.0.9/moneykit/paths/link_session/post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/link_session/post.pyi` & `moneykit-0.0.9/moneykit/paths/link_session/post.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/link_session_exchange_token/post.py` & `moneykit-0.0.9/moneykit/paths/link_session_exchange_token/post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/link_session_exchange_token/post.pyi` & `moneykit-0.0.9/moneykit/paths/link_session_exchange_token/post.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id/delete.py` & `moneykit-0.0.9/moneykit/paths/links_id/delete.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id/delete.pyi` & `moneykit-0.0.9/moneykit/paths/links_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id/get.py` & `moneykit-0.0.9/moneykit/paths/links_id/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id/patch.py` & `moneykit-0.0.9/moneykit/paths/links_id/patch.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id/patch.pyi` & `moneykit-0.0.9/moneykit/paths/links_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_accounts/get.py` & `moneykit-0.0.9/moneykit/paths/links_id_accounts/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_accounts/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_accounts/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_accounts_account_id/get.py` & `moneykit-0.0.9/moneykit/paths/links_id_accounts_account_id/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_accounts_account_id/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_accounts_account_id/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_accounts_numbers/get.py` & `moneykit-0.0.9/moneykit/paths/links_id_accounts_numbers/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_accounts_numbers/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_accounts_numbers/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_identity/get.py` & `moneykit-0.0.9/moneykit/paths/links_id_identity/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_identity/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_identity/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_products/post.py` & `moneykit-0.0.9/moneykit/paths/links_id_products/post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_products/post.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_products/post.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_transactions/get.py` & `moneykit-0.0.9/moneykit/paths/links_id_transactions/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_transactions/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_transactions/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_transactions_sync/get.py` & `moneykit-0.0.9/moneykit/paths/links_id_transactions_sync/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/links_id_transactions_sync/get.pyi` & `moneykit-0.0.9/moneykit/paths/links_id_transactions_sync/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/users_id_accounts/get.py` & `moneykit-0.0.9/moneykit/paths/users_id_accounts/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/users_id_accounts/get.pyi` & `moneykit-0.0.9/moneykit/paths/users_id_accounts/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/users_id_links/get.py` & `moneykit-0.0.9/moneykit/paths/users_id_links/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/users_id_links/get.pyi` & `moneykit-0.0.9/moneykit/paths/users_id_links/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/users_id_transactions/get.py` & `moneykit-0.0.9/moneykit/paths/users_id_transactions/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/users_id_transactions/get.pyi` & `moneykit-0.0.9/moneykit/paths/users_id_transactions/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/well_known_jwks_json/get.py` & `moneykit-0.0.9/moneykit/paths/well_known_jwks_json/get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/paths/well_known_jwks_json/get.pyi` & `moneykit-0.0.9/moneykit/paths/well_known_jwks_json/get.pyi`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/__init__.py` & `moneykit-0.0.9/moneykit/plaid_compatible/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/api/plaid_api.py` & `moneykit-0.0.9/moneykit/plaid_compatible/api/plaid_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/api_client.py` & `moneykit-0.0.9/moneykit/plaid_compatible/api_client.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/configuration.py` & `moneykit-0.0.9/moneykit/plaid_compatible/configuration.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/exceptions.py` & `moneykit-0.0.9/moneykit/plaid_compatible/exceptions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/account_balance.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/account_balance.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/account_base.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/account_base.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/account_identity.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/account_identity.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/account_subtype.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/account_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/account_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/accounts_get_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/accounts_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/accounts_get_request_options.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/accounts_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/accounts_get_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/accounts_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/address.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/address.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/address_data.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/address_data.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_numbers.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_numbers.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_request_options.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/auth_get_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/auth_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/counterparty_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/counterparty_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/country_code.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/country_code.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/credit_account_subtype.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/credit_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/credit_filter.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/credit_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/depository_account_subtype.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/depository_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/depository_filter.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/depository_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/email.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/email.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/employment_source_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/employment_source_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/http_validation_error.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/id_number_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/id_number_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/identity_get_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/identity_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/identity_get_request_options.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/identity_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/identity_get_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/identity_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/income_verification_source_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/income_verification_source_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/investment_account_subtype.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/investment_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/investment_filter.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/investment_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_error_webhook.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_error_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_get_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_get_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_public_token_exchange_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_public_token_exchange_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_public_token_exchange_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_public_token_exchange_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_remove_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_remove_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_remove_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_remove_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_investments.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_investments.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_last_webhook.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_last_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_nullable.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_nullable.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/item_status_transactions.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/item_status_transactions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_account_filters.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_account_filters.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_institution_data.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_institution_data.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_auth.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_auth.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_employment.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_employment.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_transfer.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_transfer.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_update.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_update.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_user.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_user.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_user_name.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_user_name.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_create_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_create_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_eu_config.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_eu_config.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/link_token_investments.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/link_token_investments.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/loan_account_subtype.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/loan_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/loan_filter.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/loan_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/location.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/location.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/money_link_features.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/money_link_features.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_ach.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_ach.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_bacs.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_bacs.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_eft.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_eft.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/numbers_international.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/numbers_international.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/owner.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/owner.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/payment_meta.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/payment_meta.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/personal_finance_category.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/personal_finance_category.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/phone_number.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/phone_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/plaid_error.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/plaid_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/plaid_error_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/plaid_error_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/products.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/products.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/removed_transaction.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/removed_transaction.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transaction.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transaction.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transaction_code.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transaction_code.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transaction_counterparty.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transaction_counterparty.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_get_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_get_request_options.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_get_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_refresh_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_refresh_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_refresh_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_refresh_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_sync_request.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_sync_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_sync_request_options.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_sync_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/transactions_sync_response.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/transactions_sync_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/user_address.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/user_address.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/user_id_number.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/user_id_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/user_stated_income_source_category.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/user_stated_income_source_category.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/validation_error.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model/webhook_environment_values.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model/webhook_environment_values.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/model_utils.py` & `moneykit-0.0.9/moneykit/plaid_compatible/model_utils.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/models/__init__.py` & `moneykit-0.0.9/moneykit/plaid_compatible/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/plaid_compatible/rest.py` & `moneykit-0.0.9/moneykit/plaid_compatible/rest.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/rest.py` & `moneykit-0.0.9/moneykit/rest.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/moneykit/schemas.py` & `moneykit-0.0.9/moneykit/schemas.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.8/pyproject.toml` & `moneykit-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "moneykit"
-version = "0.0.8"
+version = "0.0.9"
 description = "MoneyKit API SDK"
 authors = ["MoneyKit"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/moneykit/moneykit-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "MoneyKit"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 urllib3 = ">= 1.26.73"
 certifi = ">= 14.5.14"
-frozendict = "~= 2.7.0"
-python-dateutil = ">=2.8.2"
+frozendict = "~= 2.3.4"
+python-dateutil = "~2.7.0"
 
 [tool.poetry.dev-dependencies]
 ruff = ">=0.0.254"
 black = ">=23.3.0"
 mypy = ">=1.2"
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `moneykit-0.0.8/PKG-INFO` & `moneykit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: moneykit
-Version: 0.0.8
+Version: 0.0.9
 Summary: MoneyKit API SDK
 Home-page: https://github.com/moneykit/moneykit-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,MoneyKit
 Author: MoneyKit
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=14.5.14)
-Requires-Dist: frozendict (>=2.7.0,<2.8.0)
-Requires-Dist: python-dateutil (>=2.8.2)
+Requires-Dist: frozendict (>=2.3.4,<2.4.0)
+Requires-Dist: python-dateutil (>=2.7.0,<2.8.0)
 Requires-Dist: urllib3 (>=1.26.73)
 Project-URL: Repository, https://github.com/moneykit/moneykit-python
 Description-Content-Type: text/markdown
 
 # moneykit
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
```

