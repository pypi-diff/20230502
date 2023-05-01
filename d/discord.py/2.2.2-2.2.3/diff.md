# Comparing `tmp/discord.py-2.2.2.tar.gz` & `tmp/discord.py-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord.py-2.2.2.tar", last modified: Thu Mar  2 03:49:03 2023, max compression
+gzip compressed data, was "discord.py-2.2.3.tar", last modified: Mon May  1 22:22:20 2023, max compression
```

## Comparing `discord.py-2.2.2.tar` & `discord.py-2.2.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.735011 discord.py-2.2.2/
--rw-rw-rw-   0        0        0     1081 2021-02-02 07:58:56.000000 discord.py-2.2.2/LICENSE
--rw-rw-rw-   0        0        0      111 2021-08-22 06:25:27.000000 discord.py-2.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4212 2023-03-02 03:49:03.735011 discord.py-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-02-11 23:42:40.000000 discord.py-2.2.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.672640 discord.py-2.2.2/discord/
--rw-rw-rw-   0        0        0     1886 2023-03-02 03:48:02.000000 discord.py-2.2.2/discord/__init__.py
--rw-rw-rw-   0        0        0    11051 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/__main__.py
--rw-rw-rw-   0        0        0     1410 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/_types.py
--rw-rw-rw-   0        0        0    65763 2023-02-25 10:27:47.000000 discord.py-2.2.2/discord/abc.py
--rw-rw-rw-   0        0        0    26864 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/activity.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.691973 discord.py-2.2.2/discord/app_commands/
--rw-rw-rw-   0        0        0      424 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/__init__.py
--rw-rw-rw-   0        0        0    18077 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/checks.py
--rw-rw-rw-   0        0        0    95614 2023-02-25 10:27:47.000000 discord.py-2.2.2/discord/app_commands/commands.py
--rw-rw-rw-   0        0        0    19006 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/errors.py
--rw-rw-rw-   0        0        0    38500 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/models.py
--rw-rw-rw-   0        0        0    13123 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/namespace.py
--rw-rw-rw-   0        0        0    32499 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/transformers.py
--rw-rw-rw-   0        0        0    10686 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/app_commands/translator.py
--rw-rw-rw-   0        0        0    47965 2023-02-25 10:27:47.000000 discord.py-2.2.2/discord/app_commands/tree.py
--rw-rw-rw-   0        0        0    10921 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/appinfo.py
--rw-rw-rw-   0        0        0    15837 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/asset.py
--rw-rw-rw-   0        0        0    34509 2023-02-25 11:04:50.000000 discord.py-2.2.2/discord/audit_logs.py
--rw-rw-rw-   0        0        0    23488 2023-02-27 01:22:42.000000 discord.py-2.2.2/discord/automod.py
--rw-rw-rw-   0        0        0     3751 2022-02-22 03:41:08.000000 discord.py-2.2.2/discord/backoff.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.693975 discord.py-2.2.2/discord/bin/
--rw-rw-rw-   0        0        0   441856 2021-02-02 07:58:56.000000 discord.py-2.2.2/discord/bin/libopus-0.x64.dll
--rw-rw-rw-   0        0        0   366080 2021-02-02 07:58:56.000000 discord.py-2.2.2/discord/bin/libopus-0.x86.dll
--rw-rw-rw-   0        0        0   114410 2023-02-25 10:27:47.000000 discord.py-2.2.2/discord/channel.py
--rw-rw-rw-   0        0        0    84965 2023-03-02 03:47:33.000000 discord.py-2.2.2/discord/client.py
--rw-rw-rw-   0        0        0    14168 2023-02-28 14:02:42.000000 discord.py-2.2.2/discord/colour.py
--rw-rw-rw-   0        0        0    16836 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/components.py
--rw-rw-rw-   0        0        0     3032 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/context_managers.py
--rw-rw-rw-   0        0        0    22722 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/embeds.py
--rw-rw-rw-   0        0        0     8574 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/emoji.py
--rw-rw-rw-   0        0        0    22131 2023-02-28 05:32:35.000000 discord.py-2.2.2/discord/enums.py
--rw-rw-rw-   0        0        0     8952 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/errors.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.627599 discord.py-2.2.2/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.704985 discord.py-2.2.2/discord/ext/commands/
--rw-rw-rw-   0        0        0      437 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     2638 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    51719 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/bot.py
--rw-rw-rw-   0        0        0    30163 2023-02-28 07:20:21.000000 discord.py-2.2.2/discord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    34547 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/context.py
--rw-rw-rw-   0        0        0    45392 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/converter.py
--rw-rw-rw-   0        0        0     9716 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    89352 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/core.py
--rw-rw-rw-   0        0        0    36151 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22966 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    57705 2023-02-25 10:27:47.000000 discord.py-2.2.2/discord/ext/commands/help.py
--rw-rw-rw-   0        0        0    36595 2023-03-02 03:47:33.000000 discord.py-2.2.2/discord/ext/commands/hybrid.py
--rw-rw-rw-   0        0        0     8361 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/parameters.py
--rw-rw-rw-   0        0        0     6247 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.705985 discord.py-2.2.2/discord/ext/tasks/
--rw-rw-rw-   0        0        0    29180 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     5378 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/file.py
--rw-rw-rw-   0        0        0    52208 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/flags.py
--rw-rw-rw-   0        0        0    34937 2023-03-02 00:44:50.000000 discord.py-2.2.2/discord/gateway.py
--rw-rw-rw-   0        0        0   140799 2023-02-28 07:20:21.000000 discord.py-2.2.2/discord/guild.py
--rw-rw-rw-   0        0        0    89365 2023-02-28 05:32:35.000000 discord.py-2.2.2/discord/http.py
--rw-rw-rw-   0        0        0    13334 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/integrations.py
--rw-rw-rw-   0        0        0    44412 2023-02-14 04:54:29.000000 discord.py-2.2.2/discord/interactions.py
--rw-rw-rw-   0        0        0    20595 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/invite.py
--rw-rw-rw-   0        0        0    40760 2023-02-25 08:13:35.000000 discord.py-2.2.2/discord/member.py
--rw-rw-rw-   0        0        0     5592 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/mentions.py
--rw-rw-rw-   0        0        0    82150 2023-02-28 05:32:35.000000 discord.py-2.2.2/discord/message.py
--rw-rw-rw-   0        0        0     1485 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/mixins.py
--rw-rw-rw-   0        0        0     3702 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/object.py
--rw-rw-rw-   0        0        0     3646 2022-02-20 10:26:28.000000 discord.py-2.2.2/discord/oggparse.py
--rw-rw-rw-   0        0        0    15065 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/opus.py
--rw-rw-rw-   0        0        0     7950 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/partial_emoji.py
--rw-rw-rw-   0        0        0    28320 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/permissions.py
--rw-rw-rw-   0        0        0    26456 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/player.py
--rw-rw-rw-   0        0        0        0 2021-08-22 06:25:27.000000 discord.py-2.2.2/discord/py.typed
--rw-rw-rw-   0        0        0    16826 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/raw_models.py
--rw-rw-rw-   0        0        0     8229 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/reaction.py
--rw-rw-rw-   0        0        0    17906 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/role.py
--rw-rw-rw-   0        0        0    23655 2023-02-28 05:32:35.000000 discord.py-2.2.2/discord/scheduled_event.py
--rw-rw-rw-   0        0        0    20129 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/shard.py
--rw-rw-rw-   0        0        0     6498 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/stage_instance.py
--rw-rw-rw-   0        0        0    73314 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/state.py
--rw-rw-rw-   0        0        0    16029 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/sticker.py
--rw-rw-rw-   0        0        0     4607 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/team.py
--rw-rw-rw-   0        0        0     9574 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/template.py
--rw-rw-rw-   0        0        0    32449 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/threads.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.726003 discord.py-2.2.2/discord/types/
--rw-rw-rw-   0        0        0      149 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/types/__init__.py
--rw-rw-rw-   0        0        0     2707 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/activity.py
--rw-rw-rw-   0        0        0     2386 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/appinfo.py
--rw-rw-rw-   0        0        0     8192 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/audit_log.py
--rw-rw-rw-   0        0        0     4009 2023-02-27 01:22:42.000000 discord.py-2.2.2/discord/types/automod.py
--rw-rw-rw-   0        0        0     4557 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/channel.py
--rw-rw-rw-   0        0        0     6266 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/command.py
--rw-rw-rw-   0        0        0     3057 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/components.py
--rw-rw-rw-   0        0        0     2329 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/embed.py
--rw-rw-rw-   0        0        0     1528 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/types/emoji.py
--rw-rw-rw-   0        0        0     8453 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/gateway.py
--rw-rw-rw-   0        0        0     5197 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/guild.py
--rw-rw-rw-   0        0        0     2288 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/integration.py
--rw-rw-rw-   0        0        0     6923 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/interactions.py
--rw-rw-rw-   0        0        0     2704 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/invite.py
--rw-rw-rw-   0        0        0     1898 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/member.py
--rw-rw-rw-   0        0        0     4182 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/message.py
--rw-rw-rw-   0        0        0     1746 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/role.py
--rw-rw-rw-   0        0        0     3294 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1182 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/types/snowflake.py
--rw-rw-rw-   0        0        0     2244 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/sticker.py
--rw-rw-rw-   0        0        0     1499 2022-02-20 10:26:29.000000 discord.py-2.2.2/discord/types/team.py
--rw-rw-rw-   0        0        0     1609 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/types/template.py
--rw-rw-rw-   0        0        0     2454 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/threads.py
--rw-rw-rw-   0        0        0     1540 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/types/user.py
--rw-rw-rw-   0        0        0     2268 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/voice.py
--rw-rw-rw-   0        0        0     1978 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/webhook.py
--rw-rw-rw-   0        0        0     1460 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1883 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.732008 discord.py-2.2.2/discord/ui/
--rw-rw-rw-   0        0        0      285 2022-02-20 10:13:32.000000 discord.py-2.2.2/discord/ui/__init__.py
--rw-rw-rw-   0        0        0    10620 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ui/button.py
--rw-rw-rw-   0        0        0     5899 2023-02-28 07:04:17.000000 discord.py-2.2.2/discord/ui/dynamic.py
--rw-rw-rw-   0        0        0     4372 2023-03-02 00:44:50.000000 discord.py-2.2.2/discord/ui/item.py
--rw-rw-rw-   0        0        0     7012 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ui/modal.py
--rw-rw-rw-   0        0        0    34049 2023-03-02 00:44:50.000000 discord.py-2.2.2/discord/ui/select.py
--rw-rw-rw-   0        0        0     8058 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/ui/text_input.py
--rw-rw-rw-   0        0        0    22878 2023-02-14 04:54:29.000000 discord.py-2.2.2/discord/ui/view.py
--rw-rw-rw-   0        0        0    15390 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/user.py
--rw-rw-rw-   0        0        0    41360 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/utils.py
--rw-rw-rw-   0        0        0    24974 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.734010 discord.py-2.2.2/discord/webhook/
--rw-rw-rw-   0        0        0      182 2021-08-15 18:01:53.000000 discord.py-2.2.2/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0    69566 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/webhook/async_.py
--rw-rw-rw-   0        0        0    42519 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/webhook/sync.py
--rw-rw-rw-   0        0        0     7539 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/welcome_screen.py
--rw-rw-rw-   0        0        0    10162 2023-02-11 23:42:40.000000 discord.py-2.2.2/discord/widget.py
-drwxrwxrwx   0        0        0        0 2023-03-02 03:49:03.684966 discord.py-2.2.2/discord.py.egg-info/
--rw-rw-rw-   0        0        0     4212 2023-03-02 03:49:03.000000 discord.py-2.2.2/discord.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3092 2023-03-02 03:49:03.000000 discord.py-2.2.2/discord.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 03:49:03.000000 discord.py-2.2.2/discord.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      330 2023-03-02 03:49:03.000000 discord.py-2.2.2/discord.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-02 03:49:03.000000 discord.py-2.2.2/discord.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      869 2023-02-11 23:42:40.000000 discord.py-2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       18 2023-02-11 23:42:40.000000 discord.py-2.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-02 03:49:03.735011 discord.py-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2946 2023-02-11 23:42:40.000000 discord.py-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.584710 discord.py-2.2.3/
+-rw-rw-rw-   0        0        0     1081 2021-02-02 07:58:56.000000 discord.py-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0      111 2021-08-22 06:25:27.000000 discord.py-2.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4212 2023-05-01 22:22:20.584710 discord.py-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-02-11 23:42:40.000000 discord.py-2.2.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.459598 discord.py-2.2.3/discord/
+-rw-rw-rw-   0        0        0     1886 2023-05-01 22:14:33.000000 discord.py-2.2.3/discord/__init__.py
+-rw-rw-rw-   0        0        0    11051 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/__main__.py
+-rw-rw-rw-   0        0        0     1410 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/_types.py
+-rw-rw-rw-   0        0        0    65763 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/abc.py
+-rw-rw-rw-   0        0        0    26864 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/activity.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.472610 discord.py-2.2.3/discord/app_commands/
+-rw-rw-rw-   0        0        0      424 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18077 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    95614 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19006 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    38500 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13123 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    32499 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    10686 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    47965 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    10921 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/appinfo.py
+-rw-rw-rw-   0        0        0    15837 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/asset.py
+-rw-rw-rw-   0        0        0    34880 2023-05-01 22:00:03.000000 discord.py-2.2.3/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    23488 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/automod.py
+-rw-rw-rw-   0        0        0     3751 2022-02-22 03:41:08.000000 discord.py-2.2.3/discord/backoff.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.513646 discord.py-2.2.3/discord/bin/
+-rw-rw-rw-   0        0        0   441856 2021-02-02 07:58:56.000000 discord.py-2.2.3/discord/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2021-02-02 07:58:56.000000 discord.py-2.2.3/discord/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0   114410 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/channel.py
+-rw-rw-rw-   0        0        0    84965 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/client.py
+-rw-rw-rw-   0        0        0    14168 2023-02-28 14:02:42.000000 discord.py-2.2.3/discord/colour.py
+-rw-rw-rw-   0        0        0    16836 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/components.py
+-rw-rw-rw-   0        0        0     3032 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/context_managers.py
+-rw-rw-rw-   0        0        0    22722 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/embeds.py
+-rw-rw-rw-   0        0        0     8574 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/emoji.py
+-rw-rw-rw-   0        0        0    22131 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/enums.py
+-rw-rw-rw-   0        0        0     8952 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.392538 discord.py-2.2.3/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.534666 discord.py-2.2.3/discord/ext/commands/
+-rw-rw-rw-   0        0        0      437 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    51719 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    30163 2023-02-28 07:20:21.000000 discord.py-2.2.3/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    34547 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    45392 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0     9716 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    89352 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36151 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22966 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    57705 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    36595 2023-03-02 03:47:33.000000 discord.py-2.2.3/discord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     8361 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6247 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.535666 discord.py-2.2.3/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    29180 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5378 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/file.py
+-rw-rw-rw-   0        0        0    52208 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/flags.py
+-rw-rw-rw-   0        0        0    34937 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/gateway.py
+-rw-rw-rw-   0        0        0   140799 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/guild.py
+-rw-rw-rw-   0        0        0    89365 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/http.py
+-rw-rw-rw-   0        0        0    13334 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/integrations.py
+-rw-rw-rw-   0        0        0    44412 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/interactions.py
+-rw-rw-rw-   0        0        0    20595 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/invite.py
+-rw-rw-rw-   0        0        0    40760 2023-02-25 08:13:35.000000 discord.py-2.2.3/discord/member.py
+-rw-rw-rw-   0        0        0     5592 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/mentions.py
+-rw-rw-rw-   0        0        0    82150 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/message.py
+-rw-rw-rw-   0        0        0     1485 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/mixins.py
+-rw-rw-rw-   0        0        0     3702 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/object.py
+-rw-rw-rw-   0        0        0     3646 2022-02-20 10:26:28.000000 discord.py-2.2.3/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15065 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/opus.py
+-rw-rw-rw-   0        0        0     7950 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    28320 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/permissions.py
+-rw-rw-rw-   0        0        0    26456 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/player.py
+-rw-rw-rw-   0        0        0        0 2021-08-22 06:25:27.000000 discord.py-2.2.3/discord/py.typed
+-rw-rw-rw-   0        0        0    16826 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8229 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/reaction.py
+-rw-rw-rw-   0        0        0    17906 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/role.py
+-rw-rw-rw-   0        0        0    23655 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    20129 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/shard.py
+-rw-rw-rw-   0        0        0     6498 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/stage_instance.py
+-rw-rw-rw-   0        0        0    73314 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/state.py
+-rw-rw-rw-   0        0        0    16039 2023-05-01 21:59:43.000000 discord.py-2.2.3/discord/sticker.py
+-rw-rw-rw-   0        0        0     4607 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/team.py
+-rw-rw-rw-   0        0        0     9574 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/template.py
+-rw-rw-rw-   0        0        0    32449 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/threads.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.572699 discord.py-2.2.3/discord/types/
+-rw-rw-rw-   0        0        0      149 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/activity.py
+-rw-rw-rw-   0        0        0     2386 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8192 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4009 2023-02-27 01:22:42.000000 discord.py-2.2.3/discord/types/automod.py
+-rw-rw-rw-   0        0        0     4557 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/channel.py
+-rw-rw-rw-   0        0        0     6266 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/command.py
+-rw-rw-rw-   0        0        0     3057 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/components.py
+-rw-rw-rw-   0        0        0     2329 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1528 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     8453 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5197 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2288 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/integration.py
+-rw-rw-rw-   0        0        0     6923 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2704 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1898 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/member.py
+-rw-rw-rw-   0        0        0     4182 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/message.py
+-rw-rw-rw-   0        0        0     1746 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/role.py
+-rw-rw-rw-   0        0        0     3294 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1182 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2257 2023-05-01 21:59:43.000000 discord.py-2.2.3/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1499 2022-02-20 10:26:29.000000 discord.py-2.2.3/discord/types/team.py
+-rw-rw-rw-   0        0        0     1609 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/template.py
+-rw-rw-rw-   0        0        0     2454 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1540 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/user.py
+-rw-rw-rw-   0        0        0     2268 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/voice.py
+-rw-rw-rw-   0        0        0     1978 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1460 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1883 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.580706 discord.py-2.2.3/discord/ui/
+-rw-rw-rw-   0        0        0      285 2022-02-20 10:13:32.000000 discord.py-2.2.3/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0    10620 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ui/button.py
+-rw-rw-rw-   0        0        0     5899 2023-02-28 07:04:17.000000 discord.py-2.2.3/discord/ui/dynamic.py
+-rw-rw-rw-   0        0        0     4372 2023-03-02 00:44:50.000000 discord.py-2.2.3/discord/ui/item.py
+-rw-rw-rw-   0        0        0     7012 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ui/modal.py
+-rw-rw-rw-   0        0        0    34049 2023-03-02 00:44:50.000000 discord.py-2.2.3/discord/ui/select.py
+-rw-rw-rw-   0        0        0     8058 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ui/text_input.py
+-rw-rw-rw-   0        0        0    22878 2023-02-14 04:54:29.000000 discord.py-2.2.3/discord/ui/view.py
+-rw-rw-rw-   0        0        0    15390 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/user.py
+-rw-rw-rw-   0        0        0    41360 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/utils.py
+-rw-rw-rw-   0        0        0    24974 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.583709 discord.py-2.2.3/discord/webhook/
+-rw-rw-rw-   0        0        0      182 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    69567 2023-05-01 22:00:19.000000 discord.py-2.2.3/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42520 2023-05-01 22:00:19.000000 discord.py-2.2.3/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7539 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10162 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.463602 discord.py-2.2.3/discord.py.egg-info/
+-rw-rw-rw-   0        0        0     4212 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3092 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      330 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      869 2023-02-11 23:42:40.000000 discord.py-2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       18 2023-02-11 23:42:40.000000 discord.py-2.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 22:22:20.584710 discord.py-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2946 2023-02-11 23:42:40.000000 discord.py-2.2.3/setup.py
```

### Comparing `discord.py-2.2.2/LICENSE` & `discord.py-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/PKG-INFO` & `discord.py-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.py
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/Rapptz/discord.py
 Author: Rapptz
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Rapptz/discord.py/issues
 Platform: UNKNOWN
```

### Comparing `discord.py-2.2.2/README.rst` & `discord.py-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/__init__.py` & `discord.py-2.2.3/discord/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 """
 
 __title__ = 'discord'
 __author__ = 'Rapptz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2015-present Rapptz'
-__version__ = '2.2.2'
+__version__ = '2.2.3'
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
 from .client import *
@@ -74,12 +74,12 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=2, minor=2, micro=2, releaselevel='final', serial=0)
+version_info: VersionInfo = VersionInfo(major=2, minor=2, micro=3, releaselevel='final', serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 del logging, NamedTuple, Literal, VersionInfo
```

### Comparing `discord.py-2.2.2/discord/__main__.py` & `discord.py-2.2.3/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/_types.py` & `discord.py-2.2.3/discord/_types.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/abc.py` & `discord.py-2.2.3/discord/abc.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/activity.py` & `discord.py-2.2.3/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/checks.py` & `discord.py-2.2.3/discord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/commands.py` & `discord.py-2.2.3/discord/app_commands/commands.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/errors.py` & `discord.py-2.2.3/discord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/models.py` & `discord.py-2.2.3/discord/app_commands/models.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/namespace.py` & `discord.py-2.2.3/discord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/transformers.py` & `discord.py-2.2.3/discord/app_commands/transformers.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/translator.py` & `discord.py-2.2.3/discord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/app_commands/tree.py` & `discord.py-2.2.3/discord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/appinfo.py` & `discord.py-2.2.3/discord/appinfo.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/asset.py` & `discord.py-2.2.3/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/audit_logs.py` & `discord.py-2.2.3/discord/audit_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 class _AuditLogProxyMessageBulkDelete(_AuditLogProxy):
     count: int
 
 
 class _AuditLogProxyAutoModAction(_AuditLogProxy):
     automod_rule_name: str
     automod_rule_trigger_type: str
-    channel: Union[abc.GuildChannel, Thread]
+    channel: Optional[Union[abc.GuildChannel, Thread]]
 
 
 class AuditLogEntry(Hashable):
     r"""Represents an Audit Log entry.
 
     You retrieve these via :meth:`Guild.audit_logs`.
 
@@ -640,21 +640,25 @@
                     message_id=int(extra['message_id']),
                 )
             elif (
                 self.action is enums.AuditLogAction.automod_block_message
                 or self.action is enums.AuditLogAction.automod_flag_message
                 or self.action is enums.AuditLogAction.automod_timeout_member
             ):
-                channel_id = int(extra['channel_id'])
+                channel_id = utils._get_as_snowflake(extra, 'channel_id')
+                channel = None
+                if channel_id is not None:
+                    channel = self.guild.get_channel_or_thread(channel_id) or Object(id=channel_id)
+
                 self.extra = _AuditLogProxyAutoModAction(
                     automod_rule_name=extra['auto_moderation_rule_name'],
                     automod_rule_trigger_type=enums.try_enum(
                         enums.AutoModRuleTriggerType, extra['auto_moderation_rule_trigger_type']
                     ),
-                    channel=self.guild.get_channel_or_thread(channel_id) or Object(id=channel_id),
+                    channel=channel,
                 )
 
             elif self.action.name.startswith('overwrite_'):
                 # the overwrite_ actions have a dict with some information
                 instance_id = int(extra['id'])
                 the_type = extra.get('type')
                 if the_type == '1':
@@ -719,20 +723,19 @@
         return utils.snowflake_time(self.id)
 
     @utils.cached_property
     def target(self) -> TargetType:
         if self.action.target_type is None:
             return None
 
-        if self._target_id is None:
-            return None
-
         try:
             converter = getattr(self, '_convert_target_' + self.action.target_type)
         except AttributeError:
+            if self._target_id is None:
+                return None
             return Object(id=self._target_id)
         else:
             return converter(self._target_id)
 
     @utils.cached_property
     def category(self) -> Optional[enums.AuditLogActionCategory]:
         """Optional[:class:`AuditLogActionCategory`]: The category of the action, if applicable."""
@@ -757,15 +760,20 @@
 
     def _convert_target_guild(self, target_id: int) -> Guild:
         return self.guild
 
     def _convert_target_channel(self, target_id: int) -> Union[abc.GuildChannel, Object]:
         return self.guild.get_channel(target_id) or Object(id=target_id)
 
-    def _convert_target_user(self, target_id: int) -> Union[Member, User, Object]:
+    def _convert_target_user(self, target_id: Optional[int]) -> Optional[Union[Member, User, Object]]:
+        # For some reason the member_disconnect and member_move action types
+        # do not have a non-null target_id so safeguard against that
+        if target_id is None:
+            return None
+
         return self._get_member(target_id) or Object(id=target_id, type=Member)
 
     def _convert_target_role(self, target_id: int) -> Union[Role, Object]:
         return self.guild.get_role(target_id) or Object(id=target_id, type=Role)
 
     def _convert_target_invite(self, target_id: None) -> Invite:
         # invites have target_id set to null
```

### Comparing `discord.py-2.2.2/discord/automod.py` & `discord.py-2.2.3/discord/automod.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/backoff.py` & `discord.py-2.2.3/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/bin/libopus-0.x64.dll` & `discord.py-2.2.3/discord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/bin/libopus-0.x86.dll` & `discord.py-2.2.3/discord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/channel.py` & `discord.py-2.2.3/discord/channel.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/client.py` & `discord.py-2.2.3/discord/client.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/colour.py` & `discord.py-2.2.3/discord/colour.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/components.py` & `discord.py-2.2.3/discord/components.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/context_managers.py` & `discord.py-2.2.3/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/embeds.py` & `discord.py-2.2.3/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/emoji.py` & `discord.py-2.2.3/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/enums.py` & `discord.py-2.2.3/discord/enums.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/errors.py` & `discord.py-2.2.3/discord/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/_types.py` & `discord.py-2.2.3/discord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/bot.py` & `discord.py-2.2.3/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/cog.py` & `discord.py-2.2.3/discord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/context.py` & `discord.py-2.2.3/discord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/converter.py` & `discord.py-2.2.3/discord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/cooldowns.py` & `discord.py-2.2.3/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/core.py` & `discord.py-2.2.3/discord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/errors.py` & `discord.py-2.2.3/discord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/flags.py` & `discord.py-2.2.3/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/help.py` & `discord.py-2.2.3/discord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/hybrid.py` & `discord.py-2.2.3/discord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/parameters.py` & `discord.py-2.2.3/discord/ext/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/commands/view.py` & `discord.py-2.2.3/discord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ext/tasks/__init__.py` & `discord.py-2.2.3/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/file.py` & `discord.py-2.2.3/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/flags.py` & `discord.py-2.2.3/discord/flags.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/gateway.py` & `discord.py-2.2.3/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/guild.py` & `discord.py-2.2.3/discord/guild.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/http.py` & `discord.py-2.2.3/discord/http.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/integrations.py` & `discord.py-2.2.3/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/interactions.py` & `discord.py-2.2.3/discord/interactions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/invite.py` & `discord.py-2.2.3/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/member.py` & `discord.py-2.2.3/discord/member.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/mentions.py` & `discord.py-2.2.3/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/message.py` & `discord.py-2.2.3/discord/message.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/mixins.py` & `discord.py-2.2.3/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/object.py` & `discord.py-2.2.3/discord/object.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/oggparse.py` & `discord.py-2.2.3/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/opus.py` & `discord.py-2.2.3/discord/opus.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/partial_emoji.py` & `discord.py-2.2.3/discord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/permissions.py` & `discord.py-2.2.3/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/player.py` & `discord.py-2.2.3/discord/player.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/raw_models.py` & `discord.py-2.2.3/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/reaction.py` & `discord.py-2.2.3/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/role.py` & `discord.py-2.2.3/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/scheduled_event.py` & `discord.py-2.2.3/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/shard.py` & `discord.py-2.2.3/discord/shard.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/stage_instance.py` & `discord.py-2.2.3/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/state.py` & `discord.py-2.2.3/discord/state.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/sticker.py` & `discord.py-2.2.3/discord/sticker.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         The name of a unicode emoji that represents this sticker.
     """
 
     __slots__ = ('available', 'guild_id', 'user', 'emoji', 'type', '_cs_guild')
 
     def _from_data(self, data: GuildStickerPayload) -> None:
         super()._from_data(data)
-        self.available: bool = data['available']
+        self.available: bool = data.get('available', True)
         self.guild_id: int = int(data['guild_id'])
         user = data.get('user')
         self.user: Optional[User] = self._state.store_user(user) if user else None
         self.emoji: str = data['tags']
         self.type: StickerType = StickerType.guild
 
     def __repr__(self) -> str:
```

### Comparing `discord.py-2.2.2/discord/team.py` & `discord.py-2.2.3/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/template.py` & `discord.py-2.2.3/discord/template.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/threads.py` & `discord.py-2.2.3/discord/threads.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/activity.py` & `discord.py-2.2.3/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/appinfo.py` & `discord.py-2.2.3/discord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/audit_log.py` & `discord.py-2.2.3/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/automod.py` & `discord.py-2.2.3/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/channel.py` & `discord.py-2.2.3/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/command.py` & `discord.py-2.2.3/discord/types/command.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/components.py` & `discord.py-2.2.3/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/embed.py` & `discord.py-2.2.3/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/emoji.py` & `discord.py-2.2.3/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/gateway.py` & `discord.py-2.2.3/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/guild.py` & `discord.py-2.2.3/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/integration.py` & `discord.py-2.2.3/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/interactions.py` & `discord.py-2.2.3/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/invite.py` & `discord.py-2.2.3/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/member.py` & `discord.py-2.2.3/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/message.py` & `discord.py-2.2.3/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/role.py` & `discord.py-2.2.3/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/scheduled_event.py` & `discord.py-2.2.3/discord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/snowflake.py` & `discord.py-2.2.3/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/sticker.py` & `discord.py-2.2.3/discord/types/sticker.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     type: Literal[1]
     sort_value: int
     pack_id: Snowflake
 
 
 class GuildSticker(BaseSticker):
     type: Literal[2]
-    available: bool
+    available: NotRequired[bool]
     guild_id: Snowflake
     user: NotRequired[User]
 
 
 Sticker = Union[StandardSticker, GuildSticker]
```

### Comparing `discord.py-2.2.2/discord/types/team.py` & `discord.py-2.2.3/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/template.py` & `discord.py-2.2.3/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/threads.py` & `discord.py-2.2.3/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/user.py` & `discord.py-2.2.3/discord/types/user.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/voice.py` & `discord.py-2.2.3/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/webhook.py` & `discord.py-2.2.3/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/welcome_screen.py` & `discord.py-2.2.3/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/types/widget.py` & `discord.py-2.2.3/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/button.py` & `discord.py-2.2.3/discord/ui/button.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/dynamic.py` & `discord.py-2.2.3/discord/ui/dynamic.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/item.py` & `discord.py-2.2.3/discord/ui/item.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/modal.py` & `discord.py-2.2.3/discord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/select.py` & `discord.py-2.2.3/discord/ui/select.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/text_input.py` & `discord.py-2.2.3/discord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/ui/view.py` & `discord.py-2.2.3/discord/ui/view.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/user.py` & `discord.py-2.2.3/discord/user.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/utils.py` & `discord.py-2.2.3/discord/utils.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/voice_client.py` & `discord.py-2.2.3/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/webhook/async_.py` & `discord.py-2.2.3/discord/webhook/async_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1507,16 +1507,15 @@
                 self.auth_token,
                 payload=payload,
                 session=self.session,
                 proxy=self.proxy,
                 proxy_auth=self.proxy_auth,
                 reason=reason,
             )
-
-        if prefer_auth and self.auth_token:
+        elif prefer_auth and self.auth_token:
             data = await adapter.edit_webhook(
                 self.id,
                 self.auth_token,
                 payload=payload,
                 session=self.session,
                 proxy=self.proxy,
                 proxy_auth=self.proxy_auth,
```

### Comparing `discord.py-2.2.2/discord/webhook/sync.py` & `discord.py-2.2.3/discord/webhook/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -831,16 +831,15 @@
         # If a channel is given, always use the authenticated endpoint
         if channel is not None:
             if self.auth_token is None:
                 raise ValueError('Editing channel requires authenticated webhook')
 
             payload['channel_id'] = channel.id
             data = adapter.edit_webhook(self.id, self.auth_token, payload=payload, session=self.session, reason=reason)
-
-        if prefer_auth and self.auth_token:
+        elif prefer_auth and self.auth_token:
             data = adapter.edit_webhook(self.id, self.auth_token, payload=payload, session=self.session, reason=reason)
         elif self.token:
             data = adapter.edit_webhook_with_token(self.id, self.token, payload=payload, session=self.session, reason=reason)
 
         if data is None:
             raise RuntimeError('Unreachable code hit: data was not assigned')
```

### Comparing `discord.py-2.2.2/discord/welcome_screen.py` & `discord.py-2.2.3/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord/widget.py` & `discord.py-2.2.3/discord/widget.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/discord.py.egg-info/PKG-INFO` & `discord.py-2.2.3/discord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.py
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/Rapptz/discord.py
 Author: Rapptz
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Rapptz/discord.py/issues
 Platform: UNKNOWN
```

### Comparing `discord.py-2.2.2/discord.py.egg-info/SOURCES.txt` & `discord.py-2.2.3/discord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/pyproject.toml` & `discord.py-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.2/setup.py` & `discord.py-2.2.3/setup.py`

 * *Files identical despite different names*

