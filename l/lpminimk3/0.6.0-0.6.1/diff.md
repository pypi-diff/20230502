# Comparing `tmp/lpminimk3-0.6.0.tar.gz` & `tmp/lpminimk3-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpminimk3-0.6.0.tar", last modified: Sat Apr 15 10:13:35 2023, max compression
+gzip compressed data, was "lpminimk3-0.6.1.tar", last modified: Tue May  2 04:40:00 2023, max compression
```

## Comparing `lpminimk3-0.6.0.tar` & `lpminimk3-0.6.1.tar`

### file list

```diff
@@ -1,56 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.657907 lpminimk3-0.6.0/lpminimk3/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/colors/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    38543 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/display_character.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/light_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/party.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/print_text_scroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/sync_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/examples/text_scroll_region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29194 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_renderable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/art.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/bitmaps/smiley.bitmap.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/glyphs/basic_latin.glyph.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/movies/
--rw-r--r--   0 runner    (1001) docker     (123)   130587 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/movies/ping_pong.movie.json
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/lpminimk3/graphics/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/schema/bitmap.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/schema/glyph.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/schema/movie.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/graphics/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/midi_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    21494 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/lpminimk3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:13:35.657907 lpminimk3-0.6.0/lpminimk3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 10:13:35.000000 lpminimk3-0.6.0/lpminimk3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:13:35.661907 lpminimk3-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-15 10:13:25.000000 lpminimk3-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.757160 lpminimk3-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-02 04:40:00.753160 lpminimk3-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.745160 lpminimk3-0.6.1/lpminimk3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.745160 lpminimk3-0.6.1/lpminimk3/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/colors/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/colors/web_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99836 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/colors/web_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/colors/web_colors.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.745160 lpminimk3-0.6.1/lpminimk3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/display_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/light_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/logos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/party.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/print_text_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/examples/text_scroll_region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.745160 lpminimk3-0.6.1/lpminimk3/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29194 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/_renderable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/art.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.749160 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/alien.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/apple.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33665 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/apple_old.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28771 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/chair.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37216 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/critical.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25854 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/data.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/diagonal.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22352 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/duck.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45791 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/facebook.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33753 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/ghost.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45792 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/gmail.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30085 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/google.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/green_arrow.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/green_plus.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/happy_face.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/heart.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24495 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/house.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31522 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/information.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34400 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/itunes.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28662 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/ludo.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45044 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/pacman.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34460 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/panic.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/perplexed_face.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/plug.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/red_green_arrow.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/running_arrow.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/satellite.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/skull.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18723 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/smiley.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31586 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/smiley_solid.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/surprised_face.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/umbrella.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34354 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/windows.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18750 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/xbox.bitmap.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/bitmaps/youtube.bitmap.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.749160 lpminimk3-0.6.1/lpminimk3/graphics/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/glyphs/basic_latin.glyph.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.753160 lpminimk3-0.6.1/lpminimk3/graphics/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)   336812 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/movies/heart_beat.movie.json
+-rw-r--r--   0 runner    (1001) docker     (123)   113110 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/movies/heart_trace.movie.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130588 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/movies/ping_pong.movie.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3316230 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/movies/ring.movie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.753160 lpminimk3-0.6.1/lpminimk3/graphics/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/schema/bitmap.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/schema/glyph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/schema/movie.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/graphics/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/midi_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/lpminimk3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:40:00.745160 lpminimk3-0.6.1/lpminimk3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-02 04:40:00.000000 lpminimk3-0.6.1/lpminimk3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-02 04:40:00.000000 lpminimk3-0.6.1/lpminimk3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:40:00.000000 lpminimk3-0.6.1/lpminimk3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 04:40:00.000000 lpminimk3-0.6.1/lpminimk3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 04:40:00.000000 lpminimk3-0.6.1/lpminimk3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:40:00.757160 lpminimk3-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-02 04:39:50.000000 lpminimk3-0.6.1/setup.py
```

### Comparing `lpminimk3-0.6.0/LICENSE` & `lpminimk3-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/PKG-INFO` & `lpminimk3-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpminimk3
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python API for the Novation Launchpad Mini MK3
 Home-page: https://github.com/obeezzy/lpminimk3
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpminimk3
 Python API for the [Novation Launchpad Mini MK3](https://novationmusic.com/en/launch/launchpad-mini)
 
 [![CI](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.1)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
 [![Documentation Status](https://readthedocs.org/projects/lpminimk3/badge/?version=latest)](https://lpminimk3.readthedocs.io/en/latest/?badge=latest)
 
+![image description](media/logos.gif)
+
 The goals of this project are as follows:
 * Intuitive, object-oriented design
 * Convenient for use in script and shell
 * Access to all (or most) of the Launchpad Mini MK3 MIDI features
 
 
 ## Installation
@@ -71,18 +73,15 @@
 from lpminimk3.graphics import Text
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-print('Watch text scroll across the Launchpad\'s surface.\n'
-      'Press Ctrl+C to quit.\n')
-
-lp.grid.render(Text(' Hello, world!').scroll())  # Scroll text indefinitely
+lp.grid.render(Text(' Hello, world!').scroll())  # Scroll text once
 ```
 See more examples [here](https://github.com/obeezzy/lpminimk3/tree/main/lpminimk3/examples).
 
 ### In shell
 Start by finding a connected device and opening the device for reading and writing:
 ```bash
 $ python
@@ -94,26 +93,28 @@
 ```python
 >>> lp.device_inquiry()  # Query device
 MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=150.938086752)
 ```
 Switch to `programmer` mode to start manipulating button LEDs:
 ```python
 >>> lp.mode = 'prog'  # Switch to programmer mode
->>> lp.grid.led('0x0').color = 10  # Set color to yellow (Valid values: 0 - 127)
+>>> lp.grid.led(0).color = 10  # Set color of LED at grid position 0 to yellow (Valid values: 0 - 127)
 >>> lp.grid.led(1,0).color = lpminimk3.colors.ColorPalette.Red.SHADE_1  # Set from palette
+>>> lp.grid.led('0x1').color = lpminimk3.colors.WebColor("amethyst")  # Set color from web colors
 >>> lp.panel.led('logo').color = 'violet'  # Set logo LED color to violet
 >>> lp.panel.led('drums').color = 'green2'  # Set 'Drums' LED color to second shade of green
 >>> lp.panel.led('stop').color = 'w1'  # Set 'Stop/Solo/Mute' LED color to first shade of white
 >>> lp.panel.led('mute').color = 'o3'  # Set 'Stop/Solo/Mute' LED color to third shade of orange
 >>> lp.panel.led('mute').color = 'r0'  # Invalid but okay, will default to 'r1'
 >>> lp.panel.led('scene_launch_1').color = '#ff0000'  # Set color to red using hex
 >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)  # Set color to blue using rgb
 >>> lp.panel.led('mute').color = 0  # Turn off LED
 >>> lp.panel.led('logo').reset()  # Another way to turn off LED
 >>> del lp.panel.led('stop').color  # Another way to turn off LED
+>>> lp.panel.reset()  # Turn off all LEDs
 ```
 Note in the above snippet that `lp.grid` only contains the __*grid*__ buttons
 (i.e. the translucent, faceless buttons) and `lp.panel` contains all buttons
 (including the __*logo*__ LED at the top right corner).  
 
 Wait for and respond to button presses and releases:
 ```python
@@ -143,17 +144,17 @@
  XXXX   
 XX  XX  
 XX  XX  
 XXXXXX  
 XX  XX  
 XX  XX  
 ```
-Scroll `Hello, world!` on Launchpad's surface once:
+Scroll `Hello, world!` on Launchpad's surface indefinitely:
 ```python
->>> lp.grid.render(Text(' Hello, world!').scroll(count=1))
+>>> lp.grid.render(Text(' Hello, world!').scroll(count=-1))
 ```
 
 
 ## Extended graphics support
 `lpminimk3` is also capable of rendering graphics from _**bitmaps**_ and _**movies**_. These are JSON files that describe the rendering data in a high-level format. Data in these files are grouped as _**frames**_. A **frame** is a sequence of bits and their color configurations. A **bitmap** file consists of a single frame while a **movie** file consists of a sequence of frames. 
 
 ### Syncing with LP Sketch
@@ -167,49 +168,48 @@
 Render `smiley.bitmap.json` on Launchpad's surface:
 ```python
 """Render "Smiley" bitmap.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Bitmap
+from lpminimk3.graphics.art import Bitmaps
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))  # Display bitmap
+lp.grid.render(Bitmap(Bitmaps.SMILEY))  # Display bitmap
+# OR
+# lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))
 ```
 Render `ping_pong.movie.json` on Launchpad's surface:
 ```python
 """Render "Ping/Pong" movie.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Movie
+from lpminimk3.graphics.art import Movies
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-print('Watch movie played on the Launchpad\'s surface.\n'
-      'Press Ctrl+C to quit.\n')
-
-lp.grid.render(Movie("/path/to/ping_pong.movie.json").play())  # Play movie indefinitely
+lp.grid.render(Movie(Movies.PING_PONG).play())  # Play movie once
+# OR
+# lp.grid.render(Movie("/path/to/ping_pong.movie.json").play())
 ```
 For convenience, you can use the render script, `render.py`:
 ```bash
 $ python -m lpminimk3.graphics.render -f /path/to/bitmap/or/movie.json
 ```
 `render.py` can be used to render text, bitmaps and movies on the Launchpad and on the console. For more options, run:
 ```bash
 $ python -m lpminimk3.graphics.render -h
 ```
 
 
-## Notes
-* Work in progress, so expect things to break!
-
-
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lpminimk3-0.6.0/README.md` & `lpminimk3-0.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # lpminimk3
 Python API for the [Novation Launchpad Mini MK3](https://novationmusic.com/en/launch/launchpad-mini)
 
 [![CI](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.1)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
 [![Documentation Status](https://readthedocs.org/projects/lpminimk3/badge/?version=latest)](https://lpminimk3.readthedocs.io/en/latest/?badge=latest)
 
+![image description](media/logos.gif)
+
 The goals of this project are as follows:
 * Intuitive, object-oriented design
 * Convenient for use in script and shell
 * Access to all (or most) of the Launchpad Mini MK3 MIDI features
 
 
 ## Installation
@@ -57,18 +59,15 @@
 from lpminimk3.graphics import Text
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-print('Watch text scroll across the Launchpad\'s surface.\n'
-      'Press Ctrl+C to quit.\n')
-
-lp.grid.render(Text(' Hello, world!').scroll())  # Scroll text indefinitely
+lp.grid.render(Text(' Hello, world!').scroll())  # Scroll text once
 ```
 See more examples [here](https://github.com/obeezzy/lpminimk3/tree/main/lpminimk3/examples).
 
 ### In shell
 Start by finding a connected device and opening the device for reading and writing:
 ```bash
 $ python
@@ -80,26 +79,28 @@
 ```python
 >>> lp.device_inquiry()  # Query device
 MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=150.938086752)
 ```
 Switch to `programmer` mode to start manipulating button LEDs:
 ```python
 >>> lp.mode = 'prog'  # Switch to programmer mode
->>> lp.grid.led('0x0').color = 10  # Set color to yellow (Valid values: 0 - 127)
+>>> lp.grid.led(0).color = 10  # Set color of LED at grid position 0 to yellow (Valid values: 0 - 127)
 >>> lp.grid.led(1,0).color = lpminimk3.colors.ColorPalette.Red.SHADE_1  # Set from palette
+>>> lp.grid.led('0x1').color = lpminimk3.colors.WebColor("amethyst")  # Set color from web colors
 >>> lp.panel.led('logo').color = 'violet'  # Set logo LED color to violet
 >>> lp.panel.led('drums').color = 'green2'  # Set 'Drums' LED color to second shade of green
 >>> lp.panel.led('stop').color = 'w1'  # Set 'Stop/Solo/Mute' LED color to first shade of white
 >>> lp.panel.led('mute').color = 'o3'  # Set 'Stop/Solo/Mute' LED color to third shade of orange
 >>> lp.panel.led('mute').color = 'r0'  # Invalid but okay, will default to 'r1'
 >>> lp.panel.led('scene_launch_1').color = '#ff0000'  # Set color to red using hex
 >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)  # Set color to blue using rgb
 >>> lp.panel.led('mute').color = 0  # Turn off LED
 >>> lp.panel.led('logo').reset()  # Another way to turn off LED
 >>> del lp.panel.led('stop').color  # Another way to turn off LED
+>>> lp.panel.reset()  # Turn off all LEDs
 ```
 Note in the above snippet that `lp.grid` only contains the __*grid*__ buttons
 (i.e. the translucent, faceless buttons) and `lp.panel` contains all buttons
 (including the __*logo*__ LED at the top right corner).  
 
 Wait for and respond to button presses and releases:
 ```python
@@ -129,17 +130,17 @@
  XXXX   
 XX  XX  
 XX  XX  
 XXXXXX  
 XX  XX  
 XX  XX  
 ```
-Scroll `Hello, world!` on Launchpad's surface once:
+Scroll `Hello, world!` on Launchpad's surface indefinitely:
 ```python
->>> lp.grid.render(Text(' Hello, world!').scroll(count=1))
+>>> lp.grid.render(Text(' Hello, world!').scroll(count=-1))
 ```
 
 
 ## Extended graphics support
 `lpminimk3` is also capable of rendering graphics from _**bitmaps**_ and _**movies**_. These are JSON files that describe the rendering data in a high-level format. Data in these files are grouped as _**frames**_. A **frame** is a sequence of bits and their color configurations. A **bitmap** file consists of a single frame while a **movie** file consists of a sequence of frames. 
 
 ### Syncing with LP Sketch
@@ -153,49 +154,48 @@
 Render `smiley.bitmap.json` on Launchpad's surface:
 ```python
 """Render "Smiley" bitmap.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Bitmap
+from lpminimk3.graphics.art import Bitmaps
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))  # Display bitmap
+lp.grid.render(Bitmap(Bitmaps.SMILEY))  # Display bitmap
+# OR
+# lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))
 ```
 Render `ping_pong.movie.json` on Launchpad's surface:
 ```python
 """Render "Ping/Pong" movie.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Movie
+from lpminimk3.graphics.art import Movies
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-print('Watch movie played on the Launchpad\'s surface.\n'
-      'Press Ctrl+C to quit.\n')
-
-lp.grid.render(Movie("/path/to/ping_pong.movie.json").play())  # Play movie indefinitely
+lp.grid.render(Movie(Movies.PING_PONG).play())  # Play movie once
+# OR
+# lp.grid.render(Movie("/path/to/ping_pong.movie.json").play())
 ```
 For convenience, you can use the render script, `render.py`:
 ```bash
 $ python -m lpminimk3.graphics.render -f /path/to/bitmap/or/movie.json
 ```
 `render.py` can be used to render text, bitmaps and movies on the Launchpad and on the console. For more options, run:
 ```bash
 $ python -m lpminimk3.graphics.render -h
 ```
 
 
-## Notes
-* Work in progress, so expect things to break!
-
-
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lpminimk3-0.6.0/lpminimk3/__init__.py` & `lpminimk3-0.6.1/lpminimk3/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """Python API for the Launchpad Mini MK3.
 
 This module exposes API to discover connected Launchpads
 on your computer and control them.
 
 Examples
 --------
+
 Find a connected device and open the device for reading and writing:
     >>> import lpminimk3
     >>> lp = lpminimk3.find_launchpads()[0]
     >>> lp.open()
 
 Query the device to ensure reading and writing works:
     >>> lp.device_inquiry()
-    MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247],
-              deltatime=150.938086752)
+    MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=0.0)
 
 Switch to the programmer mode:
     >>> lp.mode = Mode.PROG
 
 After a Launchpad is initialized, its `Grid` and `Panel` can be manipulated.
 
 Set color of LED at "0x0" to yellow (Valid values: 0 - 127):
     >>> lp.grid.led('0x0').color = 10
 
 Set color of LED at "1x0" to the first shade of palette color "red":
-    >>> lp.grid.led('1x0').color = lpminimk3.colors.ColorPalette.Red.SHADE_1
+    >>> import lpminimk3
+    >>> from lpminimk3.colors import ColorPalette
+    >>> lp.grid.led('1x0').color = ColorPalette.Red.SHADE_1
 
 Set color of LED at "logo" (in panel) to violet:
     >>> lp.panel.led('logo').color = 'violet'
 
 Set color of LED at "Drums" to second shade of "green":
     >>> lp.panel.led('drums').color = 'green2'
 
@@ -43,30 +45,41 @@
 
 Set color of LED at "Scene Launch 1" to "red" using hex:
     >>> lp.panel.led('scene_launch_1').color = '#ff0000'
 
 Set color of LED at "Scene Launch 2" to "blue" using RGB:
     >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)
 
+Set color of LED at "Scene Launch 2" to "magenta" using web colors:
+    >>> from lpminimk3.colors import WebColor
+    >>> lp.panel.led('scene_launch_3').color = WebColor("magenta")
+
 Turn off "Stop/Solo/Mute" LED:
     >>> lp.panel.led('mute').color = 0
 
 Another way to turn off LED:
     >>> lp.panel.led('mute').reset()
 
 Another way to turn off LED:
     >>> del lp.panel.led('mute').color
 
 Wait for and respond to button presses and releases:
     >>> lp.panel.buttons().poll_for_event()
+    ButtonEvent(button='4x1', type='press', deltatime=4.202155996)
 
 Wait for button releases:
     >>> lp.panel.buttons().poll_for_event(type='release')
+    ButtonEvent(button='4x1', type='release', deltatime=0.171533228)
 
 Wait for "Up", "0x0" or "Stop/Solo/Mute" button to be pressed or released:
     >>> lp.panel.buttons('up', '0x0', 'stop').poll_for_event()
+    ButtonEvent(button='4x1', type='release', deltatime=0.040492674)
 """
 
 from .__version__ import __version__, VERSION  # noqa
 from .components import Grid, Panel, Led, ButtonFace  # noqa
 from .utils import Interface, Mode, Layout, ButtonEvent  # noqa
 from .device import LaunchpadMiniMk3, find_launchpads  # noqa
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `lpminimk3-0.6.0/lpminimk3/_logging.py` & `lpminimk3-0.6.1/lpminimk3/_logging.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/colors/_colors.py` & `lpminimk3-0.6.1/lpminimk3/colors/_colors.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/components.py` & `lpminimk3-0.6.1/lpminimk3/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Components that make up the Launchpad Mini MK3.
 """
 
 import math
 import re
 from abc import ABC
-from .colors._colors import ColorShade, ColorShadeStore, RgbColor
-from .midi_messages import Colorspec,\
-                           ColorspecFragment,\
-                           Constants,\
-                           Lighting
+from .colors._colors import (ColorShade,
+                             ColorShadeStore,
+                             RgbColor)
+from .colors.web_color import WebColor
+from .midi_messages import (Colorspec,
+                            ColorspecFragment,
+                            Constants,
+                            Lighting)
 from .match import ButtonMatch
 from .utils import ButtonEvent
 from .region import Region
 
 
 class Matrix(ABC):
     """A matrix of pad buttons/LEDs on the surface of the Launchpad.
@@ -53,14 +56,19 @@
         pass
 
     def render(self, renderable):
         """Render `renderable` on matrix.
         """
         renderable.render(self)
 
+    def reset(self):
+        """Turn off all LEDs.
+        """
+        pass
+
 
 class FlipAxis:
     """Flip axis.
     """
     X = 'x'
     Y = 'y'
     XY = 'xy'
@@ -326,31 +334,37 @@
 
         assert isinstance(lighting_mode, int)
         assert isinstance(lighting_type, int)
 
         if not value:
             self._message = self._create_reset_message(lighting_mode,
                                                        midi_value)
-        elif (not isinstance(value, ColorShade)
+        elif (not isinstance(value, (ColorShade, WebColor))
                 and not isinstance(value, str)
                 and not isinstance(value, int)
                 and not isinstance(value, (tuple, list))):
-            raise TypeError('Must be of type ColorShade or str '
-                            'or int or tuple or list.')
+            raise TypeError('Must be of type ColorShade, WebColor, str, '
+                            'int, tuple or list.')
         elif ((isinstance(value, str)
                 and not ColorShadeStore().contains(value)
+                and not isinstance(value, WebColor)
                 and not RgbColor.is_valid(value))
                 or (isinstance(value, (tuple, list))
                     and not RgbColor.is_valid(value))):
             raise ValueError('Invalid color.')
         elif RgbColor.is_valid(value):
             colorspec = self._create_colorspec_message(value,
                                                        lighting_type,
                                                        midi_value)
             self._message = colorspec
+        elif isinstance(value, WebColor):
+            colorspec = self._create_colorspec_message(value.rgb_normalized,
+                                                       lighting_type,
+                                                       midi_value)
+            self._message = colorspec
         else:
             lighting = self._create_lighting_message(value,
                                                      lighting_mode,
                                                      midi_value)
             self._message = lighting
 
     @property
@@ -995,14 +1009,20 @@
         return ButtonGroup(launchpad=self._launchpad,
                            layout=(Panel._CUSTOM_MODE_MIDI_LAYOUT
                                    if layout == Panel.CUSTOM
                                    else Panel._PROG_MODE_MIDI_LAYOUT),
                            button_names=Panel._BUTTON_NAMES,
                            args=list(args))
 
+    def reset(self):
+        """Turns off all LEDs.
+        """
+        for led in self.led_range():
+            del led.color
+
 
 class Grid(Matrix):
     """Grid of Launchpad.
 
     The grid represents the 8x8 grid of translucent, faceless
     buttons of the Launchpad.
     """
@@ -1186,7 +1206,13 @@
                       for button_name in button_row])
         return ButtonGroup(launchpad=self._launchpad,
                            layout=(Grid._CUSTOM_MODE_MIDI_LAYOUT
                                    if layout == Grid.CUSTOM
                                    else Grid._PROG_MODE_MIDI_LAYOUT),
                            button_names=Grid._BUTTON_NAMES,
                            args=list(args))
+
+    def reset(self):
+        """Turns off all LEDs.
+        """
+        for led in self.led_range():
+            del led.color
```

### Comparing `lpminimk3-0.6.0/lpminimk3/device.py` & `lpminimk3-0.6.1/lpminimk3/device.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/examples/display_character.py` & `lpminimk3-0.6.1/lpminimk3/examples/display_character.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,40 +4,42 @@
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 import sys
 import termios
 import tty
 
 
-def getchar():
+def _getchar():
     fd = sys.stdin.fileno()
     old_settings = termios.tcgetattr(fd)
     try:
         tty.setraw(sys.stdin.fileno())
         ch = sys.stdin.read(1)
     finally:
         termios.tcsetattr(fd, termios.TCSADRAIN, old_settings)
     return ch
 
 
-def render_character(lp):
+def _render_character(lp):
     while True:
-        c = getchar()
+        c = _getchar()
         if ord(c) == 0x03:
             sys.exit()
         else:
             lp.grid.render(Text(c))
 
 
 def main():
+    """Runs script.
+    """
     lp = find_launchpads()[0]  # Get the first available launchpad
     lp.open()  # Open device for reading and writing on MIDI interface (by default)  # noqa
 
     lp.mode = Mode.PROG  # Switch to the programmer mode
 
     print('Press a key on your keyboard to display a character on your Launchpad.\n'  # noqa
           'Press Ctrl+C to quit.\n')
-    render_character(lp)  # Render character on Launchpad's surface
+    _render_character(lp)  # Render character on Launchpad's surface
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lpminimk3-0.6.0/lpminimk3/examples/flash.py` & `lpminimk3-0.6.1/lpminimk3/examples/flash.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from lpminimk3 import Mode, find_launchpads
 import random
 import time
 
 
 def main():
+    """Runs script.
+    """
     lp = find_launchpads()[0]  # Get the first available launchpad
     lp.open()  # Open device for reading and writing on MIDI interface (by default)  # noqa
 
     lp.mode = Mode.PROG  # Switch to the programmer mode
 
     for led in lp.panel.led_range():  # Loop through all LEDs
         led.color = random.randint(1, 127)  # Set LED to a random color  # noqa
```

### Comparing `lpminimk3-0.6.0/lpminimk3/examples/light_on_push.py` & `lpminimk3-0.6.1/lpminimk3/examples/light_on_push.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         button_event.button.led.color = 0  # Turn LED off once button is released  # noqa
         print(f"Button '{button_event.button.name}' released.")
     else:
         sys.exit()  # Exit on KeyboardInterrupt
 
 
 def main():
+    """Runs script.
+    """
     lp = find_launchpads()[0]  # Get the first available launchpad
     lp.open()  # Open device for reading and writing on MIDI interface (by default)  # noqa
 
     lp.mode = Mode.PROG  # Switch to the programmer mode
 
     print('Push any button on your Launchpad to see it light up!\n'
           'Press Ctrl+C to quit.\n')
```

### Comparing `lpminimk3-0.6.0/lpminimk3/examples/party.py` & `lpminimk3-0.6.1/lpminimk3/examples/party.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-"""Random party mode with some interactivity
+"""Random party mode with some interactivity.
 
 Author: Matthew Wachter
 """
 
 from lpminimk3 import Mode, find_launchpads, colors
 import random
 import math
 
 
 def main():  # noqa
+    """Runs script.
+    """
     lp = find_launchpads()[0]  # Get the first available launchpad
     lp.open()  # Open device for reading and writing on MIDI interface (by default)  # noqa
 
     lp.mode = Mode.PROG  # Switch to the programmer mode
 
     for led in lp.panel.led_range():
         del led.color  # Turn off LED
```

### Comparing `lpminimk3-0.6.0/lpminimk3/examples/text_scroll_region.py` & `lpminimk3-0.6.1/lpminimk3/examples/text_scroll_region.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Text
 from lpminimk3.region import Labeled as LabeledRegion
 import random
 
 
-def cycle_func(fraction, lp):
+def _cycle_func(fraction, lp):
     labeled_region = LabeledRegion()  # Region of labeled buttons
-    scroll_index = int(fraction * len(labeled_region))  # position in scroll
+    scroll_index = int(fraction * len(labeled_region))  # Position in scroll
     for index, led in enumerate(lp.panel.led_range(region=labeled_region)):  # Loop through all labeled buttons  # noqa
         if scroll_index == index:
             led.color = 'green4'  # Light up LED to green
         else:
             del led.color  # Turn off all other LEDs
 
 
 def main():
+    """Runs script.
+    """
     lp = find_launchpads()[0]  # Get the first available launchpad
     lp.open()  # Open device for reading and writing on MIDI interface (by default)  # noqa
 
     lp.mode = Mode.PROG  # Switch to the programmer mode
 
     print('Watch text scroll across the Launchpad\'s surface.\n'  # noqa
           'Press Ctrl+C to quit.\n')
 
     while True:
         try:
-            lp.grid.render(Text(' The entrance of your word giveth light...')
-                           .scroll(count=1,
-                                   cycle_func=cycle_func)
+            lp.grid.render(Text(" Don't read this.")
+                           .scroll(cycle_func=_cycle_func)
                            .rotate(-90)
                            .fg_color.set(random.randint(1, 127)))
         except KeyboardInterrupt:
             print('\n')
             break
```

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/_graphics.py` & `lpminimk3-0.6.1/lpminimk3/graphics/_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,19 +168,18 @@
         self._string.rotate(angle)
         return self
 
     def scroll(self, *,
                period=.05,
                direction=ScrollDirection.LEFT,
                cycle_func=None,
-               count=None,
+               count=1,
                timeout=None):
         """Scrolls rendered text, shifting every `period` seconds in the
-        `direction` direction; scrolls indefinitely if `count` is not
-        set.
+        `direction` direction.
 
         Parameters
         ----------
         period : float
             Delay before every text render call.
         direction : str
             Direction of scroll, either left or right.
@@ -188,21 +187,21 @@
         cycle_func : callable
             Function to be called right after text render call but
             before period delay. The function signature is:
                     cycle_func(fraction, launchpad)
             where `fraction` is the fraction of the scroll (ranging
             from 0 to 1) and `launchpad` is the Launchpad reference.
         count : int
-            Number of complete scrolls. Scrolls
-            indefinitely if `count` and `timeout` are not set.
+            Number of complete scrolls. Scrolls indefinitely if
+            `count` is set to -1.
         timeout : float
             Duration in seconds for scroll. Scrolls indefinitely if
-            `count` and `timeout` are not set. If both `timeout`
-            and `count` are set, the scroll will end depending on
-            which value is reached first.
+            `count` is set to -1 and `timeout` is not set. If both
+            `timeout` and `count` are set, the scroll will end
+            depending on which value is reached first.
 
         Returns
         -------
         Text
             `Text` reference.
 
         Raises
@@ -467,15 +466,15 @@
 
     def render(self, matrix):
         """Render on matrix `matrix`.
         """
         self._movie.render(matrix)
 
     def play(self, *,
-             count=None,
+             count=1,
              cycle_func=None):
         """Plays movie on the Launchpad's surface.
 
         Parameters
         ----------
         count : int or None
             Number of times to play movie.
```

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/_parser.py` & `lpminimk3-0.6.1/lpminimk3/graphics/_parser.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/_renderable.py` & `lpminimk3-0.6.1/lpminimk3/graphics/_renderable.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/_renderer.py` & `lpminimk3-0.6.1/lpminimk3/graphics/_renderer.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/_utils.py` & `lpminimk3-0.6.1/lpminimk3/graphics/_utils.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/glyphs/basic_latin.glyph.json` & `lpminimk3-0.6.1/lpminimk3/graphics/glyphs/basic_latin.glyph.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/movies/ping_pong.movie.json` & `lpminimk3-0.6.1/lpminimk3/graphics/movies/ping_pong.movie.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'description'": "'Bounces brick between two surfaces'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "description": "Bounce brick between two surfaces",
+    "description": "Bounces brick between two surfaces",
     "framerate": 4,
     "frames": [
         {
             "config": {
                 "0x0": {
                     "lighting_data": {
                         "off_state": {
```

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/render.py` & `lpminimk3-0.6.1/lpminimk3/graphics/render.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Renders texts, bitmaps and movies on the Launchpad's surface.
 """
 
+import os
 import json
 import sys
 from argparse import (ArgumentParser,
                       FileType,
                       RawDescriptionHelpFormatter)
 from lpminimk3 import find_launchpads, Mode
 from lpminimk3.graphics import Text, Bitmap, Movie
@@ -57,23 +58,44 @@
         lp = found_lps[0]
         lp.open()
         lp.mode = Mode.PROG
         return lp
     return None
 
 
+def _find_art(tag):
+    path_prefix = os.path.dirname(os.path.realpath(__file__))
+    if tag.startswith("bitmap:"):
+        tag = tag.replace("bitmap:", "bitmaps/")
+        tag = f"{path_prefix}/{tag}.bitmap.json"
+        return tag
+    elif tag.startswith("movie:"):
+        tag = tag.replace("movie:", "movies/")
+        tag = f"{path_prefix}/{tag}.movie.json"
+        return tag
+
+    return ""
+
+
 def _render(args, *, lp=None):
-    if args.f:
-        data = json.load(args.f)
+    if args.f or args.t:
+        filename = _find_art(args.t)
+        filename = (os.path.abspath(args.f.name)
+                    if not filename
+                    else filename)
+        data = None
+        with open(filename) as f:
+            data = json.load(f)
+
         if "bitmap" in data:
-            render_bitmap(args.f.name,
+            render_bitmap(filename,
                           on_screen=args.s,
                           lp=lp)
         elif "frames" in data:
-            render_movie(args.f.name,
+            render_movie(filename,
                          on_screen=args.s,
                          count=args.c,
                          lp=lp)
     elif len(args.text) == 1:
         render_character(args.text,
                          on_screen=args.s,
                          lp=lp)
@@ -92,22 +114,27 @@
                                             "Launchpad Mini MK3")
         parser = ArgumentParser(description=__doc__,
                                 formatter_class=RawDescriptionHelpFormatter)
 
         parser.add_argument("-c",
                             type=int,
                             metavar="COUNT",
+                            default=1,
                             help="Stop after looping COUNT times")
         parser.add_argument("-f",
                             type=FileType('r', encoding='latin-1'),
                             metavar="FILE",
                             help="Bitmap/movie file to render")
         parser.add_argument("-s",
                             action="store_true",
                             help="Print to screen")
+        parser.add_argument("-t",
+                            type=str,
+                            metavar="TAG",
+                            help="Art tag")
         parser.add_argument("text",
                             nargs="?",
                             metavar="TEXT",
                             help="Text to render")
         parser.add_argument("--version",
                             action="version",
                             version="%(prog) 0.1")
```

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/schema/bitmap.schema.json` & `lpminimk3-0.6.1/lpminimk3/graphics/schema/bitmap.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/schema/glyph.schema.json` & `lpminimk3-0.6.1/lpminimk3/graphics/schema/glyph.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/schema/movie.schema.json` & `lpminimk3-0.6.1/lpminimk3/graphics/schema/movie.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/graphics/sync.py` & `lpminimk3-0.6.1/lpminimk3/graphics/sync.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/match.py` & `lpminimk3-0.6.1/lpminimk3/match.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.6.0/lpminimk3/midi_messages.py` & `lpminimk3-0.6.1/lpminimk3/midi_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,25 +50,31 @@
     """Constants.
     """
     DEFAULT_COLOR_ID = 9
     MIDI_MIN_VALUE = 0
     MIDI_MAX_VALUE = 0x7f
 
     class LightingMode:
+        """Lighting mode.
+        """
         OFF = 0x80
         STATIC = 0x90
         FLASH = 0x91
 
     class LightingType:
+        """Lighting type.
+        """
         STATIC = 0x00
         FLASH = 0x01
         PULSE = 0x02
         RGB = 0x03
 
     class MidiWord:
+        """MIDI word.
+        """
         NOTE_HEADER = 0x90
         CC_HEADER = 0xb0
 
 
 class ColorspecFragment:
     """Colorspec fragment.
     """
```

### Comparing `lpminimk3-0.6.0/lpminimk3/region.py` & `lpminimk3-0.6.1/lpminimk3/region.py`

 * *Files 27% similar despite different names*

```diff
@@ -39,7 +39,30 @@
                 'scene_launch_2',
                 'scene_launch_3',
                 'scene_launch_4',
                 'scene_launch_5',
                 'scene_launch_6',
                 'scene_launch_7',
                 'stop_solo_mute']
+
+
+class Custom(Region):
+    """Custom region.
+    """
+
+    def __init__(self, button_names):
+        """Constructs a region whose buttons
+        can be specified through `button_names`.
+
+        Parameters
+        ----------
+        button_names : list of str
+            List of buttons to be included
+            in region.
+        """
+        self._button_names = button_names
+
+    @Region.button_names.getter
+    def button_names(self):
+        """Button names for custom region.
+        """
+        return self._button_names
```

### Comparing `lpminimk3-0.6.0/lpminimk3/utils.py` & `lpminimk3-0.6.1/lpminimk3/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 """Utility classes for Launchpad Mini MK3.
+
+This module contains classes that represent the logical
+parts of the Launchpad i.e. parts that have not physical
+representation (like components).
 """
 
 import enum
 import time
 import re
 import platform
 from collections import namedtuple
```

### Comparing `lpminimk3-0.6.0/lpminimk3.egg-info/PKG-INFO` & `lpminimk3-0.6.1/lpminimk3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpminimk3
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python API for the Novation Launchpad Mini MK3
 Home-page: https://github.com/obeezzy/lpminimk3
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpminimk3
 Python API for the [Novation Launchpad Mini MK3](https://novationmusic.com/en/launch/launchpad-mini)
 
 [![CI](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/lpminimk3/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.0)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml/badge.svg?branch=v0.6.1)](https://github.com/obeezzy/lpminimk3/actions/workflows/deploy.yml)
 [![Documentation Status](https://readthedocs.org/projects/lpminimk3/badge/?version=latest)](https://lpminimk3.readthedocs.io/en/latest/?badge=latest)
 
+![image description](media/logos.gif)
+
 The goals of this project are as follows:
 * Intuitive, object-oriented design
 * Convenient for use in script and shell
 * Access to all (or most) of the Launchpad Mini MK3 MIDI features
 
 
 ## Installation
@@ -71,18 +73,15 @@
 from lpminimk3.graphics import Text
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-print('Watch text scroll across the Launchpad\'s surface.\n'
-      'Press Ctrl+C to quit.\n')
-
-lp.grid.render(Text(' Hello, world!').scroll())  # Scroll text indefinitely
+lp.grid.render(Text(' Hello, world!').scroll())  # Scroll text once
 ```
 See more examples [here](https://github.com/obeezzy/lpminimk3/tree/main/lpminimk3/examples).
 
 ### In shell
 Start by finding a connected device and opening the device for reading and writing:
 ```bash
 $ python
@@ -94,26 +93,28 @@
 ```python
 >>> lp.device_inquiry()  # Query device
 MidiEvent(message=[240, 0, 32, 41, 2, 13, 14, 1, 247], deltatime=150.938086752)
 ```
 Switch to `programmer` mode to start manipulating button LEDs:
 ```python
 >>> lp.mode = 'prog'  # Switch to programmer mode
->>> lp.grid.led('0x0').color = 10  # Set color to yellow (Valid values: 0 - 127)
+>>> lp.grid.led(0).color = 10  # Set color of LED at grid position 0 to yellow (Valid values: 0 - 127)
 >>> lp.grid.led(1,0).color = lpminimk3.colors.ColorPalette.Red.SHADE_1  # Set from palette
+>>> lp.grid.led('0x1').color = lpminimk3.colors.WebColor("amethyst")  # Set color from web colors
 >>> lp.panel.led('logo').color = 'violet'  # Set logo LED color to violet
 >>> lp.panel.led('drums').color = 'green2'  # Set 'Drums' LED color to second shade of green
 >>> lp.panel.led('stop').color = 'w1'  # Set 'Stop/Solo/Mute' LED color to first shade of white
 >>> lp.panel.led('mute').color = 'o3'  # Set 'Stop/Solo/Mute' LED color to third shade of orange
 >>> lp.panel.led('mute').color = 'r0'  # Invalid but okay, will default to 'r1'
 >>> lp.panel.led('scene_launch_1').color = '#ff0000'  # Set color to red using hex
 >>> lp.panel.led('scene_launch_2').color = (0, 0, 255)  # Set color to blue using rgb
 >>> lp.panel.led('mute').color = 0  # Turn off LED
 >>> lp.panel.led('logo').reset()  # Another way to turn off LED
 >>> del lp.panel.led('stop').color  # Another way to turn off LED
+>>> lp.panel.reset()  # Turn off all LEDs
 ```
 Note in the above snippet that `lp.grid` only contains the __*grid*__ buttons
 (i.e. the translucent, faceless buttons) and `lp.panel` contains all buttons
 (including the __*logo*__ LED at the top right corner).  
 
 Wait for and respond to button presses and releases:
 ```python
@@ -143,17 +144,17 @@
  XXXX   
 XX  XX  
 XX  XX  
 XXXXXX  
 XX  XX  
 XX  XX  
 ```
-Scroll `Hello, world!` on Launchpad's surface once:
+Scroll `Hello, world!` on Launchpad's surface indefinitely:
 ```python
->>> lp.grid.render(Text(' Hello, world!').scroll(count=1))
+>>> lp.grid.render(Text(' Hello, world!').scroll(count=-1))
 ```
 
 
 ## Extended graphics support
 `lpminimk3` is also capable of rendering graphics from _**bitmaps**_ and _**movies**_. These are JSON files that describe the rendering data in a high-level format. Data in these files are grouped as _**frames**_. A **frame** is a sequence of bits and their color configurations. A **bitmap** file consists of a single frame while a **movie** file consists of a sequence of frames. 
 
 ### Syncing with LP Sketch
@@ -167,49 +168,48 @@
 Render `smiley.bitmap.json` on Launchpad's surface:
 ```python
 """Render "Smiley" bitmap.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Bitmap
+from lpminimk3.graphics.art import Bitmaps
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))  # Display bitmap
+lp.grid.render(Bitmap(Bitmaps.SMILEY))  # Display bitmap
+# OR
+# lp.grid.render(Bitmap("/path/to/smiley.bitmap.json"))
 ```
 Render `ping_pong.movie.json` on Launchpad's surface:
 ```python
 """Render "Ping/Pong" movie.
 """
 
 from lpminimk3 import Mode, find_launchpads
 from lpminimk3.graphics import Movie
+from lpminimk3.graphics.art import Movies
 
 lp = find_launchpads()[0]  # Get the first available launchpad
 lp.open()  # Open device for reading and writing on MIDI interface (by default)
 
 lp.mode = Mode.PROG  # Switch to the programmer mode
 
-print('Watch movie played on the Launchpad\'s surface.\n'
-      'Press Ctrl+C to quit.\n')
-
-lp.grid.render(Movie("/path/to/ping_pong.movie.json").play())  # Play movie indefinitely
+lp.grid.render(Movie(Movies.PING_PONG).play())  # Play movie once
+# OR
+# lp.grid.render(Movie("/path/to/ping_pong.movie.json").play())
 ```
 For convenience, you can use the render script, `render.py`:
 ```bash
 $ python -m lpminimk3.graphics.render -f /path/to/bitmap/or/movie.json
 ```
 `render.py` can be used to render text, bitmaps and movies on the Launchpad and on the console. For more options, run:
 ```bash
 $ python -m lpminimk3.graphics.render -h
 ```
 
 
-## Notes
-* Work in progress, so expect things to break!
-
-
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lpminimk3-0.6.0/setup.py` & `lpminimk3-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="lpminimk3",
-    version="0.6.0",
+    version="0.6.1",
     description="Python API for the Novation Launchpad Mini MK3",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/lpminimk3",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

