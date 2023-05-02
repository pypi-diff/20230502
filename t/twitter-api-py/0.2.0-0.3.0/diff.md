# Comparing `tmp/twitter_api_py-0.2.0.tar.gz` & `tmp/twitter_api_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.2.0.tar", max compression
+gzip compressed data, was "twitter_api_py-0.3.0.tar", max compression
```

## Comparing `twitter_api_py-0.2.0.tar` & `twitter_api_py-0.3.0.tar`

### file list

```diff
@@ -1,218 +1,216 @@
--rw-r--r--   0        0        0     2159 2023-04-26 11:13:09.330123 twitter_api_py-0.2.0/README.md
--rw-r--r--   0        0        0     1516 2023-05-01 05:35:27.146293 twitter_api_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      480 2023-05-01 05:34:09.265632 twitter_api_py-0.2.0/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:09.975602 twitter_api_py-0.2.0/twitter_api/api/__init__.py
--rw-r--r--   0        0        0      281 2023-04-22 04:51:08.637342 twitter_api_py-0.2.0/twitter_api/api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2299 2023-04-24 16:07:45.386094 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-24 16:08:44.345977 twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      541 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-24 16:07:45.566094 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      441 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      673 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
--rw-r--r--   0        0        0     8955 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
--rw-r--r--   0        0        0      676 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/__init__.py
--rw-r--r--   0        0        0     2410 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
--rw-r--r--   0        0        0      429 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-24 12:44:19.060255 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3128 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      458 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6593 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     3017 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2954 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      438 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     5944 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      471 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     6043 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      471 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     3522 2023-04-27 14:28:44.152903 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      770 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2123 2023-04-24 16:07:45.546094 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3099 2023-04-24 16:07:45.616093 twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      275 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2812 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      371 2023-04-22 10:21:01.801508 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6542 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      376 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-24 16:07:45.656093 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      391 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7987 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      367 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1927 2023-04-24 16:07:45.706093 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      331 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8404 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      279 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2712 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0      299 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by/get_v2_users_by.py
--rw-r--r--   0        0        0      396 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by_username/__init__.py
--rw-r--r--   0        0        0     3057 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by_username/get_v2_users_by_username.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.025603 twitter_api_py-0.2.0/twitter_api/api/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 17:04:18.882718 twitter_api_py-0.2.0/twitter_api/api/types/oauth1/__init__.py
--rw-r--r--   0        0        0      843 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     2825 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.323030 twitter_api_py-0.2.0/twitter_api/api/types/oauth2/__init__.py
--rw-r--r--   0        0        0      856 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     2855 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       63 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/pagination_token.py
--rw-r--r--   0        0        0        0 2023-04-04 00:14:28.746398 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      345 2023-04-09 09:46:44.353033 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      205 2023-04-04 14:28:03.516388 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       64 2023-04-04 00:15:15.770562 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      598 2023-04-05 12:42:42.545017 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-04-04 00:15:59.434445 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0      331 2023-04-25 14:01:08.860602 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_expansion.py
--rw-r--r--   0        0        0      437 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_field.py
--rw-r--r--   0        0        0       57 2023-04-04 00:16:14.175754 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      238 2023-04-25 13:49:11.742866 twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_event/dm_event_type.py
--rw-r--r--   0        0        0      315 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_domain.py
--rw-r--r--   0        0        0      248 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_entity.py
--rw-r--r--   0        0        0        0 2023-04-15 05:54:42.060789 twitter_api_py-0.2.0/twitter_api/api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      209 2023-04-15 05:55:44.170800 twitter_api_py-0.2.0/twitter_api/api/types/v2_geo/geo.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.035603 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1389 2023-04-15 06:07:09.620870 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media.py
--rw-r--r--   0        0        0      570 2023-04-15 15:58:56.812733 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      100 2023-04-01 16:14:08.728923 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       56 2023-04-01 09:17:10.035603 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-04-15 06:00:40.800828 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-04-15 06:02:11.910834 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-04-15 06:03:23.150843 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-04-15 06:04:09.220847 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-04-15 06:06:05.030862 twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.035603 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      643 2023-04-15 05:56:35.000801 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place.py
--rw-r--r--   0        0        0      348 2023-04-15 15:58:30.892600 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       94 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place_id.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      601 2023-04-15 06:10:52.180889 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      272 2023-04-15 15:58:36.582629 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       54 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-04-15 06:09:28.320883 twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-04-02 02:04:07.967716 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-04 14:56:44.417296 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      400 2023-04-04 14:28:04.506389 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      929 2023-04-04 14:28:04.676389 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      184 2023-04-24 13:31:22.645664 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      184 2023-04-23 16:29:08.693648 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      250 2023-04-04 14:57:14.027308 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-04-02 02:13:19.847028 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-04-02 02:10:33.754809 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      258 2023-04-10 15:48:58.984612 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-04-02 02:26:55.269961 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      352 2023-04-02 02:04:56.864520 twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:44.373033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      319 2023-04-09 09:46:44.433033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       54 2023-04-09 09:46:44.373033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       55 2023-04-09 09:46:44.433033 twitter_api_py-0.2.0/twitter_api/api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-04-23 06:01:36.209583 twitter_api_py-0.2.0/twitter_api/api/types/v2_scope.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.045603 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     6442 2023-04-18 13:43:34.885017 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-04-04 14:19:50.365994 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      229 2023-04-04 14:30:09.146468 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-04-01 09:17:36.515599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      317 2023-04-04 14:57:19.327310 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-04-15 03:52:45.757502 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0      632 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_expansion.py
--rw-r--r--   0        0        0     1910 2023-04-23 06:33:19.778673 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-04-01 09:17:37.035599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0      100 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-04-01 09:17:37.035599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-04-01 09:17:36.415599 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-04-09 15:28:28.034225 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      256 2023-04-15 10:39:45.485596 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     6983 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      387 2023-04-02 01:59:57.044158 twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.065603 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      977 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user.py
--rw-r--r--   0        0        0      157 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_expantion.py
--rw-r--r--   0        0        0      608 2023-04-15 16:00:19.963155 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       54 2023-04-01 09:17:10.065603 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_id.py
--rw-r--r--   0        0        0       97 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_verified_type.py
--rw-r--r--   0        0        0      128 2023-04-02 07:41:55.232378 twitter_api_py-0.2.0/twitter_api/api/types/v2_user/username.py
--rw-r--r--   0        0        0        0 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     1039 2023-05-01 05:03:58.580612 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0      310 2023-05-01 05:01:04.629161 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
--rw-r--r--   0        0        0     1380 2023-05-01 05:01:51.409552 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      305 2023-05-01 05:01:45.139500 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
--rw-r--r--   0        0        0      806 2023-05-01 05:02:17.969774 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0      314 2023-05-01 05:02:27.359852 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
--rw-r--r--   0        0        0     1209 2023-05-01 05:02:59.990124 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      310 2023-05-01 05:03:15.690255 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
--rw-r--r--   0        0        0      829 2023-05-01 05:03:36.810430 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0      305 2023-05-01 05:03:51.400552 twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.2.0/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      364 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0     1143 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      450 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      801 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      432 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      721 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      391 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      797 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      500 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      759 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      647 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      375 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1599 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0     1940 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     4048 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1546 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0     1681 2023-05-01 04:37:46.697568 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     3519 2023-04-30 18:13:50.196233 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0     1030 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.2.0/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-24 12:44:19.060255 twitter_api_py-0.2.0/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.2.0/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5357 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1973 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3316 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     7427 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    32408 2023-05-01 04:10:39.294049 twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0    14522 2023-05-01 05:15:05.866148 twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0    14747 2023-05-01 04:55:52.126573 twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    32167 2023-05-01 05:09:26.123325 twitter_api_py-0.2.0/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    27102 2023-05-01 05:11:36.014406 twitter_api_py-0.2.0/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0    13587 2023-05-01 04:54:04.605683 twitter_api_py-0.2.0/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    10799 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.2.0/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0      410 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0      525 2023-04-23 01:32:37.383610 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
--rw-r--r--   0        0        0     3040 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
--rw-r--r--   0        0        0      675 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1242 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3424 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0        0 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/types/__init__.py
--rw-r--r--   0        0        0      297 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/types/rate_limit_info.py
--rw-r--r--   0        0        0       91 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/rate_limit/types/rate_limit_target.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.2.0/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.2.0/twitter_api/types/chainable.py
--rw-r--r--   0        0        0      697 2023-04-26 11:13:40.460129 twitter_api_py-0.2.0/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.2.0/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1580 2023-04-24 17:04:45.312148 twitter_api_py-0.2.0/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      570 2023-04-30 18:19:53.998491 twitter_api_py-0.2.0/twitter_api/types/generic_client.py
--rw-r--r--   0        0        0      616 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/types/http.py
--rw-r--r--   0        0        0      734 2023-04-30 18:08:45.644350 twitter_api_py-0.2.0/twitter_api/types/httpx.py
--rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.2.0/twitter_api/types/model.py
--rw-r--r--   0        0        0     1742 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/types/oauth.py
--rw-r--r--   0        0        0     3531 2023-04-30 17:48:26.846710 twitter_api_py-0.2.0/twitter_api/types/paging.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.2.0/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-04-23 15:17:02.699271 twitter_api_py-0.2.0/twitter_api/utils/_datetime.py
--rw-r--r--   0        0        0      716 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/utils/_functional.py
--rw-r--r--   0        0        0      904 2023-04-25 11:39:31.648198 twitter_api_py-0.2.0/twitter_api/utils/_oauth.py
--rw-r--r--   0        0        0      775 2023-05-01 04:02:26.399958 twitter_api_py-0.2.0/twitter_api/utils/json.py
--rw-r--r--   0        0        0      637 2023-04-27 14:28:44.162902 twitter_api_py-0.2.0/twitter_api/warning.py
--rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 twitter_api_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-01 07:19:33.892883 twitter_api_py-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2180 2023-05-01 15:19:44.023115 twitter_api_py-0.3.0/README.md
+-rw-r--r--   0        0        0     1516 2023-05-02 15:00:14.117603 twitter_api_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-01 05:34:09.265632 twitter_api_py-0.3.0/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-01 05:03:58.580612 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      310 2023-05-01 05:01:04.629161 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0     1386 2023-05-01 15:37:14.131307 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      305 2023-05-01 05:01:45.139500 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      806 2023-05-01 05:02:17.969774 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      314 2023-05-01 05:02:27.359852 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0     1209 2023-05-01 05:02:59.990124 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      310 2023-05-01 05:03:15.690255 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      829 2023-05-01 05:03:36.810430 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      305 2023-05-01 05:03:51.400552 twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.3.0/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      364 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      450 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      801 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      432 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      391 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      500 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      759 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      647 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      375 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1920 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     4053 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1513 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1644 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3507 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0      997 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.3.0/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-24 12:44:19.060255 twitter_api_py-0.3.0/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.3.0/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5182 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1967 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3368 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7253 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    14518 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14743 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32062 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    26895 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13583 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    10588 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.3.0/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-01 15:29:32.247704 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0     2232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0      976 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/handlers/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
+-rw-r--r--   0        0        0     3316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
+-rw-r--r--   0        0        0      705 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1232 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3303 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/rate_limit_info.py
+-rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/rate_limit/rate_limit_target.py
+-rw-r--r--   0        0        0      281 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      541 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2316 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      441 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      673 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8906 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      676 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2390 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3088 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      458 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6560 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     2977 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2926 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      438 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     5900 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     5999 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      471 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3486 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      770 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3096 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      275 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      371 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6509 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      376 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      391 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7930 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      367 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      331 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8343 2023-05-02 14:54:51.834995 twitter_api_py-0.3.0/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      279 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      299 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2755 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      396 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3025 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.3.0/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-09 09:46:11.323030 twitter_api_py-0.3.0/twitter_api/types/chainable.py
+-rw-r--r--   0        0        0      697 2023-04-26 11:13:40.460129 twitter_api_py-0.3.0/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.3.0/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1580 2023-04-24 17:04:45.312148 twitter_api_py-0.3.0/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      570 2023-04-30 18:19:53.998491 twitter_api_py-0.3.0/twitter_api/types/generic_client.py
+-rw-r--r--   0        0        0      616 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/types/http.py
+-rw-r--r--   0        0        0      734 2023-04-30 18:08:45.644350 twitter_api_py-0.3.0/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     2362 2023-04-20 12:43:51.415589 twitter_api_py-0.3.0/twitter_api/types/model.py
+-rw-r--r--   0        0        0     1942 2023-05-01 15:41:37.413361 twitter_api_py-0.3.0/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0      839 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     2825 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0      852 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     2855 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       63 2023-05-02 14:52:07.203654 twitter_api_py-0.3.0/twitter_api/types/pagination_token.py
+-rw-r--r--   0        0        0     3529 2023-05-02 14:56:28.715783 twitter_api_py-0.3.0/twitter_api/types/paging.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      201 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       64 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      594 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       57 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      238 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      315 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_domain.py
+-rw-r--r--   0        0        0      248 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_entity.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media.py
+-rw-r--r--   0        0        0      570 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       56 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      635 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_place/place.py
+-rw-r--r--   0        0        0      348 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       94 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      272 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      392 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      913 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      184 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      246 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      254 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      352 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       55 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     6434 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      229 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      313 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      632 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1910 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      100 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      256 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     7049 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      387 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/user.py
+-rw-r--r--   0        0        0      157 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      608 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       54 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0       97 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      128 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.3.0/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-23 15:17:02.699271 twitter_api_py-0.3.0/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-04-27 14:28:44.162902 twitter_api_py-0.3.0/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-04-25 11:39:31.648198 twitter_api_py-0.3.0/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      775 2023-05-01 04:02:26.399958 twitter_api_py-0.3.0/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      630 2023-05-02 14:52:07.213654 twitter_api_py-0.3.0/twitter_api/warning.py
+-rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 twitter_api_py-0.3.0/PKG-INFO
```

### Comparing `twitter_api_py-0.2.0/README.md` & `twitter_api_py-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,29 +29,30 @@
 The simplest way to use the library is as follows:
 
 ```python
 from twitter_api import TwitterApiClient
 
 with TwitterApiClient.from_oauth2_app_env() as twitter_client:
     response_body = (
-        twitter_client.request("https://api.twitter.com/2/tweets")
+        twitter_client.chain()
+        .request("https://api.twitter.com/2/tweets")
         .get({
             "ids": "1460323737035677698",
             "expansions": ["referenced_tweets.id"]
         })
     )
 ```
 
 As a characteristic feature of the library, it explicitly prompts the user to write the Endpoint URL, which makes it clear from the source code which Twitter API is being called.
 
 ## Test Code
 
 A mock client is provided by the library to simplify the writing of test code.
 
-This client has the same interface as TwitterApiClient/TwitterApiAsyncClient, and also provides methods (`inject_*_response_body`) for injecting test data.
+This client has the same interface as `TwitterApiClient`/`TwitterApiAsyncClient`, and also provides methods (`inject_*_response_body`) for injecting test data.
 
 ```python
 from twitter_api import TwitterApiClient
 from twitter_api.client.twitter_api_mock_client import TwitterApiMockClient
 
 def your_logic(twitter_client: TwitterApiClient):
     ...
```

### Comparing `twitter_api_py-0.2.0/pyproject.toml` & `twitter_api_py-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
 packages = [{include = "twitter_api"}]
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.3.0/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 from typing import TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
 from twitter_api.error import TwitterApiOAuthVersionWrong
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
 from twitter_api.types.oauth import AccessToken, ApiKey, ApiSecret
 
 ENDPOINT: Endpoint = Endpoint("POST", "https://api.twitter.com/oauth2/invalidate_token")
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.3.0/twitter_api/resources/oauth2_token/post_oauth2_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 from typing import Literal, TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
 from twitter_api.error import TwitterApiOAuthVersionWrong
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
 from twitter_api.types.oauth import AccessToken, ApiKey, ApiSecret
 
 ENDPOINT: Endpoint = Endpoint("POST", "https://api.twitter.com/oauth2/token")
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_dm_conversation.dm_conversation import DmConversation
-from twitter_api.api.types.v2_dm_conversation.dm_conversation_id import DmConversationId
-from twitter_api.api.types.v2_dm_conversation.dm_conversation_message import (
-    DmConversationMessage,
-)
-from twitter_api.api.types.v2_scope import oauth2_scopes
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_dm_conversation.dm_conversation import DmConversation
+from twitter_api.types.v2_dm_conversation.dm_conversation_id import DmConversationId
+from twitter_api.types.v2_dm_conversation.dm_conversation_message import (
+    DmConversationMessage,
+)
+from twitter_api.types.v2_scope import oauth2_scopes
 
 ENDPOINT = Endpoint(
     "POST", "https://api.twitter.com/2/dm_conversations/:dm_conversation_id/messages"
 )
 
 
 PostV2DmConversationMessagesRequestBody = DmConversationMessage
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Literal, TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_dm_conversation.dm_conversation import DmConversation
-from twitter_api.api.types.v2_dm_conversation.dm_conversation_message import (
-    DmConversationMessage,
-)
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_dm_conversation.dm_conversation import DmConversation
+from twitter_api.types.v2_dm_conversation.dm_conversation_message import (
+    DmConversationMessage,
+)
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/dm_conversations")
 
 
 PostV2DmConversationsRequestBody = TypedDict(
     "PostV2DmConversationsRequestBody",
     {
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from datetime import datetime
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_dm_conversation.dm_conversation_id import DmConversationId
-from twitter_api.api.types.v2_dm_event.dm_event_expansion import DmEventExpansion
-from twitter_api.api.types.v2_dm_event.dm_event_field import DmEventField
-from twitter_api.api.types.v2_dm_event.dm_event_id import DmEventId
-from twitter_api.api.types.v2_dm_event.dm_event_type import DmEventType
-from twitter_api.api.types.v2_media.media_key import MediaKey
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_dm_conversation.dm_conversation_id import DmConversationId
+from twitter_api.types.v2_dm_event.dm_event_expansion import DmEventExpansion
+from twitter_api.types.v2_dm_event.dm_event_field import DmEventField
+from twitter_api.types.v2_dm_event.dm_event_id import DmEventId
+from twitter_api.types.v2_dm_event.dm_event_type import DmEventType
+from twitter_api.types.v2_media.media_key import MediaKey
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint(
     "GET",
     "https://api.twitter.com/2/dm_conversations/with/:participant_id/dm_events",
 )
 
 
@@ -111,15 +111,15 @@
     meta: GetV2DmConversationsWithParticipantDmEventsResponseBodyMeta
     includes: GetV2DmConversationsWithParticipantDmEventsResponseBodyIncludes = Field(
         default_factory=GetV2DmConversationsWithParticipantDmEventsResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> PaginationToken | None:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         if self.meta is None:
             return None
 
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/__init__.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_dm_conversation.dm_conversation import DmConversation
-from twitter_api.api.types.v2_dm_conversation.dm_conversation_message import (
-    DmConversationMessage,
-)
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_dm_conversation.dm_conversation import DmConversation
+from twitter_api.types.v2_dm_conversation.dm_conversation_message import (
+    DmConversationMessage,
+)
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint(
     "POST", "https://api.twitter.com/2/dm_conversations/with/:participant_id/messages"
 )
 
 
 PostV2DmConversationsWithParticipantMessagesRequestBody = DmConversationMessage
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_id import TweetId
 
 ENDPOINT = Endpoint("DELETE", "https://api.twitter.com/2/tweets/:id")
 
 
 class DeleteV2TweetResponseBodyData(ExtraPermissiveModel):
     deleted: bool
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweet/get_v2_tweet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import NotRequired, Optional, TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_tweet.tweet_response_body import TweetResponseBody
-from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_tweet.tweet_response_body import TweetResponseBody
+from twitter_api.types.v2_user.user_field import UserField
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/:id")
 
 GetV2TweetQueryParameters = TypedDict(
     "GetV2TweetQueryParameters",
     {
         "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_retweet.retweet import Retweet
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_retweet.retweet import Retweet
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_user.user_field import UserField
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/:id/retweeted_by")
 
 GetV2TweetRetweetedByQueryParameters = TypedDict(
     "GetV2TweetRetweetedByQueryParameters",
     {
         "expansions": NotRequired[Optional[CommaSeparatable[TweetExpansion]]],
@@ -71,15 +71,15 @@
     meta: GetV2TweetRetweetedByResponseBodyMeta
     includes: GetV2TweetRetweetedByResponseBodyIncludes = Field(
         default_factory=GetV2TweetRetweetedByResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> PaginationToken | None:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.meta.extend(other.meta)
         self.includes.extend(other.includes)
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets/get_v2_tweets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import NotRequired, Optional, TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsResponseBody
-from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_tweet.tweet_response_body import TweetsResponseBody
+from twitter_api.types.v2_user.user_field import UserField
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets")
 
 GetV2TweetsQueryParameters = TypedDict(
     "GetV2TweetsQueryParameters",
     {
         "ids": CommaSeparatable[TweetId],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets/post_v2_tweets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Literal, NotRequired, Optional, TypedDict, Union
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_media.media_id import MediaId
-from twitter_api.api.types.v2_place.place_id import PlaceId
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import Url, downcast_dict
+from twitter_api.types.v2_media.media_id import MediaId
+from twitter_api.types.v2_place.place_id import PlaceId
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/tweets")
 
 
 class PostV2TweetsGeospatialInformation(TypedDict):
     place_id: PlaceId
     tagged_user_ids: UserId
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from datetime import datetime
 from typing import AsyncGenerator, Generator, Literal, NotRequired, Optional, TypedDict
 from urllib import parse
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
-from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
+from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.utils._datetime import rfc3339
 from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/all")
 
 GetV2TweetsSearchAllQueryParameters = TypedDict(
     "GetV2TweetsSearchAllQueryParameters",
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from datetime import datetime
 from typing import AsyncGenerator, Generator, Literal, NotRequired, Optional, TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
-from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
+from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.utils._datetime import rfc3339
 from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/recent")
 
 GetV2TweetsSearchRecentQueryParameters = TypedDict(
     "GetV2TweetsSearchRecentQueryParameters",
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
 from typing import NotRequired, Optional, TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_expansion import TweetExpansion
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
-from twitter_api.api.types.v2_user.user_field import UserField
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_expansion import TweetExpansion
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_response_body import TweetsSearchResponseBody
+from twitter_api.types.v2_user.user_field import UserField
 from twitter_api.utils._datetime import rfc3339
 from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/stream")
 
 GetV2TweetsSearchStreamQueryParameters = TypedDict(
     "GetV2TweetsSearchStreamQueryParameters",
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import datetime
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_rule.rule import Rule
-from twitter_api.api.types.v2_rule.rule_id import RuleId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_rule.rule import Rule
+from twitter_api.types.v2_rule.rule_id import RuleId
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/tweets/search/stream/rules")
 
 GetV2TweetsSearchStreamRulesQueryParameters = TypedDict(
     "GetV2TweetsSearchStreamRulesQueryParameters",
     {
         "ids": NotRequired[Optional[list[RuleId]]],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from datetime import datetime
-from typing import NotRequired, Optional, TypedDict
+from typing import NotRequired, Optional, TypedDict, Union
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_rule.rule import Rule
-from twitter_api.api.types.v2_rule.rule_id import RuleId
-from twitter_api.api.types.v2_rule.rule_tag import RuleTag
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_rule.rule import Rule
+from twitter_api.types.v2_rule.rule_id import RuleId
+from twitter_api.types.v2_rule.rule_tag import RuleTag
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/tweets/search/stream/rules")
 
 PostV2TweetsSearchStreamRulesQueryParameters = TypedDict(
     "PostV2TweetsSearchStreamRulesQueryParameters",
     {
         "dry_run": NotRequired[Optional[bool]],
@@ -31,15 +31,15 @@
     ids: list[RuleId]
 
 
 class DeleteDataByValues(TypedDict):
     values: list[str]
 
 
-DeleteData = DeleteDataByIds | DeleteDataByValues
+DeleteData = Union[DeleteDataByIds, DeleteDataByValues]
 
 
 class PostV2TweetsSearchStreamRulesRequestBody(TypedDict):
     add: NotRequired[list[AddData]]
     delete: NotRequired[Optional[DeleteData]]
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_user/get_v2_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id")
 
 GetV2UserQueryParameters = TypedDict(
     "GetV2UserQueryParameters",
     {
         "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/followers")
 
 GetV2UserFollowersQueryParameters = TypedDict(
     "GetV2UserFollowersQueryParameters",
     {
         "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
@@ -71,15 +71,15 @@
     meta: GetV2UserFollowersResponseBodyMeta
     includes: GetV2UserFollowersResponseBodyIncludes = Field(
         default_factory=GetV2UserFollowersResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> PaginationToken | None:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.meta.extend(other.meta)
         self.includes.extend(other.includes)
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_user_following/post_v2_user_following.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/users/:id/following")
 
 PostV2UserFollowingRequestBody = TypedDict(
     "PostV2UserFollowingRequestBody",
     {
         "target_user_id": UserId,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from functools import partial
 from typing import AsyncGenerator, Generator, NotRequired, Optional, Self, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_media.media import Media
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place import Place
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll import Poll
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_media.media import Media
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place import Place
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll import Poll
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/liked_tweets")
 
 GetV2UserLikedTweetsQueryParameters = TypedDict(
     "GetV2UserLikedTweetsQueryParameters",
     {
         "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
@@ -91,15 +91,15 @@
     meta: Optional[GetV2UserLikedTweetsResponseBodyMeta] = None
     includes: GetV2UserLikedTweetsResponseBodyIncludes = Field(
         default_factory=GetV2UserLikedTweetsResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> PaginationToken | None:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         if self.meta is None:
             return None
 
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import TypedDict
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import downcast_dict
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/users/:id/retweets")
 
 PostV2UserRetweetsRequestBody = TypedDict(
     "PostV2UserRetweetsRequestBody",
     {
         "tweet_id": TweetId,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_user_tweets/get_v2_user_tweets.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,41 +8,41 @@
     Optional,
     Self,
     TypedDict,
 )
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_media.media import Media
-from twitter_api.api.types.v2_media.media_field import MediaField
-from twitter_api.api.types.v2_place.place import Place
-from twitter_api.api.types.v2_place.place_field import PlaceField
-from twitter_api.api.types.v2_poll.poll import Poll
-from twitter_api.api.types.v2_poll.poll_field import PollField
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import (
     PageResponseBody,
     get_collected_paging_response_body_async,
     get_collected_paging_response_body_sync,
     get_paging_response_body_iter_async,
     get_paging_response_body_iter_sync,
 )
+from twitter_api.types.v2_media.media import Media
+from twitter_api.types.v2_media.media_field import MediaField
+from twitter_api.types.v2_place.place import Place
+from twitter_api.types.v2_place.place_field import PlaceField
+from twitter_api.types.v2_poll.poll import Poll
+from twitter_api.types.v2_poll.poll_field import PollField
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.user_id import UserId
 from twitter_api.utils._datetime import rfc3339
 from twitter_api.utils._functional import map_optional
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/:id/tweets")
 
 GetV2UserTweetsQueryParameters = TypedDict(
     "GetV2UserTweetsQueryParameters",
@@ -115,15 +115,15 @@
     includes: GetV2UserTweetsResponseBodyIncludes = Field(
         default_factory=GetV2UserTweetsResponseBodyIncludes,
     )
     meta: GetV2UserTweetsResponseBodyMeta
     errors: Optional[list[dict]] = None
 
     @property
-    def meta_next_token(self) -> PaginationToken | None:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.meta.extend(other.meta)
         self.includes.extend(other.includes)
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_users/get_v2_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.user_id import UserId
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users")
 
 GetV2UsersQueryParameters = TypedDict(
     "GetV2UsersQueryParameters",
     {
         "ids": CommaSeparatable[UserId],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by/get_v2_users_by.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_users_by/get_v2_users_by.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.username import Username
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.username import Username
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/by")
 
 GetV2UsersByQueryParameters = TypedDict(
     "GetV2UsersByQueryParameters",
     {
         "usernames": CommaSeparatable[Username],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/resources/v2_users_by_username/get_v2_users_by_username.py` & `twitter_api_py-0.3.0/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import NotRequired, Optional, TypedDict
 
 from pydantic import Field
 
-from twitter_api.api.resources.api_resources import ApiResources
-from twitter_api.api.types.v2_scope import oauth2_scopes
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_field import TweetField
-from twitter_api.api.types.v2_user.user import User
-from twitter_api.api.types.v2_user.user_expantion import UserExpansion
-from twitter_api.api.types.v2_user.user_field import UserField
-from twitter_api.api.types.v2_user.username import Username
 from twitter_api.rate_limit.rate_limit import rate_limit
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.comma_separatable import CommaSeparatable, comma_separated_str
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_scope import oauth2_scopes
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_field import TweetField
+from twitter_api.types.v2_user.user import User
+from twitter_api.types.v2_user.user_expantion import UserExpansion
+from twitter_api.types.v2_user.user_field import UserField
+from twitter_api.types.v2_user.username import Username
 
 ENDPOINT = Endpoint("GET", "https://api.twitter.com/2/users/by/username/:username")
 
 GetV2UsersByUsernameQueryParameters = TypedDict(
     "GetV2UsersByUsernameQueryParameters",
     {
         "expansions": NotRequired[Optional[CommaSeparatable[UserExpansion]]],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_access_token.py` & `twitter_api_py-0.3.0/twitter_api/types/oauth1/oauth1_access_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Generic
 
-from twitter_api.api.types.v2_user.user_id import UserId
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.types.chainable import Chainable
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import AccessSecret, AccessToken
+from twitter_api.types.v2_user.user_id import UserId
 
 
 class OAuth1AccessToken(
     Chainable, ExtraPermissiveModel, Generic[TwitterApiGenericClient]
 ):
     oauth_token: AccessToken
     oauth_token_secret: AccessSecret
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.3.0/twitter_api/types/oauth1/oauth1_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_access_token.py` & `twitter_api_py-0.3.0/twitter_api/types/oauth2/oauth2_access_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Generic
 
 from typing_extensions import Literal
 
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types.chainable import Chainable
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import AccessToken
+from twitter_api.types.v2_scope import Scope
 
 
 class OAuth2AccessToken(
     Chainable, ExtraPermissiveModel, Generic[TwitterApiGenericClient]
 ):
     token_type: Literal["bearer"]
     expires_in: int
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.3.0/twitter_api/types/oauth2/oauth2_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import NotRequired, Optional, TypedDict, Union
 
-from twitter_api.api.types.v2_dm_conversation.dm_conversation_attachment import (
+from twitter_api.types.v2_dm_conversation.dm_conversation_attachment import (
     DmConversationAttachment,
 )
 
 DmConversationAttachmentOnly = TypedDict(
     "DmConversationMessage",
     {
         "attachments": list[DmConversationAttachment],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_media/media.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Literal, Optional
 
-from twitter_api.api.types.v2_media.media_key import MediaKey
-from twitter_api.api.types.v2_media.media_non_public_metrics import (
-    MediaNonPublicMetrics,
-)
-from twitter_api.api.types.v2_media.media_organic_metrics import MediaOrganicMetrics
-from twitter_api.api.types.v2_media.media_promoted_metrics import MediaPromotedMetrics
-from twitter_api.api.types.v2_media.media_public_metrics import MediaPublicMetrics
-from twitter_api.api.types.v2_media.media_variants import MediaVariants
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import Url
+from twitter_api.types.v2_media.media_key import MediaKey
+from twitter_api.types.v2_media.media_non_public_metrics import MediaNonPublicMetrics
+from twitter_api.types.v2_media.media_organic_metrics import MediaOrganicMetrics
+from twitter_api.types.v2_media.media_promoted_metrics import MediaPromotedMetrics
+from twitter_api.types.v2_media.media_public_metrics import MediaPublicMetrics
+from twitter_api.types.v2_media.media_variants import MediaVariants
 
 
 class Media(ExtraPermissiveModel):
     """
     メディアの情報。
 
     refer: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/media
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_media/media_field.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_place/place.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_place/place.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Optional
 
-from twitter_api.api.types.v2_geo.geo import Geo
-from twitter_api.api.types.v2_place.place_id import PlaceId
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_geo.geo import Geo
+from twitter_api.types.v2_place.place_id import PlaceId
 
 
 class Place(ExtraPermissiveModel):
     """
     場所情報。
 
     refer: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/place
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_poll/poll.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_poll/poll.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Optional
 
-from twitter_api.api.types.v2_poll.poll_id import PollId
-from twitter_api.api.types.v2_poll.poll_option import PollOption
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_poll.poll_id import PollId
+from twitter_api.types.v2_poll.poll_option import PollOption
 
 
 class Poll(ExtraPermissiveModel):
     """
     投票情報。
 
     refer: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/poll
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from typing import Optional
 
-from twitter_api.api.types.v2_retweet.retweet_entities import RetweetEntities
-from twitter_api.api.types.v2_retweet.retweet_includes import RetweetIncludes
-from twitter_api.api.types.v2_retweet.retweet_public_metrics import RetweetPublicMetrics
-from twitter_api.api.types.v2_user.username import Username
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import Url
+from twitter_api.types.v2_retweet.retweet_entities import RetweetEntities
+from twitter_api.types.v2_retweet.retweet_includes import RetweetIncludes
+from twitter_api.types.v2_retweet.retweet_public_metrics import RetweetPublicMetrics
+from twitter_api.types.v2_user.username import Username
 
 from ..v2_tweet.tweet_id import TweetId
 from .retweet_withheld import RetweetWithheld
 
 DomainId = str
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_retweet/retweet_entities_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional
 
-from twitter_api.api.types.v2_retweet.retweet_entities_description_cashtag import (
+from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_retweet.retweet_entities_description_cashtag import (
     RetweetEntitiesDescriptionCashtag,
 )
-from twitter_api.api.types.v2_retweet.retweet_entities_description_hashtag import (
+from twitter_api.types.v2_retweet.retweet_entities_description_hashtag import (
     RetweetEntitiesDescriptionHashtag,
 )
-from twitter_api.api.types.v2_retweet.retweet_entities_description_mention import (
+from twitter_api.types.v2_retweet.retweet_entities_description_mention import (
     RetweetEntitiesDescriptionMention,
 )
-from twitter_api.api.types.v2_retweet.retweet_entities_description_url import (
+from twitter_api.types.v2_retweet.retweet_entities_description_url import (
     RetweetEntitiesDescriptionUrl,
 )
-from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 
 
 class RetweetEntitiesDescription(ExtraPermissiveModel):
     urls: Optional[list[RetweetEntitiesDescriptionUrl]] = None
     hashtags: Optional[list[RetweetEntitiesDescriptionHashtag]] = None
     mentions: Optional[list[RetweetEntitiesDescriptionMention]] = None
     cashtags: Optional[list[RetweetEntitiesDescriptionCashtag]] = None
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_scope.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import textwrap
 from datetime import datetime
 from typing import Optional
 
-from twitter_api.api.types.v2_tweet.tweet_entities_mention import TweetEntitiesMention
-from twitter_api.api.types.v2_tweet.tweet_entities_url import TweetEntitiesUrl
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.v2_tweet.tweet_entities_mention import TweetEntitiesMention
+from twitter_api.types.v2_tweet.tweet_entities_url import TweetEntitiesUrl
 
 from ..v2_user.user_id import UserId
 from .tweet_attachments import TweetAttachments
 from .tweet_context_annotation import TweetContextAnnotation
 from .tweet_edit_controls import TweetEditControls
 from .tweet_entities import TweetEntities
 from .tweet_geo import TweetGeo
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_expansion.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_expansion.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_tweet/tweet_response_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import ABCMeta, abstractmethod
-from typing import Optional, Self
+from typing import Optional, Self, Union
 
 from pydantic import Field
 
-from twitter_api.api.types.pagination_token import PaginationToken
-from twitter_api.api.types.v2_media.media import Media
-from twitter_api.api.types.v2_place.place import Place
-from twitter_api.api.types.v2_poll.poll import Poll
-from twitter_api.api.types.v2_tweet.tweet import Tweet
-from twitter_api.api.types.v2_tweet.tweet_id import TweetId
-from twitter_api.api.types.v2_user.user import User
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
+from twitter_api.types.pagination_token import PaginationToken
 from twitter_api.types.paging import PageResponseBody
+from twitter_api.types.v2_media.media import Media
+from twitter_api.types.v2_place.place import Place
+from twitter_api.types.v2_poll.poll import Poll
+from twitter_api.types.v2_tweet.tweet import Tweet
+from twitter_api.types.v2_tweet.tweet_id import TweetId
+from twitter_api.types.v2_user.user import User
 
 
 class TweetsResponseBodyIncludes(ExtraPermissiveModel):
     users: list[User] = Field(default_factory=list)
     tweets: list[Tweet] = Field(default_factory=list)
     places: list[Place] = Field(default_factory=list)
     media: list[Media] = Field(default_factory=list)
@@ -32,23 +32,25 @@
 class FindTweets(ExtraPermissiveModel, metaclass=ABCMeta):
     includes: TweetsResponseBodyIncludes = Field(
         default_factory=TweetsResponseBodyIncludes,
     )
     errors: Optional[list[dict]] = None
 
     @abstractmethod
-    def find_tweet_by(self, id: TweetId | Tweet) -> Optional[Tweet]:
+    def find_tweet_by(self, id: Union[TweetId, Tweet]) -> Optional[Tweet]:
         """
         TweetId からツイートを検索する。
 
         Tweet を入力とした場合、入力した Tweet が Response の中にあるかを調べる。
         """
         ...
 
-    def find_retweeted_tweet_by(self, retweet: TweetId | Tweet) -> Optional[Tweet]:
+    def find_retweeted_tweet_by(
+        self, retweet: Union[TweetId, Tweet]
+    ) -> Optional[Tweet]:
         """
         リツイート元のツイートを検索する。
         """
 
         target = self.find_tweet_by(retweet)
 
         if target is None or self.includes is None:
@@ -61,15 +63,17 @@
 
         for tweet in self.includes.tweets:
             if retweeted_id == tweet.id:
                 return tweet
 
         return None
 
-    def find_quoted_tweet_by(self, quote_tweet: TweetId | Tweet) -> Optional[Tweet]:
+    def find_quoted_tweet_by(
+        self, quote_tweet: Union[TweetId, Tweet]
+    ) -> Optional[Tweet]:
         """
         引用元のツイートを検索する。
         """
 
         target = self.find_tweet_by(quote_tweet)
 
         if target is None or self.includes is None:
@@ -82,15 +86,17 @@
 
         for tweet in self.includes.tweets:
             if quote_tweet_id == tweet.id:
                 return tweet
 
         return None
 
-    def find_replied_tweet_by(self, reply_tweet: TweetId | Tweet) -> Optional[Tweet]:
+    def find_replied_tweet_by(
+        self, reply_tweet: Union[TweetId, Tweet]
+    ) -> Optional[Tweet]:
         """
         返信元のツイートを検索する。
         """
 
         target = self.find_tweet_by(reply_tweet)
 
         if target is None or self.includes is None:
@@ -103,15 +109,15 @@
 
         for tweet in self.includes.tweets:
             if reply_tweet_id == tweet.id:
                 return tweet
 
         return None
 
-    def find_mentioned_users_by(self, tweet: TweetId | Tweet) -> list[User]:
+    def find_mentioned_users_by(self, tweet: Union[TweetId, Tweet]) -> list[User]:
         """
         メンションしているユーザのリストを検索する。
         """
 
         target = self.find_tweet_by(tweet)
 
         if target is None or self.includes is None:
@@ -128,15 +134,15 @@
 
 
 class TweetResponseBodyData(ExtraPermissiveModel):
     data: Tweet
 
 
 class TweetResponseBody(FindTweets, TweetResponseBodyData):
-    def find_tweet_by(self, id: TweetId | Tweet) -> Optional[Tweet]:
+    def find_tweet_by(self, id: Union[TweetId, Tweet]) -> Optional[Tweet]:
         if isinstance(id, Tweet):
             id = id.id
 
         if _check_self(id, self.data):
             return self.data
 
         if self.includes is None:
@@ -150,15 +156,15 @@
 
 
 class _TweetsResponseBodyData(ExtraPermissiveModel):
     data: list[Tweet] = Field(default_factory=list)
 
 
 class TweetsResponseBody(FindTweets, _TweetsResponseBodyData):
-    def find_tweet_by(self, id: TweetId | Tweet) -> Optional[Tweet]:
+    def find_tweet_by(self, id: Union[TweetId, Tweet]) -> Optional[Tweet]:
         if isinstance(id, Tweet):
             id = id.id
 
         for tweet in self.data:
             if _check_self(id, tweet):
                 return tweet
 
@@ -202,15 +208,15 @@
     meta: TweetsResponseBodyMeta
 
 
 class TweetsSearchResponseBody(
     TweetsResponseBody, _TweetsSearchResponseBody, PageResponseBody
 ):
     @property
-    def meta_next_token(self) -> PaginationToken | None:
+    def meta_next_token(self) -> Optional[PaginationToken]:
         return self.meta.next_token
 
     def extend(self, other: Self) -> None:
         self.data.extend(other.data)
         self.includes.extend(other.includes)
         self.meta.extend(other.meta)
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_user/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Any, Optional
 
-from twitter_api.api.types.v2_user.user_verified_type import UserVerifiedType
-from twitter_api.api.types.v2_user.username import Username
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 from twitter_api.types.http import Url
+from twitter_api.types.v2_user.user_verified_type import UserVerifiedType
+from twitter_api.types.v2_user.username import Username
 
 from ..v2_tweet.tweet_id import TweetId
 from .user_id import UserId
 
 
 class User(ExtraPermissiveModel):
     id: UserId
```

### Comparing `twitter_api_py-0.2.0/twitter_api/api/types/v2_user/user_field.py` & `twitter_api_py-0.3.0/twitter_api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class TwitterOAuth1AuthorizeClient(Chainable, Generic[TwitterApiGenericClient]):
     def __init__(self, session: TwitterOAuth1Session[TwitterApiGenericClient]) -> None:
         self._session = session
 
     def request(
-        self, url: OauthAuth1enticateUrl | Oauth1AuthorizeUrl
+        self, url: Union[OauthAuth1enticateUrl, Oauth1AuthorizeUrl]
     ) -> Union[
         OAuth1AuthenticateSessionResources[TwitterApiGenericClient],
         OAuth1AuthorizeSessionResources[TwitterApiGenericClient],
     ]:
         if url == "https://api.twitter.com/oauth/authenticate":
             return OAuth1AuthenticateSessionResources(
                 self._session,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth1SessionResources,
 )
 from twitter_api.client.oauth_session.twitter_oauth1_session import TwitterOAuth1Session
 from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
+from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
 
 class PostOauth1AccessTokenResources(OAuth1SessionResources[TwitterApiGenericClient]):
     def __init__(
         self,
         authorization_response_url: CallbackUrl,
         session: TwitterOAuth1Session[TwitterApiGenericClient],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/session_resources.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/session_resources.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Generic
 
-from twitter_api.api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 from twitter_api.client.oauth_session.resources.session_resources import (
     OAuth2SessionResources,
 )
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import CallbackUrl
+from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 
 ENDPOINT = Endpoint("POST", "https://api.twitter.com/2/oauth2/token")
 
 
 class PostV2OAuth2TokenRerources(
     OAuth2SessionResources, Generic[TwitterApiGenericClient]
 ):
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Union
 
 from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
     TwitterOAuth1AuthorizeClient,
 )
 from twitter_api.client.oauth_session.resources.oauth1_authenticate import (
     OauthAuth1enticateUrl,
 )
@@ -24,30 +24,28 @@
         self._client_generator = client_generator
 
     def request_token(self) -> TwitterOAuth1AuthorizeClient:
         return TwitterOAuth1AuthorizeClient(session=self)
 
     def generate_authorization_url(
         self,
-        url: OauthAuth1enticateUrl | Oauth1AuthorizeUrl,
+        url: Union[OauthAuth1enticateUrl, Oauth1AuthorizeUrl],
     ):
-        from twitter_api.api.types.oauth1.oauth1_authorization import (
-            OAuth1Authorization,
-        )
+        from twitter_api.types.oauth1.oauth1_authorization import OAuth1Authorization
 
         return OAuth1Authorization(
             authorization_url="https://authorization.url.com",
             session=self,
         )
 
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
     ):
-        from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
+        from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
         return OAuth1AccessToken(
             oauth_token="oauth_token",
             oauth_token_secret="oauth_token_secret",
             user_id="user_id",
             screen_name="screen_name",
             _session=self,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth1_real_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from typing import Callable, Mapping, Optional
+from typing import Callable, Mapping, Optional, Union
 
 from authlib.integrations.httpx_client.oauth1_client import OAuth1Client
 
-from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
-from twitter_api.api.types.oauth1.oauth1_authorization import OAuth1Authorization
 from twitter_api.client.oauth_flow.twitter_oauth1_authorization_client import (
     TwitterOAuth1AuthorizeClient,
 )
 from twitter_api.client.oauth_session.resources.oauth1_access_token import (
     Oauth1AccessTokenUrl,
 )
 from twitter_api.client.oauth_session.resources.oauth1_authenticate import (
@@ -25,14 +23,16 @@
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
 )
+from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
+from twitter_api.types.oauth1.oauth1_authorization import OAuth1Authorization
 
 
 class TwitterOAuth1RealSession(TwitterOAuth1Session[TwitterApiGenericClient]):
     def __init__(
         self,
         client_generator: Callable[
             [AccessToken, AccessSecret], TwitterApiGenericClient
@@ -77,15 +77,15 @@
 
         self._session.fetch_request_token(url)
 
         return TwitterOAuth1AuthorizeClient(session=self)
 
     def generate_authorization_url(
         self,
-        url: OauthAuth1enticateUrl | Oauth1AuthorizeUrl,
+        url: Union[OauthAuth1enticateUrl, Oauth1AuthorizeUrl],
     ) -> OAuth1Authorization[TwitterApiGenericClient]:
         return OAuth1Authorization(
             authorization_url=self._session.create_authorization_url(url),
             session=self,
         )
 
     def fetch_token(
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,28 @@
         return _
 
     @abstractmethod
     def generate_authorization_url(
         self,
         url: Url,
     ):
-        from twitter_api.api.types.oauth1.oauth1_authorization import (
-            OAuth1Authorization,
-        )
+        from twitter_api.types.oauth1.oauth1_authorization import OAuth1Authorization
 
         _: OAuth1Authorization[TwitterApiGenericClient] = ...  # type: ignore
 
         return _
 
     @abstractmethod
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
     ):
         # NOTE: 本来実装は不要だが、モジュールの循環読み込みを防ぐため、
         #       偽のデータを作っている。
-        from twitter_api.api.types.oauth1.oauth1_access_token import OAuth1AccessToken
+        from twitter_api.types.oauth1.oauth1_access_token import OAuth1AccessToken
 
         _: OAuth1AccessToken[TwitterApiGenericClient] = ...  # type: ignore
 
         return _
 
     @abstractmethod
     def generate_client(
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from datetime import datetime
 from typing import Callable
 
-from twitter_api.api.types.oauth2.oauth2_access_token import OAuth2AccessToken
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types.generic_client import TwitterApiGenericMockClient
 from twitter_api.types.oauth import AccessToken, CallbackUrl
+from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
+from twitter_api.types.v2_scope import Scope
 
 
 class TwitterOAuth2MockSession(TwitterOAuth2Session[TwitterApiGenericMockClient]):
     def __init__(
         self,
         client_generator: Callable[[AccessToken], TwitterApiGenericMockClient],
         *,
         scope: list[Scope],
     ) -> None:
         self._client_generator = client_generator
         self._scope = scope
 
     def generate_authorization_url(self):
-        from twitter_api.api.types.oauth2.oauth2_authorization import (
-            OAuth2Authorization,
-        )
+        from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
 
         return OAuth2Authorization(
             authorization_url="https://authorization.url.com",
             state="state",
             code_verifier="code_verifier",
             session=self,
         )
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth2_real_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, Callable, Generic, Mapping, Optional
 
 from authlib.integrations.httpx_client.oauth2_client import OAuth2Client
 
-from twitter_api.api.types.oauth2.oauth2_access_token import OAuth2AccessToken
-from twitter_api.api.types.oauth2.oauth2_authorization import OAuth2Authorization
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.oauth_session.resources.oauth2_authorize import (
     Oauth2AuthorizeUrl,
 )
 from twitter_api.client.oauth_session.resources.v2_oauth2_token import V2Oauth2TokenUrl
 from twitter_api.client.oauth_session.twitter_oauth2_session import TwitterOAuth2Session
 from twitter_api.types import httpx
 from twitter_api.types.generic_client import TwitterApiGenericClient
 from twitter_api.types.oauth import AccessToken, CallbackUrl, ClientId, ClientSecret
+from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
+from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
+from twitter_api.types.v2_scope import Scope
 from twitter_api.utils._oauth import generate_code_verifier
 
 
 class TwitterOAuth2RealSession(TwitterOAuth2Session, Generic[TwitterApiGenericClient]):
     def __init__(
         self,
         client_generator: Callable[[AccessToken], TwitterApiGenericClient],
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/oauth_session/twitter_oauth2_session.py` & `twitter_api_py-0.3.0/twitter_api/client/oauth_session/twitter_oauth2_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 
 
 class TwitterOAuth2Session(Generic[TwitterApiGenericClient], metaclass=ABCMeta):
     @abstractmethod
     def generate_authorization_url(
         self,
     ):
-        from twitter_api.api.types.oauth2.oauth2_authorization import (
-            OAuth2Authorization,
-        )
+        from twitter_api.types.oauth2.oauth2_authorization import OAuth2Authorization
 
         _: OAuth2Authorization[TwitterApiGenericClient] = ...  # type: ignore
 
         return _
 
     @abstractmethod
     def fetch_token(
         self,
         authorization_response_url: CallbackUrl,
         state: str,
         code_verifier: str,
     ):
-        from twitter_api.api.types.oauth2.oauth2_access_token import OAuth2AccessToken
+        from twitter_api.types.oauth2.oauth2_access_token import OAuth2AccessToken
 
         _: OAuth2AccessToken[TwitterApiGenericClient] = ...  # type: ignore
 
         return _
 
     @abstractmethod
     def generate_client(self, access_token: AccessToken) -> TwitterApiGenericClient:
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.3.0/twitter_api/client/request/request_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.3.0/twitter_api/client/request/request_async_real_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from typing import Mapping, Optional, Self, Type
 
-from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
-from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
-
 from twitter_api.client.request.request_async_client import RequestAsyncClient
 from twitter_api.client.request.request_real_client import (
     _parse_response,
     _remove_none_field,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
 from twitter_api.types import httpx
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import Url
-from twitter_api.types.oauth import OAuthVersion
+from twitter_api.types.oauth import OAuth, OAuthVersion
 
 from .request_client import Headers, QuryParameters, RequestJsonBody, ResponseModelBody
 
-OAuth = OAuth2Auth | OAuth1Auth
-
 
 class RequestAsyncRealClient(RequestAsyncClient):
     def __init__(
         self,
         *,
         auth: Optional[OAuth],
         oauth_version: OAuthVersion,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/request/request_client.py` & `twitter_api_py-0.3.0/twitter_api/client/request/request_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional, Self, Type
 
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import (
     Headers,
     QuryParameters,
     RequestJsonBody,
     ResponseModelBody,
     Url,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.3.0/twitter_api/client/request/request_mock_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Generic, Optional, Type
+from typing import Generic, Optional, Type, Union
 
 from twitter_api.error import (
     MockInjectionResponseWrong,
     MockResponseNotFound,
     TwitterApiError,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import Url
 from twitter_api.types.oauth import OAuthVersion
 
 from .request_client import (
     Headers,
     QuryParameters,
@@ -27,15 +27,17 @@
     def __init__(
         self,
         *,
         oauth_version: OAuthVersion,
         rate_limit_target: RateLimitTarget,
         rate_limit_manager: RateLimitManager,
     ):
-        self._store: list[tuple[Endpoint, ResponseModelBody | TwitterApiError]] = []
+        self._store: list[
+            tuple[Endpoint, Union[ResponseModelBody, TwitterApiError]]
+        ] = []
         self._oauth_version: OAuthVersion = oauth_version
         self._rate_limit_target: RateLimitTarget = rate_limit_target
 
         if rate_limit_manager is None:
             rate_limit_manager = NoOperationRateLimitManager()
 
         self._rate_limit_manager = rate_limit_manager
@@ -49,15 +51,17 @@
         return self._rate_limit_target
 
     @property
     def rate_limit_manager(self) -> RateLimitManager:
         return self._rate_limit_manager
 
     def inject_response_body(
-        self, endpoint: Endpoint, response_body: ResponseModelBody | TwitterApiError
+        self,
+        endpoint: Endpoint,
+        response_body: Union[ResponseModelBody, TwitterApiError],
     ):
         self._store.append((endpoint, response_body))
 
     def _extract_response_body(self, endpoint: Endpoint) -> ResponseModelBody:
         if len(self._store) == 0:
             raise MockResponseNotFound()
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.3.0/twitter_api/client/request/request_real_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 from typing import Mapping, Optional, Self, Type
 
 import pydantic
-from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
-from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
 
 from twitter_api.error import (
     TwitterApiOAuthTokenV1NotFound,
     TwitterApiResponseError,
     TwitterApiResponseFailed,
     TwitterApiResponseModelBodyDecodeError,
     TwitterApiResponseValidationError,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
 from twitter_api.types import httpx
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.http import Url
-from twitter_api.types.oauth import OAuthVersion
+from twitter_api.types.oauth import OAuth, OAuthVersion
 
 from .request_client import (
     Headers,
     QuryParameters,
     RequestClient,
     RequestJsonBody,
     ResponseModelBody,
 )
 
-OAuth = OAuth2Auth | OAuth1Auth
-
 
 class RequestRealClient(RequestClient):
     def __init__(
         self,
         *,
         auth: Optional[OAuth],
         oauth_version: OAuthVersion,
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_client.py` & `twitter_api_py-0.3.0/twitter_api/client/twitter_api_async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,101 +1,98 @@
 import os
 from abc import ABCMeta, abstractmethod
 from typing import Mapping, Optional, Self, Union, overload
 
-from twitter_api.api.resources.oauth2_invalidate_token import (
+from twitter_api.client.request.request_async_client import RequestAsyncClient
+from twitter_api.error import NeverError
+from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
+from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
+from twitter_api.resources.oauth2_invalidate_token import (
     AsyncOauth2InvalidateTokenResources,
     Oauth2InvalidateTokenUrl,
 )
-from twitter_api.api.resources.oauth2_token import (
-    AsyncOauth2TokenResources,
-    Oauth2TokenUrl,
-)
-from twitter_api.api.resources.v2_dm_conversation_messages import (
+from twitter_api.resources.oauth2_token import AsyncOauth2TokenResources, Oauth2TokenUrl
+from twitter_api.resources.v2_dm_conversation_messages import (
     AsyncV2DmConversationMessagesResources,
     V2DmConversationsMessagesUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations import (
+from twitter_api.resources.v2_dm_conversations import (
     AsyncV2DmConversationsResources,
     V2DmConversationsUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_dm_events import (
+from twitter_api.resources.v2_dm_conversations_with_participant_dm_events import (
     AsyncV2DmConversationsWithParticipantDmEventsResources,
     V2DmConversationsWithParticipantDmEventsUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_messages import (
+from twitter_api.resources.v2_dm_conversations_with_participant_messages import (
     AsyncV2DmConversationsWithParticipantMessagesResources,
     V2DmConversationsWithParticipantMessagesUrl,
 )
-from twitter_api.api.resources.v2_tweet import AsyncV2TweetResources, V2TweetUrl
-from twitter_api.api.resources.v2_tweet_retweeted_by import (
+from twitter_api.resources.v2_tweet import AsyncV2TweetResources, V2TweetUrl
+from twitter_api.resources.v2_tweet_retweeted_by import (
     AsyncV2TweetRetweetedByRerources,
     V2TweetRetweetedByUrl,
 )
-from twitter_api.api.resources.v2_tweets import AsyncV2TweetsResources, V2TweetsUrl
-from twitter_api.api.resources.v2_tweets_search_all import (
+from twitter_api.resources.v2_tweets import AsyncV2TweetsResources, V2TweetsUrl
+from twitter_api.resources.v2_tweets_search_all import (
     AsyncV2TweetsSearchAllResources,
     V2TweetsSearchAllUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_recent import (
+from twitter_api.resources.v2_tweets_search_recent import (
     AsyncV2TweetsSearchRecentResources,
     V2TweetsSearchRecentUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_stream import (
+from twitter_api.resources.v2_tweets_search_stream import (
     AsyncV2TweetsSearchStreamResources,
     V2TweetsSearchStreamUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_stream_rules import (
+from twitter_api.resources.v2_tweets_search_stream_rules import (
     AsyncV2TweetsSearchStreamRulesResources,
     V2TweetsSearchStreamRulesUrl,
 )
-from twitter_api.api.resources.v2_user import AsyncV2UserResources, V2UserUrl
-from twitter_api.api.resources.v2_user_followers import (
+from twitter_api.resources.v2_user import AsyncV2UserResources, V2UserUrl
+from twitter_api.resources.v2_user_followers import (
     AsyncV2UserFollowersResources,
     V2UserFollowersUrl,
 )
-from twitter_api.api.resources.v2_user_following import (
+from twitter_api.resources.v2_user_following import (
     AsyncV2UserFollowingResources,
     V2UserFollowingUrl,
 )
-from twitter_api.api.resources.v2_user_liked_tweets import (
+from twitter_api.resources.v2_user_liked_tweets import (
     AsyncV2UserLikedTweetsResources,
     V2UserLikedTweetsUrl,
 )
-from twitter_api.api.resources.v2_user_retweets import (
+from twitter_api.resources.v2_user_retweets import (
     AsyncV2UserRetweetsResources,
     V2UserRetweetsUrl,
 )
-from twitter_api.api.resources.v2_user_tweets import (
+from twitter_api.resources.v2_user_tweets import (
     AsyncV2UserTweetsResources,
     V2UserTweetsUrl,
 )
-from twitter_api.api.resources.v2_users import AsyncV2UsersResources, V2UsersUrl
-from twitter_api.api.resources.v2_users_by import AsyncV2UsersByResources, V2UsersByUrl
-from twitter_api.api.resources.v2_users_by_username import (
+from twitter_api.resources.v2_users import AsyncV2UsersResources, V2UsersUrl
+from twitter_api.resources.v2_users_by import AsyncV2UsersByResources, V2UsersByUrl
+from twitter_api.resources.v2_users_by_username import (
     AsyncV2UsersByUsernameResources,
     V2UsersByUsernameUrl,
 )
-from twitter_api.api.types.v2_scope import Scope
-from twitter_api.client.request.request_async_client import RequestAsyncClient
-from twitter_api.error import NeverError
-from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
-from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
 from twitter_api.types import httpx
 from twitter_api.types.chainable import Chainable
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
     ClientSecret,
     Env,
 )
+from twitter_api.types.v2_scope import Scope
 
 
 class TwitterApiAsyncClient(Chainable, metaclass=ABCMeta):
     """
     Twitter API を非同期に操作するためのクライアント
     """
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_mock_client.py` & `twitter_api_py-0.3.0/twitter_api/client/twitter_api_async_mock_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Mapping, Optional, Self
 
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.twitter_api_async_client import TwitterApiAsyncClient
 from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
 from twitter_api.types import httpx
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
     ClientSecret,
     Env,
 )
+from twitter_api.types.v2_scope import Scope
 
 from .twitter_api_mock_client import _BaseTwitterApiMockClient
 
 
 class TwitterApiAsyncMockClient(_BaseTwitterApiMockClient, TwitterApiAsyncClient):
     @classmethod
     def from_oauth2_bearer_token(
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/twitter_api_async_real_client.py` & `twitter_api_py-0.3.0/twitter_api/client/twitter_api_async_real_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Mapping, Optional, Self
 
 from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
 from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
 
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.request.request_async_real_client import RequestAsyncRealClient
 from twitter_api.client.request.request_real_client import RequestRealClient
 from twitter_api.client.twitter_api_async_client import TwitterApiAsyncClient
 from twitter_api.client.twitter_api_real_client import TwitterApiRealClient
 from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
 from twitter_api.types import httpx
@@ -16,14 +15,15 @@
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
     ClientSecret,
 )
+from twitter_api.types.v2_scope import Scope
 
 from .request.request_client import RequestClient
 
 
 class TwitterApiAsyncRealClient(TwitterApiAsyncClient):
     """
     Twitter API V2 を操作するためのクライアント
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/twitter_api_client.py` & `twitter_api_py-0.3.0/twitter_api/client/twitter_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,97 +1,94 @@
 import os
 from abc import ABCMeta, abstractmethod
 from typing import Mapping, Optional, Self, Union, overload
 
-from twitter_api.api.resources.oauth2_invalidate_token import (
+from twitter_api.error import NeverError
+from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
+from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
+from twitter_api.resources.oauth2_invalidate_token import (
     Oauth2InvalidateTokenResources,
     Oauth2InvalidateTokenUrl,
 )
-from twitter_api.api.resources.oauth2_token import Oauth2TokenResources, Oauth2TokenUrl
-from twitter_api.api.resources.v2_dm_conversation_messages import (
+from twitter_api.resources.oauth2_token import Oauth2TokenResources, Oauth2TokenUrl
+from twitter_api.resources.v2_dm_conversation_messages import (
     V2DmConversationMessagesResources,
     V2DmConversationsMessagesUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations import (
+from twitter_api.resources.v2_dm_conversations import (
     V2DmConversationsResources,
     V2DmConversationsUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_dm_events import (
+from twitter_api.resources.v2_dm_conversations_with_participant_dm_events import (
     V2DmConversationsWithParticipantDmEventsResources,
     V2DmConversationsWithParticipantDmEventsUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_messages import (
+from twitter_api.resources.v2_dm_conversations_with_participant_messages import (
     V2DmConversationsWithParticipantMessagesResources,
     V2DmConversationsWithParticipantMessagesUrl,
 )
-from twitter_api.api.resources.v2_tweet import V2TweetResources, V2TweetUrl
-from twitter_api.api.resources.v2_tweet_retweeted_by import (
+from twitter_api.resources.v2_tweet import V2TweetResources, V2TweetUrl
+from twitter_api.resources.v2_tweet_retweeted_by import (
     V2TweetRetweetedByRerources,
     V2TweetRetweetedByUrl,
 )
-from twitter_api.api.resources.v2_tweets import V2TweetsResources, V2TweetsUrl
-from twitter_api.api.resources.v2_tweets_search_all import (
+from twitter_api.resources.v2_tweets import V2TweetsResources, V2TweetsUrl
+from twitter_api.resources.v2_tweets_search_all import (
     V2TweetsSearchAllResources,
     V2TweetsSearchAllUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_recent import (
+from twitter_api.resources.v2_tweets_search_recent import (
     V2TweetsSearchRecentResources,
     V2TweetsSearchRecentUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_stream import (
+from twitter_api.resources.v2_tweets_search_stream import (
     V2TweetsSearchStreamResources,
     V2TweetsSearchStreamUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_stream_rules import (
+from twitter_api.resources.v2_tweets_search_stream_rules import (
     V2TweetsSearchStreamRulesResources,
     V2TweetsSearchStreamRulesUrl,
 )
-from twitter_api.api.resources.v2_user import V2UserResources, V2UserUrl
-from twitter_api.api.resources.v2_user_followers import (
+from twitter_api.resources.v2_user import V2UserResources, V2UserUrl
+from twitter_api.resources.v2_user_followers import (
     V2UserFollowersResources,
     V2UserFollowersUrl,
 )
-from twitter_api.api.resources.v2_user_following import (
+from twitter_api.resources.v2_user_following import (
     V2UserFollowingResources,
     V2UserFollowingUrl,
 )
-from twitter_api.api.resources.v2_user_liked_tweets import (
+from twitter_api.resources.v2_user_liked_tweets import (
     V2UserLikedTweetsResources,
     V2UserLikedTweetsUrl,
 )
-from twitter_api.api.resources.v2_user_retweets import (
+from twitter_api.resources.v2_user_retweets import (
     V2UserRetweetsResources,
     V2UserRetweetsUrl,
 )
-from twitter_api.api.resources.v2_user_tweets import (
-    V2UserTweetsResources,
-    V2UserTweetsUrl,
-)
-from twitter_api.api.resources.v2_users import V2UsersResources, V2UsersUrl
-from twitter_api.api.resources.v2_users_by import V2UsersByResources, V2UsersByUrl
-from twitter_api.api.resources.v2_users_by_username import (
+from twitter_api.resources.v2_user_tweets import V2UserTweetsResources, V2UserTweetsUrl
+from twitter_api.resources.v2_users import V2UsersResources, V2UsersUrl
+from twitter_api.resources.v2_users_by import V2UsersByResources, V2UsersByUrl
+from twitter_api.resources.v2_users_by_username import (
     V2UsersByUsernameResources,
     V2UsersByUsernameUrl,
 )
-from twitter_api.api.types.v2_scope import Scope
-from twitter_api.error import NeverError
-from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
-from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
 from twitter_api.types import httpx
 from twitter_api.types.chainable import Chainable
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
     ClientSecret,
     Env,
 )
+from twitter_api.types.v2_scope import Scope
 
 from .request.request_client import RequestClient
 
 
 class TwitterApiClient(Chainable, metaclass=ABCMeta):
     """
     Twitter API を操作するためのクライアント
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/twitter_api_mock_client.py` & `twitter_api_py-0.3.0/twitter_api/client/twitter_api_mock_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,120 +1,118 @@
 from typing import Mapping, Optional, Self, Union, overload
 
-from twitter_api.api.resources.oauth2_invalidate_token import Oauth2InvalidateTokenUrl
-from twitter_api.api.resources.oauth2_invalidate_token.post_oauth2_invalidate_token import (
+from twitter_api.error import TwitterApiError
+from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
+from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
+from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
+from twitter_api.resources.oauth2_invalidate_token import Oauth2InvalidateTokenUrl
+from twitter_api.resources.oauth2_invalidate_token.post_oauth2_invalidate_token import (
     PostOauth2InvalidateTokenResponseBody,
 )
-from twitter_api.api.resources.oauth2_token import Oauth2TokenUrl
-from twitter_api.api.resources.oauth2_token.post_oauth2_token import (
+from twitter_api.resources.oauth2_token import Oauth2TokenUrl
+from twitter_api.resources.oauth2_token.post_oauth2_token import (
     PostOauth2TokenResponseBody,
 )
-from twitter_api.api.resources.v2_dm_conversation_messages import (
+from twitter_api.resources.v2_dm_conversation_messages import (
     V2DmConversationsMessagesUrl,
 )
-from twitter_api.api.resources.v2_dm_conversation_messages.post_v2_dm_conversations_messages import (
+from twitter_api.resources.v2_dm_conversation_messages.post_v2_dm_conversations_messages import (
     PostV2DmConversationMessagesResponseBody,
 )
-from twitter_api.api.resources.v2_dm_conversations import V2DmConversationsUrl
-from twitter_api.api.resources.v2_dm_conversations.post_v2_dm_conversations import (
+from twitter_api.resources.v2_dm_conversations import V2DmConversationsUrl
+from twitter_api.resources.v2_dm_conversations.post_v2_dm_conversations import (
     PostV2DmConversationsResponseBody,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_dm_events import (
+from twitter_api.resources.v2_dm_conversations_with_participant_dm_events import (
     V2DmConversationsWithParticipantDmEventsUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_dm_events.get_v2_dm_conversations_with_participant_dm_events import (
+from twitter_api.resources.v2_dm_conversations_with_participant_dm_events.get_v2_dm_conversations_with_participant_dm_events import (
     GetV2DmConversationsWithParticipantDmEventsResponseBody,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_messages import (
+from twitter_api.resources.v2_dm_conversations_with_participant_messages import (
     V2DmConversationsWithParticipantMessagesUrl,
 )
-from twitter_api.api.resources.v2_dm_conversations_with_participant_messages.post_v2_dm_conversations_with_participant_messages import (
+from twitter_api.resources.v2_dm_conversations_with_participant_messages.post_v2_dm_conversations_with_participant_messages import (
     PostV2DmConversationsWithParticipantMessagesResponseBody,
 )
-from twitter_api.api.resources.v2_tweet import V2TweetUrl
-from twitter_api.api.resources.v2_tweet.delete_v2_tweet import DeleteV2TweetResponseBody
-from twitter_api.api.resources.v2_tweet.get_v2_tweet import GetV2TweetResponseBody
-from twitter_api.api.resources.v2_tweet_retweeted_by import V2TweetRetweetedByUrl
-from twitter_api.api.resources.v2_tweet_retweeted_by.get_v2_tweet_retweeted_by import (
+from twitter_api.resources.v2_tweet import V2TweetUrl
+from twitter_api.resources.v2_tweet.delete_v2_tweet import DeleteV2TweetResponseBody
+from twitter_api.resources.v2_tweet.get_v2_tweet import GetV2TweetResponseBody
+from twitter_api.resources.v2_tweet_retweeted_by import V2TweetRetweetedByUrl
+from twitter_api.resources.v2_tweet_retweeted_by.get_v2_tweet_retweeted_by import (
     GetV2TweetRetweetedByResponseBody,
 )
-from twitter_api.api.resources.v2_tweets import V2TweetsUrl
-from twitter_api.api.resources.v2_tweets.get_v2_tweets import GetV2TweetsResponseBody
-from twitter_api.api.resources.v2_tweets.post_v2_tweets import PostV2TweetsResponseBody
-from twitter_api.api.resources.v2_tweets_search_all import V2TweetsSearchAllUrl
-from twitter_api.api.resources.v2_tweets_search_all.get_v2_tweets_search_all import (
+from twitter_api.resources.v2_tweets import V2TweetsUrl
+from twitter_api.resources.v2_tweets.get_v2_tweets import GetV2TweetsResponseBody
+from twitter_api.resources.v2_tweets.post_v2_tweets import PostV2TweetsResponseBody
+from twitter_api.resources.v2_tweets_search_all import V2TweetsSearchAllUrl
+from twitter_api.resources.v2_tweets_search_all.get_v2_tweets_search_all import (
     GetV2TweetsSearchAllResponseBody,
 )
-from twitter_api.api.resources.v2_tweets_search_recent import V2TweetsSearchRecentUrl
-from twitter_api.api.resources.v2_tweets_search_recent.get_v2_tweets_search_recent import (
+from twitter_api.resources.v2_tweets_search_recent import V2TweetsSearchRecentUrl
+from twitter_api.resources.v2_tweets_search_recent.get_v2_tweets_search_recent import (
     GetV2TweetsSearchRecentResponseBody,
 )
-from twitter_api.api.resources.v2_tweets_search_stream import V2TweetsSearchStreamUrl
-from twitter_api.api.resources.v2_tweets_search_stream.get_v2_tweets_search_stream import (
+from twitter_api.resources.v2_tweets_search_stream import V2TweetsSearchStreamUrl
+from twitter_api.resources.v2_tweets_search_stream.get_v2_tweets_search_stream import (
     GetV2TweetsSearchStreamResponseBody,
 )
-from twitter_api.api.resources.v2_tweets_search_stream_rules import (
+from twitter_api.resources.v2_tweets_search_stream_rules import (
     V2TweetsSearchStreamRulesUrl,
 )
-from twitter_api.api.resources.v2_tweets_search_stream_rules.get_v2_tweets_search_stream_rules import (
+from twitter_api.resources.v2_tweets_search_stream_rules.get_v2_tweets_search_stream_rules import (
     GetV2TweetsSearchStreamRulesResponseBody,
 )
-from twitter_api.api.resources.v2_tweets_search_stream_rules.post_v2_tweets_search_stream_rules import (
+from twitter_api.resources.v2_tweets_search_stream_rules.post_v2_tweets_search_stream_rules import (
     PostV2TweetsSearchStreamRulesResponseBody,
 )
-from twitter_api.api.resources.v2_user import V2UserUrl
-from twitter_api.api.resources.v2_user.get_v2_user import GetV2UserResponseBody
-from twitter_api.api.resources.v2_user_followers import V2UserFollowersUrl
-from twitter_api.api.resources.v2_user_followers.get_v2_user_followers import (
+from twitter_api.resources.v2_user import V2UserUrl
+from twitter_api.resources.v2_user.get_v2_user import GetV2UserResponseBody
+from twitter_api.resources.v2_user_followers import V2UserFollowersUrl
+from twitter_api.resources.v2_user_followers.get_v2_user_followers import (
     GetV2UserFollowersResponseBody,
 )
-from twitter_api.api.resources.v2_user_following import V2UserFollowingUrl
-from twitter_api.api.resources.v2_user_following.post_v2_user_following import (
+from twitter_api.resources.v2_user_following import V2UserFollowingUrl
+from twitter_api.resources.v2_user_following.post_v2_user_following import (
     PostV2UserFollowingResponseBody,
 )
-from twitter_api.api.resources.v2_user_liked_tweets import V2UserLikedTweetsUrl
-from twitter_api.api.resources.v2_user_liked_tweets.get_v2_user_liked_tweets import (
+from twitter_api.resources.v2_user_liked_tweets import V2UserLikedTweetsUrl
+from twitter_api.resources.v2_user_liked_tweets.get_v2_user_liked_tweets import (
     GetV2UserLikedTweetsResponseBody,
 )
-from twitter_api.api.resources.v2_user_retweets import V2UserRetweetsUrl
-from twitter_api.api.resources.v2_user_retweets.post_v2_user_retweets import (
+from twitter_api.resources.v2_user_retweets import V2UserRetweetsUrl
+from twitter_api.resources.v2_user_retweets.post_v2_user_retweets import (
     PostV2UserRetweetsResponseBody,
 )
-from twitter_api.api.resources.v2_user_tweets import V2UserTweetsUrl
-from twitter_api.api.resources.v2_user_tweets.get_v2_user_tweets import (
+from twitter_api.resources.v2_user_tweets import V2UserTweetsUrl
+from twitter_api.resources.v2_user_tweets.get_v2_user_tweets import (
     GetV2UserTweetsResponseBody,
 )
-from twitter_api.api.resources.v2_users import V2UsersUrl
-from twitter_api.api.resources.v2_users.get_v2_users import GetV2UsersResponseBody
-from twitter_api.api.resources.v2_users_by import V2UsersByUrl
-from twitter_api.api.resources.v2_users_by.get_v2_users_by import (
-    GetV2UsersByResponseBody,
-)
-from twitter_api.api.resources.v2_users_by_username import V2UsersByUsernameUrl
-from twitter_api.api.resources.v2_users_by_username.get_v2_users_by_username import (
+from twitter_api.resources.v2_users import V2UsersUrl
+from twitter_api.resources.v2_users.get_v2_users import GetV2UsersResponseBody
+from twitter_api.resources.v2_users_by import V2UsersByUrl
+from twitter_api.resources.v2_users_by.get_v2_users_by import GetV2UsersByResponseBody
+from twitter_api.resources.v2_users_by_username import V2UsersByUsernameUrl
+from twitter_api.resources.v2_users_by_username.get_v2_users_by_username import (
     GetV2UsersByUsernameResponseBody,
 )
-from twitter_api.api.types.v2_scope import Scope
-from twitter_api.error import TwitterApiError
-from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
-from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
 from twitter_api.types import httpx
 from twitter_api.types.endpoint import Endpoint
 from twitter_api.types.oauth import (
     AccessSecret,
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
     ClientSecret,
     Env,
     OAuthVersion,
 )
+from twitter_api.types.v2_scope import Scope
 
 from .request.request_client import RequestClient
 from .request.request_mock_client import RequestMockClient
 from .twitter_api_client import TwitterApiClient
 
 
 class _BaseTwitterApiMockClient:
```

### Comparing `twitter_api_py-0.2.0/twitter_api/client/twitter_api_real_client.py` & `twitter_api_py-0.3.0/twitter_api/client/twitter_api_real_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Mapping, Optional, Self
 
 from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
 from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
 
-from twitter_api.api.types.v2_scope import Scope
 from twitter_api.client.oauth_flow.twitter_oauth1_request_token_client import (
     TwitterOAuth1RequestTokenClient,
 )
 from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
 from twitter_api.types import httpx
 from twitter_api.types.oauth import (
@@ -15,14 +14,15 @@
     AccessToken,
     ApiKey,
     ApiSecret,
     CallbackUrl,
     ClientId,
     ClientSecret,
 )
+from twitter_api.types.v2_scope import Scope
 
 from .request.request_client import RequestClient
 from .request.request_real_client import RequestRealClient
 from .twitter_api_client import TwitterApiClient
 
 
 class TwitterApiRealClient(TwitterApiClient):
```

### Comparing `twitter_api_py-0.2.0/twitter_api/error.py` & `twitter_api_py-0.3.0/twitter_api/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from abc import abstractmethod
 from collections import OrderedDict
 from enum import Enum
 from textwrap import dedent
-from typing import Any, Never, Optional
+from typing import Any, Never, Optional, Union
 
 import pydantic
 
-from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
 from twitter_api.types.extra_permissive_model import ExtraPermissiveModel
 
 from .types.endpoint import Endpoint
 from .types.http import Headers, QuryParameters, RequestJsonBody, ResponseJsonBody
 from .types.oauth import OAuthVersion
 from .utils._functional import exclude_none
 
@@ -136,15 +136,15 @@
         self,
         endpoint: Endpoint,
         url: str,
         request_headers: Optional[Headers],
         query: Optional[QuryParameters],
         request_body: Optional[RequestJsonBody],
         response_status_code: int,
-        response_body: Optional[ResponseJsonBody | bytes],
+        response_body: Optional[Union[ResponseJsonBody, bytes]],
     ):
         self._endpoint = endpoint
         self._url = url
         self._request_headers = request_headers
         self._query = query
         self._request_body = request_body
         self.status_code = response_status_code
@@ -203,20 +203,14 @@
                     if not isinstance(self._response_body, bytes)
                     else self._response_body
                 ),
             ),
         )
 
 
-class OAuth2UserAccessTokenExpired(TwitterApiError):
-    @property
-    def message(self) -> str:
-        return "OAuth2.0 のユーザ認証の ACCESS_TOKEN が失効しました。再度発行してください。"
-
-
 class TwitterApiResponseError(TwitterApiError):
     def __init__(self, endpoint: Endpoint, data: Any, **extra):
         self._endpoint = endpoint
         self._data = data
         self._extra = extra
 
     @property
```

### Comparing `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.3.0/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Optional
 
 from twitter_api.rate_limit.manager.handlers.raise_rate_limit_handler import (
     RaiseRateLimitHandler,
 )
-from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
 
 
 @dataclass
 class RateLimitStatus:
     start_datetime: datetime
     request_datetimes: list[datetime]
```

### Comparing `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py` & `twitter_api_py-0.3.0/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 import asyncio
 import random
 import time
-from abc import ABCMeta
 from contextlib import asynccontextmanager, contextmanager
 from logging import getLogger
 
 from twitter_api.error import TwitterApiErrorCode, TwitterApiResponseFailed
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
-from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
 from twitter_api.warning import RateLimitOverWarning, UnmanagedRateLimitOverWarning
 
 logger = getLogger(__file__)
 
+DEFAULT_MIN_RANDOM_SLEEP_SECONDS = 5 * 60
+DEFAULT_MAX_RANDOM_SLEEP_SECONDS = 15 * 60
 
-class SleepRateLimitHandler(RateLimitManager, metaclass=ABCMeta):
+
+class SleepRateLimitHandler(RateLimitManager):
     """
     レートリミットに遭遇した場合、スリープする handler。
     """
 
-    def random_sleep_seconds(self) -> float:
+    def __init__(
+        self,
+        *,
+        min_random_sleep_seconds: int = DEFAULT_MIN_RANDOM_SLEEP_SECONDS,
+        max_random_sleep_seconds: int = DEFAULT_MAX_RANDOM_SLEEP_SECONDS,
+    ):
+        self._min_random_sleep_seconds = min_random_sleep_seconds
+        self._max_random_sleep_seconds = max_random_sleep_seconds
+
+    def random_sleep_seconds(self) -> int:
         """
         予期しないレートリミットに遭遇した場合にランダムに休む時間[秒]。
         """
 
-        # デフォルトは 5 ~ 15 分。
-        return random.randint(5 * 60, 15 * 60)
+        return random.randint(
+            self._min_random_sleep_seconds, self._max_random_sleep_seconds
+        )
 
     @contextmanager
     def handle_rate_limit_sync(self, rate_limit_info: RateLimitInfo):
         while True:
             # レートリミットを超えてしまっていたら、必要な待ち時間分だけ待つ。
-            wait_time_seconds = self.check_limit_over(rate_limit_info)
-            if wait_time_seconds is not None:
+            if wait_time_seconds := self.check_limit_over(rate_limit_info):
                 logger.warning(RateLimitOverWarning(rate_limit_info))
                 time.sleep(wait_time_seconds)
                 continue
 
             try:
                 yield
+                return
+
             except TwitterApiResponseFailed as error:
                 # レートリミット以外のエラーなら上流に投げる。
                 if error.status_code != TwitterApiErrorCode.TooManyRequests.value:
                     raise error
 
                 # 予期しないレートリミットに遭遇した場合、投機的な待機を行う
                 logger.warning(UnmanagedRateLimitOverWarning())
                 time.sleep(self.random_sleep_seconds())
-            else:
-                return
 
     @asynccontextmanager
     async def handle_rate_limit_async(self, rate_limit_info: RateLimitInfo):
         while True:
             # レートリミットを超えてしまっていたら、必要な待ち時間分だけ待つ。
-            wait_time_seconds = self.check_limit_over(rate_limit_info)
-            if wait_time_seconds is not None:
+            if wait_time_seconds := self.check_limit_over(rate_limit_info):
                 logger.warning(RateLimitOverWarning(rate_limit_info))
                 await asyncio.sleep(wait_time_seconds)
                 continue
 
             try:
                 yield
+                return
+
             except TwitterApiResponseFailed as error:
                 # レートリミットのエラーでないなら上流に投げる。
                 if error.status_code != TwitterApiErrorCode.TooManyRequests.value:
                     raise error
 
                 # 予期しないレートリミットに遭遇した場合、投機的な待機を行う
                 logger.warning(UnmanagedRateLimitOverWarning())
                 await asyncio.sleep(self.random_sleep_seconds())
-            else:
-                return
```

### Comparing `twitter_api_py-0.2.0/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.3.0/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from contextlib import asynccontextmanager, contextmanager
 from datetime import datetime
 from typing import AsyncGenerator, Generator, Optional
 
-from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
 
 
 class RateLimitManager(metaclass=ABCMeta):
     @abstractmethod
     def check_limit_over(
         self,
         rate_limit_info: RateLimitInfo,
@@ -24,19 +24,19 @@
     def handle_rate_limit_sync(
         self, rate_limit_info: RateLimitInfo
     ) -> Generator[None, None, None]:
         """
         同期的な TwitterApiClient を用いている場合のレートリミットの対応方法。
         """
 
-        yield
+        ...
 
     @abstractmethod
     @asynccontextmanager
     async def handle_rate_limit_async(
         self, rate_limit_info: RateLimitInfo
     ) -> AsyncGenerator[None, None]:
         """
         非同期的な TwitterApiAsyncClient を用いている場合のレートリミットの対応方法。
         """
 
-        yield
+        ...
```

### Comparing `twitter_api_py-0.2.0/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.3.0/twitter_api/rate_limit/rate_limit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable, Literal, Optional, overload
 
-from twitter_api.api.resources.api_resources import ApiResources
 from twitter_api.client.request.request_async_client import RequestAsyncClient
-from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
-from twitter_api.rate_limit.types.rate_limit_target import RateLimitTarget
+from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
+from twitter_api.resources.api_resources import ApiResources
 from twitter_api.types.endpoint import Endpoint
 
 
 @overload
 def rate_limit(
     endpoint: Endpoint,
     target: RateLimitTarget,
@@ -54,32 +54,30 @@
     hours: Optional[int] = None,
     mins: Optional[int] = None,
     seconds: Optional[int] = None,
 ) -> Callable:
     """
     レートリミットに関する情報を付与します。
 
-    将来的には、レートリミットを回避するように非同期で api を実行する機能を提供します。
-
-    また、公式には明らかになっていないレートリミットを追加する機能、
-    特定のアカウント用にレートリミットを上書きする機能も提供します。
+    将来的には、公式には明らかになっていないレートリミットを追加する機能、
+    特定のアカウント用にレートリミットを上書きする機能を提供するかもしれません。
     """
 
     def _rate_limit(func):
-        async def async_wrapper(
+        async def handle_async(
             rate_limit_info: RateLimitInfo, self: ApiResources, *args, **kwargs
         ):
             rate_limit_manager = self.request_client.rate_limit_manager
 
             async with rate_limit_manager.handle_rate_limit_async(
                 rate_limit_info,
             ):
                 return await func(self, *args, **kwargs)
 
-        def sync_wrapper(
+        def handle_sync(
             rate_limit_info: RateLimitInfo, self: ApiResources, *args, **kwargs
         ):
             rate_limit_manager = self.request_client.rate_limit_manager
 
             with rate_limit_manager.handle_rate_limit_sync(
                 rate_limit_info,
             ):
@@ -102,14 +100,14 @@
                 target=target,
                 endpoint=endpoint,
                 requests=requests,
                 total_seconds=total_seconds,
             )
 
             if isinstance(self.request_client, RequestAsyncClient):
-                return async_wrapper(rate_limit_info, self, *args, **kwargs)
+                return handle_async(rate_limit_info, self, *args, **kwargs)
             else:
-                return sync_wrapper(rate_limit_info, self, *args, **kwargs)
+                return handle_sync(rate_limit_info, self, *args, **kwargs)
 
         return _wrapper
 
     return _rate_limit
```

### Comparing `twitter_api_py-0.2.0/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.3.0/twitter_api/types/comma_separatable.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.3.0/twitter_api/types/extra_permissive_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/types/generic_client.py` & `twitter_api_py-0.3.0/twitter_api/types/generic_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/types/http.py` & `twitter_api_py-0.3.0/twitter_api/types/http.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/types/httpx.py` & `twitter_api_py-0.3.0/twitter_api/types/httpx.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/types/model.py` & `twitter_api_py-0.3.0/twitter_api/types/model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/types/oauth.py` & `twitter_api_py-0.3.0/twitter_api/types/oauth.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 
 型を作るほどなのか難しい所であるが、同じことを指す用語がたくさん存在するため、
 あえて型を作ることで説明文を用意している。
 
 refer: https://developer.twitter.com/en/docs/authentication/oauth-1-0a/obtaining-user-access-tokens
 """
 
-from typing import Annotated, Literal, TypeAlias, TypeVar
+from typing import Annotated, Literal, TypeAlias, TypeVar, Union
+
+from authlib.integrations.httpx_client.oauth1_client import OAuth1Auth
+from authlib.integrations.httpx_client.oauth2_client import OAuth2Auth
 
 T = TypeVar("T", bound=str)
 
 OAuthVersion = Literal["1.0a", "2.0"]
+OAuth: TypeAlias = Union[OAuth2Auth, OAuth1Auth]
+
 
 Env = Annotated[T, ...]
 """
 環境変数名。
 """
```

### Comparing `twitter_api_py-0.2.0/twitter_api/types/paging.py` & `twitter_api_py-0.3.0/twitter_api/types/paging.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Generator,
     Optional,
     Self,
     TypedDict,
     TypeVar,
 )
 
-from twitter_api.api.types.pagination_token import PaginationToken
+from twitter_api.types.pagination_token import PaginationToken
 
 
 class PageResponseBody(metaclass=ABCMeta):
     @property
     @abstractmethod
     def meta_next_token(self) -> Optional[PaginationToken]:
         ...
@@ -75,14 +75,15 @@
     ページングされたレスポンスを返す API に対して、最後までデータを読み取り、結合した状態で返す。
     """
     paging = get_paging_response_body_iter_sync(get_func, query, pagination_token_key)
     first = next(paging)
 
     for page in paging:
         first.extend(page)
+
     return first
 
 
 async def get_paging_response_body_iter_async(
     get_func: Callable[
         [AnyQueryParameters],
         Coroutine[Any, Any, AnyPageResponseBody],
@@ -123,8 +124,9 @@
     ページングされたレスポンスを返す API に対して、最後までデータを読み取り、結合した状態で返す。
     """
     paging = get_paging_response_body_iter_async(get_func, query, pagination_token_key)
     first = await paging.__anext__()
 
     async for page in paging:
         first.extend(page)
+
     return first
```

### Comparing `twitter_api_py-0.2.0/twitter_api/utils/_functional.py` & `twitter_api_py-0.3.0/twitter_api/utils/_functional.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/utils/_oauth.py` & `twitter_api_py-0.3.0/twitter_api/utils/_oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/utils/json.py` & `twitter_api_py-0.3.0/twitter_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.2.0/twitter_api/warning.py` & `twitter_api_py-0.3.0/twitter_api/warning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from twitter_api.error import TwitterApiException
-from twitter_api.rate_limit.types.rate_limit_info import RateLimitInfo
+from twitter_api.rate_limit.rate_limit_info import RateLimitInfo
 
 
 class TwitterApiWarning(TwitterApiException):
     ...
 
 
 class RateLimitOverWarning(TwitterApiWarning):
@@ -14,8 +14,8 @@
     def message(self) -> str:
         return f"レートリミットを超えています。{self._rate_limit}"
 
 
 class UnmanagedRateLimitOverWarning(TwitterApiWarning):
     @property
     def message(self) -> str:
-        return f"管理していないレートリミットに遭遇しました。"
+        return "管理していないレートリミットに遭遇しました。"
```

### Comparing `twitter_api_py-0.2.0/PKG-INFO` & `twitter_api_py-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Twitter API Client by Typed Python.
 Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -53,29 +53,30 @@
 The simplest way to use the library is as follows:
 
 ```python
 from twitter_api import TwitterApiClient
 
 with TwitterApiClient.from_oauth2_app_env() as twitter_client:
     response_body = (
-        twitter_client.request("https://api.twitter.com/2/tweets")
+        twitter_client.chain()
+        .request("https://api.twitter.com/2/tweets")
         .get({
             "ids": "1460323737035677698",
             "expansions": ["referenced_tweets.id"]
         })
     )
 ```
 
 As a characteristic feature of the library, it explicitly prompts the user to write the Endpoint URL, which makes it clear from the source code which Twitter API is being called.
 
 ## Test Code
 
 A mock client is provided by the library to simplify the writing of test code.
 
-This client has the same interface as TwitterApiClient/TwitterApiAsyncClient, and also provides methods (`inject_*_response_body`) for injecting test data.
+This client has the same interface as `TwitterApiClient`/`TwitterApiAsyncClient`, and also provides methods (`inject_*_response_body`) for injecting test data.
 
 ```python
 from twitter_api import TwitterApiClient
 from twitter_api.client.twitter_api_mock_client import TwitterApiMockClient
 
 def your_logic(twitter_client: TwitterApiClient):
     ...
```

