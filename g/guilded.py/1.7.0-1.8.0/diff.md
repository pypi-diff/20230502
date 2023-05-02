# Comparing `tmp/guilded.py-1.7.0.tar.gz` & `tmp/guilded.py-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\shay\Documents\GitHub\guilded.py\dist\.tmp-o0fqf4a1\guilded.py-1.7.0.tar", last modified: Sat Mar  4 22:54:33 2023, max compression
+gzip compressed data, was "C:\Users\shay\Documents\GitHub\guilded.py\dist\.tmp-mvl_fg2u\guilded.py-1.8.0.tar", last modified: Tue May  2 00:02:33 2023, max compression
```

## Comparing `guilded.py-1.7.0.tar` & `guilded.py-1.8.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:33.308623 guilded.py-1.7.0/
--rw-rw-rw-   0        0        0     2402 2021-08-25 00:53:36.000000 guilded.py-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     2101 2023-03-04 22:54:33.307623 guilded.py-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2022-12-18 15:12:28.000000 guilded.py-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:32.979623 guilded.py-1.7.0/guilded/
--rw-rw-rw-   0        0        0      756 2023-03-04 22:47:59.000000 guilded.py-1.7.0/guilded/__init__.py
--rw-rw-rw-   0        0        0    25648 2023-02-09 20:51:56.000000 guilded.py-1.7.0/guilded/abc.py
--rw-rw-rw-   0        0        0     2724 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/activity.py
--rw-rw-rw-   0        0        0    20033 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/asset.py
--rw-rw-rw-   0        0        0     3254 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/backoff.py
--rw-rw-rw-   0        0        0   121895 2023-02-09 22:16:25.000000 guilded.py-1.7.0/guilded/channel.py
--rw-rw-rw-   0        0        0    31234 2022-11-21 13:50:28.000000 guilded.py-1.7.0/guilded/client.py
--rw-rw-rw-   0        0        0    12981 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/colour.py
--rw-rw-rw-   0        0        0    20078 2023-02-28 00:33:59.000000 guilded.py-1.7.0/guilded/embed.py
--rw-rw-rw-   0        0        0     9002 2023-01-20 17:23:19.000000 guilded.py-1.7.0/guilded/emote.py
--rw-rw-rw-   0        0        0    13786 2023-02-07 18:15:39.000000 guilded.py-1.7.0/guilded/enums.py
--rw-rw-rw-   0        0        0     4836 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/errors.py
--rw-rw-rw-   0        0        0    73035 2023-03-04 14:37:33.000000 guilded.py-1.7.0/guilded/events.py
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:32.594870 guilded.py-1.7.0/guilded/ext/
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:33.122623 guilded.py-1.7.0/guilded/ext/commands/
--rw-rw-rw-   0        0        0      199 2022-10-16 15:08:32.000000 guilded.py-1.7.0/guilded/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     1938 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/commands/_types.py
--rw-rw-rw-   0        0        0    35354 2022-10-16 15:22:10.000000 guilded.py-1.7.0/guilded/ext/commands/bot.py
--rw-rw-rw-   0        0        0    18115 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/commands/cog.py
--rw-rw-rw-   0        0        0     6658 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/commands/context.py
--rw-rw-rw-   0        0        0    35791 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/commands/converters.py
--rw-rw-rw-   0        0        0    15030 2022-10-16 15:09:19.000000 guilded.py-1.7.0/guilded/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    60064 2022-10-16 17:11:48.000000 guilded.py-1.7.0/guilded/ext/commands/core.py
--rw-rw-rw-   0        0        0    30211 2022-10-16 17:27:04.000000 guilded.py-1.7.0/guilded/ext/commands/errors.py
--rw-rw-rw-   0        0        0    50177 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/commands/help.py
--rw-rw-rw-   0        0        0     7466 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:33.135622 guilded.py-1.7.0/guilded/ext/tasks/
--rw-rw-rw-   0        0        0    18800 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0    13190 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/file.py
--rw-rw-rw-   0        0        0     5232 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/flowbot.py
--rw-rw-rw-   0        0        0    53214 2023-03-04 14:30:44.000000 guilded.py-1.7.0/guilded/gateway.py
--rw-rw-rw-   0        0        0     8221 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/group.py
--rw-rw-rw-   0        0        0    40982 2023-02-28 00:39:00.000000 guilded.py-1.7.0/guilded/http.py
--rw-rw-rw-   0        0        0     3803 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/invite.py
--rw-rw-rw-   0        0        0    35155 2022-11-21 13:48:53.000000 guilded.py-1.7.0/guilded/message.py
--rw-rw-rw-   0        0        0     2873 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/mixins.py
--rw-rw-rw-   0        0        0    32359 2022-11-20 03:58:31.000000 guilded.py-1.7.0/guilded/permissions.py
--rw-rw-rw-   0        0        0     3224 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/presence.py
--rw-rw-rw-   0        0        0    10648 2022-11-21 13:58:08.000000 guilded.py-1.7.0/guilded/reaction.py
--rw-rw-rw-   0        0        0    12987 2023-03-01 00:08:28.000000 guilded.py-1.7.0/guilded/reply.py
--rw-rw-rw-   0        0        0     7459 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/role.py
--rw-rw-rw-   0        0        0    40337 2022-12-16 17:33:10.000000 guilded.py-1.7.0/guilded/server.py
--rw-rw-rw-   0        0        0     5309 2022-10-15 20:18:59.000000 guilded.py-1.7.0/guilded/status.py
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:33.284624 guilded.py-1.7.0/guilded/types/
--rw-rw-rw-   0        0        0     2814 2023-02-07 13:47:48.000000 guilded.py-1.7.0/guilded/types/calendar_event.py
--rw-rw-rw-   0        0        0     1967 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/types/channel.py
--rw-rw-rw-   0        0        0      225 2023-01-23 20:13:53.000000 guilded.py-1.7.0/guilded/types/comment.py
--rw-rw-rw-   0        0        0     1639 2023-02-09 20:44:26.000000 guilded.py-1.7.0/guilded/types/doc.py
--rw-rw-rw-   0        0        0     1995 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/types/embed.py
--rw-rw-rw-   0        0        0     1324 2023-01-20 17:10:42.000000 guilded.py-1.7.0/guilded/types/emote.py
--rw-rw-rw-   0        0        0     1774 2023-02-02 18:56:59.000000 guilded.py-1.7.0/guilded/types/forum_topic.py
--rw-rw-rw-   0        0        0     5040 2023-03-04 14:14:52.000000 guilded.py-1.7.0/guilded/types/gateway.py
--rw-rw-rw-   0        0        0     2027 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/types/list_item.py
--rw-rw-rw-   0        0        0     1927 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/types/message.py
--rw-rw-rw-   0        0        0     1880 2023-02-28 23:34:51.000000 guilded.py-1.7.0/guilded/types/reaction.py
--rw-rw-rw-   0        0        0     1799 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/types/role.py
--rw-rw-rw-   0        0        0     1689 2022-10-27 15:22:52.000000 guilded.py-1.7.0/guilded/types/server.py
--rw-rw-rw-   0        0        0     1508 2023-02-28 00:17:19.000000 guilded.py-1.7.0/guilded/types/social_link.py
--rw-rw-rw-   0        0        0     2604 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/types/user.py
--rw-rw-rw-   0        0        0     3029 2023-02-02 16:43:38.000000 guilded.py-1.7.0/guilded/types/webhook.py
--rw-rw-rw-   0        0        0    23646 2023-02-28 00:26:43.000000 guilded.py-1.7.0/guilded/user.py
--rw-rw-rw-   0        0        0    13639 2022-12-16 17:30:53.000000 guilded.py-1.7.0/guilded/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:33.306623 guilded.py-1.7.0/guilded/webhook/
--rw-rw-rw-   0        0        0       23 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/webhook/__init__.py
--rw-rw-rw-   0        0        0    37555 2022-10-15 20:19:00.000000 guilded.py-1.7.0/guilded/webhook/async_.py
--rw-rw-rw-   0        0        0        0 2022-08-13 03:46:11.000000 guilded.py-1.7.0/guilded/webhook/sync.py
-drwxrwxrwx   0        0        0        0 2023-03-04 22:54:33.000623 guilded.py-1.7.0/guilded.py.egg-info/
--rw-rw-rw-   0        0        0     2101 2023-03-04 22:54:32.000000 guilded.py-1.7.0/guilded.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1585 2023-03-04 22:54:32.000000 guilded.py-1.7.0/guilded.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 22:54:32.000000 guilded.py-1.7.0/guilded.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-03-04 22:54:32.000000 guilded.py-1.7.0/guilded.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-04 22:54:32.000000 guilded.py-1.7.0/guilded.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-04 22:54:33.308623 guilded.py-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1608 2022-09-23 00:42:16.000000 guilded.py-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.159072 guilded.py-1.8.0/
+-rw-rw-rw-   0        0        0     2402 2021-08-25 00:53:36.000000 guilded.py-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2101 2023-05-02 00:02:33.158071 guilded.py-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2022-12-18 15:12:28.000000 guilded.py-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.108071 guilded.py-1.8.0/guilded/
+-rw-rw-rw-   0        0        0      756 2023-05-02 00:01:04.000000 guilded.py-1.8.0/guilded/__init__.py
+-rw-rw-rw-   0        0        0    25648 2023-02-09 20:51:56.000000 guilded.py-1.8.0/guilded/abc.py
+-rw-rw-rw-   0        0        0     2724 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/activity.py
+-rw-rw-rw-   0        0        0    20033 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/asset.py
+-rw-rw-rw-   0        0        0     3254 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/backoff.py
+-rw-rw-rw-   0        0        0   126012 2023-04-30 21:55:55.000000 guilded.py-1.8.0/guilded/channel.py
+-rw-rw-rw-   0        0        0    31299 2023-04-18 03:46:37.000000 guilded.py-1.8.0/guilded/client.py
+-rw-rw-rw-   0        0        0    12981 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/colour.py
+-rw-rw-rw-   0        0        0    19980 2023-04-05 23:14:18.000000 guilded.py-1.8.0/guilded/embed.py
+-rw-rw-rw-   0        0        0     9002 2023-01-20 17:23:19.000000 guilded.py-1.8.0/guilded/emote.py
+-rw-rw-rw-   0        0        0    13786 2023-02-07 18:15:39.000000 guilded.py-1.8.0/guilded/enums.py
+-rw-rw-rw-   0        0        0     4836 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/errors.py
+-rw-rw-rw-   0        0        0    85178 2023-04-18 04:05:51.000000 guilded.py-1.8.0/guilded/events.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.065070 guilded.py-1.8.0/guilded/ext/
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.135073 guilded.py-1.8.0/guilded/ext/commands/
+-rw-rw-rw-   0        0        0      199 2022-10-16 15:08:32.000000 guilded.py-1.8.0/guilded/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1938 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    35354 2022-10-16 15:22:10.000000 guilded.py-1.8.0/guilded/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    18115 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/cog.py
+-rw-rw-rw-   0        0        0     6658 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/context.py
+-rw-rw-rw-   0        0        0    35791 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/converters.py
+-rw-rw-rw-   0        0        0    15030 2022-10-16 15:09:19.000000 guilded.py-1.8.0/guilded/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    60064 2022-10-16 17:11:48.000000 guilded.py-1.8.0/guilded/ext/commands/core.py
+-rw-rw-rw-   0        0        0    30211 2022-10-16 17:27:04.000000 guilded.py-1.8.0/guilded/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    50177 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/help.py
+-rw-rw-rw-   0        0        0     7466 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.136073 guilded.py-1.8.0/guilded/ext/tasks/
+-rw-rw-rw-   0        0        0    18800 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0    13190 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/file.py
+-rw-rw-rw-   0        0        0     5232 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/flowbot.py
+-rw-rw-rw-   0        0        0    57511 2023-04-17 23:12:58.000000 guilded.py-1.8.0/guilded/gateway.py
+-rw-rw-rw-   0        0        0     8221 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/group.py
+-rw-rw-rw-   0        0        0    45910 2023-04-30 21:58:18.000000 guilded.py-1.8.0/guilded/http.py
+-rw-rw-rw-   0        0        0     3803 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/invite.py
+-rw-rw-rw-   0        0        0    35256 2023-04-30 22:02:49.000000 guilded.py-1.8.0/guilded/message.py
+-rw-rw-rw-   0        0        0     2873 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/mixins.py
+-rw-rw-rw-   0        0        0    32359 2022-11-20 03:58:31.000000 guilded.py-1.8.0/guilded/permissions.py
+-rw-rw-rw-   0        0        0     3224 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/presence.py
+-rw-rw-rw-   0        0        0    10648 2022-11-21 13:58:08.000000 guilded.py-1.8.0/guilded/reaction.py
+-rw-rw-rw-   0        0        0    16453 2023-04-30 21:56:02.000000 guilded.py-1.8.0/guilded/reply.py
+-rw-rw-rw-   0        0        0     7459 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/role.py
+-rw-rw-rw-   0        0        0    40337 2023-03-31 00:17:06.000000 guilded.py-1.8.0/guilded/server.py
+-rw-rw-rw-   0        0        0     5309 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/status.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.154072 guilded.py-1.8.0/guilded/types/
+-rw-rw-rw-   0        0        0     1600 2023-04-17 22:54:44.000000 guilded.py-1.8.0/guilded/types/announcement.py
+-rw-rw-rw-   0        0        0     3011 2023-03-25 15:03:09.000000 guilded.py-1.8.0/guilded/types/calendar_event.py
+-rw-rw-rw-   0        0        0     1967 2023-04-30 22:01:39.000000 guilded.py-1.8.0/guilded/types/channel.py
+-rw-rw-rw-   0        0        0      225 2023-01-23 20:13:53.000000 guilded.py-1.8.0/guilded/types/comment.py
+-rw-rw-rw-   0        0        0     1639 2023-02-09 20:44:26.000000 guilded.py-1.8.0/guilded/types/doc.py
+-rw-rw-rw-   0        0        0     1995 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/embed.py
+-rw-rw-rw-   0        0        0     1324 2023-01-20 17:10:42.000000 guilded.py-1.8.0/guilded/types/emote.py
+-rw-rw-rw-   0        0        0     1774 2023-02-02 18:56:59.000000 guilded.py-1.8.0/guilded/types/forum_topic.py
+-rw-rw-rw-   0        0        0     5515 2023-04-17 22:58:37.000000 guilded.py-1.8.0/guilded/types/gateway.py
+-rw-rw-rw-   0        0        0     2027 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/list_item.py
+-rw-rw-rw-   0        0        0     1958 2023-04-30 22:01:12.000000 guilded.py-1.8.0/guilded/types/message.py
+-rw-rw-rw-   0        0        0     2050 2023-04-17 22:55:33.000000 guilded.py-1.8.0/guilded/types/reaction.py
+-rw-rw-rw-   0        0        0     1799 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/role.py
+-rw-rw-rw-   0        0        0     1689 2022-10-27 15:22:52.000000 guilded.py-1.8.0/guilded/types/server.py
+-rw-rw-rw-   0        0        0     1508 2023-02-28 00:17:19.000000 guilded.py-1.8.0/guilded/types/social_link.py
+-rw-rw-rw-   0        0        0     2604 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/user.py
+-rw-rw-rw-   0        0        0     3029 2023-02-02 16:43:38.000000 guilded.py-1.8.0/guilded/types/webhook.py
+-rw-rw-rw-   0        0        0    23674 2023-03-28 22:16:34.000000 guilded.py-1.8.0/guilded/user.py
+-rw-rw-rw-   0        0        0    13639 2022-12-16 17:30:53.000000 guilded.py-1.8.0/guilded/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.157074 guilded.py-1.8.0/guilded/webhook/
+-rw-rw-rw-   0        0        0       23 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/webhook/__init__.py
+-rw-rw-rw-   0        0        0    37555 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/webhook/async_.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 03:46:11.000000 guilded.py-1.8.0/guilded/webhook/sync.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.122099 guilded.py-1.8.0/guilded.py.egg-info/
+-rw-rw-rw-   0        0        0     2101 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1615 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 00:02:33.159072 guilded.py-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2022-09-23 00:42:16.000000 guilded.py-1.8.0/setup.py
```

### Comparing `guilded.py-1.7.0/LICENSE` & `guilded.py-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/PKG-INFO` & `guilded.py-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guilded.py
-Version: 1.7.0
+Version: 1.8.0
 Summary: An API wrapper in Python for Guilded's bot API
 Home-page: https://github.com/shayypy/guilded.py
 Author: shay (shayypy)
 License: MIT
 Project-URL: Documentation, https://guildedpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/shayypy/guilded.py/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `guilded.py-1.7.0/README.md` & `guilded.py-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/__init__.py` & `guilded.py-1.8.0/guilded/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 __copyright__ = 'shay 2020-present'
-__version__ = '1.7.0'
+__version__ = '1.8.0'
 
 import logging
 
 from . import abc as abc, utils as utils
 from .utils import Object as Object
 from .asset import *
 from .channel import *
```

### Comparing `guilded.py-1.7.0/guilded/abc.py` & `guilded.py-1.8.0/guilded/abc.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/activity.py` & `guilded.py-1.8.0/guilded/activity.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/asset.py` & `guilded.py-1.8.0/guilded/asset.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/backoff.py` & `guilded.py-1.8.0/guilded/backoff.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/channel.py` & `guilded.py-1.8.0/guilded/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,33 +59,35 @@
 
 from .asset import Asset
 from .colour import Colour
 from .enums import ChannelType, CustomRepeatInterval, DeleteSeriesType, FileType, RSVPStatus, RepeatInterval, Weekday, try_enum
 from .group import Group
 from .message import HasContentMixin
 from .mixins import Hashable
-from .reply import CalendarEventReply, DocReply, ForumTopicReply
+from .reply import AnnouncementReply, CalendarEventReply, DocReply, ForumTopicReply
 from .user import Member
 from .utils import GUILDED_EPOCH_DATETIME, MISSING, ISO8601, Object
 from .status import Game
 
 if TYPE_CHECKING:
+    from .types.announcement import Announcement as AnnouncementPayload
     from .types.calendar_event import (
         CalendarEvent as CalendarEventPayload,
         CalendarEventRsvp as CalendarEventRsvpPayload,
         RepeatInfo as RepeatInfoPayload,
     )
     from .types.doc import Doc as DocPayload
     from .types.list_item import (
         ListItem as ListItemPayload,
         ListItemNote as ListItemNotePayload,
     )
     from .types.forum_topic import ForumTopic as ForumTopicPayload
 
     from .emote import Emote
+    from .role import Role
     from .server import Server
     from .user import User
     from .webhook import Webhook
 
 
 __all__ = (
     'Announcement',
@@ -118,53 +120,76 @@
     """Represents a calendar channel in a :class:`.Server`."""
     def __init__(self, **fields):
         super().__init__(**fields)
         self.type = ChannelType.calendar
 
     async def create_event(
         self,
-        *,
         name: str,
+        *,
         starts_at: Optional[datetime.datetime],
-        duration: Optional[Union[datetime.timedelta, int]],
+        duration: Optional[Union[datetime.timedelta, int]] = MISSING,
         description: Optional[str] = MISSING,
         location: Optional[str] = MISSING,
         url: Optional[str] = MISSING,
         colour: Optional[Union[Colour, int]] = MISSING,
         color: Optional[Union[Colour, int]] = MISSING,
+        all_day: bool = MISSING,
         rsvp_limit: Optional[int] = MISSING,
+        rsvp_disabled: bool = MISSING,
+        autofill_waitlist: bool = MISSING,
         private: bool = MISSING,
+        roles: Optional[List[Role]] = MISSING,
         repeat: Optional[Union[RepeatInterval, RepeatInfo]] = MISSING,
     ) -> CalendarEvent:
         """|coro|
 
         Create an event in this channel.
 
         Parameters
         -----------
         name: :class:`str`
             The name of the event.
         starts_at: :class:`datetime.datetime`
             When the event starts.
-        duration: Union[:class:`datetime.timedelta`, :class:`int`]
+        duration: Optional[Union[:class:`datetime.timedelta`, :class:`int`]]
             The duration of the event.
             If this is an :class:`int`, the value must be in minutes.
         description: Optional[:class:`str`]
             The description of the event.
         location: Optional[:class:`str`]
             The location of the event.
         url: Optional[:class:`str`]
             A URL to associate with the event.
         colour: Optional[Union[:class:`.Colour`, :class:`int`]]
             The colour of the event when viewing in the channel.
             This parameter is also aliased to ``color``.
+        all_day: Optional[:class:`bool`]
+            Whether the event should last all day.
+
+            .. versionadded:: 1.8
         rsvp_limit: Optional[:class:`int`]
             The number of RSVPs to allow before waitlisting.
+
+            .. versionadded:: 1.7
+        rsvp_disabled: Optional[:class:`bool`]
+            Whether users should be disallowed from creating RSVPs for the event.
+
+            .. versionadded:: 1.8
+        autofill_waitlist: Optional[:class:`bool`]
+            When ``rsvp_limit`` is set, whether users from the waitlist should
+            be added as space becomes available in the event.
+
+            .. versionadded:: 1.8
         private: Optional[:class:`bool`]
             Whether the event should be private.
+        roles: Optional[List[:class:`Role`]]
+            The roles to restrict the event to.
+
+            .. versionadded:: 1.8
         repeat: Optional[Union[:class:`RepeatInterval`, :class:`RepeatInfo`]]
             A basic interval for repeating the event or a :class:`RepeatInfo`
             for more detailed repeat options.
 
             .. versionadded:: 1.7
 
         Returns
@@ -212,17 +237,29 @@
                 duration = duration.seconds / 60
 
             payload['duration'] = duration
 
         if private is not MISSING:
             payload['isPrivate'] = private
 
+        if all_day is not MISSING:
+            payload['isAllDay'] = all_day
+
         if rsvp_limit is not MISSING:
             payload['rsvpLimit'] = rsvp_limit
 
+        if rsvp_disabled is not MISSING:
+            payload['rsvpDisabled'] = rsvp_disabled
+
+        if autofill_waitlist is not MISSING:
+            payload['autofillWaitlist'] = autofill_waitlist
+
+        if roles is not MISSING and roles is not None:
+            payload['roleIds'] = [role.id for role in roles]
+
         if repeat is not MISSING:
             if isinstance(repeat, RepeatInterval):
                 payload['repeatInfo'] = RepeatInfo(repeat).to_dict()
             elif isinstance(repeat, RepeatInfo):
                 payload['repeatInfo'] = repeat.to_dict()
 
         data = await self._state.create_calendar_event(self.id, payload=payload)
@@ -388,18 +425,40 @@
         users while creating the event.
     private: :class:`bool`
         Whether the event is private.
     repeats: :class:`bool`
         Whether the event is set to repeat.
 
         .. versionadded:: 1.7
+    series_id: Optional[:class:`str`]
+        The ID of the event series, if applicable.
+
+        .. versionadded:: 1.8
+    role_ids: List[:class:`int`]
+        The role IDs that the event is restricted to.
+        If the event is not restricted, this list is empty.
+
+        .. versionadded:: 1.8
+    all_day: :class:`bool`
+        Whether the event lasts all day.
+
+        .. versionadded:: 1.8
     rsvp_limit: Optional[:class:`int`]
         The number of RSVPs to allow before waitlisting RSVPs.
 
         .. versionadded:: 1.7
+    rsvp_disabled: Optional[:class:`bool`]
+        Whether users are disallowed from creating RSVPs for the event.
+
+        .. versionadded:: 1.8
+    autofill_waitlist: Optional[:class:`bool`]
+        When ``rsvp_limit`` is set, whether users from the waitlist should
+        be added as space becomes available in the event.
+
+        .. versionadded:: 1.8
     duration: Optional[:class:`datetime.timedelta`]
         The duration of the event. Minimum 60 seconds.
     cancellation_description: Optional[:class:`str`]
         The description of the event cancellation, if any.
 
         There is an alias for this attribute called :attr:`.cancelation_description`.
     """
@@ -416,15 +475,20 @@
         '_mentions',
         'location',
         'url',
         'starts_at',
         'created_at',
         'private',
         'repeats',
+        'series_id',
+        'role_ids',
+        'all_day',
         'rsvp_limit',
+        'rsvp_disabled',
+        'autofill_waitlist',
         '_colour',
         'duration',
         'cancellation_description',
         'cancelled_by_id',
     )
 
     def __init__(self, *, state, data: CalendarEventPayload, channel: CalendarChannel):
@@ -444,15 +508,20 @@
 
         self.location = data.get('location')
         self.url = data.get('url')
         self.starts_at: datetime.datetime = ISO8601(data.get('startsAt'))
         self.created_at: datetime.datetime = ISO8601(data.get('createdAt'))
         self.private = data.get('isPrivate') or False
         self.repeats = data.get('repeats') or False
+        self.series_id = data.get('seriesId')
+        self.role_ids = data.get('roleIds') or []
+        self.all_day = data.get('isAllDay') or False
         self.rsvp_limit = data.get('rsvpLimit')
+        self.rsvp_disabled = data.get('rsvpDisabled') or False
+        self.autofill_waitlist = data.get('autofillWaitlist') or False
         self._colour = data.get('color')
 
         self.duration: Optional[datetime.timedelta]
         _duration = data.get('duration')  # minutes
         if _duration is not None:
             self.duration = datetime.timedelta(minutes=_duration)
         else:
@@ -536,27 +605,40 @@
         """
         return self.server.get_member(self.cancelled_by_id)
 
     @property
     def share_url(self) -> str:
         return f'{self.channel.share_url}/{self.id}'
 
+    @property
+    def roles(self) -> List[Role]:
+        """List[:class:`Role`]: The roles that the event is restricted to.
+        If the event is not restricted, this list is empty.
+
+        .. versionadded:: 1.8
+        """
+        return [self.server.get_role(role_id) for role_id in self.role_ids]
+
     async def edit(
         self,
         *,
         name: str = MISSING,
         description: Optional[str] = MISSING,
         location: Optional[str] = MISSING,
         starts_at: Optional[datetime.datetime] = MISSING,
         url: Optional[str] = MISSING,
         colour: Optional[Union[Colour, int]] = MISSING,
         color: Optional[Union[Colour, int]] = MISSING,
         duration: Optional[Union[datetime.timedelta, int]] = MISSING,
+        all_day: bool = MISSING,
         rsvp_limit: Optional[int] = MISSING,
+        rsvp_disabled: bool = MISSING,
+        autofill_waitlist: bool = MISSING,
         private: bool = MISSING,
+        roles: Optional[List[Role]] = MISSING,
         repeat: Optional[Union[RepeatInterval, RepeatInfo]] = MISSING,
         edit_series: bool = MISSING,
     ) -> CalendarEvent:
         """|coro|
 
         Edit this event.
 
@@ -576,18 +658,37 @@
             A URL to associate with the event.
         colour: Union[:class:`.Colour`, :class:`int`]
             The colour of the event when viewing in the channel.
             This parameter is also aliased to ``color``.
         duration: Union[:class:`datetime.timedelta`, :class:`int`]
             The duration of the event.
             If this is an :class:`int`, the value must be in minutes.
+        all_day: Optional[:class:`bool`]
+            Whether the event should last all day.
+
+            .. versionadded:: 1.8
         rsvp_limit: Optional[:class:`int`]
             The number of RSVPs to allow before waitlisting.
+
+            .. versionadded:: 1.7
+        rsvp_disabled: Optional[:class:`bool`]
+            Whether users should be disallowed from creating RSVPs for the event.
+
+            .. versionadded:: 1.8
+        autofill_waitlist: Optional[:class:`bool`]
+            When ``rsvp_limit`` is set, whether users from the waitlist should
+            be added as space becomes available in the event.
+
+            .. versionadded:: 1.8
         private: :class:`bool`
             Whether the event should be private.
+        roles: Optional[List[:class:`Role`]]
+            The roles to restrict the event to.
+
+            .. versionadded:: 1.8
         repeat: Optional[Union[:class:`RepeatInterval`, :class:`RepeatInfo`]]
             A basic interval for repeating the event or a :class:`RepeatInfo`
             for more detailed repeat options.
 
             .. versionadded:: 1.7
         edit_series: :class:`bool`
             Whether to also edit all future events in the series, if
@@ -643,17 +744,29 @@
                 duration = duration.seconds / 60
 
             payload['duration'] = duration
 
         if private is not MISSING:
             payload['isPrivate'] = private
 
+        if all_day is not MISSING:
+            payload['isAllDay'] = all_day
+
         if rsvp_limit is not MISSING:
             payload['rsvpLimit'] = rsvp_limit
 
+        if rsvp_disabled is not MISSING:
+            payload['rsvpDisabled'] = rsvp_disabled
+
+        if autofill_waitlist is not MISSING:
+            payload['autofillWaitlist'] = autofill_waitlist
+
+        if roles is not MISSING:
+            payload['roleIds'] = [role.id for role in (roles or [])]
+
         if repeat is not MISSING:
             if isinstance(repeat, RepeatInterval):
                 payload['repeatInfo'] = RepeatInfo(repeat).to_dict()
             elif isinstance(repeat, RepeatInfo):
                 payload['repeatInfo'] = repeat.to_dict()
             else:
                 payload['repeatInfo'] = None
@@ -726,27 +839,56 @@
         -------
         Forbidden
             You do not have permissions to create an RSVP for another user.
         HTTPException
             Failed to create an RSVP.
         """
 
-        payload = {
-            'status': status.value,
-        }
-
         data = await self._state.put_calendar_event_rsvp(
             self.channel_id,
             self.id,
             user.id,
-            payload=payload,
+            status=status.value,
         )
         rsvp = CalendarEventRSVP(data=data['calendarEventRsvp'], event=self)
         return rsvp
 
+    async def upsert_rsvps(
+        self,
+        *users: guilded.abc.User,
+        status: RSVPStatus,
+    ) -> None:
+        """|coro|
+
+        Upsert (conditionally create or edit) RSVPs for multiple users.
+
+        .. versionadded:: 1.8
+
+        Parameters
+        -----------
+        \*users: :class:`~.abc.User`
+            The users to upsert RSVPs for.
+        status: :class:`.RSVPStatus`
+            The status of the RSVPs.
+
+        Raises
+        -------
+        Forbidden
+            You do not have permissions to upsert RSVPs for other users.
+        HTTPException
+            Failed to upsert RSVPs.
+        """
+
+        await self._state.upsert_calendar_event_rsvps(
+            self.channel_id,
+            self.id,
+            [user.id for user in users],
+            status=status.value,
+        )
+
     async def fetch_rsvp(self, user: guilded.abc.User, /) -> CalendarEventRSVP:
         """|coro|
 
         Fetch a user's RSVP to this event.
 
         Returns
         --------
@@ -798,30 +940,30 @@
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_calendar_event_reaction_emote(self.channel_id, self.id, emote_id)
+        await self._state.add_calendar_event_reaction(self.channel_id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this event.
 
         .. versionadded:: 1.7
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_calendar_event_reaction_emote(self.channel_id, self.id, emote_id)
+        await self._state.remove_calendar_event_reaction(self.channel_id, self.id, emote_id)
 
     async def reply(self, content: str) -> CalendarEventReply:
         """|coro|
 
         Reply to this event.
 
         .. versionadded:: 1.7
@@ -860,15 +1002,15 @@
         --------
         :class:`CalendarEventReply`
             The reply from the ID.
 
         Raises
         -------
         NotFound
-            This reply or topic does not exist.
+            This reply or event does not exist.
         Forbidden
             You do not have permission to read this event's replies.
         HTTPException
             Failed to fetch the reply.
         """
 
         data = await self._state.get_calendar_event_comment(self.channel_id, self.id, reply_id)
@@ -1318,14 +1460,40 @@
         return self.server.get_member(self.author_id)
 
     @property
     def updated_by(self) -> Optional[Member]:
         """Optional[:class:`.Member`]: The :class:`.Member` that last updated the doc."""
         return self.server.get_member(self.updated_by_id)
 
+    async def add_reaction(self, emote: Emote, /) -> None:
+        """|coro|
+
+        Add a reaction to this doc.
+
+        Parameters
+        -----------
+        emote: :class:`.Emote`
+            The emote to add.
+        """
+        emote_id: int = getattr(emote, 'id', emote)
+        await self._state.add_doc_reaction(self.channel.id, self.id, emote_id)
+
+    async def remove_self_reaction(self, emote: Emote, /) -> None:
+        """|coro|
+
+        Remove one of your reactions from this doc.
+
+        Parameters
+        -----------
+        emote: :class:`.Emote`
+            The emote to remove.
+        """
+        emote_id: int = getattr(emote, 'id', emote)
+        await self._state.remove_doc_reaction(self.channel.id, self.id, emote_id)
+
     async def delete(self) -> None:
         """|coro|
 
         Delete this doc.
         """
         await self._state.delete_doc(self.channel.id, self.id)
 
@@ -1402,15 +1570,15 @@
         --------
         :class:`DocReply`
             The reply from the ID.
 
         Raises
         -------
         NotFound
-            This reply or topic does not exist.
+            This reply or doc does not exist.
         Forbidden
             You do not have permission to read this doc's replies.
         HTTPException
             Failed to fetch the reply.
         """
 
         data = await self._state.get_doc_comment(self.channel_id, self.id, reply_id)
@@ -1660,28 +1828,28 @@
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_forum_topic_reaction_emote(self.channel.id, self.id, emote_id)
+        await self._state.add_forum_topic_reaction(self.channel.id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this topic.
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_forum_topic_reaction_emote(self.channel.id, self.id, emote_id)
+        await self._state.remove_forum_topic_reaction(self.channel.id, self.id, emote_id)
 
     async def edit(
         self,
         *,
         title: str = MISSING,
         content: str = MISSING,
     ) -> ForumTopic:
@@ -2241,54 +2409,58 @@
 
             Returns the hash of the announcement.
 
         .. describe:: str(x)
 
             Returns the title of the announcement.
 
+    .. versionadded:: 1.8
+
     Attributes
     -----------
     id: :class:`str`
         The announcement's ID.
     title: :class:`str`
         The announcement's title.
     content: :class:`str`
         The announcement's text content.
     channel: :class:`.AnnouncementChannel`
         The channel that the announcement is in.
-    public: :class:`bool`
-        Whether the announcement is public.
-    pinned: :class:`bool`
-        Whether the announcement is pinned.
     created_at: :class:`datetime.datetime`
         When the announcement was created.
-    updated_at: Optional[:class:`datetime.datetime`]
-        When the announcement was last updated.
-    slug: Optional[:class:`str`]
-        The announcement's blog URL slug.
     """
 
-    def __init__(self, *, state, data, channel: AnnouncementChannel):
+    __slots__: Tuple[str, ...] = (
+        '_state',
+        'channel',
+        'channel_id',
+        'server_id',
+        'id',
+        'title',
+        'content',
+        '_mentions',
+        'author_id',
+        'created_at',
+    )
+
+    def __init__(self, *, state, data: AnnouncementPayload, channel: AnnouncementChannel):
         super().__init__()
         self._state = state
         self.channel = channel
-        self.tags: str = data.get('tags')
-        self._replies = {}
-
-        self.public: bool = data.get('isPublic', False)
-        self.pinned: bool = data.get('isPinned', False)
-        self.slug: Optional[str] = data.get('slug')
+        self.channel_id = data['channelId']
+        self.server_id = data.get('serverId')
 
-        self.author_id: str = data.get('createdBy')
-        self.created_at: datetime.datetime = ISO8601(data.get('createdAt'))
-        self.updated_at: Optional[datetime.datetime] = ISO8601(data.get('editedAt'))
+        self.author_id = data.get('createdBy')
+        self.created_at = ISO8601(data.get('createdAt'))
 
-        self.id: str = data['id']
-        self.title: str = data['title']
-        self.content: str = self._get_full_content(data['content'])
+        self.id = data['id']
+        self.title = data['title']
+        self.content = data['content']
+        self._mentions = self._create_mentions(data.get('mentions'))
+        self._extract_attachments(self.content)
 
     def __repr__(self) -> str:
         return f'<Announcement id={self.id!r} title={self.title!r} channel={self.channel!r}>'
 
     def __str__(self) -> str:
         return self.title
 
@@ -2314,114 +2486,165 @@
 
     @property
     def author(self) -> Optional[Member]:
         """Optional[:class:`.Member`]: The :class:`.Member` that created the announcement."""
         return self.server.get_member(self.author_id)
 
     @property
-    def blog_url(self) -> Optional[str]:
-        """Optional[:class:`str`]: The blog URL of the announcement."""
-        if self.channel.blog_url and self.slug:
-            return f'{self.channel.blog_url}/{self.slug}'
-        return None
-
-    @property
     def share_url(self) -> str:
         return f'{self.channel.share_url}/{self.id}'
 
-    async def sticky(self) -> None:
-        """|coro|
-
-        Sticky (pin) this announcement.
-        """
-        await self._state.toggle_announcement_pin(self.channel.id, self.id, pinned=True)
-        self.pinned = True
-
-    async def unsticky(self) -> None:
-        """|coro|
-
-        Unsticky (unpin) this announcement.
-        """
-        await self._state.toggle_announcement_pin(self.channel.id, self.id, pinned=False)
-        self.pinned = False
-
-    async def pin(self) -> None:
-        """|coro|
-
-        Pin (sticky) this announcement. This is an alias of :meth:`.sticky`.
-        """
-        await self.sticky()
-
-    async def unpin(self) -> None:
-        """|coro|
-
-        Unpin (unsticky) this announcement. This is an alias of :meth:`.unsticky`.
-        """
-        await self.unsticky()
-
     async def delete(self) -> None:
         """|coro|
 
         Delete this announcement.
         """
         await self._state.delete_announcement(self.channel.id, self.id)
 
-    async def edit(self, *content, **kwargs) -> None:
+    async def edit(self, *, title: str = MISSING, content: str = MISSING) -> Announcement:
         """|coro|
 
         Edit this announcement.
 
+        All parameters are optional.
+
         Parameters
         -----------
-        \*content: Any
-            The content of the announcement.
         title: :class:`str`
             The title of the announcement.
+        content: :class:`str`
+            The content of the announcement.
+
+        Returns
+        --------
+        :class:`.Announcement`
+            The newly edited announcement.
         """
 
-        payload = {
-            'title': kwargs.pop('title', self.title),
-            'content': content,
-        }
+        payload = {}
 
-        await self._state.update_announcement(self.channel.id, self.id, payload=payload)
+        if title is not MISSING:
+            payload['title'] = title
+
+        if content is not MISSING:
+            payload['content'] = content
+
+        data = await self._state.update_announcement(self.channel.id, self.id, payload=payload)
+        return Announcement(state=self._state, data=data['announcement'], channel=self.channel)
 
     async def add_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Add a reaction to this announcement.
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
-        await self._state.add_content_reaction(self.channel.type.value, self.id, emote.id)
+        emote_id: int = getattr(emote, 'id', emote)
+        await self._state.add_announcement_reaction(self.channel.id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this announcement.
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_reaction_emote(self.channel.id, self.id, emote_id)
+        await self._state.remove_announcement_reaction(self.channel.id, self.id, emote_id)
+
+    async def reply(self, content: str) -> AnnouncementReply:
+        """|coro|
+
+        Reply to this announcement.
+
+        Parameters
+        -----------
+        content: :class:`str`
+            The content of the reply.
+
+        Returns
+        --------
+        :class:`AnnouncementReply`
+            The created reply.
+
+        Raises
+        -------
+        NotFound
+            This topic does not exist.
+        Forbidden
+            You do not have permission to reply to this topic.
+        HTTPException
+            Failed to reply to this topic.
+        """
+
+        data = await self._state.create_announcement_comment(self.channel_id, self.id, content=content)
+        return AnnouncementReply(state=self._state, data=data['announcementComment'], parent=self)
+
+    async def fetch_reply(self, reply_id: int, /) -> AnnouncementReply:
+        """|coro|
+
+        Fetch a reply to this announcement.
+
+        Returns
+        --------
+        :class:`AnnouncementReply`
+            The reply from the ID.
+
+        Raises
+        -------
+        NotFound
+            This reply or announcement does not exist.
+        Forbidden
+            You do not have permission to read this announcement's replies.
+        HTTPException
+            Failed to fetch the reply.
+        """
+
+        data = await self._state.get_announcement_comment(self.channel_id, self.id, reply_id)
+        return AnnouncementReply(state=self._state, data=data['announcementComment'], parent=self)
+
+    async def fetch_replies(self) -> List[AnnouncementReply]:
+        """|coro|
+
+        Fetch all replies to this announcement.
+
+        Returns
+        --------
+        List[:class:`AnnouncementReply`]
+            The replies under the announcement.
+
+        Raises
+        -------
+        NotFound
+            This announcement does not exist.
+        Forbidden
+            You do not have permission to read this announcement's replies.
+        HTTPException
+            Failed to fetch the replies to this announcement.
+        """
+
+        data = await self._state.get_announcement_comments(self.channel_id, self.id)
+        return [
+            AnnouncementReply(state=self._state, data=reply_data, parent=self)
+            for reply_data in data['announcementComments']
+        ]
 
 
 class AnnouncementChannel(guilded.abc.ServerChannel):
     """Represents an announcement channel in a :class:`.Server`."""
     def __init__(self, **fields):
         super().__init__(**fields)
 
         self.type = ChannelType.announcements
-        self._announcements = {}
 
     @property
     def blog_url(self) -> Optional[str]:
         """Optional[:class:`str`]: The blog URL of the announcement channel.
 
         .. note::
 
@@ -2438,123 +2661,78 @@
         if not channel_slug:
             # Guilded does not let you save an empty-when-stripped blog name
             return None
 
         server_portion = self.server.slug if self.server.slug is not None else f'teams/{self.server.id}'
         return f'https://guilded.gg/{server_portion}/blog/{channel_slug}'
 
-    @property
-    def announcements(self) -> List[Announcement]:
-        """List[:class:`.Announcement`]: The list of announcements in this channel."""
-        return list(self._announcements.values())
-
-    def get_announcement(self, id) -> Optional[Announcement]:
-        """Optional[:class:`.Announcement`]: Get an announcement from this channel."""
-        return self._announcements.get(id)
-
-    #async def getch_announcement(self, id: str) -> Announcement:
-    #    return self.get_announcement(id) or await self.fetch_announcement(id)
-
-    #async def fetch_announcement(self, id: str) -> Announcement:
-    #    """|coro|
-
-    #    Fetch an announcement in this channel.
-
-    #    Parameters
-    #    -----------
-    #    id: :class:`str`
-    #        The announcement's ID.
-
-    #    Returns
-    #    --------
-    #    :class:`.Announcement`
-    #    """
-    #    data = await self._state.get_announcement(self.id, id)
-    #    announcement = Announcement(data=data['announcement'], channel=self, state=self._state)
-    #    return announcement
-
-    #async def fetch_announcements(self, *, limit: int = 50, before: datetime.datetime = None) -> List[Announcement]:
-    #    """|coro|
-
-    #    Fetch multiple announcements in this channel.
+    async def fetch_announcement(self, announcement_id: str, /) -> Announcement:
+        """|coro|
 
-    #    All parameters are optional.
+        Fetch an announcement in this channel.
 
-    #    Parameters
-    #    -----------
-    #    limit: :class:`int`
-    #        The maximum number of announcements to return. Defaults to 50.
-    #    before: :class:`datetime.datetime`
-    #        The latest date that an announcement can be from. Defaults to the
-    #        current time.
+        Returns
+        --------
+        :class:`.Announcement`
+            The announcement from the ID.
+        """
 
-    #    Returns
-    #    --------
-    #    List[:class:`.Announcement`]
-    #    """
+        data = await self._state.get_announcement(self.id, announcement_id)
+        announcement = Announcement(data=data['announcement'], channel=self, state=self._state)
+        return announcement
 
-    #    before = before or datetime.datetime.now(datetime.timezone.utc)
-    #    data = await self._state.get_announcements(self.id, limit=limit, before=before)
-    #    announcements = []
-    #    for announcement_data in data['announcements']:
-    #        announcements.append(Announcement(data=announcement_data, channel=self, state=self._state))
+    async def fetch_announcements(self, *, limit: int = None, before: datetime.datetime = None) -> List[Announcement]:
+        """|coro|
 
-    #    return announcements
+        Fetch multiple announcements in this channel.
 
-    #async def fetch_pinned_announcements(self) -> List[Announcement]:
-    #    """|coro|
+        All parameters are optional.
 
-    #    Fetch all pinned announcements in this channel.
+        Parameters
+        -----------
+        limit: :class:`int`
+            The maximum number of announcements to return. Defaults to 25.
+        before: :class:`datetime.datetime`
+            The latest date that an announcement can be from. Defaults to the
+            current time.
 
-    #    Returns
-    #    --------
-    #    List[:class:`.Announcement`]
-    #    """
-    #    data = await self._state.get_pinned_announcements(self.id)
-    #    announcements = []
-    #    for announcement_data in data['announcements']:
-    #        announcements.append(Announcement(data=announcement_data, channel=self, state=self._state))
+        Returns
+        --------
+        List[:class:`.Announcement`]
+            The announcements in the channel.
+        """
 
-    #    return announcements
+        data = await self._state.get_announcements(self.id, limit=limit, before=before)
+        return [Announcement(data=announcement_data, channel=self, state=self._state) for announcement_data in data['announcements']]
 
-    #async def create_announcement(self, *content, **kwargs) -> Announcement:
-    #    """|coro|
+    async def create_announcement(self, *, title: str, content: str) -> Announcement:
+        """|coro|
 
-    #    Create an announcement in this channel.
+        Create an announcement in this channel.
 
-    #    Parameters
-    #    -----------
-    #    content: Any
-    #        The content of the announcement.
-    #    title: :class:`str`
-    #        The title of the announcement.
-    #    game: Optional[:class:`.Game`]
-    #        The game to be associated with this announcement.
-    #    send_notifications: Optional[:class:`bool`]
-    #        Whether to send notifications to all members ("Notify all
-    #        members" in the client). Defaults to ``True`` if not specified.
+        Parameters
+        -----------
+        title: :class:`str`
+            The title of the announcement.
+        content: :class:`str`
+            The content of the announcement.
 
-    #    Returns
-    #    --------
-    #    :class:`.Announcement`
-    #        The created announcement.
-    #    """
-    #    title = kwargs.pop('title')
-    #    game = kwargs.pop('game', None)
-    #    dont_send_notifications = not kwargs.pop('send_notifications', True)
+        Returns
+        --------
+        :class:`.Announcement`
+            The created announcement.
+        """
 
-    #    data = await self._state.create_announcement(
-    #        self.id,
-    #        title=title,
-    #        content=content,
-    #        game_id=(game.id if game else None),
-    #        dont_send_notifications=dont_send_notifications
-    #    )
-    #    announcement = Announcement(data=data['announcement'], channel=self, game=game, state=self._state)
-    #    return announcement
+        data = await self._state.create_announcement(
+            self.id,
+            title=title,
+            content=content,
+        )
+        announcement = Announcement(data=data['announcement'], channel=self, state=self._state)
+        return announcement
 
 
 class Media(Hashable, HasContentMixin):
     """Represents a media post in a :class:`.MediaChannel`.
 
     .. container:: operations
 
@@ -2685,40 +2863,14 @@
         return self.channel.group
 
     @property
     def author(self) -> Optional[Member]:
         """Optional[:class:`.Member`]: The member that created this media."""
         return self.server.get_member(self.author_id)
 
-    async def add_reaction(self, emote: Emote, /) -> None:
-        """|coro|
-
-        Add a reaction to this media post.
-
-        Parameters
-        -----------
-        emote: :class:`.Emote`
-            The emote to add.
-        """
-        emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_reaction_emote(self.channel.id, self.id, emote_id)
-
-    async def remove_self_reaction(self, emote: Emote, /) -> None:
-        """|coro|
-
-        Remove one of your reactions from this media post.
-
-        Parameters
-        -----------
-        emote: :class:`.Emote`
-            The emote to remove.
-        """
-        emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_reaction_emote(self.channel.id, self.id, emote_id)
-
     #async def reply(self, *content, **kwargs) -> MediaReply:
     #    """|coro|
 
     #    Reply to this media.
 
     #    Parameters
     #    -----------
@@ -2977,17 +3129,15 @@
 
         Returns
         --------
         :class:`.ListItemNote`
             The newly edited note.
         """
 
-        payload = {
-            'message': self.parent.message,
-        }
+        payload = {}
         if content is not MISSING and content is not None:
             payload['note'] = {
                 'content': content,
             }
 
         data = await self._state.update_list_item(
             self.channel.id,
@@ -3019,25 +3169,20 @@
     -----------
     id: :class:`str`
         The item's ID.
     created_at: :class:`datetime.datetime`
         When the item was created.
     message: :class:`str`
         The main message of the item.
-    position: :class:`int`
-        Where the item is in its :attr:`.channel`. A value of ``0`` is
-        at the bottom of the list visually.
     note: :class:`.ListItemNote`
         The item's note.
     updated_at: Optional[:class:`datetime.datetime`]
         When the item was last updated.
     completed_at: Optional[:class:`datetime.datetime`]
         When the item was marked as completed.
-    deleted_at: Optional[:class:`datetime.datetime`]
-        When the item was deleted.
     parent_id: Optional[:class:`str`]
         The ID of the item's parent, if the item is nested.
     webhook_id: Optional[:class:`str`]
         The ID of the webhook that created the item, if applicable.
     """
 
     def __init__(self, *, state, data: ListItemPayload, channel: ListChannel):
@@ -3224,16 +3369,14 @@
 
         # The parameter is named ``message`` for API compliance but we use ``content`` internally for consistency.
         content = message
 
         payload = {}
         if content is not MISSING:
             payload['message'] = content
-        else:
-            payload['message'] = self.message
 
         if note_content is not MISSING and note_content is not None:
             payload['note'] = {
                 'content': note_content
             }
 
         data = await self._state.update_list_item(
```

### Comparing `guilded.py-1.7.0/guilded/client.py` & `guilded.py-1.8.0/guilded/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -652,14 +652,30 @@
         Returns
         --------
         :class:`.Server`
             The server from the ID.
         """
         return self.get_server(server_id) or await self.fetch_server(server_id)
 
+    async def fetch_servers(self) -> List[Server]:
+        """|coro|
+
+        Fetch your list of servers from the API.
+
+        .. versionadded:: 1.8
+
+        Returns
+        --------
+        List[:class:`.Servers`]
+            The servers you are a member of.
+        """
+
+        data = await self.http.get_my_servers()
+        return [Server(state=self.http, data=server_data) for server_data in data['servers']]
+
     async def fetch_channel(self, channel_id: str) -> ServerChannel:
         """|coro|
 
         Fetch a channel from the API.
 
         Returns
         --------
@@ -718,36 +734,25 @@
             )
 
         self.http.session = aiohttp.ClientSession()
 
         await self._async_setup_hook()
         await self.setup_hook()
 
-        # Cache our internal server
-        if self.internal_server_id:
-            try:
-                server = await self.fetch_server(self.internal_server_id)
-            except HTTPException as exc:
-                # This shouldn't happen
-                log.warn(
-                    'Internal server (ID: %s) could not be fetched (%s: %s). Constructing a partial server instance instead.',
-                    self.internal_server_id,
-                    exc.status,
-                    exc.message,
-                )
-                server = Server(
-                    state=self.http,
-                    data={
-                        'id': self.internal_server_id,
-                    }
-                )
-
-            await server.fill_members()
+        # The gateway does not send the client's servers upon connecting
+        servers = await self.fetch_servers()
+        for server in servers:
             self.http.add_to_server_cache(server)
 
+        if self.internal_server_id and not self.get_server(self.internal_server_id):
+            log.warn(
+                'Internal server (ID: %s) was not found in the list of client servers.',
+                self.internal_server_id,
+            )
+
         await self.connect(token, reconnect=reconnect)
 
     async def connect(self, token: str = None, *, reconnect: bool = True) -> None:
         self.http.token = token or self.http.token
         if not self.http.token:
             raise ClientException(
                 'You must provide a token to this method explicitly, or have '
```

### Comparing `guilded.py-1.7.0/guilded/colour.py` & `guilded.py-1.8.0/guilded/colour.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/embed.py` & `guilded.py-1.8.0/guilded/embed.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,16 +97,15 @@
     Certain properties return an ``EmbedProxy``, a type
     that acts similar to a regular :class:`dict` except using dotted access,
     e.g. ``embed.author.icon_url``. If the attribute
     is invalid or empty, then a special sentinel value is returned,
     :attr:`Embed.Empty`.
 
     URL parameters (both as text and for images) accept any string, even those
-    that are not a valid URI. If an ``attachment://`` URI is passed to an image
-    parameter then it will be handled for you.
+    that are not a valid URI.
 
     For ease of use, all parameters that expect a :class:`str` are implicitly
     casted to :class:`str` for you.
 
     Attributes
     -----------
     title: :class:`str`
```

### Comparing `guilded.py-1.7.0/guilded/emote.py` & `guilded.py-1.8.0/guilded/emote.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/enums.py` & `guilded.py-1.8.0/guilded/enums.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/errors.py` & `guilded.py-1.8.0/guilded/errors.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/events.py` & `guilded.py-1.8.0/guilded/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,28 +25,30 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
 import datetime
 
 from .channel import (
+    Announcement,
+    AnnouncementChannel,
     CalendarChannel,
     CalendarEvent,
     CalendarEventRSVP,
     ChatChannel,
     Doc,
     DMChannel,
     ForumTopic,
     ListItem,
     Thread,
     VoiceChannel,
 )
 from .emote import Emote
 from .message import ChatMessage
-from .reply import CalendarEventReply, DocReply, ForumTopicReply
+from .reply import AnnouncementReply, CalendarEventReply, DocReply, ForumTopicReply
 from .user import Member, MemberBan, SocialLink
 from .utils import ISO8601
 from .webhook.async_ import Webhook
 
 if TYPE_CHECKING:
     from .types import gateway as gw
 
@@ -80,14 +82,24 @@
     'MemberSocialLinkDeleteEvent',
     'BulkMemberXpAddEvent',
     'ServerChannelCreateEvent',
     'ServerChannelUpdateEvent',
     'ServerChannelDeleteEvent',
     'WebhookCreateEvent',
     'WebhookUpdateEvent',
+    'AnnouncementCreateEvent',
+    'AnnouncementUpdateEvent',
+    'AnnouncementDeleteEvent',
+    'AnnouncementReactionAddEvent',
+    'AnnouncementReactionRemoveEvent',
+    'AnnouncementReplyCreateEvent',
+    'AnnouncementReplyUpdateEvent',
+    'AnnouncementReplyDeleteEvent',
+    'AnnouncementReplyReactionAddEvent',
+    'AnnouncementReplyReactionRemoveEvent',
     'DocCreateEvent',
     'DocUpdateEvent',
     'DocDeleteEvent',
     'DocReactionAddEvent',
     'DocReactionRemoveEvent',
     'DocReplyCreateEvent',
     'DocReplyUpdateEvent',
@@ -877,14 +889,364 @@
         the webhook was deleted.
     """
 
     __gateway_event__ = 'ServerWebhookUpdated'
     __dispatch_event__ = 'webhook_update'
 
 
+class _AnnouncementEvent(ServerEvent):
+    __slots__: Tuple[str, ...] = (
+        'channel',
+        'announcement',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.AnnouncementEvent,
+        /,
+        channel: AnnouncementChannel,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.channel = channel
+        self.announcement = Announcement(state=state, data=data['announcement'], channel=channel)
+
+
+class AnnouncementCreateEvent(_AnnouncementEvent):
+    """Represents an :gdocs:`AnnouncementCreated <websockets/AnnouncementCreated>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the announcement is in.
+    server: :class:`Server`
+        The server that the announcement is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the announcement is in.
+    announcement: :class:`Announcement`
+        The announcement that was created.
+    """
+
+    __gateway_event__ = 'AnnouncementCreated'
+    __dispatch_event__ = 'announcement_create'
+
+
+class AnnouncementUpdateEvent(_AnnouncementEvent):
+    """Represents an :gdocs:`AnnouncementUpdated <websockets/AnnouncementUpdated>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the announcement is in.
+    server: :class:`Server`
+        The server that the announcement is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the announcement is in.
+    announcement: :class:`Announcement`
+        The announcement after modification.
+    """
+
+    __gateway_event__ = 'AnnouncementUpdated'
+    __dispatch_event__ = 'announcement_update'
+
+
+class AnnouncementDeleteEvent(_AnnouncementEvent):
+    """Represents an :gdocs:`AnnouncementDeleted <websockets/AnnouncementDeleted>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the announcement was in.
+    server: :class:`Server`
+        The server that the announcement was in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the announcement was in.
+    announcement: :class:`Announcement`
+        The announcement that was deleted.
+    """
+
+    __gateway_event__ = 'AnnouncementDeleted'
+    __dispatch_event__ = 'announcement_delete'
+
+
+class _AnnouncementReactionEvent(ServerEvent):
+    __slots__: Tuple[str, ...] = (
+        'channel_id',
+        'announcement_id',
+        'user_id',
+        'emote',
+        'channel',
+        'member',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.AnnouncementReactionEvent,
+        /,
+        channel: AnnouncementChannel,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.channel_id = data['reaction']['channelId']
+        self.announcement_id = data['reaction']['announcementId']
+        self.user_id = data['reaction']['createdBy']
+        self.emote = Emote(state=state, data=data['reaction']['emote'])
+
+        self.channel = channel
+        self.member = self.server.get_member(self.user_id)
+
+
+class AnnouncementReactionAddEvent(_AnnouncementReactionEvent):
+    """Represents an :gdocs:`AnnouncementReactionCreated <websockets/AnnouncementReactionCreated>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reaction is in.
+    server: :class:`Server`
+        The server that the reaction is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reaction is in.
+    member: Optional[:class:`Member`]
+        The member that added the reaction, if they are cached.
+    channel_id: :class:`str`
+        The ID of the channel that the reaction is in.
+    announcement_id: :class:`int`
+        The ID of the announcement that the reaction is on.
+    user_id: :class:`str`
+        The ID of the user that added the reaction.
+    emote: :class:`Emote`
+        The emote that the reaction shows.
+    """
+
+    __gateway_event__ = 'AnnouncementReactionCreated'
+    __dispatch_event__ = 'announcement_reaction_add'
+
+
+class AnnouncementReactionRemoveEvent(_AnnouncementReactionEvent):
+    """Represents an :gdocs:`AnnouncementReactionDeleted <websockets/AnnouncementReactionDeleted>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reaction is in.
+    server: :class:`Server`
+        The server that the reaction is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reaction is in.
+    member: Optional[:class:`Member`]
+        The member that added the reaction, if they are cached.
+    channel_id: :class:`str`
+        The ID of the channel that the reaction is in.
+    announcement_id: :class:`int`
+        The ID of the announcement that the reaction is on.
+    user_id: :class:`str`
+        The ID of the user that added the reaction.
+    emote: :class:`Emote`
+        The emote that the reaction shows.
+    """
+
+    __gateway_event__ = 'AnnouncementReactionDeleted'
+    __dispatch_event__ = 'announcement_reaction_remove'
+
+
+class _AnnouncementCommentEvent(ServerEvent):
+    __slots__: Tuple[str, ...] = (
+        'channel',
+        'announcement',
+        'reply',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.AnnouncementCommentEvent,
+        /,
+        announcement: Announcement,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.channel = announcement.channel
+        self.announcement = announcement
+        self.reply = AnnouncementReply(state=state, data=data['announcementComment'], parent=announcement)
+
+
+class AnnouncementReplyCreateEvent(_AnnouncementCommentEvent):
+    """Represents an :gdocs:`AnnouncementCommentCreated <websockets/AnnouncementCommentCreated>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reply is in.
+    server: :class:`Server`
+        The server that the reply is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reply is in.
+    announcement: :class:`Announcement`
+        The announcement that the reply is under.
+    reply: :class:`AnnouncementReply`
+        The reply that was created.
+    """
+
+    __gateway_event__ = 'AnnouncementCommentCreated'
+    __dispatch_event__ = 'announcement_reply_create'
+
+
+class AnnouncementReplyUpdateEvent(_AnnouncementCommentEvent):
+    """Represents an :gdocs:`AnnouncementCommentUpdated <websockets/AnnouncementCommentUpdated>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reply is in.
+    server: :class:`Server`
+        The server that the reply is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reply is in.
+    announcement: :class:`Announcement`
+        The announcement that the reply is under.
+    reply: :class:`AnnouncementReply`
+        The reply that was updated.
+    """
+
+    __gateway_event__ = 'AnnouncementCommentUpdated'
+    __dispatch_event__ = 'announcement_reply_update'
+
+
+class AnnouncementReplyDeleteEvent(_AnnouncementCommentEvent):
+    """Represents an :gdocs:`AnnouncementCommentDeleted <websockets/AnnouncementCommentDeleted>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reply was in.
+    server: :class:`Server`
+        The server that the reply was in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reply was in.
+    announcement: :class:`Announcement`
+        The announcement that the reply was under.
+    reply: :class:`AnnouncementReply`
+        The reply that was deleted.
+    """
+
+    __gateway_event__ = 'AnnouncementCommentDeleted'
+    __dispatch_event__ = 'announcement_reply_delete'
+
+
+class _AnnouncementReplyReactionEvent(ServerEvent):
+    __slots__: Tuple[str, ...] = (
+        'channel_id',
+        'announcement_id',
+        'reply_id',
+        'user_id',
+        'emote',
+        'channel',
+        'member',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.AnnouncementCommentReactionEvent,
+        /,
+        channel: AnnouncementChannel,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.channel_id = data['reaction']['channelId']
+        self.announcement_id = data['reaction']['announcementId']
+        self.reply_id = data['reaction']['announcementCommentId']
+        self.user_id = data['reaction']['createdBy']
+        self.emote = Emote(state=state, data=data['reaction']['emote'])
+
+        self.channel = channel
+        self.member = self.server.get_member(self.user_id)
+
+
+class AnnouncementReplyReactionAddEvent(_AnnouncementReplyReactionEvent):
+    """Represents an :gdocs:`AnnouncementCommentReactionCreated <websockets/AnnouncementCommentReactionCreated>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reaction is in.
+    server: :class:`Server`
+        The server that the reaction is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reaction is in.
+    member: Optional[:class:`Member`]
+        The member that added the reaction, if they are cached.
+    channel_id: :class:`str`
+        The ID of the channel that the reaction is in.
+    announcement_id: :class:`int`
+        The ID of the calendar event that the reply is under.
+    reply_id: :class:`int`
+        The ID of the reply that the reaction is on.
+    user_id: :class:`str`
+        The ID of the user that added the reaction.
+    emote: :class:`Emote`
+        The emote that the reaction shows.
+    """
+
+    __gateway_event__ = 'AnnouncementCommentReactionCreated'
+    __dispatch_event__ = 'announcement_reply_reaction_add'
+
+
+class AnnouncementReplyReactionRemoveEvent(_AnnouncementReplyReactionEvent):
+    """Represents an :gdocs:`AnnouncementCommentReactionDeleted <websockets/AnnouncementCommentReactionDeleted>` event for dispatching to event handlers.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reaction is in.
+    server: :class:`Server`
+        The server that the reaction is in.
+    channel: :class:`AnnouncementChannel`
+        The channel that the reaction is in.
+    member: Optional[:class:`Member`]
+        The member that added the reaction, if they are cached.
+    channel_id: :class:`str`
+        The ID of the channel that the reaction is in.
+    announcement_id: :class:`int`
+        The ID of the calendar event that the reply is under.
+    reply_id: :class:`int`
+        The ID of the reply that the reaction is on.
+    user_id: :class:`str`
+        The ID of the user that added the reaction.
+    emote: :class:`Emote`
+        The emote that the reaction shows.
+    """
+
+    __gateway_event__ = 'AnnouncementCommentReactionDeleted'
+    __dispatch_event__ = 'announcement_reply_reaction_remove'
+
+
 class _DocEvent(ServerEvent):
     __slots__: Tuple[str, ...] = (
         'channel',
         'doc',
     )
 
     def __init__(
```

### Comparing `guilded.py-1.7.0/guilded/ext/commands/_types.py` & `guilded.py-1.8.0/guilded/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/bot.py` & `guilded.py-1.8.0/guilded/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/cog.py` & `guilded.py-1.8.0/guilded/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/context.py` & `guilded.py-1.8.0/guilded/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/converters.py` & `guilded.py-1.8.0/guilded/ext/commands/converters.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/cooldowns.py` & `guilded.py-1.8.0/guilded/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/core.py` & `guilded.py-1.8.0/guilded/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/errors.py` & `guilded.py-1.8.0/guilded/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/help.py` & `guilded.py-1.8.0/guilded/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/commands/view.py` & `guilded.py-1.8.0/guilded/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/ext/tasks/__init__.py` & `guilded.py-1.8.0/guilded/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/file.py` & `guilded.py-1.8.0/guilded/file.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/flowbot.py` & `guilded.py-1.8.0/guilded/flowbot.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/gateway.py` & `guilded.py-1.8.0/guilded/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -226,16 +226,16 @@
             self.client.http.user = ClientUser(state=self.client.http, data=d['user'])
             self.client.http.my_id = self.client.http.user.id
 
         if op == self.MISSABLE:
             server = None
             should_fill = False
             try:
-                should_fill = self.client.get_server(d['serverId']) is None
                 server = await self.client.getch_server(d['serverId'])
+                should_fill = len(server.members) == 0
             except HTTPException as exc:
                 # This shouldn't happen
                 log.warn(
                     'Received unfetchable server ID %s (%s: %s). Constructing a partial server instance instead.',
                     d['serverId'],
                     exc.status,
                     exc.message,
@@ -272,17 +272,14 @@
 
             # Edge case for being provided a server
             # despite no longer being a member of it
             if server and t != 'BotServerMembershipDeleted':
                 if should_fill:
                     await server.fill_members()
 
-                # For now we add 'new' servers to cache as there is no other
-                # way to passively receive all of the client's servers, and we
-                # don't want to fetch them every time and slow down bots.
                 self.client.http.add_to_server_cache(server)
 
             coro = self._parsers.get(t)
             if coro is not None:
                 # ignore unhandled events
 
                 server_id = d.get('serverId')
@@ -634,14 +631,89 @@
 
         else:
             webhook = Webhook.from_state(data['webhook'], self._state)
             # Webhooks are not cached so having a `webhook_update` with only `after` doesn't make sense.
             # In the future this may change with the introduction of better caching control.
             self.client.dispatch('raw_webhook_update', webhook)
 
+    async def parse_announcement_created(self, data: gw.AnnouncementEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['announcement']['channelId'], server_channel_type=ChannelType.announcements)
+            event = ev.AnnouncementCreateEvent(self._state, data, channel=channel)
+            self.client.dispatch(event)
+
+    async def parse_announcement_updated(self, data: gw.AnnouncementEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['announcement']['channelId'], server_channel_type=ChannelType.announcements)
+            event = ev.AnnouncementUpdateEvent(self._state, data, channel=channel)
+            self.client.dispatch(event)
+
+    async def parse_announcement_deleted(self, data: gw.AnnouncementEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['announcement']['channelId'], server_channel_type=ChannelType.announcements)
+            event = ev.AnnouncementDeleteEvent(self._state, data, channel=channel)
+            self.client.dispatch(event)
+
+    async def parse_announcement_comment_created(self, data: gw.AnnouncementCommentEvent):
+        if self._exp_style:
+            channel: AnnouncementChannel = await self._force_resolve_channel(data['serverId'], data['announcementComment']['channelId'], ChannelType.announcement)
+            try:
+                announcement = await channel.fetch_announcement(data['announcementComment']['announcementId'])
+            except HTTPException:
+                return
+
+            event = ev.AnnouncementReplyCreateEvent(self._state, data, announcement)
+            self.client.dispatch(event)
+
+    async def parse_announcement_comment_updated(self, data: gw.AnnouncementCommentEvent):
+        if self._exp_style:
+            channel: AnnouncementChannel = await self._force_resolve_channel(data['serverId'], data['announcementComment']['channelId'], ChannelType.announcement)
+            try:
+                announcement = await channel.fetch_announcement(data['announcementComment']['announcementId'])
+            except HTTPException:
+                return
+
+            event = ev.AnnouncementReplyUpdateEvent(self._state, data, announcement)
+            self.client.dispatch(event)
+
+    async def parse_announcement_comment_deleted(self, data: gw.AnnouncementCommentEvent):
+        if self._exp_style:
+            channel: AnnouncementChannel = await self._force_resolve_channel(data['serverId'], data['announcementComment']['channelId'], ChannelType.announcement)
+            try:
+                announcement = await channel.fetch_announcement(data['announcementComment']['announcementId'])
+            except HTTPException:
+                return
+
+            event = ev.AnnouncementReplyDeleteEvent(self._state, data, announcement)
+            self.client.dispatch(event)
+
+    async def parse_announcement_reaction_created(self, data: gw.AnnouncementReactionEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'], ChannelType.announcements)
+            event = ev.AnnouncementReactionAddEvent(self._state, data, channel)
+            self.client.dispatch(event)
+
+    async def parse_announcement_reaction_deleted(self, data: gw.AnnouncementReactionEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'], ChannelType.announcements)
+            event = ev.AnnouncementReactionRemoveEvent(self._state, data, channel)
+            self.client.dispatch(event)
+
+    async def parse_announcement_comment_reaction_created(self, data: gw.AnnouncementCommentReactionEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'], ChannelType.announcements)
+            event = ev.AnnouncementReplyReactionAddEvent(self._state, data, channel)
+            self.client.dispatch(event)
+
+    async def parse_announcement_comment_reaction_deleted(self, data: gw.AnnouncementCommentReactionEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'], ChannelType.announcements)
+            event = ev.AnnouncementReplyReactionRemoveEvent(self._state, data, channel)
+            self.client.dispatch(event)
+
     async def parse_doc_created(self, data: gw.DocEvent):
         if self._exp_style:
             channel = await self._force_resolve_channel(data['serverId'], data['doc']['channelId'], server_channel_type=ChannelType.docs)
             event = ev.DocCreateEvent(self._state, data, channel=channel)
             self.client.dispatch(event)
 
     async def parse_doc_updated(self, data: gw.DocEvent):
```

### Comparing `guilded.py-1.7.0/guilded/group.py` & `guilded.py-1.8.0/guilded/group.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/http.py` & `guilded.py-1.8.0/guilded/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -387,14 +387,17 @@
 
     def get_user(self, user_id: str):
         return self.request(Route('GET', f'/users/{user_id}', override_base=Route.USER_BASE))
 
     def get_my_user(self):
         return self.request(Route('GET', '/users/@me'))
 
+    def get_my_servers(self):
+        return self.request(Route('GET', '/users/@me/servers'))
+
     # /content
 
     def get_metadata(self, route: str):
         params = {
             'route': route,
         }
         return self.request(Route('GET', '/content/route/metadata', override_base=Route.USER_BASE), params=params)
@@ -550,18 +553,40 @@
         return await self.session.ws_connect(Route.WEBSOCKET_BASE, headers=headers, autoping=False)
 
     # /channels
 
     def create_server_channel(
         self,
         server_id: str,
+        content_type: str,
         *,
-        payload: Dict[str, Any],
+        name: str,
+        topic: Optional[str] = None,
+        public: Optional[bool] = None,
+        category_id: Optional[int] = None,
+        group_id: Optional[str] = None,
     ):
-        payload['serverId'] = server_id
+        payload = {
+            'serverId': server_id,
+            'type': content_type,
+            'name': name,
+        }
+
+        if topic is not None:
+            payload['topic'] = topic
+
+        if public is not None:
+            payload['isPublic'] = public
+
+        if category_id is not None:
+            payload['categoryId'] = category_id
+
+        if group_id is not None:
+            payload['groupId'] = group_id
+
         return self.request(Route('POST', f'/channels'), json=payload)
 
     def update_channel(
         self,
         channel_id: str,
         *,
         payload: Dict[str, Any],
@@ -604,14 +629,20 @@
         if after is not None:
             params['after'] = self.valid_ISO8601(after)
         if limit is not None:
             params['limit'] = limit
 
         return self.request(Route('GET', f'/channels/{channel_id}/messages'), params=params)
 
+    def add_channel_message_reaction(self, channel_id: str, message_id: str, emote_id: int):
+        return self.request(Route('PUT', f'/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'))
+
+    def remove_channel_message_reaction(self, channel_id: str, message_id: str, emote_id: int):
+        return self.request(Route('DELETE', f'/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'))
+
     def create_forum_topic(self, channel_id: str, *, title: str, content: str):
         payload = {
             'title': title,
             'content': content,
         }
 
         return self.request(Route('POST', f'/channels/{channel_id}/topics'), json=payload)
@@ -666,24 +697,24 @@
 
     def update_forum_topic_comment(self, channel_id: str, topic_id: int, comment_id: int, *, payload: Dict[str, Any]):
         return self.request(Route('PATCH', f'/channels/{channel_id}/topics/{topic_id}/comments/{comment_id}'), json=payload)
 
     def delete_forum_topic_comment(self, channel_id: str, topic_id: int, comment_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/topics/{topic_id}/comments/{comment_id}'))
 
-    def add_forum_topic_reaction_emote(self, channel_id: str, topic_id: int, emote_id: int):
+    def add_forum_topic_reaction(self, channel_id: str, topic_id: int, emote_id: int):
         return self.request(Route('PUT', f'/channels/{channel_id}/topics/{topic_id}/emotes/{emote_id}'))
 
-    def remove_forum_topic_reaction_emote(self, channel_id: str, topic_id: int, emote_id: int):
+    def remove_forum_topic_reaction(self, channel_id: str, topic_id: int, emote_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/topics/{topic_id}/emotes/{emote_id}'))
 
-    def add_forum_topic_comment_reaction_emote(self, channel_id: str, topic_id: int, comment_id: int, emote_id: int):
+    def add_forum_topic_comment_reaction(self, channel_id: str, topic_id: int, comment_id: int, emote_id: int):
         return self.request(Route('PUT', f'/channels/{channel_id}/topics/{topic_id}/comments/{comment_id}/emotes/{emote_id}'))
 
-    def remove_forum_topic_comment_reaction_emote(self, channel_id: str, topic_id: int, comment_id: int, emote_id: int):
+    def remove_forum_topic_comment_reaction(self, channel_id: str, topic_id: int, comment_id: int, emote_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/topics/{topic_id}/comments/{comment_id}/emotes/{emote_id}'))
 
     def create_list_item(self, channel_id: str, *, message: str, note_content: Optional[str] = None):
         payload = {
             'message': message,
         }
         if note_content is not None:
@@ -696,25 +727,81 @@
     def get_list_item(self, channel_id: str, item_id: str):
         return self.request(Route('GET', f'/channels/{channel_id}/items/{item_id}'))
 
     def get_list_items(self, channel_id: str):
         return self.request(Route('GET', f'/channels/{channel_id}/items'))
 
     def update_list_item(self, channel_id: str, item_id: str, *, payload: Dict[str, Any]):
-        return self.request(Route('PUT', f'/channels/{channel_id}/items/{item_id}'), json=payload)
+        return self.request(Route('PATCH', f'/channels/{channel_id}/items/{item_id}'), json=payload)
 
     def delete_list_item(self, channel_id: str, item_id: str):
         return self.request(Route('DELETE', f'/channels/{channel_id}/items/{item_id}'))
 
     def complete_list_item(self, channel_id: str, item_id: str):
         return self.request(Route('POST', f'/channels/{channel_id}/items/{item_id}/complete'))
 
     def uncomplete_list_item(self, channel_id: str, item_id: str):
         return self.request(Route('DELETE', f'/channels/{channel_id}/items/{item_id}/complete'))
 
+    def create_announcement(self, channel_id: str, *, title: str, content: str):
+        payload = {
+            'title': title,
+            'content': content,
+        }
+
+        return self.request(Route('POST', f'/channels/{channel_id}/announcements'), json=payload)
+
+    def get_announcements(self, channel_id: str, *, limit: int = None, before: datetime.datetime = None):
+        params = {}
+        if limit is not None:
+            params['limit'] = limit
+        if before is not None:
+            params['before'] = self.valid_ISO8601(before)
+
+        return self.request(Route('GET', f'/channels/{channel_id}/announcements'), params=params)
+
+    def get_announcement(self, channel_id: str, announcement_id: str):
+        return self.request(Route('GET', f'/channels/{channel_id}/announcements/{announcement_id}'))
+
+    def update_announcement(self, channel_id: str, announcement_id: str, *, payload: Dict[str, Any]):
+        return self.request(Route('PUT', f'/channels/{channel_id}/announcements/{announcement_id}'), json=payload)
+
+    def delete_announcement(self, channel_id: str, announcement_id: str):
+        return self.request(Route('DELETE', f'/channels/{channel_id}/announcements/{announcement_id}'))
+
+    def add_announcement_reaction(self, channel_id: str, announcement_id: str, emote_id: int):
+        return self.request(Route('PUT', f'/channels/{channel_id}/announcements/{announcement_id}/emotes/{emote_id}'))
+
+    def remove_announcement_reaction(self, channel_id: str, announcement_id: str, emote_id: int):
+        return self.request(Route('DELETE', f'/channels/{channel_id}/announcements/{announcement_id}/emotes/{emote_id}'))
+
+    def create_announcement_comment(self, channel_id: str, announcement_id: str, *, content: str):
+        payload = {
+            'content': content,
+        }
+        return self.request(Route('POST', f'/channels/{channel_id}/announcements/{announcement_id}/comments'), json=payload)
+
+    def get_announcement_comment(self, channel_id: str, announcement_id: str, comment_id: int):
+        return self.request(Route('GET', f'/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}'))
+
+    def get_announcement_comments(self, channel_id: str, announcement_id: str):
+        return self.request(Route('GET', f'/channels/{channel_id}/announcements/{announcement_id}/comments'))
+
+    def update_announcement_comment(self, channel_id: str, announcement_id: str, comment_id: int, *, payload: Dict[str, Any]):
+        return self.request(Route('PATCH', f'/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}'), json=payload)
+
+    def delete_announcement_comment(self, channel_id: str, announcement_id: str, comment_id: int):
+        return self.request(Route('DELETE', f'/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}'))
+
+    def add_announcement_comment_reaction(self, channel_id: str, announcement_id: str, comment_id: int, emote_id: int):
+        return self.request(Route('PUT', f'/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}/emotes/{emote_id}'))
+
+    def remove_announcement_comment_reaction(self, channel_id: str, announcement_id: str, comment_id: int, emote_id: int):
+        return self.request(Route('DELETE', f'/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}/emotes/{emote_id}'))
+
     def create_doc(self, channel_id: str, *, title: str, content: str):
         payload = {
             'title': title,
             'content': content,
         }
 
         return self.request(Route('POST', f'/channels/{channel_id}/docs'), json=payload)
@@ -733,14 +820,20 @@
 
     def update_doc(self, channel_id: str, doc_id: int, *, payload: Dict[str, Any]):
         return self.request(Route('PUT', f'/channels/{channel_id}/docs/{doc_id}'), json=payload)
 
     def delete_doc(self, channel_id: str, doc_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/docs/{doc_id}'))
 
+    def add_doc_reaction(self, channel_id: str, doc_id: int, emote_id: int):
+        return self.request(Route('PUT', f'/channels/{channel_id}/docs/{doc_id}/emotes/{emote_id}'))
+
+    def remove_doc_reaction(self, channel_id: str, doc_id: int, emote_id: int):
+        return self.request(Route('DELETE', f'/channels/{channel_id}/docs/{doc_id}/emotes/{emote_id}'))
+
     def create_doc_comment(self, channel_id: str, doc_id: int, *, content: str):
         payload = {
             'content': content,
         }
         return self.request(Route('POST', f'/channels/{channel_id}/docs/{doc_id}/comments'), json=payload)
 
     def get_doc_comment(self, channel_id: str, doc_id: int, comment_id: int):
@@ -751,26 +844,20 @@
 
     def update_doc_comment(self, channel_id: str, doc_id: int, comment_id: int, *, payload: Dict[str, Any]):
         return self.request(Route('PATCH', f'/channels/{channel_id}/docs/{doc_id}/comments/{comment_id}'), json=payload)
 
     def delete_doc_comment(self, channel_id: str, doc_id: int, comment_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/docs/{doc_id}/comments/{comment_id}'))
 
-    def add_doc_comment_reaction_emote(self, channel_id: str, doc_id: int, comment_id: int, emote_id: int):
+    def add_doc_comment_reaction(self, channel_id: str, doc_id: int, comment_id: int, emote_id: int):
         return self.request(Route('PUT', f'/channels/{channel_id}/docs/{doc_id}/comments/{comment_id}/emotes/{emote_id}'))
 
-    def remove_doc_comment_reaction_emote(self, channel_id: str, doc_id: int, comment_id: int, emote_id: int):
+    def remove_doc_comment_reaction(self, channel_id: str, doc_id: int, comment_id: int, emote_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/docs/{doc_id}/comments/{comment_id}/emotes/{emote_id}'))
 
-    def add_reaction_emote(self, channel_id: str, content_id: Union[str, int], emote_id: int):
-        return self.request(Route('PUT', f'/channels/{channel_id}/content/{content_id}/emotes/{emote_id}'))
-
-    def remove_reaction_emote(self, channel_id: str, content_id: str, emote_id: int):
-        return self.request(Route('DELETE', f'/channels/{channel_id}/content/{content_id}/emotes/{emote_id}'))
-
     def create_calendar_event(self, channel_id: str, *, payload: Dict[str, Any]):
         return self.request(Route('POST', f'/channels/{channel_id}/events'), json=payload)
 
     def get_calendar_events(self, channel_id: str, *, limit: int = None, before: datetime.datetime = None, after: datetime.datetime = None):
         params = {}
         if limit is not None:
             params['limit'] = limit
@@ -790,18 +877,18 @@
     def delete_calendar_event(self, channel_id: str, event_id: int, *, delete_series: Optional[str] = None):
         payload = {}
         if delete_series:
             payload['deleteSeries'] = delete_series
 
         return self.request(Route('DELETE', f'/channels/{channel_id}/events/{event_id}'), json=payload)
 
-    def add_calendar_event_reaction_emote(self, channel_id: str, event_id: int, emote_id: int):
+    def add_calendar_event_reaction(self, channel_id: str, event_id: int, emote_id: int):
         return self.request(Route('PUT', f'/channels/{channel_id}/events/{event_id}/emotes/{emote_id}'))
 
-    def remove_calendar_event_reaction_emote(self, channel_id: str, event_id: int, emote_id: int):
+    def remove_calendar_event_reaction(self, channel_id: str, event_id: int, emote_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/events/{event_id}/emotes/{emote_id}'))
 
     def create_calendar_event_comment(self, channel_id: str, event_id: int, *, content: str):
         payload = {
             'content': content,
         }
         return self.request(Route('POST', f'/channels/{channel_id}/events/{event_id}/comments'), json=payload)
@@ -814,37 +901,55 @@
 
     def update_calendar_event_comment(self, channel_id: str, event_id: int, comment_id: int, *, payload: Dict[str, Any]):
         return self.request(Route('PATCH', f'/channels/{channel_id}/events/{event_id}/comments/{comment_id}'), json=payload)
 
     def delete_calendar_event_comment(self, channel_id: str, event_id: int, comment_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/events/{event_id}/comments/{comment_id}'))
 
-    def add_calendar_event_comment_reaction_emote(self, channel_id: str, event_id: int, comment_id: int, emote_id: int):
+    def add_calendar_event_comment_reaction(self, channel_id: str, event_id: int, comment_id: int, emote_id: int):
         return self.request(Route('PUT', f'/channels/{channel_id}/events/{event_id}/comments/{comment_id}/emotes/{emote_id}'))
 
-    def remove_calendar_event_comment_reaction_emote(self, channel_id: str, event_id: int, comment_id: int, emote_id: int):
+    def remove_calendar_event_comment_reaction(self, channel_id: str, event_id: int, comment_id: int, emote_id: int):
         return self.request(Route('DELETE', f'/channels/{channel_id}/events/{event_id}/comments/{comment_id}/emotes/{emote_id}'))
 
     def get_calendar_event_rsvp(self, channel_id: str, event_id: int, user_id: str):
         return self.request(Route('GET', f'/channels/{channel_id}/events/{event_id}/rsvps/{user_id}'))
 
     def get_calendar_event_rsvps(self, channel_id: str, event_id: int):
         return self.request(Route('GET', f'/channels/{channel_id}/events/{event_id}/rsvps'))
 
     def put_calendar_event_rsvp(
         self,
         channel_id: str,
         event_id: int,
         user_id: str,
         *,
-        payload: Dict[str, Any],
+        status: str,
     ):
         # This endpoint is used for creation and updating
+        payload = {
+            'status': status
+        }
         return self.request(Route('PUT', f'/channels/{channel_id}/events/{event_id}/rsvps/{user_id}'), json=payload)
 
+    def upsert_calendar_event_rsvps(
+        self,
+        channel_id: str,
+        event_id: int,
+        user_ids: List[str],
+        *,
+        status: str,
+    ):
+        # This endpoint is used for creation and updating
+        payload = {
+            'userIds': user_ids,
+            'status': status,
+        }
+        return self.request(Route('PUT', f'/channels/{channel_id}/events/{event_id}/rsvps'), json=payload)
+
     def delete_calendar_event_rsvp(self, channel_id: str, event_id: int, user_id: str):
         return self.request(Route('DELETE', f'/channels/{channel_id}/events/{event_id}/rsvps/{user_id}'))
 
     # /servers
 
     def get_server(self, server_id: str):
         return self.request(Route('GET', f'/servers/{server_id}'))
```

### Comparing `guilded.py-1.7.0/guilded/invite.py` & `guilded.py-1.8.0/guilded/invite.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/message.py` & `guilded.py-1.8.0/guilded/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,14 +572,15 @@
     """
 
     __slots__ = (
         '_state',
         'channel',
         'channel_id',
         'server_id',
+        'group_id',
         'id',
         'type',
         'webhook_id',
         'author_id',
         'created_at',
         'updated_at',
         'deleted_at',
@@ -597,14 +598,15 @@
 
         self.channel = channel
         self._author = extra.get('author')
         self._webhook = extra.get('webhook')
 
         self.channel_id: str = data.get('channelId')
         self.server_id: str = data.get('serverId') or data.get('teamId')
+        self.group_id: Optional[str] = data.get('groupId')
 
         self.id: str = data['id']
         self.type: MessageType = try_enum(MessageType, data.get('type'))
 
         self.replied_to_ids: List[str] = data.get('replyMessageIds') or data.get('repliesToIds') or []
         self.author_id: str = data.get('createdBy')
         self.webhook_id: Optional[str] = data.get('createdByWebhookId') or data.get('webhookId')
@@ -826,28 +828,28 @@
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_reaction_emote(self.channel_id, self.id, emote_id)
+        await self._state.add_channel_message_reaction(self.channel_id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this message.
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_reaction_emote(self.channel.id, self.id, emote_id)
+        await self._state.remove_channel_message_reaction(self.channel.id, self.id, emote_id)
 
     async def reply(
         self,
         content: Optional[str] = MISSING,
         *,
         embed: Optional[Embed] = MISSING,
         embeds: Optional[Sequence[Embed]] = MISSING,
```

### Comparing `guilded.py-1.7.0/guilded/mixins.py` & `guilded.py-1.8.0/guilded/mixins.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/permissions.py` & `guilded.py-1.8.0/guilded/permissions.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/presence.py` & `guilded.py-1.8.0/guilded/presence.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/reaction.py` & `guilded.py-1.8.0/guilded/reaction.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/reply.py` & `guilded.py-1.8.0/guilded/reply.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,29 +51,157 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 from .abc import Reply
 
 if TYPE_CHECKING:
+    from .types.announcement import AnnouncementComment
     from .types.calendar_event import CalendarEventComment
     from .types.doc import DocComment
     from .types.forum_topic import ForumTopicComment
 
-    from .channel import CalendarEvent, Doc, ForumTopic
+    from .channel import Announcement, CalendarEvent, Doc, ForumTopic
     from .emote import Emote
 
 
 __all__ = (
+    'AnnouncementReply',
     'CalendarEventReply',
     'DocReply',
     'ForumTopicReply',
 )
 
 
+class AnnouncementReply(Reply):
+    """Represents a reply to an :class:`Announcement`.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two replies are equal.
+
+        .. describe:: x != y
+
+            Checks if two replies are not equal.
+
+        .. describe:: hash(x)
+
+            Returns the reply's hash.
+
+    .. versionadded:: 1.8
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The reply's ID.
+    content: :class:`str`
+        The reply's content.
+    parent: :class:`.Announcement`
+        The announcement that the reply is a child of.
+    parent_id: :class:`int`
+        The ID of the parent announcement.
+    created_at: :class:`datetime.datetime`
+        When the reply was created.
+    updated_at: Optional[:class:`datetime.datetime`]
+        When the reply was last updated.
+    """
+
+    __slots__ = (
+        'parent',
+        'parent_id',
+    )
+
+    def __init__(self, *, state, data: AnnouncementComment, parent: Announcement):
+        self.parent: Announcement = parent
+        self.parent_id: str = data.get('announcementId')
+
+        super().__init__(state=state, data=data)
+
+    async def edit(
+        self,
+        *,
+        content: str,
+    ) -> AnnouncementReply:
+        """|coro|
+
+        Edit this reply.
+
+        Parameters
+        -----------
+        content: :class:`str`
+            The content of the reply.
+
+        Returns
+        --------
+        :class:`AnnouncementReply`
+            The updated reply.
+
+        Raises
+        -------
+        NotFound
+            This reply does not exist.
+        Forbidden
+            You do not have permission to update this reply.
+        HTTPException
+            Failed to update this reply.
+        """
+
+        payload = {
+            'content': content,
+        }
+
+        data = await self._state.update_announcement_comment(self.parent.channel_id, self.parent_id, self.id, payload=payload)
+        return AnnouncementReply(state=self._state, data=data['announcementComment'], parent=self.parent)
+
+    async def delete(self) -> None:
+        """|coro|
+
+        Delete this reply.
+
+        Raises
+        -------
+        NotFound
+            This reply does not exist.
+        Forbidden
+            You do not have permission to delete this reply.
+        HTTPException
+            Failed to delete this reply.
+        """
+
+        await self._state.delete_announcement_comment(self.parent.channel_id, self.parent_id, self.id)
+
+    async def add_reaction(self, emote: Emote, /) -> None:
+        """|coro|
+
+        Add a reaction to this reply.
+
+        Parameters
+        -----------
+        emote: :class:`.Emote`
+            The emote to add.
+        """
+        emote_id: int = getattr(emote, 'id', emote)
+        await self._state.add_announcement_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
+
+    async def remove_self_reaction(self, emote: Emote, /) -> None:
+        """|coro|
+
+        Remove one of your reactions from this reply.
+
+        Parameters
+        -----------
+        emote: :class:`.Emote`
+            The emote to remove.
+        """
+        emote_id: int = getattr(emote, 'id', emote)
+        await self._state.remove_announcement_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
+
+
 class CalendarEventReply(Reply):
     """Represents a reply to a :class:`CalendarEvent`.
 
     .. container:: operations
 
         .. describe:: x == y
 
@@ -176,28 +304,28 @@
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_calendar_event_comment_reaction_emote(self.channel.id, self.parent_id, self.id, emote_id)
+        await self._state.add_calendar_event_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this reply.
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_calendar_event_comment_reaction_emote(self.channel.id, self.parent_id, self.id, emote_id)
+        await self._state.remove_calendar_event_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
 
 
 class DocReply(Reply):
     """Represents a reply to a :class:`Doc`.
 
     .. container:: operations
 
@@ -302,28 +430,28 @@
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_doc_comment_reaction_emote(self.channel.id, self.parent_id, self.id, emote_id)
+        await self._state.add_doc_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this reply.
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_doc_comment_reaction_emote(self.channel.id, self.parent_id, self.id, emote_id)
+        await self._state.remove_doc_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
 
 
 class ForumTopicReply(Reply):
     """Represents a reply to a :class:`ForumTopic`.
 
     .. container:: operations
 
@@ -430,23 +558,23 @@
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.add_forum_topic_comment_reaction_emote(self.channel.id, self.parent_id, self.id, emote_id)
+        await self._state.add_forum_topic_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
 
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this reply.
 
         .. versionadded:: 1.6
 
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_forum_topic_comment_reaction_emote(self.channel.id, self.parent_id, self.id, emote_id)
+        await self._state.remove_forum_topic_comment_reaction(self.channel.id, self.parent_id, self.id, emote_id)
```

### Comparing `guilded.py-1.7.0/guilded/role.py` & `guilded.py-1.8.0/guilded/role.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/server.py` & `guilded.py-1.8.0/guilded/server.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/status.py` & `guilded.py-1.8.0/guilded/status.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/calendar_event.py` & `guilded.py-1.8.0/guilded/types/calendar_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,30 +41,35 @@
     channelId: str
     name: str
     description: NotRequired[str]
     location: NotRequired[str]
     url: NotRequired[str]
     color: NotRequired[int]
     repeats: NotRequired[bool]
+    seriesId: NotRequired[str]
+    roleIds: NotRequired[List[int]]
+    isAllDay: NotRequired[bool]
     rsvpLimit: NotRequired[int]
+    rsvpDisabled: NotRequired[bool]
+    autofillWaitlist: NotRequired[bool]
     startsAt: str
     duration: NotRequired[int]
     isPrivate: NotRequired[bool]
     mentions: NotRequired[Mentions]
     createdAt: str
     createdBy: str
     cancellation: NotRequired[CalendarEventCancellation]
 
 
 class CalendarEventRsvp(TypedDict):
     calendarEventId: int
     channelId: NotRequired[str]
     serverId: str
     userId: str
-    status: Literal['going', 'maybe', 'declined', 'invited', 'waitlisted']
+    status: Literal['going', 'maybe', 'declined', 'invited', 'waitlisted', 'not responded']
     createdBy: str
     createdAt: str
     updatedBy: NotRequired[str]
     updatedAt: NotRequired[str]
 
 
 class CalendarEventComment(ContentComment):
```

### Comparing `guilded.py-1.7.0/guilded/types/channel.py` & `guilded.py-1.8.0/guilded/types/channel.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/doc.py` & `guilded.py-1.8.0/guilded/types/doc.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/embed.py` & `guilded.py-1.8.0/guilded/types/embed.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/emote.py` & `guilded.py-1.8.0/guilded/types/emote.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/forum_topic.py` & `guilded.py-1.8.0/guilded/types/forum_topic.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/gateway.py` & `guilded.py-1.8.0/guilded/types/gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 SOFTWARE.
 """
 
 from __future__ import annotations
 from typing import Any, Dict, List, Literal, Optional, TypedDict
 from typing_extensions import NotRequired
 
+from .announcement import Announcement, AnnouncementComment
 from .calendar_event import CalendarEvent, CalendarEventComment, CalendarEventRsvp
 from .channel import ServerChannel
 from .doc import Doc, DocComment
 from .forum_topic import ForumTopic, ForumTopicComment
 from .list_item import ListItem
 from .message import ChatMessage, DeletedChatMessage
-from .reaction import CalendarEventCommentReaction, ChannelMessageReaction, CalendarEventReaction, DocCommentReaction, DocReaction, ForumTopicCommentReaction, ForumTopicReaction
+from .reaction import AnnouncementCommentReaction, AnnouncementReaction, CalendarEventCommentReaction, ChannelMessageReaction, CalendarEventReaction, DocCommentReaction, DocReaction, ForumTopicCommentReaction, ForumTopicReaction
 from .server import Server
 from .social_link import SocialLink
 from .user import ServerMember, ServerMemberBan, User
 from .webhook import Webhook
 
 
 class EventSkeleton(TypedDict):
@@ -131,14 +132,30 @@
     channel: ServerChannel
 
 
 class ServerWebhookEvent(_ServerEvent):
     webhook: Webhook
 
 
+class AnnouncementEvent(_ServerEvent):
+    announcement: Announcement
+
+
+class AnnouncementReactionEvent(_ServerEvent):
+    reaction: AnnouncementReaction
+
+
+class AnnouncementCommentEvent(_ServerEvent):
+    announcementComment: AnnouncementComment
+
+
+class AnnouncementCommentReactionEvent(_ServerEvent):
+    reaction: AnnouncementCommentReaction
+
+
 class DocEvent(_ServerEvent):
     doc: Doc
 
 
 class DocReactionEvent(_ServerEvent):
     reaction: DocReaction
```

### Comparing `guilded.py-1.7.0/guilded/types/list_item.py` & `guilded.py-1.8.0/guilded/types/list_item.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/message.py` & `guilded.py-1.8.0/guilded/types/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .embed import Embed
 
 
 class ChatMessage(TypedDict):
     id: str
     type: Literal['default', 'system']
     serverId: NotRequired[str]
+    groupId: NotRequired[str]
     channelId: str
     content: Optional[str]
     embeds: Optional[List[Embed]]
     replyMessageIds: NotRequired[str]
     isPrivate: NotRequired[bool]
     isSilent: NotRequired[bool]
     mentions: NotRequired[Mentions]
```

### Comparing `guilded.py-1.7.0/guilded/types/reaction.py` & `guilded.py-1.8.0/guilded/types/reaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,22 @@
 
 class _ContentReaction(TypedDict):
     channelId: str
     createdBy: str
     emote: Emote
 
 
+class AnnouncementReaction(_ContentReaction):
+    announcementId: str
+
+
+class AnnouncementCommentReaction(AnnouncementReaction):
+    announcementCommentId: int
+
+
 class ChannelMessageReaction(_ContentReaction):
     messageId: str
 
 
 class CalendarEventReaction(_ContentReaction):
     calendarEventId: int
```

### Comparing `guilded.py-1.7.0/guilded/types/role.py` & `guilded.py-1.8.0/guilded/types/role.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/server.py` & `guilded.py-1.8.0/guilded/types/server.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/social_link.py` & `guilded.py-1.8.0/guilded/types/social_link.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/user.py` & `guilded.py-1.8.0/guilded/types/user.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/types/webhook.py` & `guilded.py-1.8.0/guilded/types/webhook.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/user.py` & `guilded.py-1.8.0/guilded/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 from __future__ import annotations
 
 import datetime
 import inspect
 import itertools
 from operator import attrgetter
-from typing import Any, List, Dict, Optional, TYPE_CHECKING, Set, Tuple, Union
+from typing import TYPE_CHECKING, List, Optional, Tuple, TypeVar, Union
 
 import guilded.abc
 
 from .asset import Asset
 from .enums import SocialLinkType, try_enum
 from .role import Role
 from .utils import MISSING, Object, copy_doc, ISO8601
@@ -80,14 +80,16 @@
     'ClientUser',
     'Member',
     'MemberBan',
     'SocialLink',
     'User',
 )
 
+T = TypeVar('T', bound=type)
+
 
 class User(guilded.abc.User, guilded.abc.Messageable):
     """Represents a user in Guilded.
 
     .. container:: operations
 
         .. describe:: x == y
@@ -143,15 +145,15 @@
             self.banner: Optional[Asset] = Asset._from_user_banner(self._state, data.pop('profileBannerBlur'))
         elif 'banner' in data and data['banner'] is not None:
             self.banner: Optional[Asset] = Asset._from_user_banner(self._state, data.pop('banner'))
         elif 'profilePicture' in data or 'banner' in data:
             self.banner: Optional[Asset] = None
 
 
-def flatten_user(cls: Any):
+def flatten_user(cls: T) -> T:
     for attr, value in itertools.chain(guilded.abc.User.__dict__.items(), User.__dict__.items()):
         # ignore private/special methods
         if attr.startswith('_'):
             continue
 
         # don't override what we already have
         if attr in cls.__dict__:
```

### Comparing `guilded.py-1.7.0/guilded/utils.py` & `guilded.py-1.8.0/guilded/utils.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded/webhook/async_.py` & `guilded.py-1.8.0/guilded/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.7.0/guilded.py.egg-info/PKG-INFO` & `guilded.py-1.8.0/guilded.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guilded.py
-Version: 1.7.0
+Version: 1.8.0
 Summary: An API wrapper in Python for Guilded's bot API
 Home-page: https://github.com/shayypy/guilded.py
 Author: shay (shayypy)
 License: MIT
 Project-URL: Documentation, https://guildedpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/shayypy/guilded.py/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `guilded.py-1.7.0/guilded.py.egg-info/SOURCES.txt` & `guilded.py-1.8.0/guilded.py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 guilded/ext/commands/converters.py
 guilded/ext/commands/cooldowns.py
 guilded/ext/commands/core.py
 guilded/ext/commands/errors.py
 guilded/ext/commands/help.py
 guilded/ext/commands/view.py
 guilded/ext/tasks/__init__.py
+guilded/types/announcement.py
 guilded/types/calendar_event.py
 guilded/types/channel.py
 guilded/types/comment.py
 guilded/types/doc.py
 guilded/types/embed.py
 guilded/types/emote.py
 guilded/types/forum_topic.py
```

### Comparing `guilded.py-1.7.0/setup.py` & `guilded.py-1.8.0/setup.py`

 * *Files identical despite different names*

