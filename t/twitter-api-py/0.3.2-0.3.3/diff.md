# Comparing `tmp/twitter_api_py-0.3.2.tar.gz` & `tmp/twitter_api_py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.3.2.tar", max compression
+gzip compressed data, was "twitter_api_py-0.3.3.tar", max compression
```

## Comparing `twitter_api_py-0.3.2.tar` & `twitter_api_py-0.3.3.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0     1497 2023-05-01 07:19:33.892883 twitter_api_py-0.3.2/LICENSE
--rw-r--r--   0        0        0     2126 2023-05-02 15:01:57.648446 twitter_api_py-0.3.2/README.md
--rw-r--r--   0        0        0     1516 2023-05-02 16:34:01.453192 twitter_api_py-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      480 2023-05-02 15:47:39.640660 twitter_api_py-0.3.2/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     1039 2023-05-01 05:03:58.580612 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0      310 2023-05-01 05:01:04.629161 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
--rw-r--r--   0        0        0     1386 2023-05-01 15:37:14.131307 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      305 2023-05-01 05:01:45.139500 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
--rw-r--r--   0        0        0      806 2023-05-01 05:02:17.969774 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0      314 2023-05-01 05:02:27.359852 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
--rw-r--r--   0        0        0     1209 2023-05-01 05:02:59.990124 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      310 2023-05-01 05:03:15.690255 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
--rw-r--r--   0        0        0      829 2023-05-01 05:03:36.810430 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0      305 2023-05-01 05:03:51.400552 twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.3.2/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      364 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0     1139 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      450 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      792 2023-05-02 16:12:13.062596 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      432 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      721 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      391 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      797 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      500 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      750 2023-05-02 16:12:03.602519 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      647 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      375 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0     1920 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     4053 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1513 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0     1644 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     3507 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0      997 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.3.2/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-24 12:44:19.060255 twitter_api_py-0.3.2/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.3.2/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5182 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1967 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3368 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     7253 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    32303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0    14518 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0    14743 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    32062 2023-05-02 15:47:39.640660 twitter_api_py-0.3.2/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    26895 2023-05-02 15:47:39.640660 twitter_api_py-0.3.2/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0    13583 2023-05-02 15:47:39.640660 twitter_api_py-0.3.2/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    10588 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.3.2/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0      603 2023-05-01 15:29:32.247704 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0     2232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0      976 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/handlers/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
--rw-r--r--   0        0        0     3316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
--rw-r--r--   0        0        0      705 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/rate_limit_info.py
--rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/rate_limit/rate_limit_target.py
--rw-r--r--   0        0        0      281 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2295 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      541 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      441 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      673 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
--rw-r--r--   0        0        0     8906 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
--rw-r--r--   0        0        0      676 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
--rw-r--r--   0        0        0     2390 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
--rw-r--r--   0        0        0      429 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3088 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      458 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6560 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     2977 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2926 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     5900 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     5999 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-02 15:14:15.304418 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      770 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3096 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      275 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      371 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6509 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      376 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      391 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7930 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      367 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1911 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      331 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8343 2023-05-02 14:54:51.834995 twitter_api_py-0.3.2/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      279 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2680 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0      299 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_users_by/__init__.py
--rw-r--r--   0        0        0     2755 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_users_by/get_v2_users_by.py
--rw-r--r--   0        0        0      396 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_users_by_username/__init__.py
--rw-r--r--   0        0        0     3025 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.3.2/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.3.2/twitter_api/types/chainable.py
--rw-r--r--   0        0        0      697 2023-04-26 11:13:40.460129 twitter_api_py-0.3.2/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.3.2/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1580 2023-04-24 17:04:45.312148 twitter_api_py-0.3.2/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      570 2023-05-02 15:47:39.640660 twitter_api_py-0.3.2/twitter_api/types/generic_client.py
--rw-r--r--   0        0        0      616 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/types/http.py
--rw-r--r--   0        0        0      734 2023-04-30 18:08:45.644350 twitter_api_py-0.3.2/twitter_api/types/httpx.py
--rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.3.2/twitter_api/types/model.py
--rw-r--r--   0        0        0     1942 2023-05-01 15:41:37.413361 twitter_api_py-0.3.2/twitter_api/types/oauth.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/types/oauth1/__init__.py
--rw-r--r--   0        0        0      833 2023-05-02 16:32:05.932256 twitter_api_py-0.3.2/twitter_api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     3473 2023-05-02 16:25:30.009051 twitter_api_py-0.3.2/twitter_api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/types/oauth2/__init__.py
--rw-r--r--   0        0        0      785 2023-05-02 16:03:21.708292 twitter_api_py-0.3.2/twitter_api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     3592 2023-05-02 16:26:12.579396 twitter_api_py-0.3.2/twitter_api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       63 2023-05-02 14:52:07.203654 twitter_api_py-0.3.2/twitter_api/types/pagination_token.py
--rw-r--r--   0        0        0     3529 2023-05-02 14:56:28.715783 twitter_api_py-0.3.2/twitter_api/types/paging.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      337 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      201 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       64 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      594 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0      331 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_event/dm_event_expansion.py
--rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_event/dm_event_field.py
--rw-r--r--   0        0        0       57 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      238 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_dm_event/dm_event_type.py
--rw-r--r--   0        0        0      315 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_domain.py
--rw-r--r--   0        0        0      248 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_entity.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      209 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_geo/geo.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1356 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media.py
--rw-r--r--   0        0        0      570 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       56 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      635 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_place/place.py
--rw-r--r--   0        0        0      348 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       94 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_place/place_id.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      593 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      272 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      392 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      913 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      246 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      254 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      352 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      311 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       55 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_scope.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     6434 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      229 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      313 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0      632 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_expansion.py
--rw-r--r--   0        0        0     1910 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      256 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     7049 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      387 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      969 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/user.py
--rw-r--r--   0        0        0      157 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/user_expantion.py
--rw-r--r--   0        0        0      608 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/user_id.py
--rw-r--r--   0        0        0       97 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/user_verified_type.py
--rw-r--r--   0        0        0      128 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/types/v2_user/username.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.3.2/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-04-23 15:17:02.699271 twitter_api_py-0.3.2/twitter_api/utils/_datetime.py
--rw-r--r--   0        0        0      716 2023-04-27 14:28:44.162902 twitter_api_py-0.3.2/twitter_api/utils/_functional.py
--rw-r--r--   0        0        0      904 2023-04-25 11:39:31.648198 twitter_api_py-0.3.2/twitter_api/utils/_oauth.py
--rw-r--r--   0        0        0      775 2023-05-01 04:02:26.399958 twitter_api_py-0.3.2/twitter_api/utils/json.py
--rw-r--r--   0        0        0      630 2023-05-02 14:52:07.213654 twitter_api_py-0.3.2/twitter_api/warning.py
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 twitter_api_py-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-01 07:19:33.892883 twitter_api_py-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2126 2023-05-02 15:01:57.648446 twitter_api_py-0.3.3/README.md
+-rw-r--r--   0        0        0     1516 2023-05-02 17:57:54.763964 twitter_api_py-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-02 15:47:39.640660 twitter_api_py-0.3.3/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-01 05:03:58.580612 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      310 2023-05-01 05:01:04.629161 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0     1386 2023-05-01 15:37:14.131307 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      305 2023-05-01 05:01:45.139500 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      806 2023-05-01 05:02:17.969774 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      314 2023-05-01 05:02:27.359852 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0     1209 2023-05-01 05:02:59.990124 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      310 2023-05-01 05:03:15.690255 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      829 2023-05-01 05:03:36.810430 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      305 2023-05-01 05:03:51.400552 twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.3.3/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      364 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      450 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      792 2023-05-02 16:12:13.062596 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      432 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      391 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      500 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      750 2023-05-02 16:12:03.602519 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      647 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      375 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1792 2023-05-02 16:41:17.966730 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     3884 2023-05-02 17:57:16.613654 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1325 2023-05-02 16:41:04.896624 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1560 2023-05-02 16:43:35.267843 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3396 2023-05-02 16:43:15.727684 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0      866 2023-05-02 16:43:44.697919 twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.3.3/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-24 12:44:19.060255 twitter_api_py-0.3.3/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.3.3/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5182 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1967 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3368 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7253 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    14518 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14743 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32062 2023-05-02 16:44:11.348135 twitter_api_py-0.3.3/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    26895 2023-05-02 15:47:39.640660 twitter_api_py-0.3.3/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13583 2023-05-02 16:40:53.436531 twitter_api_py-0.3.3/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    10588 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.3.3/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-01 15:29:32.247704 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0     2232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0      976 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
+-rw-r--r--   0        0        0     3316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
+-rw-r--r--   0        0        0      705 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit_info.py
+-rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit_target.py
+-rw-r--r--   0        0        0      281 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      541 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      441 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      673 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8906 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      676 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2390 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3088 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      458 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6560 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     2977 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2926 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     5900 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     5999 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-02 15:14:15.304418 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      770 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3096 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      275 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      371 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6509 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      376 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      391 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7930 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      367 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      331 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8343 2023-05-02 14:54:51.834995 twitter_api_py-0.3.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      279 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      299 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2755 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      396 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3025 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.3.3/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.3.3/twitter_api/types/chainable.py
+-rw-r--r--   0        0        0      697 2023-04-26 11:13:40.460129 twitter_api_py-0.3.3/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.3.3/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1580 2023-05-02 17:35:22.073007 twitter_api_py-0.3.3/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      570 2023-05-02 15:47:39.640660 twitter_api_py-0.3.3/twitter_api/types/generic_client.py
+-rw-r--r--   0        0        0      616 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/types/http.py
+-rw-r--r--   0        0        0      734 2023-04-30 18:08:45.644350 twitter_api_py-0.3.3/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.3.3/twitter_api/types/model.py
+-rw-r--r--   0        0        0     1942 2023-05-01 15:41:37.413361 twitter_api_py-0.3.3/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-02 17:48:22.619331 twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     3473 2023-05-02 16:25:30.009051 twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0     1974 2023-05-02 17:51:03.780634 twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     3592 2023-05-02 16:26:12.579396 twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       63 2023-05-02 14:52:07.203654 twitter_api_py-0.3.3/twitter_api/types/pagination_token.py
+-rw-r--r--   0        0        0     3529 2023-05-02 14:56:28.715783 twitter_api_py-0.3.3/twitter_api/types/paging.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      201 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       64 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      594 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       57 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      238 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      315 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_domain.py
+-rw-r--r--   0        0        0      248 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_entity.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media.py
+-rw-r--r--   0        0        0      570 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       56 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      635 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/place.py
+-rw-r--r--   0        0        0      348 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       94 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      272 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      392 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      913 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      246 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      254 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      352 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       55 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     6434 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      229 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      313 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      632 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1910 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      256 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     7049 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      387 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user.py
+-rw-r--r--   0        0        0      157 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      608 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0       97 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      128 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.3.3/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-23 15:17:02.699271 twitter_api_py-0.3.3/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-04-27 14:28:44.162902 twitter_api_py-0.3.3/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-04-25 11:39:31.648198 twitter_api_py-0.3.3/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      775 2023-05-01 04:02:26.399958 twitter_api_py-0.3.3/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      630 2023-05-02 14:52:07.213654 twitter_api_py-0.3.3/twitter_api/warning.py
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 twitter_api_py-0.3.3/PKG-INFO
```

### Comparing `twitter_api_py-0.3.2/LICENSE` & `twitter_api_py-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/README.md` & `twitter_api_py-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/pyproject.toml` & `twitter_api_py-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
 packages = [{include = "twitter_api"}]
 readme = "README.md"
-version = "0.3.2"
+version = "0.3.3"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/session_resources.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/session_resources.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,12 +44,9 @@
         from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
         return OAuth1AccessToken(
             oauth_token="oauth_token",
             oauth_token_secret="oauth_token_secret",
             user_id="user_id",
             screen_name="screen_name",
-            _session=self,
+            _client_generator=self._client_generator,
         )
-
-    def generate_client(self, access_token: AccessToken, access_secret: AccessSecret):
-        return self._client_generator(access_token, access_secret)
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth1_real_session.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,9 @@
         self._session.close()
 
         return OAuth1AccessToken(
             oauth_token=data["oauth_token"],
             oauth_token_secret=data["oauth_token_secret"],
             user_id=data["user_id"],
             screen_name=data["screen_name"],
-            _session=self,
+            _client_generator=self._client_generator,
         )
-
-    def generate_client(
-        self, access_token: AccessToken, access_secret: AccessSecret
-    ) -> TwitterApiGenericClient:
-        return self._client_generator(access_token, access_secret)
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from typing import Generic
 
 from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.http import Url
-from twitter_api.types.oauth import AccessSecret, AccessToken, CallbackUrl
+from twitter_api.types.oauth import CallbackUrl
 
 
 class TwitterOAuth1Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
     @abstractmethod
     def request_token(self):
         from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
             TwitterOAuth1AuthorizeClient,
@@ -36,13 +36,7 @@
         # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
         #       偽のデータを作っている。
         from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
         _: OAuth1AccessToken[TwitterApiGenericClient] = ...  # type: ignore
 
         return _
-
-    @abstractmethod
-    def generate_client(
-        self, access_token: AccessToken, access_secret: AccessSecret
-    ) -> TwitterApiGenericClient:
-        ...
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,12 +37,9 @@
         expires_in = 7200
         return OAuth2AccessToken(
             token_type="bearer",
             expires_in=expires_in,
             expires_at=int(datetime.now().timestamp()) + expires_in,
             access_token="access_token",
             scope=self._scope,
-            _session=self,
+            _client_generator=self._client_generator,
         )
-
-    def generate_client(self, access_token: AccessToken):
-        return self._client_generator(access_token)
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth2_real_session.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,13 +84,10 @@
         scope: Any = response.pop("scope", "").split(" ")
 
         # 認証のプロセスがすべて終了したので、コネクションを閉じておく。
         self._session.close()
 
         return OAuth2AccessToken(
             scope=scope,
-            _session=self,
+            _client_generator=self._client_generator,
             **response,
         )
-
-    def generate_client(self, access_token: AccessToken) -> TwitterApiGenericClient:
-        return self._client_generator(access_token)
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/oauth_session/twitter_oauth2_session.py` & `twitter_api_py-0.3.3/twitter_api/client/oauth_session/twitter_oauth2_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABCMeta, abstractmethod
 from typing import Generic
 
 from twitter_api.types.generic_client import TwitterApiGenericClient
-from twitter_api.types.oauth import AccessToken, CallbackUrl
+from twitter_api.types.oauth import CallbackUrl
 
 
 class TwitterOAuth2Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
     @abstractmethod
     def generate_authorization_url(
         self,
     ):
@@ -24,11 +24,7 @@
         code_verifier: str,
     ):
         from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 
         _: OAuth2AccessToken[TwitterApiGenericClient] = ...  # type: ignore
 
         return _
-
-    @abstractmethod
-    def generate_client(self, access_token: AccessToken) -> TwitterApiGenericClient:
-        ...
```

### Comparing `twitter_api_py-0.3.2/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.3.3/twitter_api/client/request/request_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.3.3/twitter_api/client/request/request_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/request/request_client.py` & `twitter_api_py-0.3.3/twitter_api/client/request/request_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.3.3/twitter_api/client/request/request_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.3.3/twitter_api/client/request/request_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/twitter_api_async_client.py` & `twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/twitter_api_async_mock_client.py` & `twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/twitter_api_async_real_client.py` & `twitter_api_py-0.3.3/twitter_api/client/twitter_api_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/twitter_api_client.py` & `twitter_api_py-0.3.3/twitter_api/client/twitter_api_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/twitter_api_mock_client.py` & `twitter_api_py-0.3.3/twitter_api/client/twitter_api_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/client/twitter_api_real_client.py` & `twitter_api_py-0.3.3/twitter_api/client/twitter_api_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/error.py` & `twitter_api_py-0.3.3/twitter_api/error.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/__init__.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.3.3/twitter_api/rate_limit/rate_limit.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.3.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.3.3/twitter_api/resources/oauth2_token/post_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweet/get_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/get_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets/post_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_user/get_v2_user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_user_following/post_v2_user_following.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_users/get_v2_users.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_users_by/get_v2_users_by.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_users_by/get_v2_users_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py` & `twitter_api_py-0.3.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.3.3/twitter_api/types/comma_separatable.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.3.3/twitter_api/types/extra_permissive_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/generic_client.py` & `twitter_api_py-0.3.3/twitter_api/types/generic_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/http.py` & `twitter_api_py-0.3.3/twitter_api/types/http.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/httpx.py` & `twitter_api_py-0.3.3/twitter_api/types/httpx.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/model.py` & `twitter_api_py-0.3.3/twitter_api/types/model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/oauth.py` & `twitter_api_py-0.3.3/twitter_api/types/oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.3.3/twitter_api/types/oauth1/oauth1_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.3.3/twitter_api/types/oauth2/oauth2_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/paging.py` & `twitter_api_py-0.3.3/twitter_api/types/paging.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_media/media.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_media/media.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_media/media_field.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_place/place.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_place/place.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_poll/poll.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_poll/poll.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_retweet/retweet_entities_description.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_scope.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_expansion.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_expansion.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_tweet/tweet_response_body.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_user/user.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_user/user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/types/v2_user/user_field.py` & `twitter_api_py-0.3.3/twitter_api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/utils/_functional.py` & `twitter_api_py-0.3.3/twitter_api/utils/_functional.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/utils/_oauth.py` & `twitter_api_py-0.3.3/twitter_api/utils/_oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/utils/json.py` & `twitter_api_py-0.3.3/twitter_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/twitter_api/warning.py` & `twitter_api_py-0.3.3/twitter_api/warning.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.3.2/PKG-INFO` & `twitter_api_py-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.3.2
+Version: 0.3.3
 Summary: Twitter API Client by Typed Python.
 Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

