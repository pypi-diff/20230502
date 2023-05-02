# Comparing `tmp/chat_exporter_hikari-1.0.0.tar.gz` & `tmp/chat_exporter_hikari-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_exporter_hikari-1.0.0.tar", last modified: Sat Feb 25 23:30:09 2023, max compression
+gzip compressed data, was "chat_exporter_hikari-1.0.1.tar", last modified: Tue May  2 08:03:00 2023, max compression
```

## Comparing `chat_exporter_hikari-1.0.0.tar` & `chat_exporter_hikari-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.785150 chat_exporter_hikari-1.0.0/
--rw-rw-rw-   0        0        0    35803 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       79 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11675 2023-02-25 23:30:09.784649 chat_exporter_hikari-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10518 2023-02-02 08:26:52.000000 chat_exporter_hikari-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.723083 chat_exporter_hikari-1.0.0/chat_exporter/
--rw-rw-rw-   0        0        0      212 2023-02-25 23:29:30.000000 chat_exporter_hikari-1.0.0/chat_exporter/__init__.py
--rw-rw-rw-   0        0        0     6398 2023-01-30 16:45:05.000000 chat_exporter_hikari-1.0.0/chat_exporter/chat_exporter.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.725583 chat_exporter_hikari-1.0.0/chat_exporter/construct/
--rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.731092 chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/
--rw-rw-rw-   0        0        0      206 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/__init__.py
--rw-rw-rw-   0        0        0     4010 2023-01-30 13:28:46.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/attachment.py
--rw-rw-rw-   0        0        0     3974 2023-01-30 16:53:27.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/component.py
--rw-rw-rw-   0        0        0     5957 2023-02-25 23:23:41.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/embed.py
--rw-rw-rw-   0        0        0     1544 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/reaction.py
--rw-rw-rw-   0        0        0    16881 2023-02-25 23:28:37.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/message.py
--rw-rw-rw-   0        0        0     6669 2023-02-22 22:39:42.000000 chat_exporter_hikari-1.0.0/chat_exporter/construct/transcript.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.736600 chat_exporter_hikari-1.0.0/chat_exporter/ext/
--rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/ext/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/ext/cache.py
--rw-rw-rw-   0        0        0      199 2023-01-30 12:10:56.000000 chat_exporter_hikari-1.0.0/chat_exporter/ext/discord_import.py
--rw-rw-rw-   0        0        0     1869 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/ext/discord_utils.py
--rw-rw-rw-   0        0        0     4210 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/ext/emoji_convert.py
--rw-rw-rw-   0        0        0     4146 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/ext/html_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.738108 chat_exporter_hikari-1.0.0/chat_exporter/html/
--rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.742610 chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/
--rw-rw-rw-   0        0        0      774 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/audio.html
--rw-rw-rw-   0        0        0      140 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/image.html
--rw-rw-rw-   0        0        0      547 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/message.html
--rw-rw-rw-   0        0        0      127 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/video.html
--rw-rw-rw-   0        0        0    43437 2023-01-30 16:14:47.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/base.html
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.745608 chat_exporter_hikari-1.0.0/chat_exporter/html/component/
--rw-rw-rw-   0        0        0      229 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/component/component_button.html
--rw-rw-rw-   0        0        0      254 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/component/component_menu.html
--rw-rw-rw-   0        0        0      159 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/component/component_menu_options.html
--rw-rw-rw-   0        0        0      508 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/component/component_menu_options_emoji.html
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.755617 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/
--rw-rw-rw-   0        0        0      123 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/author.html
--rw-rw-rw-   0        0        0      225 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/author_icon.html
--rw-rw-rw-   0        0        0      667 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/body.html
--rw-rw-rw-   0        0        0      116 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/description.html
--rw-rw-rw-   0        0        0      317 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/field-inline.html
--rw-rw-rw-   0        0        0      306 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/field.html
--rw-rw-rw-   0        0        0      113 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/footer.html
--rw-rw-rw-   0        0        0      183 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/footer_image.html
--rw-rw-rw-   0        0        0      186 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/image.html
--rw-rw-rw-   0        0        0      206 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/thumbnail.html
--rw-rw-rw-   0        0        0       97 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/embed/title.html
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.765632 chat_exporter_hikari-1.0.0/chat_exporter/html/message/
--rw-rw-rw-   0        0        0      239 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/bot-tag-verified.html
--rw-rw-rw-   0        0        0       43 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/bot-tag.html
--rw-rw-rw-   0        0        0       77 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/content.html
--rw-rw-rw-   0        0        0        6 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/end.html
--rw-rw-rw-   0        0        0      528 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/interaction.html
--rw-rw-rw-   0        0        0      952 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/message.html
--rw-rw-rw-   0        0        0     1108 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/meta.html
--rw-rw-rw-   0        0        0     1021 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/pin.html
--rw-rw-rw-   0        0        0      558 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/reference.html
--rw-rw-rw-   0        0        0      131 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/reference_unknown.html
--rw-rw-rw-   0        0        0     1254 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/start.html
--rw-rw-rw-   0        0        0      895 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/message/thread.html
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.767641 chat_exporter_hikari-1.0.0/chat_exporter/html/reaction/
--rw-rw-rw-   0        0        0      206 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/reaction/custom_emoji.html
--rw-rw-rw-   0        0        0      120 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/reaction/emoji.html
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.770141 chat_exporter_hikari-1.0.0/chat_exporter/html/script/
--rw-rw-rw-   0        0        0      112 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/script/channel_subject.html
--rw-rw-rw-   0        0        0       59 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/script/channel_topic.html
--rw-rw-rw-   0        0        0     1183 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/html/script/fancy_time.html
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.772641 chat_exporter_hikari-1.0.0/chat_exporter/parse/
--rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/parse/__init__.py
--rw-rw-rw-   0        0        0    13090 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.0/chat_exporter/parse/markdown.py
--rw-rw-rw-   0        0        0     6705 2023-01-30 13:24:06.000000 chat_exporter_hikari-1.0.0/chat_exporter/parse/mention.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:30:09.783651 chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/
--rw-rw-rw-   0        0        0    11675 2023-02-25 23:30:09.000000 chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2521 2023-02-25 23:30:09.000000 chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 23:30:09.000000 chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-02-25 23:30:09.000000 chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-25 23:30:09.000000 chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1273 2023-02-25 23:29:21.000000 chat_exporter_hikari-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-25 23:30:09.785150 chat_exporter_hikari-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 08:03:00.047145 chat_exporter_hikari-1.0.1/
+-rw-rw-rw-   0        0        0    35803 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       79 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11675 2023-05-02 08:03:00.046142 chat_exporter_hikari-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10518 2023-02-02 08:26:52.000000 chat_exporter_hikari-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.748836 chat_exporter_hikari-1.0.1/chat_exporter/
+-rw-rw-rw-   0        0        0      212 2023-05-02 08:01:27.000000 chat_exporter_hikari-1.0.1/chat_exporter/__init__.py
+-rw-rw-rw-   0        0        0     6398 2023-01-30 16:45:05.000000 chat_exporter_hikari-1.0.1/chat_exporter/chat_exporter.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.762344 chat_exporter_hikari-1.0.1/chat_exporter/construct/
+-rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.790392 chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/
+-rw-rw-rw-   0        0        0      206 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/__init__.py
+-rw-rw-rw-   0        0        0     4010 2023-01-30 13:28:46.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/attachment.py
+-rw-rw-rw-   0        0        0     3974 2023-01-30 16:53:27.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/component.py
+-rw-rw-rw-   0        0        0     5950 2023-05-02 08:00:31.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/embed.py
+-rw-rw-rw-   0        0        0     1544 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/reaction.py
+-rw-rw-rw-   0        0        0    16881 2023-02-25 23:28:37.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/message.py
+-rw-rw-rw-   0        0        0     6669 2023-02-22 22:39:42.000000 chat_exporter_hikari-1.0.1/chat_exporter/construct/transcript.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.824470 chat_exporter_hikari-1.0.1/chat_exporter/ext/
+-rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/ext/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/ext/cache.py
+-rw-rw-rw-   0        0        0      199 2023-01-30 12:10:56.000000 chat_exporter_hikari-1.0.1/chat_exporter/ext/discord_import.py
+-rw-rw-rw-   0        0        0     1869 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/ext/discord_utils.py
+-rw-rw-rw-   0        0        0     4210 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/ext/emoji_convert.py
+-rw-rw-rw-   0        0        0     4146 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/ext/html_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.841053 chat_exporter_hikari-1.0.1/chat_exporter/html/
+-rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.860199 chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/
+-rw-rw-rw-   0        0        0      774 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/audio.html
+-rw-rw-rw-   0        0        0      140 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/image.html
+-rw-rw-rw-   0        0        0      547 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/message.html
+-rw-rw-rw-   0        0        0      127 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/video.html
+-rw-rw-rw-   0        0        0    43437 2023-01-30 16:14:47.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/base.html
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.879249 chat_exporter_hikari-1.0.1/chat_exporter/html/component/
+-rw-rw-rw-   0        0        0      229 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/component/component_button.html
+-rw-rw-rw-   0        0        0      254 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/component/component_menu.html
+-rw-rw-rw-   0        0        0      159 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/component/component_menu_options.html
+-rw-rw-rw-   0        0        0      508 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/component/component_menu_options_emoji.html
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.930523 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/
+-rw-rw-rw-   0        0        0      123 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/author.html
+-rw-rw-rw-   0        0        0      225 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/author_icon.html
+-rw-rw-rw-   0        0        0      667 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/body.html
+-rw-rw-rw-   0        0        0      116 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/description.html
+-rw-rw-rw-   0        0        0      317 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/field-inline.html
+-rw-rw-rw-   0        0        0      306 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/field.html
+-rw-rw-rw-   0        0        0      113 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/footer.html
+-rw-rw-rw-   0        0        0      183 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/footer_image.html
+-rw-rw-rw-   0        0        0      186 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/image.html
+-rw-rw-rw-   0        0        0      206 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/thumbnail.html
+-rw-rw-rw-   0        0        0       97 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/embed/title.html
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.987433 chat_exporter_hikari-1.0.1/chat_exporter/html/message/
+-rw-rw-rw-   0        0        0      239 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/bot-tag-verified.html
+-rw-rw-rw-   0        0        0       43 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/bot-tag.html
+-rw-rw-rw-   0        0        0       77 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/content.html
+-rw-rw-rw-   0        0        0        6 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/end.html
+-rw-rw-rw-   0        0        0      528 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/interaction.html
+-rw-rw-rw-   0        0        0      952 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/message.html
+-rw-rw-rw-   0        0        0     1108 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/meta.html
+-rw-rw-rw-   0        0        0     1021 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/pin.html
+-rw-rw-rw-   0        0        0      558 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/reference.html
+-rw-rw-rw-   0        0        0      131 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/reference_unknown.html
+-rw-rw-rw-   0        0        0     1254 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/start.html
+-rw-rw-rw-   0        0        0      895 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/message/thread.html
+drwxrwxrwx   0        0        0        0 2023-05-02 08:02:59.995968 chat_exporter_hikari-1.0.1/chat_exporter/html/reaction/
+-rw-rw-rw-   0        0        0      206 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/reaction/custom_emoji.html
+-rw-rw-rw-   0        0        0      120 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/reaction/emoji.html
+drwxrwxrwx   0        0        0        0 2023-05-02 08:03:00.012487 chat_exporter_hikari-1.0.1/chat_exporter/html/script/
+-rw-rw-rw-   0        0        0      112 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/script/channel_subject.html
+-rw-rw-rw-   0        0        0       59 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/script/channel_topic.html
+-rw-rw-rw-   0        0        0     1183 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/html/script/fancy_time.html
+drwxrwxrwx   0        0        0        0 2023-05-02 08:03:00.023554 chat_exporter_hikari-1.0.1/chat_exporter/parse/
+-rw-rw-rw-   0        0        0        0 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/parse/__init__.py
+-rw-rw-rw-   0        0        0    13090 2023-01-30 12:03:38.000000 chat_exporter_hikari-1.0.1/chat_exporter/parse/markdown.py
+-rw-rw-rw-   0        0        0     6643 2023-05-02 07:54:18.000000 chat_exporter_hikari-1.0.1/chat_exporter/parse/mention.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:03:00.045173 chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/
+-rw-rw-rw-   0        0        0    11675 2023-05-02 08:02:59.000000 chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2521 2023-05-02 08:02:59.000000 chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 08:02:59.000000 chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-02 08:02:59.000000 chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-02 08:02:59.000000 chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1273 2023-05-02 08:01:20.000000 chat_exporter_hikari-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 08:03:00.047145 chat_exporter_hikari-1.0.1/setup.cfg
```

### Comparing `chat_exporter_hikari-1.0.0/LICENSE` & `chat_exporter_hikari-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/PKG-INFO` & `chat_exporter_hikari-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat_exporter_hikari
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple Discord chat exporter for Python Discord bots.
 Author-email: h4ckd0tm3 <marcel@schnideritsch.at>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/h4ckd0tm3/DiscordChatExporterPy-hikari
 Keywords: chat exporter,discord chat exporter,discord,hikari
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chat_exporter_hikari Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: chat_exporter_hikari Version: 1.0.1 Summary: A
 simple Discord chat exporter for Python Discord bots. Author-email: h4ckd0tm3
 schnideritsch.at> License: GPL-3.0-only Project-URL: Homepage, https://
 github.com/h4ckd0tm3/DiscordChatExporterPy-hikari Keywords: chat
 exporter,discord chat exporter,discord,hikari Classifier: Operating System ::
 OS Independent Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `chat_exporter_hikari-1.0.0/README.md` & `chat_exporter_hikari-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/chat_exporter.py` & `chat_exporter_hikari-1.0.1/chat_exporter/chat_exporter.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/attachment.py` & `chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/attachment.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/component.py` & `chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/component.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/embed.py` & `chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,16 @@
 
         self.author = f'<a class="chatlog__embed-author-name-link" href="{self.embed.author.url}">{self.author}</a>' \
             if self.embed.author != self.check_against.author \
             else self.author
 
         author_icon = await fill_out(self.guild, embed_author_icon, [
             ("AUTHOR", self.author, PARSE_MODE_NONE),
-            ("AUTHOR_ICON", self.embed.author.icon.proxy_url if self.embed.author.icon else "", PARSE_MODE_NONE)
-        ]) if self.embed.author else ""
+            ("AUTHOR_ICON", self.embed.author.icon.proxy_url, PARSE_MODE_NONE)
+        ]) if self.embed.author and self.embed.author.icon else ""
 
         if author_icon == "" and self.author != "":
             self.author = await fill_out(self.guild, embed_author, [("AUTHOR", self.author, PARSE_MODE_NONE)])
         else:
             self.author = author_icon
 
     async def build_image(self):
```

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/construct/assets/reaction.py` & `chat_exporter_hikari-1.0.1/chat_exporter/construct/assets/reaction.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/construct/message.py` & `chat_exporter_hikari-1.0.1/chat_exporter/construct/message.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/construct/transcript.py` & `chat_exporter_hikari-1.0.1/chat_exporter/construct/transcript.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/ext/cache.py` & `chat_exporter_hikari-1.0.1/chat_exporter/ext/cache.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/ext/discord_utils.py` & `chat_exporter_hikari-1.0.1/chat_exporter/ext/discord_utils.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/ext/emoji_convert.py` & `chat_exporter_hikari-1.0.1/chat_exporter/ext/emoji_convert.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/ext/html_generator.py` & `chat_exporter_hikari-1.0.1/chat_exporter/ext/html_generator.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/audio.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/audio.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/attachment/message.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/attachment/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/base.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/base.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/embed/body.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/embed/body.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/interaction.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/interaction.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/message.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/meta.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/meta.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/pin.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/pin.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/reference.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/reference.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/start.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/start.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/message/thread.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/message/thread.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/html/script/fancy_time.html` & `chat_exporter_hikari-1.0.1/chat_exporter/html/script/fancy_time.html`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/parse/markdown.py` & `chat_exporter_hikari-1.0.1/chat_exporter/parse/markdown.py`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter/parse/mention.py` & `chat_exporter_hikari-1.0.1/chat_exporter/parse/mention.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,18 +100,18 @@
             while match is not None:
                 role_id = int(match.group(1))
                 role = self.guild.get_role(role_id)
 
                 if role is None:
                     replacement = '@deleted-role'
                 else:
-                    if role.color.r == 0 and role.color.g == 0 and role.color.b == 0:
+                    if role.color.rgb == (0, 0, 0):
                         colour = "#dee0fc"
                     else:
-                        colour = "#%02x%02x%02x" % (role.color.r, role.color.g, role.color.b)
+                        colour = "#%02x%02x%02x" % role.color.rgb
                     replacement = '<span style="color: %s;">@%s</span>' \
                                   % (colour, role.name)
                 self.content = self.content.replace(self.content[match.start():match.end()], replacement)
 
                 match = re.search(regex, self.content)
 
     async def member_mention(self):
```

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/PKG-INFO` & `chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-exporter-hikari
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple Discord chat exporter for Python Discord bots.
 Author-email: h4ckd0tm3 <marcel@schnideritsch.at>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/h4ckd0tm3/DiscordChatExporterPy-hikari
 Keywords: chat exporter,discord chat exporter,discord,hikari
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chat-exporter-hikari Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: chat-exporter-hikari Version: 1.0.1 Summary: A
 simple Discord chat exporter for Python Discord bots. Author-email: h4ckd0tm3
 schnideritsch.at> License: GPL-3.0-only Project-URL: Homepage, https://
 github.com/h4ckd0tm3/DiscordChatExporterPy-hikari Keywords: chat
 exporter,discord chat exporter,discord,hikari Classifier: Operating System ::
 OS Independent Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `chat_exporter_hikari-1.0.0/chat_exporter_hikari.egg-info/SOURCES.txt` & `chat_exporter_hikari-1.0.1/chat_exporter_hikari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat_exporter_hikari-1.0.0/pyproject.toml` & `chat_exporter_hikari-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chat_exporter_hikari"
 description = "A simple Discord chat exporter for Python Discord bots."
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.md"
 authors = [
     { name="h4ckd0tm3", email="marcel@schnideritsch.at" }
 ]
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-only" }
 classifiers = [
```

