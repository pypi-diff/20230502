# Comparing `tmp/pyssg-0.8.3.tar.gz` & `tmp/pyssg-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyssg-0.8.3.tar", last modified: Tue Dec 27 09:00:31 2022, max compression
+gzip compressed data, was "pyssg-0.9.0.tar", last modified: Tue May  2 06:28:39 2023, max compression
```

## Comparing `pyssg-0.8.3.tar` & `pyssg-0.9.0.tar`

### file list

```diff
@@ -1,3203 +1,120 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.970535 pyssg-0.8.3/
--rw-r--r--   0 david     (1000) david     (1000)      178 2022-12-27 09:00:31.000000 pyssg-0.8.3/AUTHORS
--rw-r--r--   0 david     (1000) david     (1000)     3974 2022-12-27 09:00:31.000000 pyssg-0.8.3/ChangeLog
--rw-r--r--   0 david     (1000) david     (1000)    35149 2022-11-26 23:43:08.000000 pyssg-0.8.3/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)    10565 2022-12-27 09:00:31.970535 pyssg-0.8.3/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     9930 2022-12-27 08:48:51.000000 pyssg-0.8.3/README.md
--rwxr-xr-x   0 david     (1000) david     (1000)      233 2022-12-13 19:56:06.000000 pyssg-0.8.3/build_upload
--rw-r--r--   0 david     (1000) david     (1000)       98 2022-11-26 23:43:08.000000 pyssg-0.8.3/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/
--rw-r--r--   0 david     (1000) david     (1000)      129 2022-12-13 02:21:07.000000 pyssg-0.8.3/pyssg.xyz/.rsyncignore
--rwxr-xr-x   0 david     (1000) david     (1000)      409 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/bs
--rw-r--r--   0 david     (1000) david     (1000)     1477 2022-12-27 08:23:10.000000 pyssg-0.8.3/pyssg.xyz/config.yaml
--rw-r--r--   0 david     (1000) david     (1000)      306 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/db.psv
--rw-r--r--   0 david     (1000) david     (1000)      214 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/db_blog.psv
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.440535 pyssg-0.8.3/pyssg.xyz/live/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/blog/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/blog/a/
--rw-r--r--   0 david     (1000) david     (1000)     3832 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/a/second.html
--rw-r--r--   0 david     (1000) david     (1000)     3718 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/first.html
--rw-r--r--   0 david     (1000) david     (1000)     3753 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/index.html
--rw-r--r--   0 david     (1000) david     (1000)     2560 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/rss.xml
--rw-r--r--   0 david     (1000) david     (1000)     1515 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/sitemap.xml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/blog/tag/
--rw-r--r--   0 david     (1000) david     (1000)     3434 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/tag/@english.html
--rw-r--r--   0 david     (1000) david     (1000)     3353 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/tag/@multiple-author.html
--rw-r--r--   0 david     (1000) david     (1000)     3428 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/tag/@short.html
--rw-r--r--   0 david     (1000) david     (1000)     3425 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/tag/@test.html
--rw-r--r--   0 david     (1000) david     (1000)     3431 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/blog/tag/@update.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/
--rw-r--r--   0 david     (1000) david     (1000)     2929 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/404.html
--rw-r--r--   0 david     (1000) david     (1000)     3167 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/index.html
--rw-r--r--   0 david     (1000) david     (1000)      633 2022-12-27 08:40:18.000000 pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/sitemap.xml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/static/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/static/css/
--rw-r--r--   0 david     (1000) david     (1000)     6023 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/css/style.css
--rw-r--r--   0 david     (1000) david     (1000)     4060 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/css/theme.css
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/
--rw-r--r--   0 david     (1000) david     (1000)     1548 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/LICENSE.txt
--rw-r--r--   0 david     (1000) david     (1000)      187 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/attribution.js
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/
--rw-r--r--   0 david     (1000) david     (1000)    73615 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/all.css
--rw-r--r--   0 david     (1000) david     (1000)    59333 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/all.min.css
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/brands.css
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/brands.min.css
--rw-r--r--   0 david     (1000) david     (1000)    71990 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/fontawesome.css
--rw-r--r--   0 david     (1000) david     (1000)    57912 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/fontawesome.min.css
--rw-r--r--   0 david     (1000) david     (1000)      734 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/regular.css
--rw-r--r--   0 david     (1000) david     (1000)      677 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/regular.min.css
--rw-r--r--   0 david     (1000) david     (1000)      727 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/solid.css
--rw-r--r--   0 david     (1000) david     (1000)      669 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/solid.min.css
--rw-r--r--   0 david     (1000) david     (1000)     8077 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/svg-with-js.css
--rw-r--r--   0 david     (1000) david     (1000)     6359 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/svg-with-js.min.css
--rw-r--r--   0 david     (1000) david     (1000)    41312 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/v4-shims.css
--rw-r--r--   0 david     (1000) david     (1000)    26702 2022-12-13 19:56:06.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/css/v4-shims.min.css
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.470535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/
--rw-r--r--   0 david     (1000) david     (1000)  1261582 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/all.js
--rw-r--r--   0 david     (1000) david     (1000)  1195450 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/all.min.js
--rw-r--r--   0 david     (1000) david     (1000)   455241 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/brands.js
--rw-r--r--   0 david     (1000) david     (1000)   447933 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/brands.min.js
--rw-r--r--   0 david     (1000) david     (1000)    33962 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/conflict-detection.js
--rw-r--r--   0 david     (1000) david     (1000)    13533 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/conflict-detection.min.js
--rw-r--r--   0 david     (1000) david     (1000)    79447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/fontawesome.js
--rw-r--r--   0 david     (1000) david     (1000)    37330 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/fontawesome.min.js
--rw-r--r--   0 david     (1000) david     (1000)   107110 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/regular.js
--rw-r--r--   0 david     (1000) david     (1000)   103386 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/regular.min.js
--rw-r--r--   0 david     (1000) david     (1000)   620342 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/solid.js
--rw-r--r--   0 david     (1000) david     (1000)   607362 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/solid.min.js
--rw-r--r--   0 david     (1000) david     (1000)    17459 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/v4-shims.js
--rw-r--r--   0 david     (1000) david     (1000)    15055 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/js/v4-shims.min.js
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.470535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/
--rw-r--r--   0 david     (1000) david     (1000)      297 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_animated.less
--rw-r--r--   0 david     (1000) david     (1000)      422 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_bordered-pulled.less
--rw-r--r--   0 david     (1000) david     (1000)      297 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_core.less
--rw-r--r--   0 david     (1000) david     (1000)      119 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_fixed-width.less
--rw-r--r--   0 david     (1000) david     (1000)    99154 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_icons.less
--rw-r--r--   0 david     (1000) david     (1000)      454 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_larger.less
--rw-r--r--   0 david     (1000) david     (1000)      322 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_list.less
--rw-r--r--   0 david     (1000) david     (1000)     1237 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_mixins.less
--rw-r--r--   0 david     (1000) david     (1000)      771 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_rotated-flipped.less
--rw-r--r--   0 david     (1000) david     (1000)      118 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_screen-reader.less
--rw-r--r--   0 david     (1000) david     (1000)    60766 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_shims.less
--rw-r--r--   0 david     (1000) david     (1000)      478 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_stacked.less
--rw-r--r--   0 david     (1000) david     (1000)    41848 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/_variables.less
--rw-r--r--   0 david     (1000) david     (1000)      811 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/brands.less
--rw-r--r--   0 david     (1000) david     (1000)      505 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/fontawesome.less
--rw-r--r--   0 david     (1000) david     (1000)      813 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/regular.less
--rw-r--r--   0 david     (1000) david     (1000)      806 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/solid.less
--rw-r--r--   0 david     (1000) david     (1000)      236 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/less/v4-shims.less
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.470535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/
--rw-r--r--   0 david     (1000) david     (1000)    40344 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/categories.yml
--rw-r--r--   0 david     (1000) david     (1000)  3279270 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/icons.json
--rw-r--r--   0 david     (1000) david     (1000)   296510 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/icons.yml
--rw-r--r--   0 david     (1000) david     (1000)    23699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/shims.json
--rw-r--r--   0 david     (1000) david     (1000)     4682 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/shims.yml
--rw-r--r--   0 david     (1000) david     (1000)    12952 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/metadata/sponsors.yml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.480535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/
--rw-r--r--   0 david     (1000) david     (1000)      300 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_animated.scss
--rw-r--r--   0 david     (1000) david     (1000)      428 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 david     (1000) david     (1000)      332 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_core.scss
--rw-r--r--   0 david     (1000) david     (1000)      121 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 david     (1000) david     (1000)   118118 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_icons.scss
--rw-r--r--   0 david     (1000) david     (1000)      393 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_larger.scss
--rw-r--r--   0 david     (1000) david     (1000)      322 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_list.scss
--rw-r--r--   0 david     (1000) david     (1000)     1266 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_mixins.scss
--rw-r--r--   0 david     (1000) david     (1000)      833 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 david     (1000) david     (1000)      130 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 david     (1000) david     (1000)    65388 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_shims.scss
--rw-r--r--   0 david     (1000) david     (1000)      505 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_stacked.scss
--rw-r--r--   0 david     (1000) david     (1000)    39157 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/_variables.scss
--rw-r--r--   0 david     (1000) david     (1000)      803 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/brands.scss
--rw-r--r--   0 david     (1000) david     (1000)      433 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/fontawesome.scss
--rw-r--r--   0 david     (1000) david     (1000)      805 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/regular.scss
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/solid.scss
--rw-r--r--   0 david     (1000) david     (1000)      224 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/scss/v4-shims.scss
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.480535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/sprites/
--rw-r--r--   0 david     (1000) david     (1000)   469277 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/sprites/brands.svg
--rw-r--r--   0 david     (1000) david     (1000)   109518 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/sprites/regular.svg
--rw-r--r--   0 david     (1000) david     (1000)   655050 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/sprites/solid.svg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.450535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.550536 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/
--rw-r--r--   0 david     (1000) david     (1000)     1425 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/500px.svg
--rw-r--r--   0 david     (1000) david     (1000)      955 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/accessible-icon.svg
--rw-r--r--   0 david     (1000) david     (1000)     1032 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/accusoft.svg
--rw-r--r--   0 david     (1000) david     (1000)     1571 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/acquisitions-incorporated.svg
--rw-r--r--   0 david     (1000) david     (1000)      447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/adn.svg
--rw-r--r--   0 david     (1000) david     (1000)     1486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/adversal.svg
--rw-r--r--   0 david     (1000) david     (1000)      584 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/affiliatetheme.svg
--rw-r--r--   0 david     (1000) david     (1000)     1029 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/airbnb.svg
--rw-r--r--   0 david     (1000) david     (1000)     1087 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/algolia.svg
--rw-r--r--   0 david     (1000) david     (1000)      925 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/alipay.svg
--rw-r--r--   0 david     (1000) david     (1000)     3646 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/amazon-pay.svg
--rw-r--r--   0 david     (1000) david     (1000)      900 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/amazon.svg
--rw-r--r--   0 david     (1000) david     (1000)      785 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/amilia.svg
--rw-r--r--   0 david     (1000) david     (1000)      561 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/android.svg
--rw-r--r--   0 david     (1000) david     (1000)     1562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/angellist.svg
--rw-r--r--   0 david     (1000) david     (1000)     2131 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/angrycreative.svg
--rw-r--r--   0 david     (1000) david     (1000)      419 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/angular.svg
--rw-r--r--   0 david     (1000) david     (1000)      906 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/app-store-ios.svg
--rw-r--r--   0 david     (1000) david     (1000)     1038 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/app-store.svg
--rw-r--r--   0 david     (1000) david     (1000)     1909 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/apper.svg
--rw-r--r--   0 david     (1000) david     (1000)     1370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/apple-pay.svg
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/apple.svg
--rw-r--r--   0 david     (1000) david     (1000)      453 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/artstation.svg
--rw-r--r--   0 david     (1000) david     (1000)      944 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/asymmetrik.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/atlassian.svg
--rw-r--r--   0 david     (1000) david     (1000)      754 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/audible.svg
--rw-r--r--   0 david     (1000) david     (1000)      459 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/autoprefixer.svg
--rw-r--r--   0 david     (1000) david     (1000)      751 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/avianex.svg
--rw-r--r--   0 david     (1000) david     (1000)     2357 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/aviato.svg
--rw-r--r--   0 david     (1000) david     (1000)     2490 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/aws.svg
--rw-r--r--   0 david     (1000) david     (1000)      360 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bandcamp.svg
--rw-r--r--   0 david     (1000) david     (1000)     2753 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/battle-net.svg
--rw-r--r--   0 david     (1000) david     (1000)      963 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/behance-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/behance.svg
--rw-r--r--   0 david     (1000) david     (1000)      665 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bimobject.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bitbucket.svg
--rw-r--r--   0 david     (1000) david     (1000)     1345 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bitcoin.svg
--rw-r--r--   0 david     (1000) david     (1000)      939 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bity.svg
--rw-r--r--   0 david     (1000) david     (1000)      357 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/black-tie.svg
--rw-r--r--   0 david     (1000) david     (1000)      856 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/blackberry.svg
--rw-r--r--   0 david     (1000) david     (1000)     1080 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/blogger-b.svg
--rw-r--r--   0 david     (1000) david     (1000)     1379 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/blogger.svg
--rw-r--r--   0 david     (1000) david     (1000)      551 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bluetooth-b.svg
--rw-r--r--   0 david     (1000) david     (1000)      550 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bluetooth.svg
--rw-r--r--   0 david     (1000) david     (1000)      786 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/bootstrap.svg
--rw-r--r--   0 david     (1000) david     (1000)      938 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/btc.svg
--rw-r--r--   0 david     (1000) david     (1000)      899 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/buffer.svg
--rw-r--r--   0 david     (1000) david     (1000)      654 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/buromobelexperte.svg
--rw-r--r--   0 david     (1000) david     (1000)     1036 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/buy-n-large.svg
--rw-r--r--   0 david     (1000) david     (1000)      477 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/buysellads.svg
--rw-r--r--   0 david     (1000) david     (1000)     1046 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/canadian-maple-leaf.svg
--rw-r--r--   0 david     (1000) david     (1000)     3608 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-amazon-pay.svg
--rw-r--r--   0 david     (1000) david     (1000)     3377 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-amex.svg
--rw-r--r--   0 david     (1000) david     (1000)     1465 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-apple-pay.svg
--rw-r--r--   0 david     (1000) david     (1000)      780 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-diners-club.svg
--rw-r--r--   0 david     (1000) david     (1000)     1417 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-discover.svg
--rw-r--r--   0 david     (1000) david     (1000)      959 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-jcb.svg
--rw-r--r--   0 david     (1000) david     (1000)     3200 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-mastercard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1942 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-paypal.svg
--rw-r--r--   0 david     (1000) david     (1000)     1468 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-stripe.svg
--rw-r--r--   0 david     (1000) david     (1000)     1114 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cc-visa.svg
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/centercode.svg
--rw-r--r--   0 david     (1000) david     (1000)     1093 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/centos.svg
--rw-r--r--   0 david     (1000) david     (1000)      757 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/chrome.svg
--rw-r--r--   0 david     (1000) david     (1000)      662 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/chromecast.svg
--rw-r--r--   0 david     (1000) david     (1000)     1290 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cloudflare.svg
--rw-r--r--   0 david     (1000) david     (1000)      811 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cloudscale.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cloudsmith.svg
--rw-r--r--   0 david     (1000) david     (1000)     1542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cloudversify.svg
--rw-r--r--   0 david     (1000) david     (1000)      925 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/codepen.svg
--rw-r--r--   0 david     (1000) david     (1000)      717 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/codiepie.svg
--rw-r--r--   0 david     (1000) david     (1000)      772 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/confluence.svg
--rw-r--r--   0 david     (1000) david     (1000)     3302 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/connectdevelop.svg
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/contao.svg
--rw-r--r--   0 david     (1000) david     (1000)     1470 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cotton-bureau.svg
--rw-r--r--   0 david     (1000) david     (1000)     1611 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cpanel.svg
--rw-r--r--   0 david     (1000) david     (1000)      759 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-by.svg
--rw-r--r--   0 david     (1000) david     (1000)     1004 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-nc-eu.svg
--rw-r--r--   0 david     (1000) david     (1000)      762 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-nc-jp.svg
--rw-r--r--   0 david     (1000) david     (1000)      922 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-nc.svg
--rw-r--r--   0 david     (1000) david     (1000)      566 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-nd.svg
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-pd-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      838 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-pd.svg
--rw-r--r--   0 david     (1000) david     (1000)      828 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-remix.svg
--rw-r--r--   0 david     (1000) david     (1000)      766 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-sa.svg
--rw-r--r--   0 david     (1000) david     (1000)     1351 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-sampling-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1415 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-sampling.svg
--rw-r--r--   0 david     (1000) david     (1000)      805 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-share.svg
--rw-r--r--   0 david     (1000) david     (1000)      844 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons-zero.svg
--rw-r--r--   0 david     (1000) david     (1000)     1142 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/creative-commons.svg
--rw-r--r--   0 david     (1000) david     (1000)     7313 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/critical-role.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/css3-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/css3.svg
--rw-r--r--   0 david     (1000) david     (1000)      510 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/cuttlefish.svg
--rw-r--r--   0 david     (1000) david     (1000)     4176 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/d-and-d-beyond.svg
--rw-r--r--   0 david     (1000) david     (1000)     4699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/d-and-d.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dailymotion.svg
--rw-r--r--   0 david     (1000) david     (1000)      500 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dashcube.svg
--rw-r--r--   0 david     (1000) david     (1000)      535 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/deezer.svg
--rw-r--r--   0 david     (1000) david     (1000)      726 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/delicious.svg
--rw-r--r--   0 david     (1000) david     (1000)     1024 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/deploydog.svg
--rw-r--r--   0 david     (1000) david     (1000)      867 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/deskpro.svg
--rw-r--r--   0 david     (1000) david     (1000)      945 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dev.svg
--rw-r--r--   0 david     (1000) david     (1000)      432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/deviantart.svg
--rw-r--r--   0 david     (1000) david     (1000)     1019 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dhl.svg
--rw-r--r--   0 david     (1000) david     (1000)      666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/diaspora.svg
--rw-r--r--   0 david     (1000) david     (1000)      564 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/digg.svg
--rw-r--r--   0 david     (1000) david     (1000)      556 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/digital-ocean.svg
--rw-r--r--   0 david     (1000) david     (1000)     1398 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/discord.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/discourse.svg
--rw-r--r--   0 david     (1000) david     (1000)      447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dochub.svg
--rw-r--r--   0 david     (1000) david     (1000)      843 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/docker.svg
--rw-r--r--   0 david     (1000) david     (1000)      959 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/draft2digital.svg
--rw-r--r--   0 david     (1000) david     (1000)     1101 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dribbble-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1311 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dribbble.svg
--rw-r--r--   0 david     (1000) david     (1000)      490 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dropbox.svg
--rw-r--r--   0 david     (1000) david     (1000)      951 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/drupal.svg
--rw-r--r--   0 david     (1000) david     (1000)      440 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/dyalog.svg
--rw-r--r--   0 david     (1000) david     (1000)     2107 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/earlybirds.svg
--rw-r--r--   0 david     (1000) david     (1000)     1277 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ebay.svg
--rw-r--r--   0 david     (1000) david     (1000)      670 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/edge-legacy.svg
--rw-r--r--   0 david     (1000) david     (1000)     1392 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/edge.svg
--rw-r--r--   0 david     (1000) david     (1000)      506 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/elementor.svg
--rw-r--r--   0 david     (1000) david     (1000)      608 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ello.svg
--rw-r--r--   0 david     (1000) david     (1000)     2113 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ember.svg
--rw-r--r--   0 david     (1000) david     (1000)     2027 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/empire.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/envira.svg
--rw-r--r--   0 david     (1000) david     (1000)      612 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/erlang.svg
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ethereum.svg
--rw-r--r--   0 david     (1000) david     (1000)      842 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/etsy.svg
--rw-r--r--   0 david     (1000) david     (1000)     1189 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/evernote.svg
--rw-r--r--   0 david     (1000) david     (1000)     1142 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/expeditedssl.svg
--rw-r--r--   0 david     (1000) david     (1000)      432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/facebook-f.svg
--rw-r--r--   0 david     (1000) david     (1000)      734 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/facebook-messenger.svg
--rw-r--r--   0 david     (1000) david     (1000)      518 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/facebook-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      524 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/facebook.svg
--rw-r--r--   0 david     (1000) david     (1000)     1319 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fantasy-flight-games.svg
--rw-r--r--   0 david     (1000) david     (1000)      999 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fedex.svg
--rw-r--r--   0 david     (1000) david     (1000)     2423 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fedora.svg
--rw-r--r--   0 david     (1000) david     (1000)      443 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/figma.svg
--rw-r--r--   0 david     (1000) david     (1000)     1860 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/firefox-browser.svg
--rw-r--r--   0 david     (1000) david     (1000)     2358 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/firefox.svg
--rw-r--r--   0 david     (1000) david     (1000)     1710 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/first-order-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1422 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/first-order.svg
--rw-r--r--   0 david     (1000) david     (1000)      447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/firstdraft.svg
--rw-r--r--   0 david     (1000) david     (1000)      559 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/flickr.svg
--rw-r--r--   0 david     (1000) david     (1000)      336 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/flipboard.svg
--rw-r--r--   0 david     (1000) david     (1000)      920 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fly.svg
--rw-r--r--   0 david     (1000) david     (1000)      994 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/font-awesome-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      837 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/font-awesome-flag.svg
--rw-r--r--   0 david     (1000) david     (1000)     3174 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/font-awesome-logo-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      879 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/font-awesome.svg
--rw-r--r--   0 david     (1000) david     (1000)      794 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fonticons-fi.svg
--rw-r--r--   0 david     (1000) david     (1000)      820 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fonticons.svg
--rw-r--r--   0 david     (1000) david     (1000)     3871 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fort-awesome-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1199 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fort-awesome.svg
--rw-r--r--   0 david     (1000) david     (1000)      797 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/forumbee.svg
--rw-r--r--   0 david     (1000) david     (1000)      803 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/foursquare.svg
--rw-r--r--   0 david     (1000) david     (1000)     1430 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/free-code-camp.svg
--rw-r--r--   0 david     (1000) david     (1000)      776 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/freebsd.svg
--rw-r--r--   0 david     (1000) david     (1000)      519 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/fulcrum.svg
--rw-r--r--   0 david     (1000) david     (1000)     1783 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/galactic-republic.svg
--rw-r--r--   0 david     (1000) david     (1000)     2864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/galactic-senate.svg
--rw-r--r--   0 david     (1000) david     (1000)      604 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/get-pocket.svg
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gg-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gg.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/git-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1396 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/git-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1279 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/git.svg
--rw-r--r--   0 david     (1000) david     (1000)     1060 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/github-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1674 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/github-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1564 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/github.svg
--rw-r--r--   0 david     (1000) david     (1000)     1534 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gitkraken.svg
--rw-r--r--   0 david     (1000) david     (1000)      534 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gitlab.svg
--rw-r--r--   0 david     (1000) david     (1000)      374 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gitter.svg
--rw-r--r--   0 david     (1000) david     (1000)      938 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/glide-g.svg
--rw-r--r--   0 david     (1000) david     (1000)     1035 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/glide.svg
--rw-r--r--   0 david     (1000) david     (1000)      620 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gofore.svg
--rw-r--r--   0 david     (1000) david     (1000)      903 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/goodreads-g.svg
--rw-r--r--   0 david     (1000) david     (1000)      991 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/goodreads.svg
--rw-r--r--   0 david     (1000) david     (1000)      397 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-drive.svg
--rw-r--r--   0 david     (1000) david     (1000)     1661 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-pay.svg
--rw-r--r--   0 david     (1000) david     (1000)      506 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-play.svg
--rw-r--r--   0 david     (1000) david     (1000)      737 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-plus-g.svg
--rw-r--r--   0 david     (1000) david     (1000)      678 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-plus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      654 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google-wallet.svg
--rw-r--r--   0 david     (1000) david     (1000)      507 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/google.svg
--rw-r--r--   0 david     (1000) david     (1000)      513 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gratipay.svg
--rw-r--r--   0 david     (1000) david     (1000)     1808 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/grav.svg
--rw-r--r--   0 david     (1000) david     (1000)      870 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gripfire.svg
--rw-r--r--   0 david     (1000) david     (1000)     5670 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/grunt.svg
--rw-r--r--   0 david     (1000) david     (1000)      647 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/guilded.svg
--rw-r--r--   0 david     (1000) david     (1000)     2781 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/gulp.svg
--rw-r--r--   0 david     (1000) david     (1000)      526 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hacker-news-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      440 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hacker-news.svg
--rw-r--r--   0 david     (1000) david     (1000)     1023 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hackerrank.svg
--rw-r--r--   0 david     (1000) david     (1000)     1625 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hips.svg
--rw-r--r--   0 david     (1000) david     (1000)     1242 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hire-a-helper.svg
--rw-r--r--   0 david     (1000) david     (1000)     1004 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hive.svg
--rw-r--r--   0 david     (1000) david     (1000)     1666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hooli.svg
--rw-r--r--   0 david     (1000) david     (1000)     1274 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hornbill.svg
--rw-r--r--   0 david     (1000) david     (1000)      530 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hotjar.svg
--rw-r--r--   0 david     (1000) david     (1000)      322 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/houzz.svg
--rw-r--r--   0 david     (1000) david     (1000)      459 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/html5.svg
--rw-r--r--   0 david     (1000) david     (1000)     1012 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/hubspot.svg
--rw-r--r--   0 david     (1000) david     (1000)     1037 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ideal.svg
--rw-r--r--   0 david     (1000) david     (1000)      933 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/imdb.svg
--rw-r--r--   0 david     (1000) david     (1000)      917 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/innosoft.svg
--rw-r--r--   0 david     (1000) david     (1000)     1217 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/instagram-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1182 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/instagram.svg
--rw-r--r--   0 david     (1000) david     (1000)      440 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/instalod.svg
--rw-r--r--   0 david     (1000) david     (1000)      842 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/intercom.svg
--rw-r--r--   0 david     (1000) david     (1000)     1117 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/internet-explorer.svg
--rw-r--r--   0 david     (1000) david     (1000)      863 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/invision.svg
--rw-r--r--   0 david     (1000) david     (1000)      883 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ioxhost.svg
--rw-r--r--   0 david     (1000) david     (1000)     1445 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/itch-io.svg
--rw-r--r--   0 david     (1000) david     (1000)      842 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/itunes-note.svg
--rw-r--r--   0 david     (1000) david     (1000)     1132 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/itunes.svg
--rw-r--r--   0 david     (1000) david     (1000)     1362 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/java.svg
--rw-r--r--   0 david     (1000) david     (1000)      916 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/jedi-order.svg
--rw-r--r--   0 david     (1000) david     (1000)     4521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/jenkins.svg
--rw-r--r--   0 david     (1000) david     (1000)      479 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/jira.svg
--rw-r--r--   0 david     (1000) david     (1000)     1057 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/joget.svg
--rw-r--r--   0 david     (1000) david     (1000)     1325 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/joomla.svg
--rw-r--r--   0 david     (1000) david     (1000)      877 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/js-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      791 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/js.svg
--rw-r--r--   0 david     (1000) david     (1000)     2083 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/jsfiddle.svg
--rw-r--r--   0 david     (1000) david     (1000)      498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/kaggle.svg
--rw-r--r--   0 david     (1000) david     (1000)     1745 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/keybase.svg
--rw-r--r--   0 david     (1000) david     (1000)     1699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/keycdn.svg
--rw-r--r--   0 david     (1000) david     (1000)      552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/kickstarter-k.svg
--rw-r--r--   0 david     (1000) david     (1000)      649 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/kickstarter.svg
--rw-r--r--   0 david     (1000) david     (1000)      510 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/korvue.svg
--rw-r--r--   0 david     (1000) david     (1000)     1889 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/laravel.svg
--rw-r--r--   0 david     (1000) david     (1000)      917 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/lastfm-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      829 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/lastfm.svg
--rw-r--r--   0 david     (1000) david     (1000)     1343 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/leanpub.svg
--rw-r--r--   0 david     (1000) david     (1000)     2020 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/less.svg
--rw-r--r--   0 david     (1000) david     (1000)     1385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/line.svg
--rw-r--r--   0 david     (1000) david     (1000)      560 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/linkedin-in.svg
--rw-r--r--   0 david     (1000) david     (1000)      684 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/linkedin.svg
--rw-r--r--   0 david     (1000) david     (1000)     1517 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/linode.svg
--rw-r--r--   0 david     (1000) david     (1000)     3748 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/linux.svg
--rw-r--r--   0 david     (1000) david     (1000)      855 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/lyft.svg
--rw-r--r--   0 david     (1000) david     (1000)      459 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/magento.svg
--rw-r--r--   0 david     (1000) david     (1000)     3317 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mailchimp.svg
--rw-r--r--   0 david     (1000) david     (1000)     6168 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mandalorian.svg
--rw-r--r--   0 david     (1000) david     (1000)      539 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/markdown.svg
--rw-r--r--   0 david     (1000) david     (1000)      875 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mastodon.svg
--rw-r--r--   0 david     (1000) david     (1000)      480 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/maxcdn.svg
--rw-r--r--   0 david     (1000) david     (1000)      813 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mdb.svg
--rw-r--r--   0 david     (1000) david     (1000)     1076 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/medapps.svg
--rw-r--r--   0 david     (1000) david     (1000)      593 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/medium-m.svg
--rw-r--r--   0 david     (1000) david     (1000)      596 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/medium.svg
--rw-r--r--   0 david     (1000) david     (1000)     1016 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/medrt.svg
--rw-r--r--   0 david     (1000) david     (1000)     2312 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/meetup.svg
--rw-r--r--   0 david     (1000) david     (1000)      609 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/megaport.svg
--rw-r--r--   0 david     (1000) david     (1000)      916 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mendeley.svg
--rw-r--r--   0 david     (1000) david     (1000)      808 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/microblog.svg
--rw-r--r--   0 david     (1000) david     (1000)      367 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/microsoft.svg
--rw-r--r--   0 david     (1000) david     (1000)      404 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mix.svg
--rw-r--r--   0 david     (1000) david     (1000)     1555 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mixcloud.svg
--rw-r--r--   0 david     (1000) david     (1000)      686 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mixer.svg
--rw-r--r--   0 david     (1000) david     (1000)      617 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/mizuni.svg
--rw-r--r--   0 david     (1000) david     (1000)      428 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/modx.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/monero.svg
--rw-r--r--   0 david     (1000) david     (1000)     1160 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/napster.svg
--rw-r--r--   0 david     (1000) david     (1000)      619 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/neos.svg
--rw-r--r--   0 david     (1000) david     (1000)      734 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/nimblr.svg
--rw-r--r--   0 david     (1000) david     (1000)     1344 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/node-js.svg
--rw-r--r--   0 david     (1000) david     (1000)     3297 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/node.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/npm.svg
--rw-r--r--   0 david     (1000) david     (1000)     2316 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ns8.svg
--rw-r--r--   0 david     (1000) david     (1000)     1678 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/nutritionix.svg
--rw-r--r--   0 david     (1000) david     (1000)     1021 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/octopus-deploy.svg
--rw-r--r--   0 david     (1000) david     (1000)      948 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/odnoklassniki-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      843 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/odnoklassniki.svg
--rw-r--r--   0 david     (1000) david     (1000)    11399 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/old-republic.svg
--rw-r--r--   0 david     (1000) david     (1000)      606 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/opencart.svg
--rw-r--r--   0 david     (1000) david     (1000)      514 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/openid.svg
--rw-r--r--   0 david     (1000) david     (1000)      674 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/opera.svg
--rw-r--r--   0 david     (1000) david     (1000)     4931 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/optin-monster.svg
--rw-r--r--   0 david     (1000) david     (1000)      623 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/orcid.svg
--rw-r--r--   0 david     (1000) david     (1000)     1135 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/osi.svg
--rw-r--r--   0 david     (1000) david     (1000)      984 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/page4.svg
--rw-r--r--   0 david     (1000) david     (1000)      744 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pagelines.svg
--rw-r--r--   0 david     (1000) david     (1000)     1022 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/palfed.svg
--rw-r--r--   0 david     (1000) david     (1000)      417 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/patreon.svg
--rw-r--r--   0 david     (1000) david     (1000)      813 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/paypal.svg
--rw-r--r--   0 david     (1000) david     (1000)     1382 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/penny-arcade.svg
--rw-r--r--   0 david     (1000) david     (1000)      926 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/perbyte.svg
--rw-r--r--   0 david     (1000) david     (1000)      788 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/periscope.svg
--rw-r--r--   0 david     (1000) david     (1000)     1208 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/phabricator.svg
--rw-r--r--   0 david     (1000) david     (1000)     2672 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/phoenix-framework.svg
--rw-r--r--   0 david     (1000) david     (1000)     1777 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/phoenix-squadron.svg
--rw-r--r--   0 david     (1000) david     (1000)     1032 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/php.svg
--rw-r--r--   0 david     (1000) david     (1000)     1852 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pied-piper-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pied-piper-hat.svg
--rw-r--r--   0 david     (1000) david     (1000)      922 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pied-piper-pp.svg
--rw-r--r--   0 david     (1000) david     (1000)      543 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pied-piper-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      809 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pied-piper.svg
--rw-r--r--   0 david     (1000) david     (1000)      755 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pinterest-p.svg
--rw-r--r--   0 david     (1000) david     (1000)      889 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pinterest-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      926 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pinterest.svg
--rw-r--r--   0 david     (1000) david     (1000)      854 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/playstation.svg
--rw-r--r--   0 david     (1000) david     (1000)      508 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/product-hunt.svg
--rw-r--r--   0 david     (1000) david     (1000)      723 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/pushed.svg
--rw-r--r--   0 david     (1000) david     (1000)     1024 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/python.svg
--rw-r--r--   0 david     (1000) david     (1000)      827 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/qq.svg
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/quinscape.svg
--rw-r--r--   0 david     (1000) david     (1000)      752 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/quora.svg
--rw-r--r--   0 david     (1000) david     (1000)      805 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/r-project.svg
--rw-r--r--   0 david     (1000) david     (1000)     3999 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/raspberry-pi.svg
--rw-r--r--   0 david     (1000) david     (1000)     1827 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ravelry.svg
--rw-r--r--   0 david     (1000) david     (1000)     3088 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/react.svg
--rw-r--r--   0 david     (1000) david     (1000)     5668 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/reacteurope.svg
--rw-r--r--   0 david     (1000) david     (1000)     1243 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/readme.svg
--rw-r--r--   0 david     (1000) david     (1000)      811 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/rebel.svg
--rw-r--r--   0 david     (1000) david     (1000)      669 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/red-river.svg
--rw-r--r--   0 david     (1000) david     (1000)     1106 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/reddit-alien.svg
--rw-r--r--   0 david     (1000) david     (1000)     1217 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/reddit-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1168 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/reddit.svg
--rw-r--r--   0 david     (1000) david     (1000)      823 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/redhat.svg
--rw-r--r--   0 david     (1000) david     (1000)      592 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/renren.svg
--rw-r--r--   0 david     (1000) david     (1000)     1477 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/replyd.svg
--rw-r--r--   0 david     (1000) david     (1000)      992 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/researchgate.svg
--rw-r--r--   0 david     (1000) david     (1000)      733 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/resolving.svg
--rw-r--r--   0 david     (1000) david     (1000)      623 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/rev.svg
--rw-r--r--   0 david     (1000) david     (1000)     1543 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/rocketchat.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/rockrms.svg
--rw-r--r--   0 david     (1000) david     (1000)     4088 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/rust.svg
--rw-r--r--   0 david     (1000) david     (1000)     1875 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/safari.svg
--rw-r--r--   0 david     (1000) david     (1000)     4458 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/salesforce.svg
--rw-r--r--   0 david     (1000) david     (1000)     3267 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sass.svg
--rw-r--r--   0 david     (1000) david     (1000)     1044 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/schlix.svg
--rw-r--r--   0 david     (1000) david     (1000)      917 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/scribd.svg
--rw-r--r--   0 david     (1000) david     (1000)      937 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/searchengin.svg
--rw-r--r--   0 david     (1000) david     (1000)     1010 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sellcast.svg
--rw-r--r--   0 david     (1000) david     (1000)     1390 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sellsy.svg
--rw-r--r--   0 david     (1000) david     (1000)      430 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/servicestack.svg
--rw-r--r--   0 david     (1000) david     (1000)     1768 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/shirtsinbulk.svg
--rw-r--r--   0 david     (1000) david     (1000)     1497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/shopify.svg
--rw-r--r--   0 david     (1000) david     (1000)      771 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/shopware.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/simplybuilt.svg
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sistrix.svg
--rw-r--r--   0 david     (1000) david     (1000)     1006 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sith.svg
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sketch.svg
--rw-r--r--   0 david     (1000) david     (1000)      919 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/skyatlas.svg
--rw-r--r--   0 david     (1000) david     (1000)      965 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/skype.svg
--rw-r--r--   0 david     (1000) david     (1000)      951 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/slack-hash.svg
--rw-r--r--   0 david     (1000) david     (1000)     1249 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/slack.svg
--rw-r--r--   0 david     (1000) david     (1000)     1042 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/slideshare.svg
--rw-r--r--   0 david     (1000) david     (1000)     1662 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/snapchat-ghost.svg
--rw-r--r--   0 david     (1000) david     (1000)     1270 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/snapchat-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1235 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/snapchat.svg
--rw-r--r--   0 david     (1000) david     (1000)     2368 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/soundcloud.svg
--rw-r--r--   0 david     (1000) david     (1000)      514 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sourcetree.svg
--rw-r--r--   0 david     (1000) david     (1000)      815 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/speakap.svg
--rw-r--r--   0 david     (1000) david     (1000)      620 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/speaker-deck.svg
--rw-r--r--   0 david     (1000) david     (1000)     1049 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/spotify.svg
--rw-r--r--   0 david     (1000) david     (1000)     1365 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/squarespace.svg
--rw-r--r--   0 david     (1000) david     (1000)      480 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stack-exchange.svg
--rw-r--r--   0 david     (1000) david     (1000)      479 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stack-overflow.svg
--rw-r--r--   0 david     (1000) david     (1000)      966 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stackpath.svg
--rw-r--r--   0 david     (1000) david     (1000)      975 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/staylinked.svg
--rw-r--r--   0 david     (1000) david     (1000)     1009 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/steam-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      874 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/steam-symbol.svg
--rw-r--r--   0 david     (1000) david     (1000)      992 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/steam.svg
--rw-r--r--   0 david     (1000) david     (1000)     1815 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/sticker-mule.svg
--rw-r--r--   0 david     (1000) david     (1000)      364 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/strava.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stripe-s.svg
--rw-r--r--   0 david     (1000) david     (1000)     1379 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stripe.svg
--rw-r--r--   0 david     (1000) david     (1000)      747 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/studiovinari.svg
--rw-r--r--   0 david     (1000) david     (1000)      767 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stumbleupon-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      678 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/stumbleupon.svg
--rw-r--r--   0 david     (1000) david     (1000)      580 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/superpowers.svg
--rw-r--r--   0 david     (1000) david     (1000)     1892 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/supple.svg
--rw-r--r--   0 david     (1000) david     (1000)     1469 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/suse.svg
--rw-r--r--   0 david     (1000) david     (1000)     1733 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/swift.svg
--rw-r--r--   0 david     (1000) david     (1000)     1363 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/symfony.svg
--rw-r--r--   0 david     (1000) david     (1000)     1255 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/teamspeak.svg
--rw-r--r--   0 david     (1000) david     (1000)      500 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/telegram-plane.svg
--rw-r--r--   0 david     (1000) david     (1000)      556 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/telegram.svg
--rw-r--r--   0 david     (1000) david     (1000)      676 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/tencent-weibo.svg
--rw-r--r--   0 david     (1000) david     (1000)     6349 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/the-red-yeti.svg
--rw-r--r--   0 david     (1000) david     (1000)      936 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/themeco.svg
--rw-r--r--   0 david     (1000) david     (1000)     3459 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/themeisle.svg
--rw-r--r--   0 david     (1000) david     (1000)      391 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/think-peaks.svg
--rw-r--r--   0 david     (1000) david     (1000)      479 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/tiktok.svg
--rw-r--r--   0 david     (1000) david     (1000)     1558 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/trade-federation.svg
--rw-r--r--   0 david     (1000) david     (1000)      664 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/trello.svg
--rw-r--r--   0 david     (1000) david     (1000)      845 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/tripadvisor.svg
--rw-r--r--   0 david     (1000) david     (1000)      737 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/tumblr-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      625 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/tumblr.svg
--rw-r--r--   0 david     (1000) david     (1000)      460 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/twitch.svg
--rw-r--r--   0 david     (1000) david     (1000)      851 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/twitter-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1051 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/twitter.svg
--rw-r--r--   0 david     (1000) david     (1000)      582 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/typo3.svg
--rw-r--r--   0 david     (1000) david     (1000)      640 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/uber.svg
--rw-r--r--   0 david     (1000) david     (1000)     1129 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ubuntu.svg
--rw-r--r--   0 david     (1000) david     (1000)      415 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/uikit.svg
--rw-r--r--   0 david     (1000) david     (1000)     1155 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/umbraco.svg
--rw-r--r--   0 david     (1000) david     (1000)     1664 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/uncharted.svg
--rw-r--r--   0 david     (1000) david     (1000)     1228 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/uniregistry.svg
--rw-r--r--   0 david     (1000) david     (1000)      526 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/unity.svg
--rw-r--r--   0 david     (1000) david     (1000)      345 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/unsplash.svg
--rw-r--r--   0 david     (1000) david     (1000)     1302 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/untappd.svg
--rw-r--r--   0 david     (1000) david     (1000)      927 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ups.svg
--rw-r--r--   0 david     (1000) david     (1000)      941 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/usb.svg
--rw-r--r--   0 david     (1000) david     (1000)      749 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/usps.svg
--rw-r--r--   0 david     (1000) david     (1000)     3436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/ussunnah.svg
--rw-r--r--   0 david     (1000) david     (1000)      945 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vaadin.svg
--rw-r--r--   0 david     (1000) david     (1000)      416 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/viacoin.svg
--rw-r--r--   0 david     (1000) david     (1000)     1065 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/viadeo-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      997 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/viadeo.svg
--rw-r--r--   0 david     (1000) david     (1000)     1637 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/viber.svg
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vimeo-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      641 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vimeo-v.svg
--rw-r--r--   0 david     (1000) david     (1000)      755 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vimeo.svg
--rw-r--r--   0 david     (1000) david     (1000)      681 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vine.svg
--rw-r--r--   0 david     (1000) david     (1000)      869 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vk.svg
--rw-r--r--   0 david     (1000) david     (1000)     1031 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vnv.svg
--rw-r--r--   0 david     (1000) david     (1000)      380 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/vuejs.svg
--rw-r--r--   0 david     (1000) david     (1000)     1087 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/watchman-monitoring.svg
--rw-r--r--   0 david     (1000) david     (1000)     1233 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/waze.svg
--rw-r--r--   0 david     (1000) david     (1000)     1188 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/weebly.svg
--rw-r--r--   0 david     (1000) david     (1000)     1180 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/weibo.svg
--rw-r--r--   0 david     (1000) david     (1000)     1128 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/weixin.svg
--rw-r--r--   0 david     (1000) david     (1000)     1208 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/whatsapp-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1146 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/whatsapp.svg
--rw-r--r--   0 david     (1000) david     (1000)     1438 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/whmcs.svg
--rw-r--r--   0 david     (1000) david     (1000)      957 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wikipedia-w.svg
--rw-r--r--   0 david     (1000) david     (1000)      395 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/windows.svg
--rw-r--r--   0 david     (1000) david     (1000)     1408 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wix.svg
--rw-r--r--   0 david     (1000) david     (1000)     8319 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wizards-of-the-coast.svg
--rw-r--r--   0 david     (1000) david     (1000)     1371 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wodu.svg
--rw-r--r--   0 david     (1000) david     (1000)     2652 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wolf-pack-battalion.svg
--rw-r--r--   0 david     (1000) david     (1000)     1143 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wordpress-simple.svg
--rw-r--r--   0 david     (1000) david     (1000)     1284 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wordpress.svg
--rw-r--r--   0 david     (1000) david     (1000)      758 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wpbeginner.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wpexplorer.svg
--rw-r--r--   0 david     (1000) david     (1000)      770 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wpforms.svg
--rw-r--r--   0 david     (1000) david     (1000)     1392 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/wpressr.svg
--rw-r--r--   0 david     (1000) david     (1000)     1151 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/xbox.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/xing-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      639 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/xing.svg
--rw-r--r--   0 david     (1000) david     (1000)      389 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/y-combinator.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yahoo.svg
--rw-r--r--   0 david     (1000) david     (1000)      875 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yammer.svg
--rw-r--r--   0 david     (1000) david     (1000)      336 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yandex-international.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yandex.svg
--rw-r--r--   0 david     (1000) david     (1000)     1592 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yarn.svg
--rw-r--r--   0 david     (1000) david     (1000)     1017 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yelp.svg
--rw-r--r--   0 david     (1000) david     (1000)      700 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/yoast.svg
--rw-r--r--   0 david     (1000) david     (1000)      706 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/youtube-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/youtube.svg
--rw-r--r--   0 david     (1000) david     (1000)     1724 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/brands/zhihu.svg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.580536 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/address-book.svg
--rw-r--r--   0 david     (1000) david     (1000)      895 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/address-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      996 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/angry.svg
--rw-r--r--   0 david     (1000) david     (1000)      565 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/arrow-alt-circle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      559 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/arrow-alt-circle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      568 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/arrow-alt-circle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      565 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/arrow-alt-circle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      971 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/bell-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      829 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/bell.svg
--rw-r--r--   0 david     (1000) david     (1000)      414 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/bookmark.svg
--rw-r--r--   0 david     (1000) david     (1000)     1057 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/building.svg
--rw-r--r--   0 david     (1000) david     (1000)     1115 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/calendar-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      835 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/calendar-check.svg
--rw-r--r--   0 david     (1000) david     (1000)      626 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/calendar-minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/calendar-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      825 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/calendar-times.svg
--rw-r--r--   0 david     (1000) david     (1000)      529 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/calendar.svg
--rw-r--r--   0 david     (1000) david     (1000)      570 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/caret-square-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      568 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/caret-square-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      568 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/caret-square-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      567 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/caret-square-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      928 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/chart-bar.svg
--rw-r--r--   0 david     (1000) david     (1000)      761 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/check-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      680 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/check-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      412 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      615 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/clipboard.svg
--rw-r--r--   0 david     (1000) david     (1000)      584 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/clock.svg
--rw-r--r--   0 david     (1000) david     (1000)      608 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/clone.svg
--rw-r--r--   0 david     (1000) david     (1000)      920 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/closed-captioning.svg
--rw-r--r--   0 david     (1000) david     (1000)      542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/comment-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      913 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/comment-dots.svg
--rw-r--r--   0 david     (1000) david     (1000)      698 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/comment.svg
--rw-r--r--   0 david     (1000) david     (1000)     1151 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/comments.svg
--rw-r--r--   0 david     (1000) david     (1000)      773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/compass.svg
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/copy.svg
--rw-r--r--   0 david     (1000) david     (1000)      964 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/copyright.svg
--rw-r--r--   0 david     (1000) david     (1000)      699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/credit-card.svg
--rw-r--r--   0 david     (1000) david     (1000)     1059 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/dizzy.svg
--rw-r--r--   0 david     (1000) david     (1000)      552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/dot-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/edit.svg
--rw-r--r--   0 david     (1000) david     (1000)     1323 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/envelope-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      754 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/envelope.svg
--rw-r--r--   0 david     (1000) david     (1000)     1044 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/eye-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      689 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/eye.svg
--rw-r--r--   0 david     (1000) david     (1000)      690 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-archive.svg
--rw-r--r--   0 david     (1000) david     (1000)      864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-audio.svg
--rw-r--r--   0 david     (1000) david     (1000)     1030 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-code.svg
--rw-r--r--   0 david     (1000) david     (1000)      852 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-excel.svg
--rw-r--r--   0 david     (1000) david     (1000)      657 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-image.svg
--rw-r--r--   0 david     (1000) david     (1000)     1058 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-pdf.svg
--rw-r--r--   0 david     (1000) david     (1000)      710 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-powerpoint.svg
--rw-r--r--   0 david     (1000) david     (1000)      764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-video.svg
--rw-r--r--   0 david     (1000) david     (1000)     1035 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file-word.svg
--rw-r--r--   0 david     (1000) david     (1000)      484 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/file.svg
--rw-r--r--   0 david     (1000) david     (1000)      972 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/flag.svg
--rw-r--r--   0 david     (1000) david     (1000)      929 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/flushed.svg
--rw-r--r--   0 david     (1000) david     (1000)      548 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/folder-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/folder.svg
--rw-r--r--   0 david     (1000) david     (1000)     3174 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/font-awesome-logo-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      721 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/frown-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/frown.svg
--rw-r--r--   0 david     (1000) david     (1000)      905 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/futbol.svg
--rw-r--r--   0 david     (1000) david     (1000)      626 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/gem.svg
--rw-r--r--   0 david     (1000) david     (1000)      902 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grimace.svg
--rw-r--r--   0 david     (1000) david     (1000)      900 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1280 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-beam-sweat.svg
--rw-r--r--   0 david     (1000) david     (1000)     1000 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)      942 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-hearts.svg
--rw-r--r--   0 david     (1000) david     (1000)     1566 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-squint-tears.svg
--rw-r--r--   0 david     (1000) david     (1000)      950 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-squint.svg
--rw-r--r--   0 david     (1000) david     (1000)     1019 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-stars.svg
--rw-r--r--   0 david     (1000) david     (1000)     1503 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-tears.svg
--rw-r--r--   0 david     (1000) david     (1000)     1213 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-tongue-squint.svg
--rw-r--r--   0 david     (1000) david     (1000)     1256 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-tongue-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      986 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-tongue.svg
--rw-r--r--   0 david     (1000) david     (1000)      901 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      722 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/grin.svg
--rw-r--r--   0 david     (1000) david     (1000)      955 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-lizard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1167 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-paper.svg
--rw-r--r--   0 david     (1000) david     (1000)     1300 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-peace.svg
--rw-r--r--   0 david     (1000) david     (1000)     1315 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-point-down.svg
--rw-r--r--   0 david     (1000) david     (1000)     1319 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-point-left.svg
--rw-r--r--   0 david     (1000) david     (1000)     1326 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-point-right.svg
--rw-r--r--   0 david     (1000) david     (1000)     1320 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-point-up.svg
--rw-r--r--   0 david     (1000) david     (1000)     1578 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-pointer.svg
--rw-r--r--   0 david     (1000) david     (1000)     1311 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-rock.svg
--rw-r--r--   0 david     (1000) david     (1000)     1301 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-scissors.svg
--rw-r--r--   0 david     (1000) david     (1000)     1667 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hand-spock.svg
--rw-r--r--   0 david     (1000) david     (1000)     1313 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/handshake.svg
--rw-r--r--   0 david     (1000) david     (1000)      722 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hdd.svg
--rw-r--r--   0 david     (1000) david     (1000)      670 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/heart.svg
--rw-r--r--   0 david     (1000) david     (1000)     1245 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hospital.svg
--rw-r--r--   0 david     (1000) david     (1000)      727 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/hourglass.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/id-badge.svg
--rw-r--r--   0 david     (1000) david     (1000)      863 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/id-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      671 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/image.svg
--rw-r--r--   0 david     (1000) david     (1000)      824 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/images.svg
--rw-r--r--   0 david     (1000) david     (1000)     1846 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/keyboard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1193 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/kiss-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)     1362 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/kiss-wink-heart.svg
--rw-r--r--   0 david     (1000) david     (1000)      912 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/kiss.svg
--rw-r--r--   0 david     (1000) david     (1000)      975 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/laugh-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)      872 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/laugh-squint.svg
--rw-r--r--   0 david     (1000) david     (1000)      895 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/laugh-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      775 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/laugh.svg
--rw-r--r--   0 david     (1000) david     (1000)     1144 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/lemon.svg
--rw-r--r--   0 david     (1000) david     (1000)      917 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/life-ring.svg
--rw-r--r--   0 david     (1000) david     (1000)     1036 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/lightbulb.svg
--rw-r--r--   0 david     (1000) david     (1000)     1038 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/list-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      759 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/map.svg
--rw-r--r--   0 david     (1000) david     (1000)      556 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/meh-blank.svg
--rw-r--r--   0 david     (1000) david     (1000)     1006 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/meh-rolling-eyes.svg
--rw-r--r--   0 david     (1000) david     (1000)      644 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/meh.svg
--rw-r--r--   0 david     (1000) david     (1000)      556 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/minus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      845 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/money-bill-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      779 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/moon.svg
--rw-r--r--   0 david     (1000) david     (1000)     1126 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/newspaper.svg
--rw-r--r--   0 david     (1000) david     (1000)     1096 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/object-group.svg
--rw-r--r--   0 david     (1000) david     (1000)     1290 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/object-ungroup.svg
--rw-r--r--   0 david     (1000) david     (1000)      621 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/paper-plane.svg
--rw-r--r--   0 david     (1000) david     (1000)      612 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/pause-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      524 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/play-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      660 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/plus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1009 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/question-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      914 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/registered.svg
--rw-r--r--   0 david     (1000) david     (1000)     1043 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/sad-cry.svg
--rw-r--r--   0 david     (1000) david     (1000)      841 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/sad-tear.svg
--rw-r--r--   0 david     (1000) david     (1000)      779 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/save.svg
--rw-r--r--   0 david     (1000) david     (1000)     1181 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/share-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1055 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/smile-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)      861 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/smile-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      769 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/smile.svg
--rw-r--r--   0 david     (1000) david     (1000)     1782 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/snowflake.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/square.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/star-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/star.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/sticky-note.svg
--rw-r--r--   0 david     (1000) david     (1000)      517 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/stop-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)     1132 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/sun.svg
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/surprise.svg
--rw-r--r--   0 david     (1000) david     (1000)     1231 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/thumbs-down.svg
--rw-r--r--   0 david     (1000) david     (1000)     1224 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/thumbs-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      728 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/times-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      950 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/tired.svg
--rw-r--r--   0 david     (1000) david     (1000)      761 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/trash-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      845 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/user-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      701 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/user.svg
--rw-r--r--   0 david     (1000) david     (1000)      783 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/window-close.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/window-maximize.svg
--rw-r--r--   0 david     (1000) david     (1000)      348 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/window-minimize.svg
--rw-r--r--   0 david     (1000) david     (1000)      498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/regular/window-restore.svg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.740535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/
--rw-r--r--   0 david     (1000) david     (1000)      960 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ad.svg
--rw-r--r--   0 david     (1000) david     (1000)      773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/address-book.svg
--rw-r--r--   0 david     (1000) david     (1000)      873 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/address-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      419 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/adjust.svg
--rw-r--r--   0 david     (1000) david     (1000)     1974 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/air-freshener.svg
--rw-r--r--   0 david     (1000) david     (1000)      731 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/align-center.svg
--rw-r--r--   0 david     (1000) david     (1000)      632 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/align-justify.svg
--rw-r--r--   0 david     (1000) david     (1000)      739 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/align-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      747 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/align-right.svg
--rw-r--r--   0 david     (1000) david     (1000)     1185 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/allergies.svg
--rw-r--r--   0 david     (1000) david     (1000)      887 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ambulance.svg
--rw-r--r--   0 david     (1000) david     (1000)     2349 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/american-sign-language-interpreting.svg
--rw-r--r--   0 david     (1000) david     (1000)     1085 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/anchor.svg
--rw-r--r--   0 david     (1000) david     (1000)      634 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-double-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      636 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-double-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      638 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-double-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      637 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-double-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      450 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      448 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      449 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      449 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      947 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/angry.svg
--rw-r--r--   0 david     (1000) david     (1000)      661 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ankh.svg
--rw-r--r--   0 david     (1000) david     (1000)     1056 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/apple-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      524 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/archive.svg
--rw-r--r--   0 david     (1000) david     (1000)      586 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/archway.svg
--rw-r--r--   0 david     (1000) david     (1000)      500 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-alt-circle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      501 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-alt-circle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      495 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-alt-circle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      495 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-alt-circle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      584 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-circle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      581 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-circle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      582 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-circle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      577 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-circle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      508 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      508 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      513 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      511 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrow-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      595 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrows-alt-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      593 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrows-alt-v.svg
--rw-r--r--   0 david     (1000) david     (1000)      939 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/arrows-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1285 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/assistive-listening-systems.svg
--rw-r--r--   0 david     (1000) david     (1000)      959 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/asterisk.svg
--rw-r--r--   0 david     (1000) david     (1000)     1157 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/at.svg
--rw-r--r--   0 david     (1000) david     (1000)     1117 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/atlas.svg
--rw-r--r--   0 david     (1000) david     (1000)     2056 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/atom.svg
--rw-r--r--   0 david     (1000) david     (1000)     1042 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/audio-description.svg
--rw-r--r--   0 david     (1000) david     (1000)     1702 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/award.svg
--rw-r--r--   0 david     (1000) david     (1000)      835 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/baby-carriage.svg
--rw-r--r--   0 david     (1000) david     (1000)      886 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/baby.svg
--rw-r--r--   0 david     (1000) david     (1000)      835 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/backspace.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/backward.svg
--rw-r--r--   0 david     (1000) david     (1000)     1080 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bacon.svg
--rw-r--r--   0 david     (1000) david     (1000)     3069 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bacteria.svg
--rw-r--r--   0 david     (1000) david     (1000)     1680 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bacterium.svg
--rw-r--r--   0 david     (1000) david     (1000)     1129 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bahai.svg
--rw-r--r--   0 david     (1000) david     (1000)     1088 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/balance-scale-left.svg
--rw-r--r--   0 david     (1000) david     (1000)     1068 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/balance-scale-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      984 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/balance-scale.svg
--rw-r--r--   0 david     (1000) david     (1000)      583 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ban.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/band-aid.svg
--rw-r--r--   0 david     (1000) david     (1000)      749 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/barcode.svg
--rw-r--r--   0 david     (1000) david     (1000)      601 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bars.svg
--rw-r--r--   0 david     (1000) david     (1000)      931 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/baseball-ball.svg
--rw-r--r--   0 david     (1000) david     (1000)      950 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/basketball-ball.svg
--rw-r--r--   0 david     (1000) david     (1000)      812 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bath.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/battery-empty.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/battery-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/battery-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/battery-quarter.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/battery-three-quarters.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bed.svg
--rw-r--r--   0 david     (1000) david     (1000)      769 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/beer.svg
--rw-r--r--   0 david     (1000) david     (1000)      875 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bell-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      657 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bell.svg
--rw-r--r--   0 david     (1000) david     (1000)     1056 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bezier-curve.svg
--rw-r--r--   0 david     (1000) david     (1000)      733 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bible.svg
--rw-r--r--   0 david     (1000) david     (1000)     1602 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bicycle.svg
--rw-r--r--   0 david     (1000) david     (1000)      702 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/biking.svg
--rw-r--r--   0 david     (1000) david     (1000)      707 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/binoculars.svg
--rw-r--r--   0 david     (1000) david     (1000)     1701 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/biohazard.svg
--rw-r--r--   0 david     (1000) david     (1000)      958 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/birthday-cake.svg
--rw-r--r--   0 david     (1000) david     (1000)     1005 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/blender-phone.svg
--rw-r--r--   0 david     (1000) david     (1000)      751 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/blender.svg
--rw-r--r--   0 david     (1000) david     (1000)     1073 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/blind.svg
--rw-r--r--   0 david     (1000) david     (1000)      879 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/blog.svg
--rw-r--r--   0 david     (1000) david     (1000)      579 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bold.svg
--rw-r--r--   0 david     (1000) david     (1000)      469 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bolt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1102 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bomb.svg
--rw-r--r--   0 david     (1000) david     (1000)      875 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bone.svg
--rw-r--r--   0 david     (1000) david     (1000)     1015 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bong.svg
--rw-r--r--   0 david     (1000) david     (1000)     1128 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/book-dead.svg
--rw-r--r--   0 david     (1000) david     (1000)      652 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/book-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/book-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/book-reader.svg
--rw-r--r--   0 david     (1000) david     (1000)      698 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/book.svg
--rw-r--r--   0 david     (1000) david     (1000)      336 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bookmark.svg
--rw-r--r--   0 david     (1000) david     (1000)      429 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/border-all.svg
--rw-r--r--   0 david     (1000) david     (1000)     2202 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/border-none.svg
--rw-r--r--   0 david     (1000) david     (1000)     1027 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/border-style.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bowling-ball.svg
--rw-r--r--   0 david     (1000) david     (1000)      761 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/box-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      560 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/box-tissue.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/box.svg
--rw-r--r--   0 david     (1000) david     (1000)      642 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/boxes.svg
--rw-r--r--   0 david     (1000) david     (1000)     1238 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/braille.svg
--rw-r--r--   0 david     (1000) david     (1000)      925 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/brain.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bread-slice.svg
--rw-r--r--   0 david     (1000) david     (1000)      629 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/briefcase-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/briefcase.svg
--rw-r--r--   0 david     (1000) david     (1000)     1660 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/broadcast-tower.svg
--rw-r--r--   0 david     (1000) david     (1000)      727 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/broom.svg
--rw-r--r--   0 david     (1000) david     (1000)      532 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/brush.svg
--rw-r--r--   0 david     (1000) david     (1000)     1129 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bug.svg
--rw-r--r--   0 david     (1000) david     (1000)     1144 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/building.svg
--rw-r--r--   0 david     (1000) david     (1000)      916 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bullhorn.svg
--rw-r--r--   0 david     (1000) david     (1000)      624 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bullseye.svg
--rw-r--r--   0 david     (1000) david     (1000)      467 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/burn.svg
--rw-r--r--   0 david     (1000) david     (1000)      987 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bus-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      870 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/bus.svg
--rw-r--r--   0 david     (1000) david     (1000)      866 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/business-time.svg
--rw-r--r--   0 david     (1000) david     (1000)     1149 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calculator.svg
--rw-r--r--   0 david     (1000) david     (1000)     1084 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      894 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-check.svg
--rw-r--r--   0 david     (1000) david     (1000)      591 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-day.svg
--rw-r--r--   0 david     (1000) david     (1000)      669 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      882 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-times.svg
--rw-r--r--   0 david     (1000) david     (1000)      592 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar-week.svg
--rw-r--r--   0 david     (1000) david     (1000)      572 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/calendar.svg
--rw-r--r--   0 david     (1000) david     (1000)      855 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/camera-retro.svg
--rw-r--r--   0 david     (1000) david     (1000)      602 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/camera.svg
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/campground.svg
--rw-r--r--   0 david     (1000) david     (1000)     1093 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/candy-cane.svg
--rw-r--r--   0 david     (1000) david     (1000)     1334 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cannabis.svg
--rw-r--r--   0 david     (1000) david     (1000)      788 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/capsules.svg
--rw-r--r--   0 david     (1000) david     (1000)      918 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/car-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      781 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/car-battery.svg
--rw-r--r--   0 david     (1000) david     (1000)     2160 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/car-crash.svg
--rw-r--r--   0 david     (1000) david     (1000)      764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/car-side.svg
--rw-r--r--   0 david     (1000) david     (1000)     1044 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/car.svg
--rw-r--r--   0 david     (1000) david     (1000)      653 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caravan.svg
--rw-r--r--   0 david     (1000) david     (1000)      379 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      412 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-square-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-square-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      538 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-square-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-square-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/caret-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/carrot.svg
--rw-r--r--   0 david     (1000) david     (1000)     1093 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cart-arrow-down.svg
--rw-r--r--   0 david     (1000) david     (1000)     1110 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cart-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1354 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cash-register.svg
--rw-r--r--   0 david     (1000) david     (1000)      818 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cat.svg
--rw-r--r--   0 david     (1000) david     (1000)     1091 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/certificate.svg
--rw-r--r--   0 david     (1000) david     (1000)      658 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chair.svg
--rw-r--r--   0 david     (1000) david     (1000)      779 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chalkboard-teacher.svg
--rw-r--r--   0 david     (1000) david     (1000)      463 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chalkboard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1088 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/charging-station.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chart-area.svg
--rw-r--r--   0 david     (1000) david     (1000)      922 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chart-bar.svg
--rw-r--r--   0 david     (1000) david     (1000)      726 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chart-line.svg
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chart-pie.svg
--rw-r--r--   0 david     (1000) david     (1000)      616 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/check-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      643 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/check-double.svg
--rw-r--r--   0 david     (1000) david     (1000)      639 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/check-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      534 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/check.svg
--rw-r--r--   0 david     (1000) david     (1000)      385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cheese.svg
--rw-r--r--   0 david     (1000) david     (1000)      699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-bishop.svg
--rw-r--r--   0 david     (1000) david     (1000)      920 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-board.svg
--rw-r--r--   0 david     (1000) david     (1000)      564 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-king.svg
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-knight.svg
--rw-r--r--   0 david     (1000) david     (1000)      609 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-pawn.svg
--rw-r--r--   0 david     (1000) david     (1000)      840 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-queen.svg
--rw-r--r--   0 david     (1000) david     (1000)      618 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess-rook.svg
--rw-r--r--   0 david     (1000) david     (1000)     1235 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chess.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-circle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-circle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      518 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-circle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      516 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-circle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      539 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      541 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/chevron-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      705 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/child.svg
--rw-r--r--   0 david     (1000) david     (1000)      762 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/church.svg
--rw-r--r--   0 david     (1000) david     (1000)      728 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/circle-notch.svg
--rw-r--r--   0 david     (1000) david     (1000)      329 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/circle.svg
--rw-r--r--   0 david     (1000) david     (1000)     1713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/city.svg
--rw-r--r--   0 david     (1000) david     (1000)      770 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/clinic-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      667 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/clipboard-check.svg
--rw-r--r--   0 david     (1000) david     (1000)      952 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/clipboard-list.svg
--rw-r--r--   0 david     (1000) david     (1000)      577 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/clipboard.svg
--rw-r--r--   0 david     (1000) david     (1000)      482 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/clock.svg
--rw-r--r--   0 david     (1000) david     (1000)      502 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/clone.svg
--rw-r--r--   0 david     (1000) david     (1000)      834 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/closed-captioning.svg
--rw-r--r--   0 david     (1000) david     (1000)      691 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-download-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1255 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-meatball.svg
--rw-r--r--   0 david     (1000) david     (1000)     1350 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-moon-rain.svg
--rw-r--r--   0 david     (1000) david     (1000)      856 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-moon.svg
--rw-r--r--   0 david     (1000) david     (1000)      874 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-rain.svg
--rw-r--r--   0 david     (1000) david     (1000)     1231 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-showers-heavy.svg
--rw-r--r--   0 david     (1000) david     (1000)     1630 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-sun-rain.svg
--rw-r--r--   0 david     (1000) david     (1000)     1045 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-sun.svg
--rw-r--r--   0 david     (1000) david     (1000)      691 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud-upload-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      514 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cloud.svg
--rw-r--r--   0 david     (1000) david     (1000)      704 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cocktail.svg
--rw-r--r--   0 david     (1000) david     (1000)      935 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/code-branch.svg
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/code.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/coffee.svg
--rw-r--r--   0 david     (1000) david     (1000)     1070 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cog.svg
--rw-r--r--   0 david     (1000) david     (1000)     2645 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cogs.svg
--rw-r--r--   0 david     (1000) david     (1000)      791 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/coins.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/columns.svg
--rw-r--r--   0 david     (1000) david     (1000)      402 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comment-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1187 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comment-dollar.svg
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comment-dots.svg
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comment-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comment-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      480 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comment.svg
--rw-r--r--   0 david     (1000) david     (1000)     1498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comments-dollar.svg
--rw-r--r--   0 david     (1000) david     (1000)      759 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/comments.svg
--rw-r--r--   0 david     (1000) david     (1000)      526 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/compact-disc.svg
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/compass.svg
--rw-r--r--   0 david     (1000) david     (1000)      775 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/compress-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      982 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/compress-arrows-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      765 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/compress.svg
--rw-r--r--   0 david     (1000) david     (1000)      559 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/concierge-bell.svg
--rw-r--r--   0 david     (1000) david     (1000)      931 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cookie-bite.svg
--rw-r--r--   0 david     (1000) david     (1000)      964 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cookie.svg
--rw-r--r--   0 david     (1000) david     (1000)      611 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/copy.svg
--rw-r--r--   0 david     (1000) david     (1000)      833 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/copyright.svg
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/couch.svg
--rw-r--r--   0 david     (1000) david     (1000)      583 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/credit-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      576 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/crop-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      670 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/crop.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cross.svg
--rw-r--r--   0 david     (1000) david     (1000)     1210 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/crosshairs.svg
--rw-r--r--   0 david     (1000) david     (1000)      807 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/crow.svg
--rw-r--r--   0 david     (1000) david     (1000)      763 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/crown.svg
--rw-r--r--   0 david     (1000) david     (1000)      749 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/crutch.svg
--rw-r--r--   0 david     (1000) david     (1000)      554 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cube.svg
--rw-r--r--   0 david     (1000) david     (1000)      867 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cubes.svg
--rw-r--r--   0 david     (1000) david     (1000)      866 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/cut.svg
--rw-r--r--   0 david     (1000) david     (1000)      657 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/database.svg
--rw-r--r--   0 david     (1000) david     (1000)     1179 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/deaf.svg
--rw-r--r--   0 david     (1000) david     (1000)     1493 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/democrat.svg
--rw-r--r--   0 david     (1000) david     (1000)      488 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/desktop.svg
--rw-r--r--   0 david     (1000) david     (1000)     2218 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dharmachakra.svg
--rw-r--r--   0 david     (1000) david     (1000)     1087 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/diagnoses.svg
--rw-r--r--   0 david     (1000) david     (1000)     1186 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-d20.svg
--rw-r--r--   0 david     (1000) david     (1000)      707 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-d6.svg
--rw-r--r--   0 david     (1000) david     (1000)      755 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-five.svg
--rw-r--r--   0 david     (1000) david     (1000)      681 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-four.svg
--rw-r--r--   0 david     (1000) david     (1000)      451 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-one.svg
--rw-r--r--   0 david     (1000) david     (1000)      829 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-six.svg
--rw-r--r--   0 david     (1000) david     (1000)      603 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-three.svg
--rw-r--r--   0 david     (1000) david     (1000)      529 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice-two.svg
--rw-r--r--   0 david     (1000) david     (1000)     1151 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dice.svg
--rw-r--r--   0 david     (1000) david     (1000)     1044 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/digital-tachograph.svg
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/directions.svg
--rw-r--r--   0 david     (1000) david     (1000)      846 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/disease.svg
--rw-r--r--   0 david     (1000) david     (1000)      529 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/divide.svg
--rw-r--r--   0 david     (1000) david     (1000)      808 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dizzy.svg
--rw-r--r--   0 david     (1000) david     (1000)     1025 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dna.svg
--rw-r--r--   0 david     (1000) david     (1000)      666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dog.svg
--rw-r--r--   0 david     (1000) david     (1000)      861 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dollar-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      698 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dolly-flatbed.svg
--rw-r--r--   0 david     (1000) david     (1000)      844 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dolly.svg
--rw-r--r--   0 david     (1000) david     (1000)     1195 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/donate.svg
--rw-r--r--   0 david     (1000) david     (1000)      530 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/door-closed.svg
--rw-r--r--   0 david     (1000) david     (1000)      598 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/door-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      431 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dot-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dove.svg
--rw-r--r--   0 david     (1000) david     (1000)      702 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/download.svg
--rw-r--r--   0 david     (1000) david     (1000)     1143 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/drafting-compass.svg
--rw-r--r--   0 david     (1000) david     (1000)     1100 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dragon.svg
--rw-r--r--   0 david     (1000) david     (1000)     1273 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/draw-polygon.svg
--rw-r--r--   0 david     (1000) david     (1000)      911 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/drum-steelpan.svg
--rw-r--r--   0 david     (1000) david     (1000)      904 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/drum.svg
--rw-r--r--   0 david     (1000) david     (1000)      680 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/drumstick-bite.svg
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dumbbell.svg
--rw-r--r--   0 david     (1000) david     (1000)     1164 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dumpster-fire.svg
--rw-r--r--   0 david     (1000) david     (1000)      719 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dumpster.svg
--rw-r--r--   0 david     (1000) david     (1000)     2102 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/dungeon.svg
--rw-r--r--   0 david     (1000) david     (1000)      767 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/edit.svg
--rw-r--r--   0 david     (1000) david     (1000)      326 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/egg.svg
--rw-r--r--   0 david     (1000) david     (1000)      545 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/eject.svg
--rw-r--r--   0 david     (1000) david     (1000)      477 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ellipsis-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      471 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ellipsis-v.svg
--rw-r--r--   0 david     (1000) david     (1000)     1016 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/envelope-open-text.svg
--rw-r--r--   0 david     (1000) david     (1000)     1051 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/envelope-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      859 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/envelope-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      724 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/envelope.svg
--rw-r--r--   0 david     (1000) david     (1000)      490 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/equals.svg
--rw-r--r--   0 david     (1000) david     (1000)      596 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/eraser.svg
--rw-r--r--   0 david     (1000) david     (1000)      522 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ethernet.svg
--rw-r--r--   0 david     (1000) david     (1000)     1138 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/euro-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      655 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/exchange-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      642 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/exclamation-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      708 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/exclamation-triangle.svg
--rw-r--r--   0 david     (1000) david     (1000)      527 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/exclamation.svg
--rw-r--r--   0 david     (1000) david     (1000)      769 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/expand-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      763 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/expand-arrows-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/expand.svg
--rw-r--r--   0 david     (1000) david     (1000)      603 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/external-link-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      639 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/external-link-square-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      681 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/eye-dropper.svg
--rw-r--r--   0 david     (1000) david     (1000)      995 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/eye-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/eye.svg
--rw-r--r--   0 david     (1000) david     (1000)      762 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fan.svg
--rw-r--r--   0 david     (1000) david     (1000)      526 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fast-backward.svg
--rw-r--r--   0 david     (1000) david     (1000)      529 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fast-forward.svg
--rw-r--r--   0 david     (1000) david     (1000)      791 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/faucet.svg
--rw-r--r--   0 david     (1000) david     (1000)      919 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fax.svg
--rw-r--r--   0 david     (1000) david     (1000)      659 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/feather-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      678 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/feather.svg
--rw-r--r--   0 david     (1000) david     (1000)      610 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/female.svg
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fighter-jet.svg
--rw-r--r--   0 david     (1000) david     (1000)      737 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      767 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-archive.svg
--rw-r--r--   0 david     (1000) david     (1000)      826 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-audio.svg
--rw-r--r--   0 david     (1000) david     (1000)     1120 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-code.svg
--rw-r--r--   0 david     (1000) david     (1000)     1142 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-contract.svg
--rw-r--r--   0 david     (1000) david     (1000)     1296 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-csv.svg
--rw-r--r--   0 david     (1000) david     (1000)      644 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-download.svg
--rw-r--r--   0 david     (1000) david     (1000)      822 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-excel.svg
--rw-r--r--   0 david     (1000) david     (1000)      626 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-export.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-image.svg
--rw-r--r--   0 david     (1000) david     (1000)      630 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-import.svg
--rw-r--r--   0 david     (1000) david     (1000)     1293 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-invoice-dollar.svg
--rw-r--r--   0 david     (1000) david     (1000)      858 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-invoice.svg
--rw-r--r--   0 david     (1000) david     (1000)      677 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-medical-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      630 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)     1068 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-pdf.svg
--rw-r--r--   0 david     (1000) david     (1000)      693 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-powerpoint.svg
--rw-r--r--   0 david     (1000) david     (1000)      954 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-prescription.svg
--rw-r--r--   0 david     (1000) david     (1000)     1076 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-signature.svg
--rw-r--r--   0 david     (1000) david     (1000)      647 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-upload.svg
--rw-r--r--   0 david     (1000) david     (1000)      738 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-video.svg
--rw-r--r--   0 david     (1000) david     (1000)      924 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file-word.svg
--rw-r--r--   0 david     (1000) david     (1000)      447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/file.svg
--rw-r--r--   0 david     (1000) david     (1000)      882 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fill-drip.svg
--rw-r--r--   0 david     (1000) david     (1000)      820 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fill.svg
--rw-r--r--   0 david     (1000) david     (1000)     1352 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/film.svg
--rw-r--r--   0 david     (1000) david     (1000)      465 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/filter.svg
--rw-r--r--   0 david     (1000) david     (1000)     2123 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fingerprint.svg
--rw-r--r--   0 david     (1000) david     (1000)      686 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fire-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      888 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fire-extinguisher.svg
--rw-r--r--   0 david     (1000) david     (1000)      531 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fire.svg
--rw-r--r--   0 david     (1000) david     (1000)      588 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/first-aid.svg
--rw-r--r--   0 david     (1000) david     (1000)      603 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fish.svg
--rw-r--r--   0 david     (1000) david     (1000)     1290 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/fist-raised.svg
--rw-r--r--   0 david     (1000) david     (1000)     1194 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/flag-checkered.svg
--rw-r--r--   0 david     (1000) david     (1000)     1284 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/flag-usa.svg
--rw-r--r--   0 david     (1000) david     (1000)      787 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/flag.svg
--rw-r--r--   0 david     (1000) david     (1000)      558 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/flask.svg
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/flushed.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/folder-minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      582 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/folder-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/folder-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/folder.svg
--rw-r--r--   0 david     (1000) david     (1000)     3174 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/font-awesome-logo-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      588 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/font.svg
--rw-r--r--   0 david     (1000) david     (1000)     1247 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/football-ball.svg
--rw-r--r--   0 david     (1000) david     (1000)      480 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/forward.svg
--rw-r--r--   0 david     (1000) david     (1000)      979 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/frog.svg
--rw-r--r--   0 david     (1000) david     (1000)      637 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/frown-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      646 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/frown.svg
--rw-r--r--   0 david     (1000) david     (1000)     1254 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/funnel-dollar.svg
--rw-r--r--   0 david     (1000) david     (1000)      923 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/futbol.svg
--rw-r--r--   0 david     (1000) david     (1000)      608 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gamepad.svg
--rw-r--r--   0 david     (1000) david     (1000)      738 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gas-pump.svg
--rw-r--r--   0 david     (1000) david     (1000)      976 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gavel.svg
--rw-r--r--   0 david     (1000) david     (1000)      532 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gem.svg
--rw-r--r--   0 david     (1000) david     (1000)      412 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/genderless.svg
--rw-r--r--   0 david     (1000) david     (1000)      777 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ghost.svg
--rw-r--r--   0 david     (1000) david     (1000)      758 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gift.svg
--rw-r--r--   0 david     (1000) david     (1000)     1337 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gifts.svg
--rw-r--r--   0 david     (1000) david     (1000)      962 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/glass-cheers.svg
--rw-r--r--   0 david     (1000) david     (1000)      503 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/glass-martini-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      464 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/glass-martini.svg
--rw-r--r--   0 david     (1000) david     (1000)      439 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/glass-whiskey.svg
--rw-r--r--   0 david     (1000) david     (1000)     1510 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/glasses.svg
--rw-r--r--   0 david     (1000) david     (1000)     1493 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/globe-africa.svg
--rw-r--r--   0 david     (1000) david     (1000)     1652 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/globe-americas.svg
--rw-r--r--   0 david     (1000) david     (1000)     1531 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/globe-asia.svg
--rw-r--r--   0 david     (1000) david     (1000)     1638 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/globe-europe.svg
--rw-r--r--   0 david     (1000) david     (1000)      998 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/globe.svg
--rw-r--r--   0 david     (1000) david     (1000)      879 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/golf-ball.svg
--rw-r--r--   0 david     (1000) david     (1000)      890 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/gopuram.svg
--rw-r--r--   0 david     (1000) david     (1000)      874 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/graduation-cap.svg
--rw-r--r--   0 david     (1000) david     (1000)      669 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/greater-than-equal.svg
--rw-r--r--   0 david     (1000) david     (1000)      554 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/greater-than.svg
--rw-r--r--   0 david     (1000) david     (1000)      758 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grimace.svg
--rw-r--r--   0 david     (1000) david     (1000)      848 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1071 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-beam-sweat.svg
--rw-r--r--   0 david     (1000) david     (1000)      849 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)      865 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-hearts.svg
--rw-r--r--   0 david     (1000) david     (1000)     1291 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-squint-tears.svg
--rw-r--r--   0 david     (1000) david     (1000)      736 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-squint.svg
--rw-r--r--   0 david     (1000) david     (1000)      931 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-stars.svg
--rw-r--r--   0 david     (1000) david     (1000)     1367 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-tears.svg
--rw-r--r--   0 david     (1000) david     (1000)     1027 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-tongue-squint.svg
--rw-r--r--   0 david     (1000) david     (1000)     1082 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-tongue-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      931 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-tongue.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      641 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grin.svg
--rw-r--r--   0 david     (1000) david     (1000)      943 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grip-horizontal.svg
--rw-r--r--   0 david     (1000) david     (1000)      456 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grip-lines-vertical.svg
--rw-r--r--   0 david     (1000) david     (1000)      458 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grip-lines.svg
--rw-r--r--   0 david     (1000) david     (1000)      938 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/grip-vertical.svg
--rw-r--r--   0 david     (1000) david     (1000)      867 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/guitar.svg
--rw-r--r--   0 david     (1000) david     (1000)      614 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/h-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      677 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hamburger.svg
--rw-r--r--   0 david     (1000) david     (1000)      826 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hammer.svg
--rw-r--r--   0 david     (1000) david     (1000)      846 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hamsa.svg
--rw-r--r--   0 david     (1000) david     (1000)      773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-holding-heart.svg
--rw-r--r--   0 david     (1000) david     (1000)      789 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-holding-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)     1257 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-holding-usd.svg
--rw-r--r--   0 david     (1000) david     (1000)      701 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-holding-water.svg
--rw-r--r--   0 david     (1000) david     (1000)      577 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-holding.svg
--rw-r--r--   0 david     (1000) david     (1000)      640 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-lizard.svg
--rw-r--r--   0 david     (1000) david     (1000)      717 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-middle-finger.svg
--rw-r--r--   0 david     (1000) david     (1000)      839 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-paper.svg
--rw-r--r--   0 david     (1000) david     (1000)      706 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-peace.svg
--rw-r--r--   0 david     (1000) david     (1000)      988 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-point-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      992 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-point-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      995 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-point-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      990 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-point-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      737 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-pointer.svg
--rw-r--r--   0 david     (1000) david     (1000)      774 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-rock.svg
--rw-r--r--   0 david     (1000) david     (1000)      711 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-scissors.svg
--rw-r--r--   0 david     (1000) david     (1000)     1461 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-sparkles.svg
--rw-r--r--   0 david     (1000) david     (1000)      968 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hand-spock.svg
--rw-r--r--   0 david     (1000) david     (1000)      779 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hands-helping.svg
--rw-r--r--   0 david     (1000) david     (1000)     1481 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hands-wash.svg
--rw-r--r--   0 david     (1000) david     (1000)      958 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hands.svg
--rw-r--r--   0 david     (1000) david     (1000)      865 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/handshake-alt-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      960 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/handshake-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)     1083 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/handshake.svg
--rw-r--r--   0 david     (1000) david     (1000)     1760 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hanukiah.svg
--rw-r--r--   0 david     (1000) david     (1000)      502 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hard-hat.svg
--rw-r--r--   0 david     (1000) david     (1000)     1091 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hashtag.svg
--rw-r--r--   0 david     (1000) david     (1000)      681 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hat-cowboy-side.svg
--rw-r--r--   0 david     (1000) david     (1000)      662 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hat-cowboy.svg
--rw-r--r--   0 david     (1000) david     (1000)      597 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hat-wizard.svg
--rw-r--r--   0 david     (1000) david     (1000)      705 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hdd.svg
--rw-r--r--   0 david     (1000) david     (1000)      954 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/head-side-cough-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      803 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/head-side-cough.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/head-side-mask.svg
--rw-r--r--   0 david     (1000) david     (1000)     1111 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/head-side-virus.svg
--rw-r--r--   0 david     (1000) david     (1000)      650 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/heading.svg
--rw-r--r--   0 david     (1000) david     (1000)      773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/headphones-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      728 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/headphones.svg
--rw-r--r--   0 david     (1000) david     (1000)      832 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/headset.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/heart-broken.svg
--rw-r--r--   0 david     (1000) david     (1000)      467 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/heart.svg
--rw-r--r--   0 david     (1000) david     (1000)      666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/heartbeat.svg
--rw-r--r--   0 david     (1000) david     (1000)      839 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/helicopter.svg
--rw-r--r--   0 david     (1000) david     (1000)      626 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/highlighter.svg
--rw-r--r--   0 david     (1000) david     (1000)     1086 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hiking.svg
--rw-r--r--   0 david     (1000) david     (1000)      831 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hippo.svg
--rw-r--r--   0 david     (1000) david     (1000)      981 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/history.svg
--rw-r--r--   0 david     (1000) david     (1000)      412 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hockey-puck.svg
--rw-r--r--   0 david     (1000) david     (1000)     1392 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/holly-berry.svg
--rw-r--r--   0 david     (1000) david     (1000)      745 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/home.svg
--rw-r--r--   0 david     (1000) david     (1000)      782 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/horse-head.svg
--rw-r--r--   0 david     (1000) david     (1000)     1091 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/horse.svg
--rw-r--r--   0 david     (1000) david     (1000)     1194 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hospital-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hospital-symbol.svg
--rw-r--r--   0 david     (1000) david     (1000)     1253 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hospital-user.svg
--rw-r--r--   0 david     (1000) david     (1000)     1145 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hospital.svg
--rw-r--r--   0 david     (1000) david     (1000)     1438 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hot-tub.svg
--rw-r--r--   0 david     (1000) david     (1000)     1229 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hotdog.svg
--rw-r--r--   0 david     (1000) david     (1000)     1373 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hotel.svg
--rw-r--r--   0 david     (1000) david     (1000)      696 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hourglass-end.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hourglass-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      694 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hourglass-start.svg
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hourglass.svg
--rw-r--r--   0 david     (1000) david     (1000)      843 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/house-damage.svg
--rw-r--r--   0 david     (1000) david     (1000)      855 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/house-user.svg
--rw-r--r--   0 david     (1000) david     (1000)     1139 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/hryvnia.svg
--rw-r--r--   0 david     (1000) david     (1000)      995 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/i-cursor.svg
--rw-r--r--   0 david     (1000) david     (1000)      390 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ice-cream.svg
--rw-r--r--   0 david     (1000) david     (1000)      502 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/icicles.svg
--rw-r--r--   0 david     (1000) david     (1000)     1308 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/icons.svg
--rw-r--r--   0 david     (1000) david     (1000)      691 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/id-badge.svg
--rw-r--r--   0 david     (1000) david     (1000)      691 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/id-card-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      891 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/id-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/igloo.svg
--rw-r--r--   0 david     (1000) david     (1000)      594 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/image.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/images.svg
--rw-r--r--   0 david     (1000) david     (1000)      567 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/inbox.svg
--rw-r--r--   0 david     (1000) david     (1000)      858 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/indent.svg
--rw-r--r--   0 david     (1000) david     (1000)      503 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/industry.svg
--rw-r--r--   0 david     (1000) david     (1000)      671 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/infinity.svg
--rw-r--r--   0 david     (1000) david     (1000)      659 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/info-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      568 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/info.svg
--rw-r--r--   0 david     (1000) david     (1000)      468 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/italic.svg
--rw-r--r--   0 david     (1000) david     (1000)     2071 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/jedi.svg
--rw-r--r--   0 david     (1000) david     (1000)     1136 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/joint.svg
--rw-r--r--   0 david     (1000) david     (1000)     2235 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/journal-whills.svg
--rw-r--r--   0 david     (1000) david     (1000)     1276 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/kaaba.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/key.svg
--rw-r--r--   0 david     (1000) david     (1000)     1742 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/keyboard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1857 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/khanda.svg
--rw-r--r--   0 david     (1000) david     (1000)      977 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/kiss-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)     1184 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/kiss-wink-heart.svg
--rw-r--r--   0 david     (1000) david     (1000)      781 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/kiss.svg
--rw-r--r--   0 david     (1000) david     (1000)     1001 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/kiwi-bird.svg
--rw-r--r--   0 david     (1000) david     (1000)      662 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/landmark.svg
--rw-r--r--   0 david     (1000) david     (1000)     1246 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/language.svg
--rw-r--r--   0 david     (1000) david     (1000)      992 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laptop-code.svg
--rw-r--r--   0 david     (1000) david     (1000)      966 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laptop-house.svg
--rw-r--r--   0 david     (1000) david     (1000)      684 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laptop-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laptop.svg
--rw-r--r--   0 david     (1000) david     (1000)      789 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laugh-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)      683 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laugh-squint.svg
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laugh-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      586 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/laugh.svg
--rw-r--r--   0 david     (1000) david     (1000)      899 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/layer-group.svg
--rw-r--r--   0 david     (1000) david     (1000)      634 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/leaf.svg
--rw-r--r--   0 david     (1000) david     (1000)      863 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lemon.svg
--rw-r--r--   0 david     (1000) david     (1000)      669 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/less-than-equal.svg
--rw-r--r--   0 david     (1000) david     (1000)      547 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/less-than.svg
--rw-r--r--   0 david     (1000) david     (1000)      543 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/level-down-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      547 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/level-up-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      923 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/life-ring.svg
--rw-r--r--   0 david     (1000) david     (1000)      824 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lightbulb.svg
--rw-r--r--   0 david     (1000) david     (1000)     1507 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/link.svg
--rw-r--r--   0 david     (1000) david     (1000)      898 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lira-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      964 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/list-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/list-ol.svg
--rw-r--r--   0 david     (1000) david     (1000)      671 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/list-ul.svg
--rw-r--r--   0 david     (1000) david     (1000)      818 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/list.svg
--rw-r--r--   0 david     (1000) david     (1000)      418 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/location-arrow.svg
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lock-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      472 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lock.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/long-arrow-alt-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/long-arrow-alt-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/long-arrow-alt-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/long-arrow-alt-up.svg
--rw-r--r--   0 david     (1000) david     (1000)     1304 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/low-vision.svg
--rw-r--r--   0 david     (1000) david     (1000)      852 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/luggage-cart.svg
--rw-r--r--   0 david     (1000) david     (1000)     1659 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lungs-virus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1050 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/lungs.svg
--rw-r--r--   0 david     (1000) david     (1000)      793 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/magic.svg
--rw-r--r--   0 david     (1000) david     (1000)      690 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/magnet.svg
--rw-r--r--   0 david     (1000) david     (1000)      866 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mail-bulk.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/male.svg
--rw-r--r--   0 david     (1000) david     (1000)      905 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map-marked-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      834 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map-marked.svg
--rw-r--r--   0 david     (1000) david     (1000)      504 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map-marker-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      421 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map-marker.svg
--rw-r--r--   0 david     (1000) david     (1000)      592 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map-pin.svg
--rw-r--r--   0 david     (1000) david     (1000)      756 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map-signs.svg
--rw-r--r--   0 david     (1000) david     (1000)      498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/map.svg
--rw-r--r--   0 david     (1000) david     (1000)      699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/marker.svg
--rw-r--r--   0 david     (1000) david     (1000)      994 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mars-double.svg
--rw-r--r--   0 david     (1000) david     (1000)      767 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mars-stroke-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      766 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mars-stroke-v.svg
--rw-r--r--   0 david     (1000) david     (1000)      736 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mars-stroke.svg
--rw-r--r--   0 david     (1000) david     (1000)      570 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mars.svg
--rw-r--r--   0 david     (1000) david     (1000)      846 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mask.svg
--rw-r--r--   0 david     (1000) david     (1000)      947 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/medal.svg
--rw-r--r--   0 david     (1000) david     (1000)      741 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/medkit.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/meh-blank.svg
--rw-r--r--   0 david     (1000) david     (1000)      738 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/meh-rolling-eyes.svg
--rw-r--r--   0 david     (1000) david     (1000)      533 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/meh.svg
--rw-r--r--   0 david     (1000) david     (1000)      728 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/memory.svg
--rw-r--r--   0 david     (1000) david     (1000)     1417 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/menorah.svg
--rw-r--r--   0 david     (1000) david     (1000)      910 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mercury.svg
--rw-r--r--   0 david     (1000) david     (1000)     1129 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/meteor.svg
--rw-r--r--   0 david     (1000) david     (1000)     1070 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/microchip.svg
--rw-r--r--   0 david     (1000) david     (1000)     1100 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/microphone-alt-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      920 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/microphone-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      948 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/microphone-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      723 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/microphone.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/microscope.svg
--rw-r--r--   0 david     (1000) david     (1000)      430 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/minus-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      464 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/minus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      376 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      526 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mitten.svg
--rw-r--r--   0 david     (1000) david     (1000)      536 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mobile-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mobile.svg
--rw-r--r--   0 david     (1000) david     (1000)      871 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/money-bill-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      763 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/money-bill-wave-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1097 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/money-bill-wave.svg
--rw-r--r--   0 david     (1000) david     (1000)      617 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/money-bill.svg
--rw-r--r--   0 david     (1000) david     (1000)     1317 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/money-check-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      781 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/money-check.svg
--rw-r--r--   0 david     (1000) david     (1000)      654 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/monument.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/moon.svg
--rw-r--r--   0 david     (1000) david     (1000)      686 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mortar-pestle.svg
--rw-r--r--   0 david     (1000) david     (1000)      867 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mosque.svg
--rw-r--r--   0 david     (1000) david     (1000)     1271 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/motorcycle.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mountain.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mouse-pointer.svg
--rw-r--r--   0 david     (1000) david     (1000)      400 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mouse.svg
--rw-r--r--   0 david     (1000) david     (1000)      889 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/mug-hot.svg
--rw-r--r--   0 david     (1000) david     (1000)      504 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/music.svg
--rw-r--r--   0 david     (1000) david     (1000)      802 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/network-wired.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/neuter.svg
--rw-r--r--   0 david     (1000) david     (1000)     1028 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/newspaper.svg
--rw-r--r--   0 david     (1000) david     (1000)      726 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/not-equal.svg
--rw-r--r--   0 david     (1000) david     (1000)      746 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/notes-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      859 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/object-group.svg
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/object-ungroup.svg
--rw-r--r--   0 david     (1000) david     (1000)      847 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/oil-can.svg
--rw-r--r--   0 david     (1000) david     (1000)     1600 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/om.svg
--rw-r--r--   0 david     (1000) david     (1000)      934 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/otter.svg
--rw-r--r--   0 david     (1000) david     (1000)      857 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/outdent.svg
--rw-r--r--   0 david     (1000) david     (1000)      557 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pager.svg
--rw-r--r--   0 david     (1000) david     (1000)      705 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paint-brush.svg
--rw-r--r--   0 david     (1000) david     (1000)      599 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paint-roller.svg
--rw-r--r--   0 david     (1000) david     (1000)      741 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/palette.svg
--rw-r--r--   0 david     (1000) david     (1000)      634 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pallet.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paper-plane.svg
--rw-r--r--   0 david     (1000) david     (1000)     1046 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paperclip.svg
--rw-r--r--   0 david     (1000) david     (1000)      694 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/parachute-box.svg
--rw-r--r--   0 david     (1000) david     (1000)      438 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paragraph.svg
--rw-r--r--   0 david     (1000) david     (1000)      539 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/parking.svg
--rw-r--r--   0 david     (1000) david     (1000)     1068 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/passport.svg
--rw-r--r--   0 david     (1000) david     (1000)     2295 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pastafarianism.svg
--rw-r--r--   0 david     (1000) david     (1000)      762 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paste.svg
--rw-r--r--   0 david     (1000) david     (1000)      529 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pause-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pause.svg
--rw-r--r--   0 david     (1000) david     (1000)     1047 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/paw.svg
--rw-r--r--   0 david     (1000) david     (1000)      654 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/peace.svg
--rw-r--r--   0 david     (1000) david     (1000)      705 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pen-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pen-fancy.svg
--rw-r--r--   0 david     (1000) david     (1000)      673 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pen-nib.svg
--rw-r--r--   0 david     (1000) david     (1000)      649 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pen-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      504 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pen.svg
--rw-r--r--   0 david     (1000) david     (1000)      725 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pencil-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      960 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pencil-ruler.svg
--rw-r--r--   0 david     (1000) david     (1000)     1020 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/people-arrows.svg
--rw-r--r--   0 david     (1000) david     (1000)     1408 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/people-carry.svg
--rw-r--r--   0 david     (1000) david     (1000)      682 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pepper-hot.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/percent.svg
--rw-r--r--   0 david     (1000) david     (1000)      714 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/percentage.svg
--rw-r--r--   0 david     (1000) david     (1000)     1054 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/person-booth.svg
--rw-r--r--   0 david     (1000) david     (1000)      524 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/phone-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      774 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/phone-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      720 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/phone-square-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      698 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/phone-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1425 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/phone-volume.svg
--rw-r--r--   0 david     (1000) david     (1000)      541 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/phone.svg
--rw-r--r--   0 david     (1000) david     (1000)      830 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/photo-video.svg
--rw-r--r--   0 david     (1000) david     (1000)      940 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/piggy-bank.svg
--rw-r--r--   0 david     (1000) david     (1000)      682 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pills.svg
--rw-r--r--   0 david     (1000) david     (1000)      672 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pizza-slice.svg
--rw-r--r--   0 david     (1000) david     (1000)      702 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/place-of-worship.svg
--rw-r--r--   0 david     (1000) david     (1000)      825 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plane-arrival.svg
--rw-r--r--   0 david     (1000) david     (1000)      833 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plane-departure.svg
--rw-r--r--   0 david     (1000) david     (1000)      770 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plane-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      673 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plane.svg
--rw-r--r--   0 david     (1000) david     (1000)      437 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/play-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      371 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/play.svg
--rw-r--r--   0 david     (1000) david     (1000)      498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plug.svg
--rw-r--r--   0 david     (1000) david     (1000)      534 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plus-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      569 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      499 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/plus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1573 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/podcast.svg
--rw-r--r--   0 david     (1000) david     (1000)      686 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/poll-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      685 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/poll.svg
--rw-r--r--   0 david     (1000) david     (1000)      947 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/poo-storm.svg
--rw-r--r--   0 david     (1000) david     (1000)      939 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/poo.svg
--rw-r--r--   0 david     (1000) david     (1000)      759 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/poop.svg
--rw-r--r--   0 david     (1000) david     (1000)      611 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/portrait.svg
--rw-r--r--   0 david     (1000) david     (1000)      784 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pound-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      723 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/power-off.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pray.svg
--rw-r--r--   0 david     (1000) david     (1000)     1121 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/praying-hands.svg
--rw-r--r--   0 david     (1000) david     (1000)      607 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/prescription-bottle-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      561 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/prescription-bottle.svg
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/prescription.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/print.svg
--rw-r--r--   0 david     (1000) david     (1000)      776 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/procedures.svg
--rw-r--r--   0 david     (1000) david     (1000)      659 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/project-diagram.svg
--rw-r--r--   0 david     (1000) david     (1000)      883 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pump-medical.svg
--rw-r--r--   0 david     (1000) david     (1000)      709 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/pump-soap.svg
--rw-r--r--   0 david     (1000) david     (1000)      904 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/puzzle-piece.svg
--rw-r--r--   0 david     (1000) david     (1000)      479 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/qrcode.svg
--rw-r--r--   0 david     (1000) david     (1000)      882 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/question-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      840 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/question.svg
--rw-r--r--   0 david     (1000) david     (1000)      763 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/quidditch.svg
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/quote-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/quote-right.svg
--rw-r--r--   0 david     (1000) david     (1000)     1185 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/quran.svg
--rw-r--r--   0 david     (1000) david     (1000)      925 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/radiation-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      804 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/radiation.svg
--rw-r--r--   0 david     (1000) david     (1000)      917 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/rainbow.svg
--rw-r--r--   0 david     (1000) david     (1000)      932 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/random.svg
--rw-r--r--   0 david     (1000) david     (1000)      824 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/receipt.svg
--rw-r--r--   0 david     (1000) david     (1000)      476 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/record-vinyl.svg
--rw-r--r--   0 david     (1000) david     (1000)     1390 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/recycle.svg
--rw-r--r--   0 david     (1000) david     (1000)      805 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/redo-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      602 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/redo.svg
--rw-r--r--   0 david     (1000) david     (1000)      802 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/registered.svg
--rw-r--r--   0 david     (1000) david     (1000)      698 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/remove-format.svg
--rw-r--r--   0 david     (1000) david     (1000)      848 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/reply-all.svg
--rw-r--r--   0 david     (1000) david     (1000)      581 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/reply.svg
--rw-r--r--   0 david     (1000) david     (1000)     1257 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/republican.svg
--rw-r--r--   0 david     (1000) david     (1000)      987 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/restroom.svg
--rw-r--r--   0 david     (1000) david     (1000)     1075 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/retweet.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ribbon.svg
--rw-r--r--   0 david     (1000) david     (1000)      687 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ring.svg
--rw-r--r--   0 david     (1000) david     (1000)      949 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/road.svg
--rw-r--r--   0 david     (1000) david     (1000)      756 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/robot.svg
--rw-r--r--   0 david     (1000) david     (1000)     1033 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/rocket.svg
--rw-r--r--   0 david     (1000) david     (1000)      735 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/route.svg
--rw-r--r--   0 david     (1000) david     (1000)      968 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/rss-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      903 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/rss.svg
--rw-r--r--   0 david     (1000) david     (1000)      711 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ruble-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      776 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ruler-combined.svg
--rw-r--r--   0 david     (1000) david     (1000)      636 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ruler-horizontal.svg
--rw-r--r--   0 david     (1000) david     (1000)      581 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ruler-vertical.svg
--rw-r--r--   0 david     (1000) david     (1000)      864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ruler.svg
--rw-r--r--   0 david     (1000) david     (1000)     1067 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/running.svg
--rw-r--r--   0 david     (1000) david     (1000)      832 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/rupee-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      955 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sad-cry.svg
--rw-r--r--   0 david     (1000) david     (1000)      719 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sad-tear.svg
--rw-r--r--   0 david     (1000) david     (1000)     1281 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/satellite-dish.svg
--rw-r--r--   0 david     (1000) david     (1000)     1245 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/satellite.svg
--rw-r--r--   0 david     (1000) david     (1000)      701 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/save.svg
--rw-r--r--   0 david     (1000) david     (1000)      787 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/school.svg
--rw-r--r--   0 david     (1000) david     (1000)      550 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/screwdriver.svg
--rw-r--r--   0 david     (1000) david     (1000)      581 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/scroll.svg
--rw-r--r--   0 david     (1000) david     (1000)      411 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sd-card.svg
--rw-r--r--   0 david     (1000) david     (1000)     1349 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/search-dollar.svg
--rw-r--r--   0 david     (1000) david     (1000)      943 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/search-location.svg
--rw-r--r--   0 david     (1000) david     (1000)      685 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/search-minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      789 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/search-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      605 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/search.svg
--rw-r--r--   0 david     (1000) david     (1000)      468 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/seedling.svg
--rw-r--r--   0 david     (1000) david     (1000)     1120 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/server.svg
--rw-r--r--   0 david     (1000) david     (1000)      552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shapes.svg
--rw-r--r--   0 david     (1000) david     (1000)      851 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/share-alt-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      716 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/share-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      919 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/share-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      577 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/share.svg
--rw-r--r--   0 david     (1000) david     (1000)      650 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shekel-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      519 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shield-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1145 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shield-virus.svg
--rw-r--r--   0 david     (1000) david     (1000)      957 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ship.svg
--rw-r--r--   0 david     (1000) david     (1000)      921 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shipping-fast.svg
--rw-r--r--   0 david     (1000) david     (1000)      799 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shoe-prints.svg
--rw-r--r--   0 david     (1000) david     (1000)      618 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shopping-bag.svg
--rw-r--r--   0 david     (1000) david     (1000)     1022 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shopping-basket.svg
--rw-r--r--   0 david     (1000) david     (1000)      796 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shopping-cart.svg
--rw-r--r--   0 david     (1000) david     (1000)     1396 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shower.svg
--rw-r--r--   0 david     (1000) david     (1000)      739 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/shuttle-van.svg
--rw-r--r--   0 david     (1000) david     (1000)      596 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sign-in-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1687 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sign-language.svg
--rw-r--r--   0 david     (1000) david     (1000)      600 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sign-out-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/signal.svg
--rw-r--r--   0 david     (1000) david     (1000)      822 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/signature.svg
--rw-r--r--   0 david     (1000) david     (1000)      579 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sim-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      698 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sink.svg
--rw-r--r--   0 david     (1000) david     (1000)      842 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sitemap.svg
--rw-r--r--   0 david     (1000) david     (1000)     1066 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/skating.svg
--rw-r--r--   0 david     (1000) david     (1000)     1019 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/skiing-nordic.svg
--rw-r--r--   0 david     (1000) david     (1000)     1010 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/skiing.svg
--rw-r--r--   0 david     (1000) david     (1000)     1034 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/skull-crossbones.svg
--rw-r--r--   0 david     (1000) david     (1000)      738 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/skull.svg
--rw-r--r--   0 david     (1000) david     (1000)      451 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      747 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sleigh.svg
--rw-r--r--   0 david     (1000) david     (1000)      869 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sliders-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      846 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/smile-beam.svg
--rw-r--r--   0 david     (1000) david     (1000)      729 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/smile-wink.svg
--rw-r--r--   0 david     (1000) david     (1000)      646 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/smile.svg
--rw-r--r--   0 david     (1000) david     (1000)      793 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/smog.svg
--rw-r--r--   0 david     (1000) david     (1000)      918 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/smoking-ban.svg
--rw-r--r--   0 david     (1000) david     (1000)      988 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/smoking.svg
--rw-r--r--   0 david     (1000) david     (1000)     1379 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sms.svg
--rw-r--r--   0 david     (1000) david     (1000)     1183 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/snowboarding.svg
--rw-r--r--   0 david     (1000) david     (1000)     1737 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/snowflake.svg
--rw-r--r--   0 david     (1000) david     (1000)     1383 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/snowman.svg
--rw-r--r--   0 david     (1000) david     (1000)     1209 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/snowplow.svg
--rw-r--r--   0 david     (1000) david     (1000)      649 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/soap.svg
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/socks.svg
--rw-r--r--   0 david     (1000) david     (1000)      934 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/solar-panel.svg
--rw-r--r--   0 david     (1000) david     (1000)      882 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-alpha-down-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      879 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-alpha-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      877 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-alpha-up-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      876 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-alpha-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      797 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-amount-down-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      801 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-amount-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-amount-up-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-amount-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      359 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      889 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-numeric-down-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      886 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-numeric-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      885 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-numeric-up-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      883 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-numeric-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      360 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      458 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sort.svg
--rw-r--r--   0 david     (1000) david     (1000)      844 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/spa.svg
--rw-r--r--   0 david     (1000) david     (1000)      840 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/space-shuttle.svg
--rw-r--r--   0 david     (1000) david     (1000)      928 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/spell-check.svg
--rw-r--r--   0 david     (1000) david     (1000)     1718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/spider.svg
--rw-r--r--   0 david     (1000) david     (1000)      838 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/spinner.svg
--rw-r--r--   0 david     (1000) david     (1000)      745 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/splotch.svg
--rw-r--r--   0 david     (1000) david     (1000)      984 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/spray-can.svg
--rw-r--r--   0 david     (1000) david     (1000)      281 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/square-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      953 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/square-root-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      365 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/square.svg
--rw-r--r--   0 david     (1000) david     (1000)      672 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stamp.svg
--rw-r--r--   0 david     (1000) david     (1000)      973 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/star-and-crescent.svg
--rw-r--r--   0 david     (1000) david     (1000)      802 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/star-half-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      402 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/star-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      912 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/star-of-david.svg
--rw-r--r--   0 david     (1000) david     (1000)      820 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/star-of-life.svg
--rw-r--r--   0 david     (1000) david     (1000)      516 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/star.svg
--rw-r--r--   0 david     (1000) david     (1000)      442 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/step-backward.svg
--rw-r--r--   0 david     (1000) david     (1000)      443 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/step-forward.svg
--rw-r--r--   0 david     (1000) david     (1000)      888 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stethoscope.svg
--rw-r--r--   0 david     (1000) david     (1000)      447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sticky-note.svg
--rw-r--r--   0 david     (1000) david     (1000)      430 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stop-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      365 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stop.svg
--rw-r--r--   0 david     (1000) david     (1000)     1328 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stopwatch-20.svg
--rw-r--r--   0 david     (1000) david     (1000)      682 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stopwatch.svg
--rw-r--r--   0 david     (1000) david     (1000)      705 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/store-alt-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      554 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/store-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1054 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/store-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      825 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/store.svg
--rw-r--r--   0 david     (1000) david     (1000)      580 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stream.svg
--rw-r--r--   0 david     (1000) david     (1000)      852 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/street-view.svg
--rw-r--r--   0 david     (1000) david     (1000)      848 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/strikethrough.svg
--rw-r--r--   0 david     (1000) david     (1000)     2664 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/stroopwafel.svg
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/subscript.svg
--rw-r--r--   0 david     (1000) david     (1000)      880 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/subway.svg
--rw-r--r--   0 david     (1000) david     (1000)      756 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/suitcase-rolling.svg
--rw-r--r--   0 david     (1000) david     (1000)      479 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/suitcase.svg
--rw-r--r--   0 david     (1000) david     (1000)      847 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sun.svg
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/superscript.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/surprise.svg
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/swatchbook.svg
--rw-r--r--   0 david     (1000) david     (1000)     1494 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/swimmer.svg
--rw-r--r--   0 david     (1000) david     (1000)     1345 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/swimming-pool.svg
--rw-r--r--   0 david     (1000) david     (1000)      966 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/synagogue.svg
--rw-r--r--   0 david     (1000) david     (1000)     1022 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sync-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      887 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/sync.svg
--rw-r--r--   0 david     (1000) david     (1000)      970 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/syringe.svg
--rw-r--r--   0 david     (1000) david     (1000)      674 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/table-tennis.svg
--rw-r--r--   0 david     (1000) david     (1000)      463 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/table.svg
--rw-r--r--   0 david     (1000) david     (1000)      536 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tablet-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tablet.svg
--rw-r--r--   0 david     (1000) david     (1000)      746 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tablets.svg
--rw-r--r--   0 david     (1000) david     (1000)     1197 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tachometer-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      550 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tag.svg
--rw-r--r--   0 david     (1000) david     (1000)      810 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tags.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tape.svg
--rw-r--r--   0 david     (1000) david     (1000)      966 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tasks.svg
--rw-r--r--   0 david     (1000) david     (1000)      923 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/taxi.svg
--rw-r--r--   0 david     (1000) david     (1000)     1275 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/teeth-open.svg
--rw-r--r--   0 david     (1000) david     (1000)     1166 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/teeth.svg
--rw-r--r--   0 david     (1000) david     (1000)      833 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/temperature-high.svg
--rw-r--r--   0 david     (1000) david     (1000)      832 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/temperature-low.svg
--rw-r--r--   0 david     (1000) david     (1000)      509 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tenge.svg
--rw-r--r--   0 david     (1000) david     (1000)      661 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/terminal.svg
--rw-r--r--   0 david     (1000) david     (1000)      723 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/text-height.svg
--rw-r--r--   0 david     (1000) david     (1000)      723 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/text-width.svg
--rw-r--r--   0 david     (1000) david     (1000)      753 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/th-large.svg
--rw-r--r--   0 david     (1000) david     (1000)     1030 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/th-list.svg
--rw-r--r--   0 david     (1000) david     (1000)     1455 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/th.svg
--rw-r--r--   0 david     (1000) david     (1000)     1803 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/theater-masks.svg
--rw-r--r--   0 david     (1000) david     (1000)      786 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thermometer-empty.svg
--rw-r--r--   0 david     (1000) david     (1000)      860 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thermometer-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      865 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thermometer-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thermometer-quarter.svg
--rw-r--r--   0 david     (1000) david     (1000)      873 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thermometer-three-quarters.svg
--rw-r--r--   0 david     (1000) david     (1000)      688 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thermometer.svg
--rw-r--r--   0 david     (1000) david     (1000)     1059 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thumbs-down.svg
--rw-r--r--   0 david     (1000) david     (1000)     1066 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thumbs-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/thumbtack.svg
--rw-r--r--   0 david     (1000) david     (1000)      619 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/ticket-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/times-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/times.svg
--rw-r--r--   0 david     (1000) david     (1000)      720 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tint-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tint.svg
--rw-r--r--   0 david     (1000) david     (1000)      740 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tired.svg
--rw-r--r--   0 david     (1000) david     (1000)      598 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/toggle-off.svg
--rw-r--r--   0 david     (1000) david     (1000)      448 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/toggle-on.svg
--rw-r--r--   0 david     (1000) david     (1000)      851 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/toilet-paper-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      907 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/toilet-paper.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/toilet.svg
--rw-r--r--   0 david     (1000) david     (1000)      813 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/toolbox.svg
--rw-r--r--   0 david     (1000) david     (1000)      951 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tools.svg
--rw-r--r--   0 david     (1000) david     (1000)      971 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tooth.svg
--rw-r--r--   0 david     (1000) david     (1000)     1122 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/torah.svg
--rw-r--r--   0 david     (1000) david     (1000)      656 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/torii-gate.svg
--rw-r--r--   0 david     (1000) david     (1000)     1466 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tractor.svg
--rw-r--r--   0 david     (1000) david     (1000)      914 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trademark.svg
--rw-r--r--   0 david     (1000) david     (1000)      829 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/traffic-light.svg
--rw-r--r--   0 david     (1000) david     (1000)      863 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trailer.svg
--rw-r--r--   0 david     (1000) david     (1000)      685 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/train.svg
--rw-r--r--   0 david     (1000) david     (1000)      752 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tram.svg
--rw-r--r--   0 david     (1000) david     (1000)     1055 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/transgender-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      745 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/transgender.svg
--rw-r--r--   0 david     (1000) david     (1000)      619 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trash-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      668 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trash-restore-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      680 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trash-restore.svg
--rw-r--r--   0 david     (1000) david     (1000)      494 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trash.svg
--rw-r--r--   0 david     (1000) david     (1000)      885 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tree.svg
--rw-r--r--   0 david     (1000) david     (1000)      840 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/trophy.svg
--rw-r--r--   0 david     (1000) david     (1000)      714 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/truck-loading.svg
--rw-r--r--   0 david     (1000) david     (1000)     2510 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/truck-monster.svg
--rw-r--r--   0 david     (1000) david     (1000)      892 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/truck-moving.svg
--rw-r--r--   0 david     (1000) david     (1000)      899 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/truck-pickup.svg
--rw-r--r--   0 david     (1000) david     (1000)      704 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/truck.svg
--rw-r--r--   0 david     (1000) david     (1000)      580 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tshirt.svg
--rw-r--r--   0 david     (1000) david     (1000)     2005 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tty.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/tv.svg
--rw-r--r--   0 david     (1000) david     (1000)      849 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/umbrella-beach.svg
--rw-r--r--   0 david     (1000) david     (1000)      819 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/umbrella.svg
--rw-r--r--   0 david     (1000) david     (1000)      613 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/underline.svg
--rw-r--r--   0 david     (1000) david     (1000)      804 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/undo-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      799 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/undo.svg
--rw-r--r--   0 david     (1000) david     (1000)     1249 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/universal-access.svg
--rw-r--r--   0 david     (1000) david     (1000)      666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/university.svg
--rw-r--r--   0 david     (1000) david     (1000)     1254 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/unlink.svg
--rw-r--r--   0 david     (1000) david     (1000)      622 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/unlock-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      535 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/unlock.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/upload.svg
--rw-r--r--   0 david     (1000) david     (1000)      584 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-alt-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      504 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      967 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-astronaut.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-check.svg
--rw-r--r--   0 david     (1000) david     (1000)      614 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-clock.svg
--rw-r--r--   0 david     (1000) david     (1000)     1562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-cog.svg
--rw-r--r--   0 david     (1000) david     (1000)      752 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-edit.svg
--rw-r--r--   0 david     (1000) david     (1000)      763 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-friends.svg
--rw-r--r--   0 david     (1000) david     (1000)      799 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-graduate.svg
--rw-r--r--   0 david     (1000) david     (1000)      938 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-injured.svg
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-lock.svg
--rw-r--r--   0 david     (1000) david     (1000)     1037 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-md.svg
--rw-r--r--   0 david     (1000) david     (1000)      617 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      665 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-ninja.svg
--rw-r--r--   0 david     (1000) david     (1000)      785 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-nurse.svg
--rw-r--r--   0 david     (1000) david     (1000)      721 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1094 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-secret.svg
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-shield.svg
--rw-r--r--   0 david     (1000) david     (1000)      583 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      848 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-tag.svg
--rw-r--r--   0 david     (1000) david     (1000)      511 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-tie.svg
--rw-r--r--   0 david     (1000) david     (1000)      846 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user-times.svg
--rw-r--r--   0 david     (1000) david     (1000)      516 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/user.svg
--rw-r--r--   0 david     (1000) david     (1000)     1816 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/users-cog.svg
--rw-r--r--   0 david     (1000) david     (1000)     1042 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/users-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      904 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/users.svg
--rw-r--r--   0 david     (1000) david     (1000)      477 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/utensil-spoon.svg
--rw-r--r--   0 david     (1000) david     (1000)      764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/utensils.svg
--rw-r--r--   0 david     (1000) david     (1000)      812 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vector-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1005 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/venus-double.svg
--rw-r--r--   0 david     (1000) david     (1000)     1015 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/venus-mars.svg
--rw-r--r--   0 david     (1000) david     (1000)      589 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/venus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1201 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vest-patches.svg
--rw-r--r--   0 david     (1000) david     (1000)      908 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vest.svg
--rw-r--r--   0 david     (1000) david     (1000)      556 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vial.svg
--rw-r--r--   0 david     (1000) david     (1000)      656 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vials.svg
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/video-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/video.svg
--rw-r--r--   0 david     (1000) david     (1000)      861 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vihara.svg
--rw-r--r--   0 david     (1000) david     (1000)     1234 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/virus-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      982 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/virus.svg
--rw-r--r--   0 david     (1000) david     (1000)     1608 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/viruses.svg
--rw-r--r--   0 david     (1000) david     (1000)      435 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/voicemail.svg
--rw-r--r--   0 david     (1000) david     (1000)     1015 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/volleyball-ball.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/volume-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      799 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/volume-mute.svg
--rw-r--r--   0 david     (1000) david     (1000)      376 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/volume-off.svg
--rw-r--r--   0 david     (1000) david     (1000)     1238 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/volume-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vote-yea.svg
--rw-r--r--   0 david     (1000) david     (1000)      682 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/vr-cardboard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1041 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/walking.svg
--rw-r--r--   0 david     (1000) david     (1000)      550 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wallet.svg
--rw-r--r--   0 david     (1000) david     (1000)      789 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/warehouse.svg
--rw-r--r--   0 david     (1000) david     (1000)     1517 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/water.svg
--rw-r--r--   0 david     (1000) david     (1000)      508 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wave-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/weight-hanging.svg
--rw-r--r--   0 david     (1000) david     (1000)      769 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/weight.svg
--rw-r--r--   0 david     (1000) david     (1000)     1033 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wheelchair.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wifi.svg
--rw-r--r--   0 david     (1000) david     (1000)     1086 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wind.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/window-close.svg
--rw-r--r--   0 david     (1000) david     (1000)      426 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/window-maximize.svg
--rw-r--r--   0 david     (1000) david     (1000)      368 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/window-minimize.svg
--rw-r--r--   0 david     (1000) david     (1000)      545 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/window-restore.svg
--rw-r--r--   0 david     (1000) david     (1000)      702 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wine-bottle.svg
--rw-r--r--   0 david     (1000) david     (1000)      575 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wine-glass-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wine-glass.svg
--rw-r--r--   0 david     (1000) david     (1000)     1152 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/won-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/wrench.svg
--rw-r--r--   0 david     (1000) david     (1000)     1054 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/x-ray.svg
--rw-r--r--   0 david     (1000) david     (1000)      762 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/yen-sign.svg
--rw-r--r--   0 david     (1000) david     (1000)      626 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/svgs/solid/yin-yang.svg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.750535 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/
--rw-r--r--   0 david     (1000) david     (1000)   134346 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 david     (1000) david     (1000)   747545 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 david     (1000) david     (1000)   134040 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 david     (1000) david     (1000)    90060 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 david     (1000) david     (1000)    76764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 david     (1000) david     (1000)    34034 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 david     (1000) david     (1000)   144714 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 david     (1000) david     (1000)    33736 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 david     (1000) david     (1000)    16276 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 david     (1000) david     (1000)    13276 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 david     (1000) david     (1000)   203030 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 david     (1000) david     (1000)   918991 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 david     (1000) david     (1000)   202744 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 david     (1000) david     (1000)   101652 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 david     (1000) david     (1000)    78196 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/font-awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.750535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/
--rw-r--r--   0 david     (1000) david     (1000)    28151 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.all-contributorsrc
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.450535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.github/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.750535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 david     (1000) david     (1000)      571 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.github/ISSUE_TEMPLATE/Icon_request.md
--rw-r--r--   0 david     (1000) david     (1000)      114 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)      252 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.npmignore
--rw-r--r--   0 david     (1000) david     (1000)      433 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/.travis.yml
--rw-r--r--   0 david     (1000) david     (1000)     5714 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/CHANGELOG.md
--rw-r--r--   0 david     (1000) david     (1000)     6290 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/CONTRIBUTING.md
--rw-r--r--   0 david     (1000) david     (1000)    31461 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/CONTRIBUTORS.md
--rw-r--r--   0 david     (1000) david     (1000)      167 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/Gemfile
--rw-r--r--   0 david     (1000) david     (1000)     1765 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/Gemfile.lock
--rw-r--r--   0 david     (1000) david     (1000)    25608 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/LICENSES
--rw-r--r--   0 david     (1000) david     (1000)     5065 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/README.md
--rw-r--r--   0 david     (1000) david     (1000)      134 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/_config-deploy.yml
--rw-r--r--   0 david     (1000) david     (1000)     1729 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/_config.yml
--rw-r--r--   0 david     (1000) david     (1000)      457 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/bower.json
--rw-r--r--   0 david     (1000) david     (1000)      470 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/component.json
--rw-r--r--   0 david     (1000) david     (1000)      683 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/composer.json
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.750535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/
--rw-r--r--   0 david     (1000) david     (1000)    41914 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/fork-awesome.css
--rw-r--r--   0 david     (1000) david     (1000)    34942 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/fork-awesome.min.css
--rw-r--r--   0 david     (1000) david     (1000)    14404 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/fork-awesome.min.css.map
--rw-r--r--   0 david     (1000) david     (1000)     8537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/v5-compat.css
--rw-r--r--   0 david     (1000) david     (1000)     7422 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/v5-compat.min.css
--rw-r--r--   0 david     (1000) david     (1000)     2616 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/css/v5-compat.min.css.map
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.750535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/fonts/
--rw-r--r--   0 david     (1000) david     (1000)   188946 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/fonts/forkawesome-webfont.eot
--rw-r--r--   0 david     (1000) david     (1000)   480784 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/fonts/forkawesome-webfont.svg
--rw-r--r--   0 david     (1000) david     (1000)   188756 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/fonts/forkawesome-webfont.ttf
--rw-r--r--   0 david     (1000) david     (1000)   115148 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/fonts/forkawesome-webfont.woff
--rw-r--r--   0 david     (1000) david     (1000)    91624 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/fonts/forkawesome-webfont.woff2
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/
--rw-r--r--   0 david     (1000) david     (1000)      815 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/animated.less
--rw-r--r--   0 david     (1000) david     (1000)      585 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/bordered-pulled.less
--rw-r--r--   0 david     (1000) david     (1000)      456 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/core.less
--rw-r--r--   0 david     (1000) david     (1000)      119 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/fixed-width.less
--rw-r--r--   0 david     (1000) david     (1000)     1475 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/fork-awesome.less
--rw-r--r--   0 david     (1000) david     (1000)    54986 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/icons.less
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/larger.less
--rw-r--r--   0 david     (1000) david     (1000)      377 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/list.less
--rw-r--r--   0 david     (1000) david     (1000)     1607 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/mixins.less
--rw-r--r--   0 david     (1000) david     (1000)      777 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/path.less
--rw-r--r--   0 david     (1000) david     (1000)      622 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/rotated-flipped.less
--rw-r--r--   0 david     (1000) david     (1000)      118 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/screen-reader.less
--rw-r--r--   0 david     (1000) david     (1000)      476 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/stacked.less
--rw-r--r--   0 david     (1000) david     (1000)    10455 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/v5-compat.less
--rw-r--r--   0 david     (1000) david     (1000)    24947 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/less/variables.less
--rw-r--r--   0 david     (1000) david     (1000)    63892 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/package-lock.json
--rw-r--r--   0 david     (1000) david     (1000)     1278 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/package.json
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/
--rw-r--r--   0 david     (1000) david     (1000)      805 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_animated.scss
--rw-r--r--   0 david     (1000) david     (1000)      592 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 david     (1000) david     (1000)      466 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_core.scss
--rw-r--r--   0 david     (1000) david     (1000)      120 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_fixed-width.scss
--rw-r--r--   0 david     (1000) david     (1000)      349 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_functions.scss
--rw-r--r--   0 david     (1000) david     (1000)    55862 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_icons.scss
--rw-r--r--   0 david     (1000) david     (1000)      375 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_larger.scss
--rw-r--r--   0 david     (1000) david     (1000)      378 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_list.scss
--rw-r--r--   0 david     (1000) david     (1000)     1644 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_mixins.scss
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_path.scss
--rw-r--r--   0 david     (1000) david     (1000)      672 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 david     (1000) david     (1000)      134 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_screen-reader.scss
--rw-r--r--   0 david     (1000) david     (1000)      482 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_stacked.scss
--rw-r--r--   0 david     (1000) david     (1000)    25032 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/_variables.scss
--rw-r--r--   0 david     (1000) david     (1000)     1431 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/scss/fork-awesome.scss
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.450535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/
--rw-r--r--   0 david     (1000) david     (1000)     2696 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/Makefile
--rw-r--r--   0 david     (1000) david     (1000)     5214 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/README.md-nobuild
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/accessibility/
--rw-r--r--   0 david     (1000) david     (1000)     6050 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/accessibility/accessibility-manual.html
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/accessibility/background.html
--rw-r--r--   0 david     (1000) david     (1000)     1285 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/accessibility/other.html
--rw-r--r--   0 david     (1000) david     (1000)      454 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/brand-adblock-warning.html
--rw-r--r--   0 david     (1000) david     (1000)      491 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/brand-license.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/code/
--rw-r--r--   0 david     (1000) david     (1000)      378 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/code/core.less
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/code/core.scss
--rw-r--r--   0 david     (1000) david     (1000)     1216 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/code/license.css
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.760535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/community/
--rw-r--r--   0 david     (1000) david     (1000)      870 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/community/getting-support.html
--rw-r--r--   0 david     (1000) david     (1000)      317 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/community/project-milestones.html
--rw-r--r--   0 david     (1000) david     (1000)      841 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/community/reporting-bugs.html
--rw-r--r--   0 david     (1000) david     (1000)     1503 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/community/requesting-new-icons.html
--rw-r--r--   0 david     (1000) david     (1000)      613 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/community/submitting-pull-requests.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/
--rw-r--r--   0 david     (1000) david     (1000)     3814 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/accessible.html
--rw-r--r--   0 david     (1000) david     (1000)     2870 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/animated.html
--rw-r--r--   0 david     (1000) david     (1000)     1735 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/basic.html
--rw-r--r--   0 david     (1000) david     (1000)     4438 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/bootstrap.html
--rw-r--r--   0 david     (1000) david     (1000)     1514 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/bordered-pulled.html
--rw-r--r--   0 david     (1000) david     (1000)      625 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/custom.html
--rw-r--r--   0 david     (1000) david     (1000)     1944 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/fixed-width.html
--rw-r--r--   0 david     (1000) david     (1000)     1907 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/larger.html
--rw-r--r--   0 david     (1000) david     (1000)     1417 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/list.html
--rw-r--r--   0 david     (1000) david     (1000)     1864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/rotated-flipped.html
--rw-r--r--   0 david     (1000) david     (1000)     2706 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/examples/stacked.html
--rw-r--r--   0 david     (1000) david     (1000)     1319 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/footer.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/
--rw-r--r--   0 david     (1000) david     (1000)      615 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/accessibility.html
--rw-r--r--   0 david     (1000) david     (1000)      775 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/brand.html
--rw-r--r--   0 david     (1000) david     (1000)      585 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/chart.html
--rw-r--r--   0 david     (1000) david     (1000)      600 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/currency.html
--rw-r--r--   0 david     (1000) david     (1000)      615 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/directional.html
--rw-r--r--   0 david     (1000) david     (1000)      605 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/file-type.html
--rw-r--r--   0 david     (1000) david     (1000)      619 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/form-control.html
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/gender.html
--rw-r--r--   0 david     (1000) david     (1000)      580 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/hand.html
--rw-r--r--   0 david     (1000) david     (1000)      595 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/medical.html
--rw-r--r--   0 david     (1000) david     (1000)      982 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/new.html
--rw-r--r--   0 david     (1000) david     (1000)      595 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/payment.html
--rw-r--r--   0 david     (1000) david     (1000)     1006 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/spinner.html
--rw-r--r--   0 david     (1000) david     (1000)      615 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/text-editor.html
--rw-r--r--   0 david     (1000) david     (1000)      630 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/transportation.html
--rw-r--r--   0 david     (1000) david     (1000)      620 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/video-player.html
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/icons/web-application.html
--rw-r--r--   0 david     (1000) david     (1000)     3154 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/jumbotron-carousel.html
--rw-r--r--   0 david     (1000) david     (1000)      382 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/jumbotron.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/modals/
--rw-r--r--   0 david     (1000) david     (1000)     1231 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/modals/download.html
--rw-r--r--   0 david     (1000) david     (1000)     7490 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/navbar.html
--rw-r--r--   0 david     (1000) david     (1000)     1549 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/new-features.html
--rw-r--r--   0 david     (1000) david     (1000)     5308 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/new-naming.html
--rw-r--r--   0 david     (1000) david     (1000)     1173 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/new-upgrading.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/
--rw-r--r--   0 david     (1000) david     (1000)     1442 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/camera-retro-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     1429 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/classics-tee.html
--rw-r--r--   0 david     (1000) david     (1000)      755 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/cta-suggestions.html
--rw-r--r--   0 david     (1000) david     (1000)     1328 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/fa-ther-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     1440 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/green-logo-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     1431 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/old-skool-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     1134 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/rock-paper-scissors-lizard-spock-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     1403 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/space-shuttle-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     1735 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/products/white-logo-tee.html
--rw-r--r--   0 david     (1000) david     (1000)     2195 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/stripe-social.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/
--rw-r--r--   0 david     (1000) david     (1000)      589 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/rotated-flipped-inside-anchor.html
--rw-r--r--   0 david     (1000) david     (1000)      733 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/rotated-flipped-inside-btn.html
--rw-r--r--   0 david     (1000) david     (1000)      493 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/rotated-flipped.html
--rw-r--r--   0 david     (1000) david     (1000)     1842 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/stacked-inside-anchor.html
--rw-r--r--   0 david     (1000) david     (1000)      151 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/stacked-with-text.html
--rw-r--r--   0 david     (1000) david     (1000)     1818 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/tests/stacked.html
--rw-r--r--   0 david     (1000) david     (1000)      951 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/thanks-to.html
--rw-r--r--   0 david     (1000) david     (1000)     2419 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_includes/why.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_layouts/
--rw-r--r--   0 david     (1000) david     (1000)     2807 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_layouts/base.html
--rw-r--r--   0 david     (1000) david     (1000)     3399 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_layouts/icon.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_plugins/
--rw-r--r--   0 david     (1000) david     (1000)      488 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_plugins/all-contributors-generator.rb
--rw-r--r--   0 david     (1000) david     (1000)      998 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_plugins/flatten_icon_filters.rb
--rw-r--r--   0 david     (1000) david     (1000)      895 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_plugins/icon_page_generator.rb
--rw-r--r--   0 david     (1000) david     (1000)     2978 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_plugins/site.rb
--rw-r--r--   0 david     (1000) david     (1000)      369 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/_plugins/sri_hash.rb
--rw-r--r--   0 david     (1000) david     (1000)     1156 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/accessibility.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.450535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/css/
--rw-r--r--   0 david     (1000) david     (1000)      815 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/css/prettify.css
--rw-r--r--   0 david     (1000) david     (1000)     3063 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/css/pygments.css
--rw-r--r--   0 david     (1000) david     (1000)     3150 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/css/share.min.css
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.450535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.770536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/
--rw-r--r--   0 david     (1000) david     (1000)      823 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/animated.less
--rw-r--r--   0 david     (1000) david     (1000)      594 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/bordered-pulled.less
--rw-r--r--   0 david     (1000) david     (1000)      115 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/core.less
--rw-r--r--   0 david     (1000) david     (1000)      128 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/fixed-width.less
--rw-r--r--   0 david     (1000) david     (1000)      368 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/fork-awesome.less
--rw-r--r--   0 david     (1000) david     (1000)      357 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/icons.less
--rw-r--r--   0 david     (1000) david     (1000)      379 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/larger.less
--rw-r--r--   0 david     (1000) david     (1000)      386 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/list.less
--rw-r--r--   0 david     (1000) david     (1000)     1265 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/mixins.less
--rw-r--r--   0 david     (1000) david     (1000)      777 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/path.less
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/rotated-flipped.less
--rw-r--r--   0 david     (1000) david     (1000)      118 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/screen-reader.less
--rw-r--r--   0 david     (1000) david     (1000)      485 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/stacked.less
--rw-r--r--   0 david     (1000) david     (1000)     8998 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/v5-compat.less
--rw-r--r--   0 david     (1000) david     (1000)      562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/less/variables.less
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.780536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/
--rw-r--r--   0 david     (1000) david     (1000)      813 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/animated.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      601 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/bordered-pulled.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      116 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/core.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      129 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/fixed-width.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      324 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/fork-awesome.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      357 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/functions.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      344 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/icons.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      384 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/larger.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/list.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)     1293 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/mixins.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/path.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      681 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/rotated-flipped.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      134 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/screen-reader.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      491 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/stacked.scss.txt
--rw-r--r--   0 david     (1000) david     (1000)      647 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/fork-awesome/scss/variables.scss.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.780536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/ico/
--rw-r--r--   0 david     (1000) david     (1000)   107730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/ico/favicon.ico
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.780536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/images/
--rw-r--r--   0 david     (1000) david     (1000)    69877 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/images/banner.jpg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.780536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/
--rw-r--r--   0 david     (1000) david     (1000)     8400 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/ZeroClipboard-1.1.7.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/ZeroClipboard-1.1.7.swf
--rw-r--r--   0 david     (1000) david     (1000)     2376 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/html5shiv.js
--rw-r--r--   0 david     (1000) david     (1000)    20740 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/monetization.js
--rw-r--r--   0 david     (1000) david     (1000)    13632 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/prettify.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4035 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/respond.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3080 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/search.js
--rw-r--r--   0 david     (1000) david     (1000)     1341 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/share.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/js/site.js
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.780536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.790536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/
--rw-r--r--   0 david     (1000) david     (1000)     8099 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/.csscomb.json
--rw-r--r--   0 david     (1000) david     (1000)      456 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/.csslintrc
--rw-r--r--   0 david     (1000) david     (1000)     1518 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/alerts.less
--rw-r--r--   0 david     (1000) david     (1000)     1199 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/badges.less
--rw-r--r--   0 david     (1000) david     (1000)     1291 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/bootstrap.less
--rw-r--r--   0 david     (1000) david     (1000)      594 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/breadcrumbs.less
--rw-r--r--   0 david     (1000) david     (1000)     5675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/button-groups.less
--rw-r--r--   0 david     (1000) david     (1000)     3662 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/buttons.less
--rw-r--r--   0 david     (1000) david     (1000)     5407 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/carousel.less
--rw-r--r--   0 david     (1000) david     (1000)      764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/close.less
--rw-r--r--   0 david     (1000) david     (1000)     1401 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/code.less
--rw-r--r--   0 david     (1000) david     (1000)      666 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/component-animations.less
--rw-r--r--   0 david     (1000) david     (1000)     4876 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/dropdowns.less
--rw-r--r--   0 david     (1000) david     (1000)    15859 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/forms.less
--rw-r--r--   0 david     (1000) david     (1000)    19803 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/glyphicons.less
--rw-r--r--   0 david     (1000) david     (1000)     1387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/grid.less
--rw-r--r--   0 david     (1000) david     (1000)     4246 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/input-groups.less
--rw-r--r--   0 david     (1000) david     (1000)     1062 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/jumbotron.less
--rw-r--r--   0 david     (1000) david     (1000)     1079 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/labels.less
--rw-r--r--   0 david     (1000) david     (1000)     3124 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/list-group.less
--rw-r--r--   0 david     (1000) david     (1000)      900 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/media.less
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.790536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/
--rw-r--r--   0 david     (1000) david     (1000)      257 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/alerts.less
--rw-r--r--   0 david     (1000) david     (1000)      151 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/background-variant.less
--rw-r--r--   0 david     (1000) david     (1000)      468 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/border-radius.less
--rw-r--r--   0 david     (1000) david     (1000)     1476 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/buttons.less
--rw-r--r--   0 david     (1000) david     (1000)      120 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/center-block.less
--rw-r--r--   0 david     (1000) david     (1000)      605 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/clearfix.less
--rw-r--r--   0 david     (1000) david     (1000)     2641 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/forms.less
--rw-r--r--   0 david     (1000) david     (1000)     4388 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/gradients.less
--rw-r--r--   0 david     (1000) david     (1000)     2797 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/grid-framework.less
--rw-r--r--   0 david     (1000) david     (1000)     3107 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/grid.less
--rw-r--r--   0 david     (1000) david     (1000)      574 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/hide-text.less
--rw-r--r--   0 david     (1000) david     (1000)     1062 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/image.less
--rw-r--r--   0 david     (1000) david     (1000)      161 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/labels.less
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/list-group.less
--rw-r--r--   0 david     (1000) david     (1000)      232 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/nav-divider.less
--rw-r--r--   0 david     (1000) david     (1000)      364 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/nav-vertical-align.less
--rw-r--r--   0 david     (1000) david     (1000)      148 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/opacity.less
--rw-r--r--   0 david     (1000) david     (1000)      485 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/pagination.less
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/panels.less
--rw-r--r--   0 david     (1000) david     (1000)      191 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/progress-bar.less
--rw-r--r--   0 david     (1000) david     (1000)      248 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/reset-filter.less
--rw-r--r--   0 david     (1000) david     (1000)      470 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/reset-text.less
--rw-r--r--   0 david     (1000) david     (1000)      196 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/resize.less
--rw-r--r--   0 david     (1000) david     (1000)      354 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/responsive-visibility.less
--rw-r--r--   0 david     (1000) david     (1000)      127 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/size.less
--rw-r--r--   0 david     (1000) david     (1000)      159 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/tab-focus.less
--rw-r--r--   0 david     (1000) david     (1000)      700 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/table-row.less
--rw-r--r--   0 david     (1000) david     (1000)      128 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/text-emphasis.less
--rw-r--r--   0 david     (1000) david     (1000)      162 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/text-overflow.less
--rw-r--r--   0 david     (1000) david     (1000)     6650 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins/vendor-prefixes.less
--rw-r--r--   0 david     (1000) david     (1000)     1136 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/mixins.less
--rw-r--r--   0 david     (1000) david     (1000)     3565 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/modals.less
--rw-r--r--   0 david     (1000) david     (1000)    14628 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/navbar.less
--rw-r--r--   0 david     (1000) david     (1000)     4930 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/navs.less
--rw-r--r--   0 david     (1000) david     (1000)     7559 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/normalize.less
--rw-r--r--   0 david     (1000) david     (1000)      861 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/pager.less
--rw-r--r--   0 david     (1000) david     (1000)     2059 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/pagination.less
--rw-r--r--   0 david     (1000) david     (1000)     6279 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/panels.less
--rw-r--r--   0 david     (1000) david     (1000)     3488 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/popovers.less
--rw-r--r--   0 david     (1000) david     (1000)     1939 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/print.less
--rw-r--r--   0 david     (1000) david     (1000)     1925 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/progress-bars.less
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/responsive-embed.less
--rw-r--r--   0 david     (1000) david     (1000)     4262 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/responsive-utilities.less
--rw-r--r--   0 david     (1000) david     (1000)     2988 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/scaffolding.less
--rw-r--r--   0 david     (1000) david     (1000)     4612 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/tables.less
--rw-r--r--   0 david     (1000) david     (1000)     8197 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/theme.less
--rw-r--r--   0 david     (1000) david     (1000)      753 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/thumbnails.less
--rw-r--r--   0 david     (1000) david     (1000)     2985 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/tooltip.less
--rw-r--r--   0 david     (1000) david     (1000)     5954 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/type.less
--rw-r--r--   0 david     (1000) david     (1000)      747 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/utilities.less
--rw-r--r--   0 david     (1000) david     (1000)    27473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/variables.less
--rw-r--r--   0 david     (1000) david     (1000)      527 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/bootstrap-3.3.5/wells.less
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.790536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/gandy-grid/
--rw-r--r--   0 david     (1000) david     (1000)      920 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/gandy-grid/grid.less
--rw-r--r--   0 david     (1000) david     (1000)      287 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/gandy-grid/mixins.less
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.790536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.790536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/
--rw-r--r--   0 david     (1000) david     (1000)      335 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/alerts.less
--rw-r--r--   0 david     (1000) david     (1000)      208 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/buttons.less
--rw-r--r--   0 david     (1000) david     (1000)     1972 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/jumbotron.less
--rw-r--r--   0 david     (1000) david     (1000)      284 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/labels.less
--rw-r--r--   0 david     (1000) david     (1000)      133 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/modals.less
--rw-r--r--   0 david     (1000) david     (1000)     4172 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/navbar.less
--rw-r--r--   0 david     (1000) david     (1000)      213 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/panels.less
--rw-r--r--   0 david     (1000) david     (1000)      119 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/tooltip.less
--rw-r--r--   0 david     (1000) david     (1000)      414 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/type.less
--rw-r--r--   0 david     (1000) david     (1000)     4873 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/variables.less
--rw-r--r--   0 david     (1000) david     (1000)      232 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/bootstrap/wells.less
--rw-r--r--   0 david     (1000) david     (1000)      481 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/example-rating.less
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/feature-list.less
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/fontawesome-icon-list.less
--rw-r--r--   0 david     (1000) david     (1000)     1180 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/footer.less
--rw-r--r--   0 david     (1000) david     (1000)     1810 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/jumbotron-carousel.less
--rw-r--r--   0 david     (1000) david     (1000)       30 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/layout.less
--rw-r--r--   0 david     (1000) david     (1000)     4864 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/lazy.less
--rw-r--r--   0 david     (1000) david     (1000)       62 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/print.less
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.790536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/responsive/
--rw-r--r--   0 david     (1000) david     (1000)      918 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/responsive/screen-lg.less
--rw-r--r--   0 david     (1000) david     (1000)       97 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/responsive/screen-md.less
--rw-r--r--   0 david     (1000) david     (1000)      327 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/responsive/screen-sm-up.less
--rw-r--r--   0 david     (1000) david     (1000)      874 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/responsive/screen-sm.less
--rw-r--r--   0 david     (1000) david     (1000)     1764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/responsive/screen-xs.less
--rw-r--r--   0 david     (1000) david     (1000)      781 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/social-buttons.less
--rw-r--r--   0 david     (1000) david     (1000)       68 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/stripe-ad.less
--rw-r--r--   0 david     (1000) david     (1000)    12164 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/textured-bg.less
--rw-r--r--   0 david     (1000) david     (1000)      896 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site/views.less
--rw-r--r--   0 david     (1000) david     (1000)      988 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/assets/less/site.less
--rw-r--r--   0 david     (1000) david     (1000)     1504 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/cheatsheet.html
--rw-r--r--   0 david     (1000) david     (1000)      689 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/community.html
--rw-r--r--   0 david     (1000) david     (1000)       55 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/design.html
--rw-r--r--   0 david     (1000) david     (1000)     1687 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/examples.html
--rw-r--r--   0 david     (1000) david     (1000)     7263 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/get-started.html
--rw-r--r--   0 david     (1000) david     (1000)     1115 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/icons.html
--rw-r--r--   0 david     (1000) david     (1000)      318 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/index.html
--rw-r--r--   0 david     (1000) david     (1000)     2270 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/license.html
--rw-r--r--   0 david     (1000) david     (1000)     2517 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/store.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.800536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/
--rw-r--r--   0 david     (1000) david     (1000)     1148 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/all.html
--rw-r--r--   0 david     (1000) david     (1000)     1102 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/cdn.html
--rw-r--r--   0 david     (1000) david     (1000)    36075 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/glyphicons.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.800536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/height/
--rw-r--r--   0 david     (1000) david     (1000)     2281 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/height/current.html
--rw-r--r--   0 david     (1000) david     (1000)    36410 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/index.html
--rw-r--r--   0 david     (1000) david     (1000)    79480 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/test/v5.html
--rw-r--r--   0 david     (1000) david     (1000)     1065 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/thanks.html
--rw-r--r--   0 david     (1000) david     (1000)     1941 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/doc/whats-new.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.800536 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/
--rw-r--r--   0 david     (1000) david     (1000)    67094 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/.fontcustom-manifest.json
--rw-r--r--   0 david     (1000) david     (1000)      847 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/Makefile
--rw-r--r--   0 david     (1000) david     (1000)      439 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/fontcustom.yml
--rw-r--r--   0 david     (1000) david     (1000)     3884 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/icon-template-inkscape.svg
--rw-r--r--   0 david     (1000) david     (1000)   135299 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/icons.yml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.910535 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/
--rw-r--r--   0 david     (1000) david     (1000)     1775 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/500px.svg
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/activitypub.svg
--rw-r--r--   0 david     (1000) david     (1000)      659 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/address-book-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/address-book.svg
--rw-r--r--   0 david     (1000) david     (1000)      888 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/address-card-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/address-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      221 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/adjust.svg
--rw-r--r--   0 david     (1000) david     (1000)      233 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/adn.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/align-center.svg
--rw-r--r--   0 david     (1000) david     (1000)      465 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/align-justify.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/align-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      468 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/align-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/amazon.svg
--rw-r--r--   0 david     (1000) david     (1000)      756 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ambulance.svg
--rw-r--r--   0 david     (1000) david     (1000)     1432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/american-sign-language-interpreting.svg
--rw-r--r--   0 david     (1000) david     (1000)      667 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/anchor.svg
--rw-r--r--   0 david     (1000) david     (1000)      756 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/android.svg
--rw-r--r--   0 david     (1000) david     (1000)     1275 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angellist.svg
--rw-r--r--   0 david     (1000) david     (1000)      488 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-double-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      484 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-double-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      485 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-double-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      498 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-double-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      292 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      288 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      293 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      297 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/angle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      642 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/apple.svg
--rw-r--r--   0 david     (1000) david     (1000)     3121 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/archive-org.svg
--rw-r--r--   0 david     (1000) david     (1000)      363 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/archive.svg
--rw-r--r--   0 david     (1000) david     (1000)      782 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/archlinux.svg
--rw-r--r--   0 david     (1000) david     (1000)      169 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/area-chart.svg
--rw-r--r--   0 david     (1000) david     (1000)      436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      416 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-o-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      412 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-o-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      418 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-o-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-o-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      433 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-circle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      356 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      360 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      363 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrow-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      634 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrows-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      360 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrows-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      356 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrows-v.svg
--rw-r--r--   0 david     (1000) david     (1000)      633 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/arrows.svg
--rw-r--r--   0 david     (1000) david     (1000)      612 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/artstation.svg
--rw-r--r--   0 david     (1000) david     (1000)     1077 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/assistive-listening-systems.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/asterisk.svg
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/at.svg
--rw-r--r--   0 david     (1000) david     (1000)     2393 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/att.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/audio-description.svg
--rw-r--r--   0 david     (1000) david     (1000)      259 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/backward.svg
--rw-r--r--   0 david     (1000) david     (1000)      715 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/balance-scale.svg
--rw-r--r--   0 david     (1000) david     (1000)      337 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ban.svg
--rw-r--r--   0 david     (1000) david     (1000)      200 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bandcamp.svg
--rw-r--r--   0 david     (1000) david     (1000)      232 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bar-chart.svg
--rw-r--r--   0 david     (1000) david     (1000)      408 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/barcode.svg
--rw-r--r--   0 david     (1000) david     (1000)      373 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bars.svg
--rw-r--r--   0 david     (1000) david     (1000)     1542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bath.svg
--rw-r--r--   0 david     (1000) david     (1000)      359 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/battery-empty.svg
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/battery-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/battery-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/battery-quarter.svg
--rw-r--r--   0 david     (1000) david     (1000)      386 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/battery-three-quarters.svg
--rw-r--r--   0 david     (1000) david     (1000)      340 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bed.svg
--rw-r--r--   0 david     (1000) david     (1000)      245 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/beer.svg
--rw-r--r--   0 david     (1000) david     (1000)      661 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/behance-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      569 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/behance.svg
--rw-r--r--   0 david     (1000) david     (1000)      447 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bell-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      690 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bell-slash-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      553 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bell-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      545 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bell.svg
--rw-r--r--   0 david     (1000) david     (1000)      831 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bicycle.svg
--rw-r--r--   0 david     (1000) david     (1000)      435 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/binoculars.svg
--rw-r--r--   0 david     (1000) david     (1000)      511 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/biometric.svg
--rw-r--r--   0 david     (1000) david     (1000)      912 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/birthday-cake.svg
--rw-r--r--   0 david     (1000) david     (1000)      845 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bitbucket-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      771 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bitbucket.svg
--rw-r--r--   0 david     (1000) david     (1000)      170 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/black-tie.svg
--rw-r--r--   0 david     (1000) david     (1000)      738 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/blind.svg
--rw-r--r--   0 david     (1000) david     (1000)      236 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bluetooth-b.svg
--rw-r--r--   0 david     (1000) david     (1000)      319 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bluetooth.svg
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bold.svg
--rw-r--r--   0 david     (1000) david     (1000)      343 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bolt.svg
--rw-r--r--   0 david     (1000) david     (1000)      867 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bomb.svg
--rw-r--r--   0 david     (1000) david     (1000)      812 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/book.svg
--rw-r--r--   0 david     (1000) david     (1000)      352 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bookmark-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      303 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bookmark.svg
--rw-r--r--   0 david     (1000) david     (1000)      709 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bootstrap.svg
--rw-r--r--   0 david     (1000) david     (1000)     1585 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/braille.svg
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/briefcase.svg
--rw-r--r--   0 david     (1000) david     (1000)      532 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/btc.svg
--rw-r--r--   0 david     (1000) david     (1000)      562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bug.svg
--rw-r--r--   0 david     (1000) david     (1000)     1914 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/building-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1907 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/building.svg
--rw-r--r--   0 david     (1000) david     (1000)      438 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bullhorn.svg
--rw-r--r--   0 david     (1000) david     (1000)      479 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bullseye.svg
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/bus.svg
--rw-r--r--   0 david     (1000) david     (1000)      273 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/buysellads.svg
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/c.svg
--rw-r--r--   0 david     (1000) david     (1000)     1130 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calculator.svg
--rw-r--r--   0 david     (1000) david     (1000)      660 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calendar-check-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      612 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calendar-minus-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      517 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calendar-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      716 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calendar-plus-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      760 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calendar-times-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      794 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/calendar.svg
--rw-r--r--   0 david     (1000) david     (1000)      561 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/camera-retro.svg
--rw-r--r--   0 david     (1000) david     (1000)      428 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/camera.svg
--rw-r--r--   0 david     (1000) david     (1000)      573 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/car.svg
--rw-r--r--   0 david     (1000) david     (1000)      221 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      218 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      225 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-square-o-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      433 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-square-o-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      435 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-square-o-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      431 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-square-o-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      220 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/caret-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      684 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cart-arrow-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      637 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cart-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)     2012 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-amex.svg
--rw-r--r--   0 david     (1000) david     (1000)      509 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-diners-club.svg
--rw-r--r--   0 david     (1000) david     (1000)     1184 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-discover.svg
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-jcb.svg
--rw-r--r--   0 david     (1000) david     (1000)     2556 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-mastercard.svg
--rw-r--r--   0 david     (1000) david     (1000)     1412 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-paypal.svg
--rw-r--r--   0 david     (1000) david     (1000)     1324 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-stripe.svg
--rw-r--r--   0 david     (1000) david     (1000)      773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc-visa.svg
--rw-r--r--   0 david     (1000) david     (1000)      726 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cc.svg
--rw-r--r--   0 david     (1000) david     (1000)      701 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/certificate.svg
--rw-r--r--   0 david     (1000) david     (1000)     1101 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chain-broken.svg
--rw-r--r--   0 david     (1000) david     (1000)      390 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/check-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/check-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      577 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/check-square-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      353 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/check-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      326 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/check.svg
--rw-r--r--   0 david     (1000) david     (1000)      315 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-circle-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      313 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-circle-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      314 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-circle-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      314 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-circle-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      238 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      237 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      239 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      242 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chevron-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      382 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/child.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/chrome.svg
--rw-r--r--   0 david     (1000) david     (1000)      275 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/circle-o-notch.svg
--rw-r--r--   0 david     (1000) david     (1000)      248 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      248 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/circle-thin.svg
--rw-r--r--   0 david     (1000) david     (1000)      169 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/clipboard.svg
--rw-r--r--   0 david     (1000) david     (1000)      363 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/clock-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      461 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/clone.svg
--rw-r--r--   0 david     (1000) david     (1000)      489 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cloud-download.svg
--rw-r--r--   0 david     (1000) david     (1000)      488 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cloud-upload.svg
--rw-r--r--   0 david     (1000) david     (1000)      316 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cloud.svg
--rw-r--r--   0 david     (1000) david     (1000)      606 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/code-fork.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/code.svg
--rw-r--r--   0 david     (1000) david     (1000)      478 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/codepen.svg
--rw-r--r--   0 david     (1000) david     (1000)      440 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/codiepie.svg
--rw-r--r--   0 david     (1000) david     (1000)      353 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/coffee.svg
--rw-r--r--   0 david     (1000) david     (1000)      959 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cog.svg
--rw-r--r--   0 david     (1000) david     (1000)     2075 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cogs.svg
--rw-r--r--   0 david     (1000) david     (1000)      288 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/columns.svg
--rw-r--r--   0 david     (1000) david     (1000)      481 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/comment-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      303 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/comment.svg
--rw-r--r--   0 david     (1000) david     (1000)      702 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/commenting-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      515 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/commenting.svg
--rw-r--r--   0 david     (1000) david     (1000)      717 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/comments-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      564 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/comments.svg
--rw-r--r--   0 david     (1000) david     (1000)      301 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/compass.svg
--rw-r--r--   0 david     (1000) david     (1000)      495 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/compress.svg
--rw-r--r--   0 david     (1000) david     (1000)     1589 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/connectdevelop.svg
--rw-r--r--   0 david     (1000) david     (1000)      472 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/contao.svg
--rw-r--r--   0 david     (1000) david     (1000)      513 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/copyright.svg
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/creative-commons.svg
--rw-r--r--   0 david     (1000) david     (1000)      274 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/credit-card-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      375 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/credit-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      416 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/crop.svg
--rw-r--r--   0 david     (1000) david     (1000)      675 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/crosshairs.svg
--rw-r--r--   0 david     (1000) david     (1000)      201 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/css3.svg
--rw-r--r--   0 david     (1000) david     (1000)      341 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cube.svg
--rw-r--r--   0 david     (1000) david     (1000)      619 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cubes.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/cutlery.svg
--rw-r--r--   0 david     (1000) david     (1000)      286 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/dashcube.svg
--rw-r--r--   0 david     (1000) david     (1000)      470 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/database.svg
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/deaf.svg
--rw-r--r--   0 david     (1000) david     (1000)     4773 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/debian.svg
--rw-r--r--   0 david     (1000) david     (1000)      292 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/delicious.svg
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/desktop.svg
--rw-r--r--   0 david     (1000) david     (1000)     1829 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/dev-to.svg
--rw-r--r--   0 david     (1000) david     (1000)      228 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/deviantart.svg
--rw-r--r--   0 david     (1000) david     (1000)      395 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/diamond.svg
--rw-r--r--   0 david     (1000) david     (1000)     1298 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/diaspora.svg
--rw-r--r--   0 david     (1000) david     (1000)      332 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/digg.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/digitalocean.svg
--rw-r--r--   0 david     (1000) david     (1000)     1501 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/discord-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1572 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/discord.svg
--rw-r--r--   0 david     (1000) david     (1000)     3885 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/dogmazic.svg
--rw-r--r--   0 david     (1000) david     (1000)      329 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/dot-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/download.svg
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/dribbble.svg
--rw-r--r--   0 david     (1000) david     (1000)      309 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/dropbox.svg
--rw-r--r--   0 david     (1000) david     (1000)      802 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/drupal.svg
--rw-r--r--   0 david     (1000) david     (1000)      342 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/edge.svg
--rw-r--r--   0 david     (1000) david     (1000)      538 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eercast.svg
--rw-r--r--   0 david     (1000) david     (1000)      268 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eject.svg
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ellipsis-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      369 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ellipsis-v.svg
--rw-r--r--   0 david     (1000) david     (1000)      338 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/emby.svg
--rw-r--r--   0 david     (1000) david     (1000)     1377 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/empire.svg
--rw-r--r--   0 david     (1000) david     (1000)      570 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/envelope-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      696 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/envelope-open-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/envelope-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      541 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/envelope-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/envelope.svg
--rw-r--r--   0 david     (1000) david     (1000)      341 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/envira.svg
--rw-r--r--   0 david     (1000) david     (1000)      274 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eraser.svg
--rw-r--r--   0 david     (1000) david     (1000)      216 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ethereum.svg
--rw-r--r--   0 david     (1000) david     (1000)      528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/etsy.svg
--rw-r--r--   0 david     (1000) david     (1000)      624 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eur.svg
--rw-r--r--   0 david     (1000) david     (1000)      436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/exchange.svg
--rw-r--r--   0 david     (1000) david     (1000)      389 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/exclamation-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      441 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/exclamation-triangle.svg
--rw-r--r--   0 david     (1000) david     (1000)      291 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/exclamation.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/expand.svg
--rw-r--r--   0 david     (1000) david     (1000)      802 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/expeditedssl.svg
--rw-r--r--   0 david     (1000) david     (1000)      401 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/external-link-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      537 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/external-link.svg
--rw-r--r--   0 david     (1000) david     (1000)      820 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eye-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      536 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eye.svg
--rw-r--r--   0 david     (1000) david     (1000)      408 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/eyedropper.svg
--rw-r--r--   0 david     (1000) david     (1000)     2340 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/f-droid.svg
--rw-r--r--   0 david     (1000) david     (1000)      388 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/facebook-messenger.svg
--rw-r--r--   0 david     (1000) david     (1000)      307 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/facebook-official.svg
--rw-r--r--   0 david     (1000) david     (1000)      326 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/facebook-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      216 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/facebook.svg
--rw-r--r--   0 david     (1000) david     (1000)      362 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fast-backward.svg
--rw-r--r--   0 david     (1000) david     (1000)      365 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fast-forward.svg
--rw-r--r--   0 david     (1000) david     (1000)     1255 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fax.svg
--rw-r--r--   0 david     (1000) david     (1000)      522 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/female.svg
--rw-r--r--   0 david     (1000) david     (1000)      398 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ffmpeg.svg
--rw-r--r--   0 david     (1000) david     (1000)      383 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fighter-jet.svg
--rw-r--r--   0 david     (1000) david     (1000)      657 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-archive-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      815 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-audio-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      687 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-code-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      699 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-epub.svg
--rw-r--r--   0 david     (1000) david     (1000)      576 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-excel-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      446 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-image-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      322 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1115 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-pdf-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-powerpoint-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      599 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-text-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      519 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-text.svg
--rw-r--r--   0 david     (1000) david     (1000)      547 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-video-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      598 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file-word-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      252 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/file.svg
--rw-r--r--   0 david     (1000) david     (1000)      470 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/files-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1146 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/film.svg
--rw-r--r--   0 david     (1000) david     (1000)      275 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/filter.svg
--rw-r--r--   0 david     (1000) david     (1000)      576 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fire-extinguisher.svg
--rw-r--r--   0 david     (1000) david     (1000)      345 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fire.svg
--rw-r--r--   0 david     (1000) david     (1000)      522 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/firefox.svg
--rw-r--r--   0 david     (1000) david     (1000)      919 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/first-order.svg
--rw-r--r--   0 david     (1000) david     (1000)      933 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/flag-checkered.svg
--rw-r--r--   0 david     (1000) david     (1000)      748 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/flag-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      490 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/flag.svg
--rw-r--r--   0 david     (1000) david     (1000)      288 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/flask.svg
--rw-r--r--   0 david     (1000) david     (1000)      357 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/flickr.svg
--rw-r--r--   0 david     (1000) david     (1000)      502 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/floppy-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      375 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/folder-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      582 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/folder-open-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      389 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/folder-open.svg
--rw-r--r--   0 david     (1000) david     (1000)      236 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/folder.svg
--rw-r--r--   0 david     (1000) david     (1000)      386 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/font-awesome.svg
--rw-r--r--   0 david     (1000) david     (1000)      585 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/font.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fonticons.svg
--rw-r--r--   0 david     (1000) david     (1000)     1098 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fork-awesome.svg
--rw-r--r--   0 david     (1000) david     (1000)      832 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/fort-awesome.svg
--rw-r--r--   0 david     (1000) david     (1000)      506 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/forumbee.svg
--rw-r--r--   0 david     (1000) david     (1000)      259 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/forward.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/foursquare.svg
--rw-r--r--   0 david     (1000) david     (1000)     1338 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/free-code-camp.svg
--rw-r--r--   0 david     (1000) david     (1000)     1993 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/freedombox.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/friendica.svg
--rw-r--r--   0 david     (1000) david     (1000)      553 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/frown-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      482 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/futbol-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      581 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gamepad.svg
--rw-r--r--   0 david     (1000) david     (1000)      720 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gavel.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gbp.svg
--rw-r--r--   0 david     (1000) david     (1000)      246 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/genderless.svg
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/get-pocket.svg
--rw-r--r--   0 david     (1000) david     (1000)      341 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gg-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      275 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gg.svg
--rw-r--r--   0 david     (1000) david     (1000)      574 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gift.svg
--rw-r--r--   0 david     (1000) david     (1000)     2267 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gimp.svg
--rw-r--r--   0 david     (1000) david     (1000)     1019 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/git-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      966 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/git.svg
--rw-r--r--   0 david     (1000) david     (1000)     2377 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gitea.svg
--rw-r--r--   0 david     (1000) david     (1000)      714 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/github-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1061 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/github-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1023 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/github.svg
--rw-r--r--   0 david     (1000) david     (1000)      296 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gitlab.svg
--rw-r--r--   0 david     (1000) david     (1000)      273 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/glass.svg
--rw-r--r--   0 david     (1000) david     (1000)      667 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/glide-g.svg
--rw-r--r--   0 david     (1000) david     (1000)      823 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/glide.svg
--rw-r--r--   0 david     (1000) david     (1000)     2741 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/globe-e.svg
--rw-r--r--   0 david     (1000) david     (1000)     2253 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/globe-w.svg
--rw-r--r--   0 david     (1000) david     (1000)     3316 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/globe.svg
--rw-r--r--   0 david     (1000) david     (1000)     1304 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gnu-social.svg
--rw-r--r--   0 david     (1000) david     (1000)     2350 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gnupg.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/google-plus-official.svg
--rw-r--r--   0 david     (1000) david     (1000)      470 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/google-plus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      366 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/google-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      496 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/google-wallet.svg
--rw-r--r--   0 david     (1000) david     (1000)      304 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/google.svg
--rw-r--r--   0 david     (1000) david     (1000)      536 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/graduation-cap.svg
--rw-r--r--   0 david     (1000) david     (1000)      299 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/gratipay.svg
--rw-r--r--   0 david     (1000) david     (1000)     1270 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/grav.svg
--rw-r--r--   0 david     (1000) david     (1000)      405 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/h-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     3473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hackaday.svg
--rw-r--r--   0 david     (1000) david     (1000)      301 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hacker-news.svg
--rw-r--r--   0 david     (1000) david     (1000)     1659 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hackster.svg
--rw-r--r--   0 david     (1000) david     (1000)      730 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-lizard-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      811 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-o-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      814 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-o-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      801 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-o-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      799 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-o-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      720 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-paper-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1038 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-peace-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      817 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-pointer-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      835 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-rock-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1049 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-scissors-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      908 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hand-spock-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      981 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/handshake-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      968 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hashnode.svg
--rw-r--r--   0 david     (1000) david     (1000)      677 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hashtag.svg
--rw-r--r--   0 david     (1000) david     (1000)      535 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hdd-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      852 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/header.svg
--rw-r--r--   0 david     (1000) david     (1000)      559 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/headphones.svg
--rw-r--r--   0 david     (1000) david     (1000)      451 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/heart-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      287 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/heart.svg
--rw-r--r--   0 david     (1000) david     (1000)      545 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/heartbeat.svg
--rw-r--r--   0 david     (1000) david     (1000)      558 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/history.svg
--rw-r--r--   0 david     (1000) david     (1000)      433 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/home.svg
--rw-r--r--   0 david     (1000) david     (1000)     1469 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hospital-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      531 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hourglass-end.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hourglass-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      532 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hourglass-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      476 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hourglass-start.svg
--rw-r--r--   0 david     (1000) david     (1000)      393 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hourglass.svg
--rw-r--r--   0 david     (1000) david     (1000)      193 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/houzz.svg
--rw-r--r--   0 david     (1000) david     (1000)      245 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/html5.svg
--rw-r--r--   0 david     (1000) david     (1000)     1087 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/hubzilla.svg
--rw-r--r--   0 david     (1000) david     (1000)      351 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/i-cursor.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/id-badge.svg
--rw-r--r--   0 david     (1000) david     (1000)      843 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/id-card-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      842 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/id-card.svg
--rw-r--r--   0 david     (1000) david     (1000)      435 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ils.svg
--rw-r--r--   0 david     (1000) david     (1000)      632 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/imdb.svg
--rw-r--r--   0 david     (1000) david     (1000)      318 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/inbox.svg
--rw-r--r--   0 david     (1000) david     (1000)      586 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/indent.svg
--rw-r--r--   0 david     (1000) david     (1000)      273 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/industry.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/info-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      354 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/info.svg
--rw-r--r--   0 david     (1000) david     (1000)     1519 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/inkscape.svg
--rw-r--r--   0 david     (1000) david     (1000)      508 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/inr.svg
--rw-r--r--   0 david     (1000) david     (1000)      879 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/instagram.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/internet-explorer.svg
--rw-r--r--   0 david     (1000) david     (1000)      617 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ioxhost.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/italic.svg
--rw-r--r--   0 david     (1000) david     (1000)     1016 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/jirafeau.svg
--rw-r--r--   0 david     (1000) david     (1000)      973 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/joomla.svg
--rw-r--r--   0 david     (1000) david     (1000)     1255 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/joplin.svg
--rw-r--r--   0 david     (1000) david     (1000)      516 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/jpy.svg
--rw-r--r--   0 david     (1000) david     (1000)      661 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/jsfiddle.svg
--rw-r--r--   0 david     (1000) david     (1000)      811 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/key-modern.svg
--rw-r--r--   0 david     (1000) david     (1000)      611 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/key.svg
--rw-r--r--   0 david     (1000) david     (1000)     4700 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/keybase.svg
--rw-r--r--   0 david     (1000) david     (1000)     1343 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/keyboard-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      802 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/krw.svg
--rw-r--r--   0 david     (1000) david     (1000)     1204 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/language.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/laptop.svg
--rw-r--r--   0 david     (1000) david     (1000)     1781 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/laravel.svg
--rw-r--r--   0 david     (1000) david     (1000)      742 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/lastfm-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      639 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/lastfm.svg
--rw-r--r--   0 david     (1000) david     (1000)      560 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/leaf.svg
--rw-r--r--   0 david     (1000) david     (1000)      694 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/leanpub.svg
--rw-r--r--   0 david     (1000) david     (1000)      739 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/lemon-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      295 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/level-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      301 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/level-up.svg
--rw-r--r--   0 david     (1000) david     (1000)     1499 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/liberapay-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1372 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/liberapay.svg
--rw-r--r--   0 david     (1000) david     (1000)      653 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/life-ring.svg
--rw-r--r--   0 david     (1000) david     (1000)      726 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/lightbulb-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      306 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/line-chart.svg
--rw-r--r--   0 david     (1000) david     (1000)      929 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/link.svg
--rw-r--r--   0 david     (1000) david     (1000)      469 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/linkedin-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/linkedin.svg
--rw-r--r--   0 david     (1000) david     (1000)      957 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/linode.svg
--rw-r--r--   0 david     (1000) david     (1000)     2650 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/linux.svg
--rw-r--r--   0 david     (1000) david     (1000)      845 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/list-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      841 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/list-ol.svg
--rw-r--r--   0 david     (1000) david     (1000)      596 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/list-ul.svg
--rw-r--r--   0 david     (1000) david     (1000)      841 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/list.svg
--rw-r--r--   0 david     (1000) david     (1000)      255 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/location-arrow.svg
--rw-r--r--   0 david     (1000) david     (1000)      291 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/lock.svg
--rw-r--r--   0 david     (1000) david     (1000)      266 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/long-arrow-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      260 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/long-arrow-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      266 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/long-arrow-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      260 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/long-arrow-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      985 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/low-vision.svg
--rw-r--r--   0 david     (1000) david     (1000)      501 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/magic.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/magnet.svg
--rw-r--r--   0 david     (1000) david     (1000)      402 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/male.svg
--rw-r--r--   0 david     (1000) david     (1000)      302 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/map-marker.svg
--rw-r--r--   0 david     (1000) david     (1000)      385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/map-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      367 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/map-pin.svg
--rw-r--r--   0 david     (1000) david     (1000)      461 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/map-signs.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/map.svg
--rw-r--r--   0 david     (1000) david     (1000)      848 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mars-double.svg
--rw-r--r--   0 david     (1000) david     (1000)      512 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mars-stroke-h.svg
--rw-r--r--   0 david     (1000) david     (1000)      512 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mars-stroke-v.svg
--rw-r--r--   0 david     (1000) david     (1000)      535 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mars-stroke.svg
--rw-r--r--   0 david     (1000) david     (1000)      407 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mars.svg
--rw-r--r--   0 david     (1000) david     (1000)     1252 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mastodon-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)     1353 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mastodon-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1271 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mastodon.svg
--rw-r--r--   0 david     (1000) david     (1000)     1326 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/matrix-org.svg
--rw-r--r--   0 david     (1000) david     (1000)      261 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/maxcdn.svg
--rw-r--r--   0 david     (1000) david     (1000)      746 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/meanpath.svg
--rw-r--r--   0 david     (1000) david     (1000)      614 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/medium-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      564 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/medium.svg
--rw-r--r--   0 david     (1000) david     (1000)      528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/medkit.svg
--rw-r--r--   0 david     (1000) david     (1000)     1566 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/meetup.svg
--rw-r--r--   0 david     (1000) david     (1000)      476 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/meh-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      571 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mercury.svg
--rw-r--r--   0 david     (1000) david     (1000)     1164 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/microchip.svg
--rw-r--r--   0 david     (1000) david     (1000)      620 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/microphone-slash.svg
--rw-r--r--   0 david     (1000) david     (1000)      431 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/microphone.svg
--rw-r--r--   0 david     (1000) david     (1000)      262 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/minus-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      406 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/minus-square-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      301 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/minus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      187 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      889 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mixcloud.svg
--rw-r--r--   0 david     (1000) david     (1000)      430 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mobile.svg
--rw-r--r--   0 david     (1000) david     (1000)      207 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/modx.svg
--rw-r--r--   0 david     (1000) david     (1000)      458 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/money.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/moon-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      324 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/moon.svg
--rw-r--r--   0 david     (1000) david     (1000)      910 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/motorcycle.svg
--rw-r--r--   0 david     (1000) david     (1000)      311 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/mouse-pointer.svg
--rw-r--r--   0 david     (1000) david     (1000)      327 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/music.svg
--rw-r--r--   0 david     (1000) david     (1000)      307 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/neuter.svg
--rw-r--r--   0 david     (1000) david     (1000)      455 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/newspaper-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1309 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/nextcloud-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1405 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/nextcloud.svg
--rw-r--r--   0 david     (1000) david     (1000)     1763 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/nodejs.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/object-group.svg
--rw-r--r--   0 david     (1000) david     (1000)      554 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/object-ungroup.svg
--rw-r--r--   0 david     (1000) david     (1000)      674 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/odnoklassniki-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      605 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/odnoklassniki.svg
--rw-r--r--   0 david     (1000) david     (1000)      334 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/opencart.svg
--rw-r--r--   0 david     (1000) david     (1000)      291 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/openid.svg
--rw-r--r--   0 david     (1000) david     (1000)      520 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/opera.svg
--rw-r--r--   0 david     (1000) david     (1000)     3856 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/optin-monster.svg
--rw-r--r--   0 david     (1000) david     (1000)      581 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/outdent.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pagelines.svg
--rw-r--r--   0 david     (1000) david     (1000)      394 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paint-brush.svg
--rw-r--r--   0 david     (1000) david     (1000)      368 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paper-plane-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      346 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paper-plane.svg
--rw-r--r--   0 david     (1000) david     (1000)      622 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paperclip.svg
--rw-r--r--   0 david     (1000) david     (1000)      414 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paragraph.svg
--rw-r--r--   0 david     (1000) david     (1000)      316 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/patreon.svg
--rw-r--r--   0 david     (1000) david     (1000)      434 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pause-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pause-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      281 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pause.svg
--rw-r--r--   0 david     (1000) david     (1000)      606 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paw.svg
--rw-r--r--   0 david     (1000) david     (1000)      641 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/paypal.svg
--rw-r--r--   0 david     (1000) david     (1000)      224 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/peertube.svg
--rw-r--r--   0 david     (1000) david     (1000)      630 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pencil-square-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      441 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pencil-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      391 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pencil.svg
--rw-r--r--   0 david     (1000) david     (1000)      540 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/percent.svg
--rw-r--r--   0 david     (1000) david     (1000)      562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/phone-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/phone.svg
--rw-r--r--   0 david     (1000) david     (1000)     1711 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/php.svg
--rw-r--r--   0 david     (1000) david     (1000)      417 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/picture-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      245 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pie-chart.svg
--rw-r--r--   0 david     (1000) david     (1000)      494 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pinterest-p.svg
--rw-r--r--   0 david     (1000) david     (1000)      624 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pinterest-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      616 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pinterest.svg
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pixelfed.svg
--rw-r--r--   0 david     (1000) david     (1000)      474 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/plane.svg
--rw-r--r--   0 david     (1000) david     (1000)      389 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/play-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      299 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/play-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      175 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/play.svg
--rw-r--r--   0 david     (1000) david     (1000)      333 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/pleroma.svg
--rw-r--r--   0 david     (1000) david     (1000)      323 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/plug.svg
--rw-r--r--   0 david     (1000) david     (1000)      364 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/plus-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      506 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/plus-square-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      403 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/plus-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      288 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      925 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/podcast.svg
--rw-r--r--   0 david     (1000) david     (1000)      432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/power-off.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/print.svg
--rw-r--r--   0 david     (1000) david     (1000)      298 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/product-hunt.svg
--rw-r--r--   0 david     (1000) david     (1000)      727 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/puzzle-piece.svg
--rw-r--r--   0 david     (1000) david     (1000)     1894 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/python.svg
--rw-r--r--   0 david     (1000) david     (1000)      707 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/qq.svg
--rw-r--r--   0 david     (1000) david     (1000)      507 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/qrcode.svg
--rw-r--r--   0 david     (1000) david     (1000)      633 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/question-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      543 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/question-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      487 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/question.svg
--rw-r--r--   0 david     (1000) david     (1000)      495 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/quora.svg
--rw-r--r--   0 david     (1000) david     (1000)      489 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/quote-left.svg
--rw-r--r--   0 david     (1000) david     (1000)      490 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/quote-right.svg
--rw-r--r--   0 david     (1000) david     (1000)      721 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/random.svg
--rw-r--r--   0 david     (1000) david     (1000)     1021 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ravelry.svg
--rw-r--r--   0 david     (1000) david     (1000)     4501 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/react.svg
--rw-r--r--   0 david     (1000) david     (1000)      505 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/rebel.svg
--rw-r--r--   0 david     (1000) david     (1000)      646 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/recycle.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/reddit-alien.svg
--rw-r--r--   0 david     (1000) david     (1000)      808 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/reddit-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      799 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/reddit.svg
--rw-r--r--   0 david     (1000) david     (1000)      639 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/refresh.svg
--rw-r--r--   0 david     (1000) david     (1000)      551 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/registered.svg
--rw-r--r--   0 david     (1000) david     (1000)      351 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/renren.svg
--rw-r--r--   0 david     (1000) david     (1000)      435 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/repeat.svg
--rw-r--r--   0 david     (1000) david     (1000)      539 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/reply-all.svg
--rw-r--r--   0 david     (1000) david     (1000)      398 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/reply.svg
--rw-r--r--   0 david     (1000) david     (1000)      536 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/retweet.svg
--rw-r--r--   0 david     (1000) david     (1000)      532 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/road.svg
--rw-r--r--   0 david     (1000) david     (1000)      462 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/rocket.svg
--rw-r--r--   0 david     (1000) david     (1000)      589 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/rss-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/rss.svg
--rw-r--r--   0 david     (1000) david     (1000)      432 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/rub.svg
--rw-r--r--   0 david     (1000) david     (1000)     1010 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/safari.svg
--rw-r--r--   0 david     (1000) david     (1000)     1202 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/scissors.svg
--rw-r--r--   0 david     (1000) david     (1000)      567 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/scribd.svg
--rw-r--r--   0 david     (1000) david     (1000)    10552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/scuttlebutt.svg
--rw-r--r--   0 david     (1000) david     (1000)      444 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/search-minus.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/search-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      352 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/search.svg
--rw-r--r--   0 david     (1000) david     (1000)      691 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sellsy.svg
--rw-r--r--   0 david     (1000) david     (1000)      427 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/server.svg
--rw-r--r--   0 david     (1000) david     (1000)     2644 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shaarli-o.svg
--rw-r--r--   0 david     (1000) david     (1000)     1528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shaarli.svg
--rw-r--r--   0 david     (1000) david     (1000)      542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/share-alt-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      420 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/share-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      676 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/share-square-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      475 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/share-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      408 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/share.svg
--rw-r--r--   0 david     (1000) david     (1000)      284 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shield.svg
--rw-r--r--   0 david     (1000) david     (1000)     1083 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ship.svg
--rw-r--r--   0 david     (1000) david     (1000)     1325 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shirtsinbulk.svg
--rw-r--r--   0 david     (1000) david     (1000)      512 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shopping-bag.svg
--rw-r--r--   0 david     (1000) david     (1000)      813 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shopping-basket.svg
--rw-r--r--   0 david     (1000) david     (1000)      475 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shopping-cart.svg
--rw-r--r--   0 david     (1000) david     (1000)     1281 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/shower.svg
--rw-r--r--   0 david     (1000) david     (1000)      463 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sign-in.svg
--rw-r--r--   0 david     (1000) david     (1000)     1053 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sign-language.svg
--rw-r--r--   0 david     (1000) david     (1000)      464 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sign-out.svg
--rw-r--r--   0 david     (1000) david     (1000)      568 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/signal.svg
--rw-r--r--   0 david     (1000) david     (1000)    11649 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/signalapp.svg
--rw-r--r--   0 david     (1000) david     (1000)      448 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/simplybuilt.svg
--rw-r--r--   0 david     (1000) david     (1000)      544 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sitemap.svg
--rw-r--r--   0 david     (1000) david     (1000)      636 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/skyatlas.svg
--rw-r--r--   0 david     (1000) david     (1000)      657 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/skype.svg
--rw-r--r--   0 david     (1000) david     (1000)     1401 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/slack.svg
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sliders.svg
--rw-r--r--   0 david     (1000) david     (1000)      697 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/slideshare.svg
--rw-r--r--   0 david     (1000) david     (1000)      554 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/smile-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      692 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/snapchat-ghost.svg
--rw-r--r--   0 david     (1000) david     (1000)      710 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/snapchat-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      669 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/snapchat.svg
--rw-r--r--   0 david     (1000) david     (1000)      857 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/snowdrift.svg
--rw-r--r--   0 david     (1000) david     (1000)      905 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/snowflake-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      576 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/social-home.svg
--rw-r--r--   0 david     (1000) david     (1000)      588 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-alpha-asc.svg
--rw-r--r--   0 david     (1000) david     (1000)      588 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-alpha-desc.svg
--rw-r--r--   0 david     (1000) david     (1000)      640 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-amount-asc.svg
--rw-r--r--   0 david     (1000) david     (1000)      639 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-amount-desc.svg
--rw-r--r--   0 david     (1000) david     (1000)      219 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-asc.svg
--rw-r--r--   0 david     (1000) david     (1000)      224 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-desc.svg
--rw-r--r--   0 david     (1000) david     (1000)      670 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-numeric-asc.svg
--rw-r--r--   0 david     (1000) david     (1000)      673 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort-numeric-desc.svg
--rw-r--r--   0 david     (1000) david     (1000)      348 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sort.svg
--rw-r--r--   0 david     (1000) david     (1000)     1603 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/soundcloud.svg
--rw-r--r--   0 david     (1000) david     (1000)      648 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/space-shuttle.svg
--rw-r--r--   0 david     (1000) david     (1000)     2226 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/spell-check.svg
--rw-r--r--   0 david     (1000) david     (1000)      742 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/spinner.svg
--rw-r--r--   0 david     (1000) david     (1000)      232 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/spoon.svg
--rw-r--r--   0 david     (1000) david     (1000)      742 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/spotify.svg
--rw-r--r--   0 david     (1000) david     (1000)      313 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/square-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      207 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/square.svg
--rw-r--r--   0 david     (1000) david     (1000)      289 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stack-exchange.svg
--rw-r--r--   0 david     (1000) david     (1000)      291 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stack-overflow.svg
--rw-r--r--   0 david     (1000) david     (1000)      386 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/star-half-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      244 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/star-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/star-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      373 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/star.svg
--rw-r--r--   0 david     (1000) david     (1000)      726 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/steam-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      629 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/steam.svg
--rw-r--r--   0 david     (1000) david     (1000)      269 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/step-backward.svg
--rw-r--r--   0 david     (1000) david     (1000)      271 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/step-forward.svg
--rw-r--r--   0 david     (1000) david     (1000)      638 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stethoscope.svg
--rw-r--r--   0 david     (1000) david     (1000)      333 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sticky-note-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      264 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sticky-note.svg
--rw-r--r--   0 david     (1000) david     (1000)      343 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stop-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      264 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stop-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      188 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stop.svg
--rw-r--r--   0 david     (1000) david     (1000)      552 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/street-view.svg
--rw-r--r--   0 david     (1000) david     (1000)      918 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/strikethrough.svg
--rw-r--r--   0 david     (1000) david     (1000)      466 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stumbleupon-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      419 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/stumbleupon.svg
--rw-r--r--   0 david     (1000) david     (1000)      542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/subscript.svg
--rw-r--r--   0 david     (1000) david     (1000)      453 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/subway.svg
--rw-r--r--   0 david     (1000) david     (1000)      329 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/suitcase.svg
--rw-r--r--   0 david     (1000) david     (1000)      603 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sun-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      525 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/sun.svg
--rw-r--r--   0 david     (1000) david     (1000)      344 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/superpowers.svg
--rw-r--r--   0 david     (1000) david     (1000)      542 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/superscript.svg
--rw-r--r--   0 david     (1000) david     (1000)     1990 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/syncthing.svg
--rw-r--r--   0 david     (1000) david     (1000)     1050 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/table.svg
--rw-r--r--   0 david     (1000) david     (1000)      357 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tablet.svg
--rw-r--r--   0 david     (1000) david     (1000)      739 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tachometer.svg
--rw-r--r--   0 david     (1000) david     (1000)      334 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tag.svg
--rw-r--r--   0 david     (1000) david     (1000)      521 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tags.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tasks.svg
--rw-r--r--   0 david     (1000) david     (1000)      622 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/taxi.svg
--rw-r--r--   0 david     (1000) david     (1000)      326 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/telegram.svg
--rw-r--r--   0 david     (1000) david     (1000)      398 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/television.svg
--rw-r--r--   0 david     (1000) david     (1000)      593 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tencent-weibo.svg
--rw-r--r--   0 david     (1000) david     (1000)      328 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/terminal.svg
--rw-r--r--   0 david     (1000) david     (1000)      821 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/text-height.svg
--rw-r--r--   0 david     (1000) david     (1000)      905 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/text-width.svg
--rw-r--r--   0 david     (1000) david     (1000)      515 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/th-large.svg
--rw-r--r--   0 david     (1000) david     (1000)      654 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/th-list.svg
--rw-r--r--   0 david     (1000) david     (1000)      939 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/th.svg
--rw-r--r--   0 david     (1000) david     (1000)     1855 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/themeisle.svg
--rw-r--r--   0 david     (1000) david     (1000)      510 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thermometer-empty.svg
--rw-r--r--   0 david     (1000) david     (1000)      528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thermometer-full.svg
--rw-r--r--   0 david     (1000) david     (1000)      528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thermometer-half.svg
--rw-r--r--   0 david     (1000) david     (1000)      529 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thermometer-quarter.svg
--rw-r--r--   0 david     (1000) david     (1000)      528 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thermometer-three-quarters.svg
--rw-r--r--   0 david     (1000) david     (1000)      402 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thumb-tack.svg
--rw-r--r--   0 david     (1000) david     (1000)      662 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thumbs-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      860 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thumbs-o-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      854 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thumbs-o-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      667 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/thumbs-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      453 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/ticket.svg
--rw-r--r--   0 david     (1000) david     (1000)      495 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/times-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      513 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/times-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      454 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/times.svg
--rw-r--r--   0 david     (1000) david     (1000)      394 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tint.svg
--rw-r--r--   0 david     (1000) david     (1000)     1484 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tipeee.svg
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/toggle-off.svg
--rw-r--r--   0 david     (1000) david     (1000)      271 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/toggle-on.svg
--rw-r--r--   0 david     (1000) david     (1000)      560 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/trademark.svg
--rw-r--r--   0 david     (1000) david     (1000)      355 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/train.svg
--rw-r--r--   0 david     (1000) david     (1000)      827 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/transgender-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      566 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/transgender.svg
--rw-r--r--   0 david     (1000) david     (1000)      692 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/trash-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      635 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/trash.svg
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tree.svg
--rw-r--r--   0 david     (1000) david     (1000)      377 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/trello.svg
--rw-r--r--   0 david     (1000) david     (1000)     1127 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tripadvisor.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/trophy.svg
--rw-r--r--   0 david     (1000) david     (1000)      559 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/truck.svg
--rw-r--r--   0 david     (1000) david     (1000)      546 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/try.svg
--rw-r--r--   0 david     (1000) david     (1000)     1177 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tty.svg
--rw-r--r--   0 david     (1000) david     (1000)      379 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tumblr-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      264 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/tumblr.svg
--rw-r--r--   0 david     (1000) david     (1000)      252 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/twitch.svg
--rw-r--r--   0 david     (1000) david     (1000)      592 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/twitter-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      497 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/twitter.svg
--rw-r--r--   0 david     (1000) david     (1000)      712 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/umbrella.svg
--rw-r--r--   0 david     (1000) david     (1000)      979 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/underline.svg
--rw-r--r--   0 david     (1000) david     (1000)      440 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/undo.svg
--rw-r--r--   0 david     (1000) david     (1000)      764 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/universal-access.svg
--rw-r--r--   0 david     (1000) david     (1000)      341 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/university.svg
--rw-r--r--   0 david     (1000) david     (1000)      310 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/unlock-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      320 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/unlock.svg
--rw-r--r--   0 david     (1000) david     (1000)      240 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/unslpash.svg
--rw-r--r--   0 david     (1000) david     (1000)      543 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/upload.svg
--rw-r--r--   0 david     (1000) david     (1000)      678 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/usb.svg
--rw-r--r--   0 david     (1000) david     (1000)      563 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/usd.svg
--rw-r--r--   0 david     (1000) david     (1000)      437 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-circle-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      396 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-circle.svg
--rw-r--r--   0 david     (1000) david     (1000)      757 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-md.svg
--rw-r--r--   0 david     (1000) david     (1000)      493 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      598 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-plus.svg
--rw-r--r--   0 david     (1000) david     (1000)      784 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-secret.svg
--rw-r--r--   0 david     (1000) david     (1000)      745 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user-times.svg
--rw-r--r--   0 david     (1000) david     (1000)      310 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/user.svg
--rw-r--r--   0 david     (1000) david     (1000)      761 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/users.svg
--rw-r--r--   0 david     (1000) david     (1000)      835 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/venus-double.svg
--rw-r--r--   0 david     (1000) david     (1000)      914 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/venus-mars.svg
--rw-r--r--   0 david     (1000) david     (1000)      417 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/venus.svg
--rw-r--r--   0 david     (1000) david     (1000)      241 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/viacoin.svg
--rw-r--r--   0 david     (1000) david     (1000)      782 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/viadeo-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      790 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/viadeo.svg
--rw-r--r--   0 david     (1000) david     (1000)      330 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/video-camera.svg
--rw-r--r--   0 david     (1000) david     (1000)      562 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/vimeo-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      473 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/vimeo.svg
--rw-r--r--   0 david     (1000) david     (1000)      449 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/vine.svg
--rw-r--r--   0 david     (1000) david     (1000)      678 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/vk.svg
--rw-r--r--   0 david     (1000) david     (1000)     1024 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/volume-control-phone.svg
--rw-r--r--   0 david     (1000) david     (1000)      387 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/volume-down.svg
--rw-r--r--   0 david     (1000) david     (1000)      237 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/volume-off.svg
--rw-r--r--   0 david     (1000) david     (1000)      872 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/volume-up.svg
--rw-r--r--   0 david     (1000) david     (1000)      965 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/weibo.svg
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/weixin.svg
--rw-r--r--   0 david     (1000) david     (1000)      679 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/whatsapp.svg
--rw-r--r--   0 david     (1000) david     (1000)      752 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wheelchair-alt.svg
--rw-r--r--   0 david     (1000) david     (1000)      481 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wheelchair.svg
--rw-r--r--   0 david     (1000) david     (1000)      718 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wifi.svg
--rw-r--r--   0 david     (1000) david     (1000)      423 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wikidata.svg
--rw-r--r--   0 david     (1000) david     (1000)      618 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wikipedia-w.svg
--rw-r--r--   0 david     (1000) david     (1000)      480 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/window-close-o.svg
--rw-r--r--   0 david     (1000) david     (1000)      450 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/window-close.svg
--rw-r--r--   0 david     (1000) david     (1000)      228 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/window-maximize.svg
--rw-r--r--   0 david     (1000) david     (1000)      202 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/window-minimize.svg
--rw-r--r--   0 david     (1000) david     (1000)      335 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/window-restore.svg
--rw-r--r--   0 david     (1000) david     (1000)      189 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/windows.svg
--rw-r--r--   0 david     (1000) david     (1000)      795 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wordpress.svg
--rw-r--r--   0 david     (1000) david     (1000)      483 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wpbeginner.svg
--rw-r--r--   0 david     (1000) david     (1000)      414 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wpexplorer.svg
--rw-r--r--   0 david     (1000) david     (1000)      488 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wpforms.svg
--rw-r--r--   0 david     (1000) david     (1000)      471 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/wrench.svg
--rw-r--r--   0 david     (1000) david     (1000)      540 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/xing-square.svg
--rw-r--r--   0 david     (1000) david     (1000)      454 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/xing.svg
--rw-r--r--   0 david     (1000) david     (1000)      868 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/xmpp.svg
--rw-r--r--   0 david     (1000) david     (1000)      212 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/y-combinator.svg
--rw-r--r--   0 david     (1000) david     (1000)      333 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/yahoo.svg
--rw-r--r--   0 david     (1000) david     (1000)      924 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/yelp.svg
--rw-r--r--   0 david     (1000) david     (1000)      452 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/yoast.svg
--rw-r--r--   0 david     (1000) david     (1000)      436 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/youtube-play.svg
--rw-r--r--   0 david     (1000) david     (1000)     1586 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/youtube-square.svg
--rw-r--r--   0 david     (1000) david     (1000)     1489 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/youtube.svg
--rw-r--r--   0 david     (1000) david     (1000)      385 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svg/zotero.svg
--rw-r--r--   0 david     (1000) david     (1000)      187 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/fork-awesome/src/icons/svgo_config.json
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.910535 pyssg-0.8.3/pyssg.xyz/live/static/hl/
--rw-r--r--   0 david     (1000) david     (1000)     1514 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     3197 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/highlight-ln.min.js
--rw-r--r--   0 david     (1000) david     (1000)   283805 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/highlight.js
--rw-r--r--   0 david     (1000) david     (1000)   114230 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/highlight.min.js
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.940535 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/
--rw-r--r--   0 david     (1000) david     (1000)   159551 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/1c.min.js
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/abnf.min.js
--rw-r--r--   0 david     (1000) david     (1000)      800 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/accesslog.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1331 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/actionscript.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2000 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ada.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1621 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/angelscript.min.js
--rw-r--r--   0 david     (1000) david     (1000)      943 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/apache.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2385 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/applescript.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2856 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/arcade.min.js
--rw-r--r--   0 david     (1000) david     (1000)     8183 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/arduino.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3156 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/armasm.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1774 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/asciidoc.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2482 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/aspectj.min.js
--rw-r--r--   0 david     (1000) david     (1000)      929 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/autohotkey.min.js
--rw-r--r--   0 david     (1000) david     (1000)     6469 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/autoit.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1979 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/avrasm.min.js
--rw-r--r--   0 david     (1000) david     (1000)      667 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/awk.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1388 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/axapta.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2034 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/bash.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1462 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/basic.min.js
--rw-r--r--   0 david     (1000) david     (1000)      289 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/bnf.min.js
--rw-r--r--   0 david     (1000) david     (1000)      411 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/brainfuck.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4333 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/c-like.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4388 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/c.min.js
--rw-r--r--   0 david     (1000) david     (1000)      997 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/cal.min.js
--rw-r--r--   0 david     (1000) david     (1000)      851 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/capnproto.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1114 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ceylon.min.js
--rw-r--r--   0 david     (1000) david     (1000)      555 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/clean.min.js
--rw-r--r--   0 david     (1000) david     (1000)      194 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/clojure-repl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3640 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/clojure.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2438 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/cmake.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3023 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/coffeescript.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3478 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/coq.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1344 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/cos.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4448 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/cpp.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1406 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/crmsh.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3602 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/crystal.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3853 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/csharp.min.js
--rw-r--r--   0 david     (1000) david     (1000)      441 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/csp.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1548 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/css.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2482 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/d.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1997 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dart.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1983 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/delphi.min.js
--rw-r--r--   0 david     (1000) david     (1000)      626 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/diff.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1788 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/django.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1755 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dns.min.js
--rw-r--r--   0 david     (1000) david     (1000)      424 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dockerfile.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1140 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dos.min.js
--rw-r--r--   0 david     (1000) david     (1000)      591 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dsconfig.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1368 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dts.min.js
--rw-r--r--   0 david     (1000) david     (1000)      457 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/dust.min.js
--rw-r--r--   0 david     (1000) david     (1000)      416 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ebnf.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2281 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/elixir.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1148 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/elm.min.js
--rw-r--r--   0 david     (1000) david     (1000)      212 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/erb.min.js
--rw-r--r--   0 david     (1000) david     (1000)      761 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/erlang-repl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1918 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/erlang.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4327 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/excel.min.js
--rw-r--r--   0 david     (1000) david     (1000)      400 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/fix.min.js
--rw-r--r--   0 david     (1000) david     (1000)      602 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/flix.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4647 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/fortran.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1150 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/fsharp.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2911 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gams.min.js
--rw-r--r--   0 david     (1000) david     (1000)    13012 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gauss.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1027 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gcode.min.js
--rw-r--r--   0 david     (1000) david     (1000)     5457 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gdscript.min.js
--rw-r--r--   0 david     (1000) david     (1000)      542 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gherkin.min.js
--rw-r--r--   0 david     (1000) david     (1000)     8327 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/glsl.min.js
--rw-r--r--   0 david     (1000) david     (1000)    50275 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gml.min.js
--rw-r--r--   0 david     (1000) david     (1000)      978 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/go.min.js
--rw-r--r--   0 david     (1000) david     (1000)      548 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/golo.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1548 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/gradle.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1561 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/groovy.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1053 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/haml.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2171 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/handlebars.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1712 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/haskell.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1905 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/haxe.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3391 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/hsp.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2270 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/htmlbars.min.js
--rw-r--r--   0 david     (1000) david     (1000)      583 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/http.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2959 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/hy.min.js
--rw-r--r--   0 david     (1000) david     (1000)      676 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/inform7.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1090 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ini.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4650 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/irpf90.min.js
--rw-r--r--   0 david     (1000) david     (1000)    83214 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/isbl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2723 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/java.min.js
--rw-r--r--   0 david     (1000) david     (1000)     5263 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/javascript.min.js
--rw-r--r--   0 david     (1000) david     (1000)      877 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/jboss-cli.min.js
--rw-r--r--   0 david     (1000) david     (1000)      590 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/json.min.js
--rw-r--r--   0 david     (1000) david     (1000)      221 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/julia-repl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3490 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/julia.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3086 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/kotlin.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3037 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/lasso.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3468 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/latex.min.js
--rw-r--r--   0 david     (1000) david     (1000)      345 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ldif.min.js
--rw-r--r--   0 david     (1000) david     (1000)      440 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/leaf.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1997 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/less.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1152 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/lisp.min.js
--rw-r--r--   0 david     (1000) david     (1000)     8243 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/livecodeserver.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3405 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/livescript.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2658 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/llvm.min.js
--rw-r--r--   0 david     (1000) david     (1000)    11898 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/lsl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1899 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/lua.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1086 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/makefile.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2031 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/markdown.min.js
--rw-r--r--   0 david     (1000) david     (1000)   112999 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/mathematica.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2318 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/matlab.min.js
--rw-r--r--   0 david     (1000) david     (1000)    28711 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/maxima.min.js
--rw-r--r--   0 david     (1000) david     (1000)    16530 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/mel.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2068 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/mercury.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2463 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/mipsasm.min.js
--rw-r--r--   0 david     (1000) david     (1000)      724 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/mizar.min.js
--rw-r--r--   0 david     (1000) david     (1000)      313 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/mojolicious.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1345 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/monkey.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1723 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/moonscript.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2999 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/n1ql.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1405 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/nginx.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1444 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/nim.min.js
--rw-r--r--   0 david     (1000) david     (1000)      649 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/nix.min.js
--rw-r--r--   0 david     (1000) david     (1000)      243 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/node-repl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     5201 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/nsis.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2561 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/objectivec.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1256 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ocaml.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1304 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/openscad.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1952 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/oxygene.min.js
--rw-r--r--   0 david     (1000) david     (1000)      572 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/parser3.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3493 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/perl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1271 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/pf.min.js
--rw-r--r--   0 david     (1000) david     (1000)    18891 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/pgsql.min.js
--rw-r--r--   0 david     (1000) david     (1000)      448 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/php-template.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3852 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/php.min.js
--rw-r--r--   0 david     (1000) david     (1000)      135 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/plaintext.min.js
--rw-r--r--   0 david     (1000) david     (1000)      957 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/pony.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4340 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/powershell.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3127 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/processing.min.js
--rw-r--r--   0 david     (1000) david     (1000)      505 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/profile.min.js
--rw-r--r--   0 david     (1000) david     (1000)      687 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/prolog.min.js
--rw-r--r--   0 david     (1000) david     (1000)      717 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/properties.min.js
--rw-r--r--   0 david     (1000) david     (1000)      699 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/protobuf.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4103 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/puppet.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1601 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/purebasic.min.js
--rw-r--r--   0 david     (1000) david     (1000)      244 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/python-repl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2814 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/python.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1153 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/q.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2797 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/qml.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2981 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/r.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3348 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/reasonml.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1305 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/rib.min.js
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/roboconf.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2504 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/routeros.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1074 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/rsl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3323 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ruby.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3862 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/ruleslanguage.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2246 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/rust.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3673 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/sas.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1581 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/scala.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3282 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/scheme.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1241 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/scilab.min.js
--rw-r--r--   0 david     (1000) david     (1000)     6124 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/scss.min.js
--rw-r--r--   0 david     (1000) david     (1000)      229 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/shell.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1039 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/smali.min.js
--rw-r--r--   0 david     (1000) david     (1000)      634 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/smalltalk.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1153 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/sml.min.js
--rw-r--r--   0 david     (1000) david     (1000)    32250 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/sqf.min.js
--rw-r--r--   0 david     (1000) david     (1000)    12223 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/sql.min.js
--rw-r--r--   0 david     (1000) david     (1000)     6600 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/stan.min.js
--rw-r--r--   0 david     (1000) david     (1000)    16715 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/stata.min.js
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/step21.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4980 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/stylus.min.js
--rw-r--r--   0 david     (1000) david     (1000)      523 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/subunit.min.js
--rw-r--r--   0 david     (1000) david     (1000)     3666 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/swift.min.js
--rw-r--r--   0 david     (1000) david     (1000)      411 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/taggerscript.min.js
--rw-r--r--   0 david     (1000) david     (1000)      405 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/tap.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1699 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/tcl.min.js
--rw-r--r--   0 david     (1000) david     (1000)      627 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/thrift.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1479 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/tp.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1171 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/twig.min.js
--rw-r--r--   0 david     (1000) david     (1000)     6222 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/typescript.min.js
--rw-r--r--   0 david     (1000) david     (1000)      930 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/vala.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1835 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/vbnet.min.js
--rw-r--r--   0 david     (1000) david     (1000)      176 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/vbscript-html.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1709 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/vbscript.min.js
--rw-r--r--   0 david     (1000) david     (1000)     4882 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/verilog.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1674 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/vhdl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     8599 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/vim.min.js
--rw-r--r--   0 david     (1000) david     (1000)    19048 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/x86asm.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1641 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/xl.min.js
--rw-r--r--   0 david     (1000) david     (1000)     2024 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/xml.min.js
--rw-r--r--   0 david     (1000) david     (1000)     5289 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/xquery.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1750 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/yaml.min.js
--rw-r--r--   0 david     (1000) david     (1000)     1616 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/languages/zephir.min.js
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/
--rw-r--r--   0 david     (1000) david     (1000)      942 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/a11y-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      943 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/a11y-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1102 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/agate.min.css
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/an-old-hope.min.css
--rw-r--r--   0 david     (1000) david     (1000)      572 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/androidstudio.min.css
--rw-r--r--   0 david     (1000) david     (1000)      791 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/arduino-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      648 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/arta.min.css
--rw-r--r--   0 david     (1000) david     (1000)      415 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/ascetic.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-cave-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-cave-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-dune-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-dune-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-estuary-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-estuary-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-forest-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-forest-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-heath-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-heath-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-lakeside-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-lakeside-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-plateau-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-plateau-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-savanna-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      743 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-savanna-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-seaside-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-seaside-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-sulphurpool-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      587 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atelier-sulphurpool-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1157 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atom-one-dark-reasonable.min.css
--rw-r--r--   0 david     (1000) david     (1000)      792 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atom-one-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      792 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/atom-one-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      649 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/brown-paper.min.css
--rw-r--r--   0 david     (1000) david     (1000)    18198 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/brown-papersq.png
--rw-r--r--   0 david     (1000) david     (1000)      580 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/codepen-embed.min.css
--rw-r--r--   0 david     (1000) david     (1000)      610 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/color-brewer.min.css
--rw-r--r--   0 david     (1000) david     (1000)      706 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/darcula.min.css
--rw-r--r--   0 david     (1000) david     (1000)      598 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      763 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/default.min.css
--rw-r--r--   0 david     (1000) david     (1000)      817 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/docco.min.css
--rw-r--r--   0 david     (1000) david     (1000)      641 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/dracula.min.css
--rw-r--r--   0 david     (1000) david     (1000)      667 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/far.min.css
--rw-r--r--   0 david     (1000) david     (1000)      721 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/foundation.min.css
--rw-r--r--   0 david     (1000) david     (1000)      713 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/github-gist.min.css
--rw-r--r--   0 david     (1000) david     (1000)      854 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/github.min.css
--rw-r--r--   0 david     (1000) david     (1000)      742 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/gml.min.css
--rw-r--r--   0 david     (1000) david     (1000)      815 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/googlecode.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1026 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/gradient-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1039 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/gradient-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1670 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/grayscale.min.css
--rw-r--r--   0 david     (1000) david     (1000)      990 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/gruvbox-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      990 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/gruvbox-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      684 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/hopscotch.min.css
--rw-r--r--   0 david     (1000) david     (1000)      883 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/hybrid.min.css
--rw-r--r--   0 david     (1000) david     (1000)      867 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/idea.min.css
--rw-r--r--   0 david     (1000) david     (1000)      655 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/ir-black.min.css
--rw-r--r--   0 david     (1000) david     (1000)      934 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/isbl-editor-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      901 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/isbl-editor-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      632 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/kimbie.dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      632 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/kimbie.light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      798 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/lightfair.min.css
--rw-r--r--   0 david     (1000) david     (1000)      695 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/lioshi.min.css
--rw-r--r--   0 david     (1000) david     (1000)      603 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/magula.min.css
--rw-r--r--   0 david     (1000) david     (1000)      592 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/mono-blue.min.css
--rw-r--r--   0 david     (1000) david     (1000)      779 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/monokai-sublime.min.css
--rw-r--r--   0 david     (1000) david     (1000)      751 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/monokai.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1417 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/night-owl.min.css
--rw-r--r--   0 david     (1000) david     (1000)      914 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/nnfx-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      914 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/nnfx.min.css
--rw-r--r--   0 david     (1000) david     (1000)     2504 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/nord.min.css
--rw-r--r--   0 david     (1000) david     (1000)      830 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/obsidian.min.css
--rw-r--r--   0 david     (1000) david     (1000)      631 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/ocean.min.css
--rw-r--r--   0 david     (1000) david     (1000)      617 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/paraiso-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      617 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/paraiso-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1186 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/pojoaque.jpg
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/pojoaque.min.css
--rw-r--r--   0 david     (1000) david     (1000)      708 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/purebasic.min.css
--rw-r--r--   0 david     (1000) david     (1000)      771 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/qtcreator_dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/qtcreator_light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      918 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/railscasts.min.css
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/rainbow.min.css
--rw-r--r--   0 david     (1000) david     (1000)      839 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/routeros.min.css
--rw-r--r--   0 david     (1000) david     (1000)      781 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/school-book.min.css
--rw-r--r--   0 david     (1000) david     (1000)      486 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/school-book.png
--rw-r--r--   0 david     (1000) david     (1000)      815 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/shades-of-purple.min.css
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/solarized-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/solarized-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      732 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/srcery.min.css
--rw-r--r--   0 david     (1000) david     (1000)      846 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/stackoverflow-dark.min.css
--rw-r--r--   0 david     (1000) david     (1000)      855 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/stackoverflow-light.min.css
--rw-r--r--   0 david     (1000) david     (1000)      892 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/sunburst.min.css
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/tomorrow-night-blue.min.css
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/tomorrow-night-bright.min.css
--rw-r--r--   0 david     (1000) david     (1000)      613 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/tomorrow-night-eighties.min.css
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/tomorrow-night.min.css
--rw-r--r--   0 david     (1000) david     (1000)      628 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/tomorrow.min.css
--rw-r--r--   0 david     (1000) david     (1000)      601 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/vs.min.css
--rw-r--r--   0 david     (1000) david     (1000)     1056 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/vs2015.min.css
--rw-r--r--   0 david     (1000) david     (1000)      900 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/xcode.min.css
--rw-r--r--   0 david     (1000) david     (1000)      745 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/xt256.min.css
--rw-r--r--   0 david     (1000) david     (1000)      678 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/hl/styles/zenburn.min.css
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.450535 pyssg-0.8.3/pyssg.xyz/live/static/images/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/live/static/images/icons/
--rwxr-xr-x   0 david     (1000) david     (1000)      318 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/live/static/images/icons/favicon.ico
--rw-r--r--   0 david     (1000) david     (1000)       26 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/robots.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/live/static/scripts/
--rw-r--r--   0 david     (1000) david     (1000)      925 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/live/static/scripts/theme.js
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/plt/
--rw-r--r--   0 david     (1000) david     (1000)     1326 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/plt/base.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/plt/blog/
--rw-r--r--   0 david     (1000) david     (1000)     1993 2022-12-27 08:38:20.000000 pyssg-0.8.3/pyssg.xyz/plt/blog/index.html
--rw-r--r--   0 david     (1000) david     (1000)     1803 2022-12-27 08:39:33.000000 pyssg-0.8.3/pyssg.xyz/plt/blog/page.html
--rw-r--r--   0 david     (1000) david     (1000)     1875 2022-12-27 08:40:15.000000 pyssg-0.8.3/pyssg.xyz/plt/blog/tag.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/plt/body/
--rw-r--r--   0 david     (1000) david     (1000)      835 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/plt/body/footer.html
--rw-r--r--   0 david     (1000) david     (1000)      871 2022-12-27 08:21:29.000000 pyssg-0.8.3/pyssg.xyz/plt/body/header.html
--rw-r--r--   0 david     (1000) david     (1000)      351 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/plt/highlightjs.html
--rw-r--r--   0 david     (1000) david     (1000)     1344 2022-12-15 04:25:12.000000 pyssg-0.8.3/pyssg.xyz/plt/root_page.html
--rw-r--r--   0 david     (1000) david     (1000)     1610 2022-12-13 19:56:07.000000 pyssg-0.8.3/pyssg.xyz/plt/rss.xml
--rw-r--r--   0 david     (1000) david     (1000)      748 2022-12-13 02:21:07.000000 pyssg-0.8.3/pyssg.xyz/plt/sitemap.xml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/pyssg.xyz/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/src/blog/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/src/blog/a/
--rw-r--r--   0 david     (1000) david     (1000)      370 2022-12-15 04:34:52.000000 pyssg-0.8.3/pyssg.xyz/src/blog/a/second.md
--rw-r--r--   0 david     (1000) david     (1000)      352 2022-12-15 03:51:51.000000 pyssg-0.8.3/pyssg.xyz/src/blog/first.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/pyssg.xyz/src/pyssg.xyz/
--rw-r--r--   0 david     (1000) david     (1000)      101 2022-12-14 02:44:29.000000 pyssg-0.8.3/pyssg.xyz/src/pyssg.xyz/404.md
--rw-r--r--   0 david     (1000) david     (1000)      300 2022-12-27 08:23:02.000000 pyssg-0.8.3/pyssg.xyz/src/pyssg.xyz/index.md
--rw-r--r--   0 david     (1000) david     (1000)      120 2022-12-13 02:21:07.000000 pyssg-0.8.3/requirements.txt
--rw-r--r--   0 david     (1000) david     (1000)      791 2022-12-27 09:00:31.970535 pyssg-0.8.3/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      131 2022-12-13 19:56:07.000000 pyssg-0.8.3/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.460535 pyssg-0.8.3/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/src/pyssg/
--rw-r--r--   0 david     (1000) david     (1000)      468 2022-11-26 23:43:08.000000 pyssg-0.8.3/src/pyssg/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      226 2022-11-26 23:43:08.000000 pyssg-0.8.3/src/pyssg/__main__.py
--rw-r--r--   0 david     (1000) david     (1000)     1884 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/arg_parser.py
--rw-r--r--   0 david     (1000) david     (1000)     8452 2022-12-27 08:04:10.000000 pyssg-0.8.3/src/pyssg/builder.py
--rw-r--r--   0 david     (1000) david     (1000)     3363 2022-12-15 04:11:41.000000 pyssg-0.8.3/src/pyssg/configuration.py
--rw-r--r--   0 david     (1000) david     (1000)     4727 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/database.py
--rw-r--r--   0 david     (1000) david     (1000)     1321 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/database_entry.py
--rw-r--r--   0 david     (1000) david     (1000)     4330 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/md_parser.py
--rw-r--r--   0 david     (1000) david     (1000)     6042 2022-12-27 08:37:20.000000 pyssg-0.8.3/src/pyssg/page.py
--rw-r--r--   0 david     (1000) david     (1000)     1160 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/per_level_formatter.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.970535 pyssg-0.8.3/src/pyssg/plt/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-11-26 23:43:08.000000 pyssg-0.8.3/src/pyssg/plt/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      541 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/plt/default.yaml
--rw-r--r--   0 david     (1000) david     (1000)      778 2022-12-27 08:42:32.000000 pyssg-0.8.3/src/pyssg/plt/index.html
--rw-r--r--   0 david     (1000) david     (1000)      149 2022-12-27 07:21:45.000000 pyssg-0.8.3/src/pyssg/plt/mandatory_config.yaml
--rw-r--r--   0 david     (1000) david     (1000)      569 2022-12-27 08:43:07.000000 pyssg-0.8.3/src/pyssg/plt/page.html
--rw-r--r--   0 david     (1000) david     (1000)     1523 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/plt/rss.xml
--rw-r--r--   0 david     (1000) david     (1000)      748 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/plt/sitemap.xml
--rw-r--r--   0 david     (1000) david     (1000)      114 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/plt/static_config.yaml
--rw-r--r--   0 david     (1000) david     (1000)      676 2022-12-27 08:43:47.000000 pyssg-0.8.3/src/pyssg/plt/tag.html
--rw-r--r--   0 david     (1000) david     (1000)     4852 2022-12-15 03:58:52.000000 pyssg-0.8.3/src/pyssg/pyssg.py
--rw-r--r--   0 david     (1000) david     (1000)     3675 2022-12-27 08:05:18.000000 pyssg-0.8.3/src/pyssg/utils.py
--rw-r--r--   0 david     (1000) david     (1000)     1046 2022-12-13 02:21:07.000000 pyssg-0.8.3/src/pyssg/yaml_parser.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-27 09:00:31.960535 pyssg-0.8.3/src/pyssg.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)    10565 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)   190002 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       37 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-11-26 23:53:32.000000 pyssg-0.8.3/src/pyssg.egg-info/not-zip-safe
--rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/pbr.json
--rw-r--r--   0 david     (1000) david     (1000)      120 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        6 2022-12-27 09:00:31.000000 pyssg-0.8.3/src/pyssg.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.123201 pyssg-0.9.0/
+-rw-r--r--   0 david     (1000) david     (1000)    35149 2023-02-18 21:25:05.000000 pyssg-0.9.0/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)    11717 2023-05-02 06:28:39.123201 pyssg-0.9.0/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)    10363 2023-05-02 06:27:51.000000 pyssg-0.9.0/README.md
+-rwxr-xr-x   0 david     (1000) david     (1000)      233 2023-02-18 21:27:11.000000 pyssg-0.9.0/build_upload
+-rw-r--r--   0 david     (1000) david     (1000)      580 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/
+-rw-r--r--   0 david     (1000) david     (1000)      129 2023-02-18 21:27:11.000000 pyssg-0.9.0/pyssg.xyz/.rsyncignore
+-rwxr-xr-x   0 david     (1000) david     (1000)      409 2023-05-01 15:04:35.000000 pyssg-0.9.0/pyssg.xyz/bs
+-rw-r--r--   0 david     (1000) david     (1000)     1671 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/config.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      306 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/db.psv
+-rw-r--r--   0 david     (1000) david     (1000)      323 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/db_blog.psv
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.103201 pyssg-0.9.0/pyssg.xyz/live/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/live/blog/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/live/blog/a/
+-rw-r--r--   0 david     (1000) david     (1000)     3953 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/a/second.html
+-rw-r--r--   0 david     (1000) david     (1000)     3839 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/first.html
+-rw-r--r--   0 david     (1000) david     (1000)     3997 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/index.html
+-rw-r--r--   0 david     (1000) david     (1000)     4308 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/rss.xml
+-rw-r--r--   0 david     (1000) david     (1000)     1695 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/sitemap.xml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/live/blog/tag/
+-rw-r--r--   0 david     (1000) david     (1000)     3678 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/tag/@english.html
+-rw-r--r--   0 david     (1000) david     (1000)     3474 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/tag/@multiple-author.html
+-rw-r--r--   0 david     (1000) david     (1000)     3672 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/tag/@short.html
+-rw-r--r--   0 david     (1000) david     (1000)     3669 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/tag/@test.html
+-rw-r--r--   0 david     (1000) david     (1000)     3675 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/tag/@update.html
+-rw-r--r--   0 david     (1000) david     (1000)     4879 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/blog/toc_test.html
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/
+-rw-r--r--   0 david     (1000) david     (1000)     3050 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/404.html
+-rw-r--r--   0 david     (1000) david     (1000)     3518 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/index.html
+-rw-r--r--   0 david     (1000) david     (1000)      633 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/sitemap.xml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/plt/
+-rw-r--r--   0 david     (1000) david     (1000)     1448 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/plt/base.html
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/plt/blog/
+-rw-r--r--   0 david     (1000) david     (1000)     1993 2023-05-01 13:37:42.000000 pyssg-0.9.0/pyssg.xyz/plt/blog/index.html
+-rw-r--r--   0 david     (1000) david     (1000)     1803 2023-05-01 15:16:06.000000 pyssg-0.9.0/pyssg.xyz/plt/blog/page.html
+-rw-r--r--   0 david     (1000) david     (1000)     1875 2023-05-01 13:37:28.000000 pyssg-0.9.0/pyssg.xyz/plt/blog/tag.html
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/plt/body/
+-rw-r--r--   0 david     (1000) david     (1000)      835 2023-02-18 21:27:11.000000 pyssg-0.9.0/pyssg.xyz/plt/body/footer.html
+-rw-r--r--   0 david     (1000) david     (1000)      871 2023-02-18 21:27:11.000000 pyssg-0.9.0/pyssg.xyz/plt/body/header.html
+-rw-r--r--   0 david     (1000) david     (1000)      407 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/plt/highlightjs.html
+-rw-r--r--   0 david     (1000) david     (1000)     1344 2023-05-01 13:36:32.000000 pyssg-0.9.0/pyssg.xyz/plt/root_page.html
+-rw-r--r--   0 david     (1000) david     (1000)     1610 2023-05-01 13:36:57.000000 pyssg-0.9.0/pyssg.xyz/plt/rss.xml
+-rw-r--r--   0 david     (1000) david     (1000)      748 2023-05-01 13:26:49.000000 pyssg-0.9.0/pyssg.xyz/plt/sitemap.xml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.103201 pyssg-0.9.0/pyssg.xyz/src/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/src/blog/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/src/blog/a/
+-rw-r--r--   0 david     (1000) david     (1000)      370 2023-02-18 21:27:11.000000 pyssg-0.9.0/pyssg.xyz/src/blog/a/second.md
+-rw-r--r--   0 david     (1000) david     (1000)      352 2023-02-18 21:27:11.000000 pyssg-0.9.0/pyssg.xyz/src/blog/first.md
+-rw-r--r--   0 david     (1000) david     (1000)      480 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/src/blog/toc_test.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/pyssg.xyz/src/pyssg.xyz/
+-rw-r--r--   0 david     (1000) david     (1000)      101 2023-02-18 21:27:11.000000 pyssg-0.9.0/pyssg.xyz/src/pyssg.xyz/404.md
+-rw-r--r--   0 david     (1000) david     (1000)      429 2023-05-02 06:27:51.000000 pyssg-0.9.0/pyssg.xyz/src/pyssg.xyz/index.md
+-rw-r--r--   0 david     (1000) david     (1000)      156 2023-05-02 06:27:51.000000 pyssg-0.9.0/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)      123 2023-05-02 06:27:51.000000 pyssg-0.9.0/requirements_dev.txt
+-rw-r--r--   0 david     (1000) david     (1000)     1676 2023-05-02 06:28:39.123201 pyssg-0.9.0/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      131 2023-02-18 21:27:11.000000 pyssg-0.9.0/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.103201 pyssg-0.9.0/src/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/src/pyssg/
+-rw-r--r--   0 david     (1000) david     (1000)      218 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1884 2023-02-23 07:14:42.000000 pyssg-0.9.0/src/pyssg/arg_parser.py
+-rw-r--r--   0 david     (1000) david     (1000)     8438 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/builder.py
+-rw-r--r--   0 david     (1000) david     (1000)     4040 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/configuration.py
+-rw-r--r--   0 david     (1000) david     (1000)     1676 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/custom_logger.py
+-rw-r--r--   0 david     (1000) david     (1000)     5080 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/database.py
+-rw-r--r--   0 david     (1000) david     (1000)     1864 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/database_entry.py
+-rw-r--r--   0 david     (1000) david     (1000)     5622 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/md_parser.py
+-rw-r--r--   0 david     (1000) david     (1000)     4519 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/page.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/src/pyssg/plt/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-02-18 21:26:53.000000 pyssg-0.9.0/src/pyssg/plt/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      395 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/plt/default.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      778 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/index.html
+-rw-r--r--   0 david     (1000) david     (1000)      149 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/mandatory_config.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      569 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/page.html
+-rw-r--r--   0 david     (1000) david     (1000)     1523 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/rss.xml
+-rw-r--r--   0 david     (1000) david     (1000)      748 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/sitemap.xml
+-rw-r--r--   0 david     (1000) david     (1000)      114 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/static_config.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      676 2023-02-18 21:27:11.000000 pyssg-0.9.0/src/pyssg/plt/tag.html
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/py.typed
+-rw-r--r--   0 david     (1000) david     (1000)     4794 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/pyssg.py
+-rw-r--r--   0 david     (1000) david     (1000)     4120 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/utils.py
+-rw-r--r--   0 david     (1000) david     (1000)     1109 2023-05-02 06:27:51.000000 pyssg-0.9.0/src/pyssg/yaml_parser.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/src/pyssg.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)    11717 2023-05-02 06:28:38.000000 pyssg-0.9.0/src/pyssg.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     2736 2023-05-02 06:28:39.000000 pyssg-0.9.0/src/pyssg.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-02 06:28:38.000000 pyssg-0.9.0/src/pyssg.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       37 2023-05-02 06:28:38.000000 pyssg-0.9.0/src/pyssg.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-02-18 21:28:42.000000 pyssg-0.9.0/src/pyssg.egg-info/not-zip-safe
+-rw-r--r--   0 david     (1000) david     (1000)       47 2023-05-02 06:28:38.000000 pyssg-0.9.0/src/pyssg.egg-info/pbr.json
+-rw-r--r--   0 david     (1000) david     (1000)      156 2023-05-02 06:28:38.000000 pyssg-0.9.0/src/pyssg.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        6 2023-05-02 06:28:38.000000 pyssg-0.9.0/src/pyssg.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/tests/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     7344 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/conftest.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.113201 pyssg-0.9.0/tests/sample_files/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)       83 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/checksum.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.123201 pyssg-0.9.0/tests/sample_files/config/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      401 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/default.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      328 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/default_missing_dirs.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      432 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/default_missing_mandatory_key.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      337 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/default_missing_root_dir.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      793 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/multiple_default.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      735 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/config/multiple_default_one_doc_error.yaml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.123201 pyssg-0.9.0/tests/sample_files/md/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/md/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-02 06:28:39.123201 pyssg-0.9.0/tests/sample_files/md/a/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/md/a/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      320 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/md/a/second.md
+-rw-r--r--   0 david     (1000) david     (1000)      352 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/md/first.md
+-rw-r--r--   0 david     (1000) david     (1000)      196 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/sample_files/md/new.md
+-rw-r--r--   0 david     (1000) david     (1000)     1438 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_arg_parser.py
+-rw-r--r--   0 david     (1000) david     (1000)     4420 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_configuration.py
+-rw-r--r--   0 david     (1000) david     (1000)      759 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_custom_logger.py
+-rw-r--r--   0 david     (1000) david     (1000)     7795 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_database.py
+-rw-r--r--   0 david     (1000) david     (1000)     3713 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_database_entry.py
+-rw-r--r--   0 david     (1000) david     (1000)     2422 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_page.py
+-rw-r--r--   0 david     (1000) david     (1000)     6761 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_utils.py
+-rw-r--r--   0 david     (1000) david     (1000)      873 2023-05-02 06:27:51.000000 pyssg-0.9.0/tests/test_yaml_parser.py
```

### Comparing `pyssg-0.8.3/LICENSE` & `pyssg-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/PKG-INFO` & `pyssg-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,45 @@
-Metadata-Version: 2.1
-Name: pyssg
-Version: 0.8.3
-Summary: A Static Site Generator using markdown files
-Home-page: https://github.com/luevano/pyssg
-Author: David Luevano Alvarado
-Author-email: david@luevano.xyz
-License: GPLv3
-Keywords: python,static,site,generator,markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Unix
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 # pyssg - Static Site Generator written in Python
 
 Generates HTML files from MD files for a static site, personally using it for a blog-like site.
 
 Initially inspired by Roman Zolotarev's [`ssg5`](https://rgz.ee/bin/ssg5) and [`rssg`](https://rgz.ee/bin/rssg), Luke Smith's [`lb` and `sup`](https://github.com/LukeSmithxyz/lb) and, pedantic.software's [`blogit`](https://pedantic.software/git/blogit/).
 
 ## Features and to-do
 
-**NOTE:** WIP, there will be changes that will break the setup.
+**NOTE:** WIP, there will be changes that will break `pyssg` generations/config setup.
 
 - [x] Build static site parsing `markdown` files ( `*.md` -> `*.html`)
 	- [x] Uses [`jinja`](https://jinja.palletsprojects.com/en/3.0.x/) for templating.
 	- [x] Preserves hand-made `*.html` files.
 	- [x] Tag functionality, useful for blog-style sites.
-	- [ ] Open Graph (and similar) support.
-		- Technically, this works if you add the correct metadata to the `*.md` files and use the variables available for Jinja.
 - [x] Build `sitemap.xml` file.
 	- [ ] Include manually added `*.html` files.
 - [x] Build `rss.xml` file.
-	- [ ] Join the `static_url` to all relative URLs found to comply with the [RSS 2.0 spec](https://validator.w3.org/feed/docs/rss2.html).
-		- This would be added to the parsed HTML text extracted from the MD files, so it would be available to the created `*.html` and `*.xml` files. Note that depending on the reader, it will append the URL specified in the RSS file or use the [`xml:base`](https://www.rssboard.org/news/151/relative-links) specified (for example, [newsboat](https://newsboat.org/) parses `xml:base`).
 	- [ ] Include manually added `*.html` files.
 - [x] YAML for configuration file, uses [`PyYAML`](https://pyyaml.org/).
-	- [ ] Handle multiple "documents".
-	- [ ] More complex directory structure to support multiple subdomains and different types of pages.
+	- [x] Support for multiple "documents". `PyYAML` supports this. In `pyssg` context, it means it can generate multiple websites (I personally use it for subdomains).
+	- [x] Support for more complex directory structure to support configuration on a per directory basis.
+- [x] File checksum checking for modification of files.
 - [ ] Option/change to using an SQL database instead of the custom solution.
-- [x] Checksum checking because the timestamp of the file is not enough.
 - [ ] Use external markdown extensions.
+  - [x] So far only extension configuration is for my own extension [pymdvar](https://github.com/luevano/pymdvar).
 
 ### Markdown features
 
 This program uses the base [`markdown` syntax](https://daringfireball.net/projects/markdown/syntax) plus additional syntax, all thanks to [`python-markdown`](https://python-markdown.github.io/) that provides [extensions](https://python-markdown.github.io/extensions/). The following extensions are used:
 
 - Extra (collection of QoL extensions).
 - Meta-Data.
 - Sane Lists.
 - SmartyPants.
 - Table of Contents.
+  - With `permalink=True` and `baselevel=2`, for more: [python-markdown toc](https://python-markdown.github.io/extensions/toc/).
 - WikiLinks.
+- [pymdvar](https://github.com/luevano/pymdvar) (made by me).
 - [yafg - Yet Another Figure Generator](https://git.sr.ht/~ferruck/yafg)
 - [Markdown Checklist](https://github.com/FND/markdown-checklist)
 - [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/)
 	- [Caret](https://facelessuser.github.io/pymdown-extensions/extensions/caret/)
 	- [Tilde](https://facelessuser.github.io/pymdown-extensions/extensions/tilde/)
 	- [Mark](https://facelessuser.github.io/pymdown-extensions/extensions/mark/)
 
@@ -92,15 +73,15 @@
 pyssg -i
 ```
 
 - You can modify the basic templates as needed (see [variables available for Jinja](#available-jinja-variables)).
 
 - Strongly recommended to edit the `rss.xml` template.
 
-4. Place your `*.md` files somewhere inside the source directory. It accepts sub-directories.
+4. Place your `*.md` files somewhere inside the source directory. It accepts sub-directories. Optionally configure for subdirectories if they are to be treated a bit different.
 
 - Recommended (no longer mandatory) metadata keys that can be added to the top of `.md` files:
 
 ```
 title: the title of your blog entry or whatever
 author: your name or online handle
 	another name maybe for multiple authors?
@@ -108,34 +89,36 @@
 summary: a summary of the entry
 tags: english
 	short
 	tutorial
 	etc
 ```
 
-- You can add more meta-data keys as long as it is [Python-Markdown compliant](https://python-markdown.github.io/extensions/meta_data/), and these will ve [available as Jinja variables](#available-jinja-variables).
+- You can add more meta-data keys as long as it is [Python-Markdown compliant](https://python-markdown.github.io/extensions/meta_data/), and these will ve [available as Jinja variables](#available-jinja-variables) in the `meta` object (`dict[str, Any]`).
 
 5. Build the `*.html` with:
 
 ```sh
 pyssg -b
 ```
 
-- After this, you have ready to deploy `*.html` files.
+- After this, you have ready to deploy `*.html` files from the `dst` directory.
 
 ## Config file
 
 All sections/options need to be compliant with [`PyYAML`](https://pyyaml.org/) which should be compliant with [`YAML 1.2`](https://yaml.org/spec/1.2.2/). Additionaly, I've added the custom tag `!join` which concatenates strings from an array, which an be used as follows:
 
 ```yaml
 variable: &variable_reference_name "value"
 other_variable: !join [*variable_reference_name, "other_value", 1]
 ```
 
-Which would produce `other_variable: "valueother_value1"`. Also environment variables will be expanded internally.
+Which would produce `other_variable: "valueother_value1"`. Also **environment variables will be expanded internally**.
+
+**Note**: URL's shouldn't have the trailing slash `/`.
 
 The following is a list of config items that need to be present in the config unless stated otherwise:
 
 ```yaml
 %YAML 1.2
 ---
 # not needed, shown here as an example of the !join tag
@@ -145,87 +128,114 @@
 path:
   src: !join [*root, "src"] # $HOME/path/to/src
   dst: "$HOME/some/other/path/to/dst"
   plt: "plt"
   db: !join [*root, "src/", "db.psv"]
 url:
   main: "https://example.com"
+  # I personally use a "static" url for images/scripts/css/etc, not necessary
+  static: "https://static.example.com"
 fmt:
   date: "%a, %b %d, %Y @ %H:%M %Z"
-  list_date: "%b %d"
-  list_sep_date: "%B %Y"
+  list_date: "%b %d" # not necessary
+  list_sep_date: "%B %Y" # not necessary
 dirs:
   /: # root "dir_path", whatever is sitting directly under "src"
-	cfg:
-	  plt: "page.html"
-	  # the template can be specified instead of just True/False, a default template will used
-	  tags: False
-	  index: True
-	  rss: True
-	  sitemap: True
-	  exclude_dirs: ["articles", "blog"] # optional; list of subdirectories to exclude when parsing the / dir_path
-# below are other example "dir_paths", can be named anything, only the / (above) is mandatory
-  articles:
     cfg:
-	  plt: "page.html"
-	  tags: True
-	  index: True
-	  rss: True
-	  sitemap: True
-  blog:
-    cfg:
-	  # ...
+      plt: "page.html" # each page template, relative to path/plt
+      tags: False
+      index: True
+      rss: True
+      sitemap: True
+      exclude_dirs: ["articles", "blog"] # optional; list of subdirs to exclude when parsing this "dir_path"
 ...
 ```
 
-The config under `dirs` are just per-subdirectory configuration of directories under `src`. Only the `/` "dir_path" is required as it is the config for the root `src` path files.
+So far only [pymdvar](https://github.com/luevano/pymdvar) can be configured by including the following to the config:
+
+```yaml
+exts:
+  pymdvar:
+    variables:
+      SOME_VAR: "some value"
+      some_other_variable: 123
+    enable_env: True # to read environment variables
+```
+
+The config under `dirs` are just per-subdirectory configuration of directories under `src`, which I called "dir_paths" for lack of creativity. Only the `/` "dir_path" is required as it is the config for the root `src` path files. Mandatory config items for each "dir_path":
+
+```yaml
+cfg:
+  plt: "template.html"
+  tags: True
+  index: True
+  rss: True
+  sitemap: True
+  exclude: [] # not necessary
+```
+
+So that extra "dir_paths" can be added under `dirs`:
 
-The following will be added on runtime:
+```yaml
+dirs:
+  /:
+    cfg:
+      ...
+  articles:
+    cfg:
+      ...
+  gallery:
+    cfg:
+      ...
+  etc:
+    ...
+```
+
+The following will be added on runtime to the configuration:
 
 ```yaml
 %YAML 1.2
 ---
 fmt:
   rss_date: "%a, %d %b %Y %H:%M:%S GMT" # fixed
   sitemap_date: "%Y-%m-%d" # fixed
 info:
   version: "x.y.z" # current 'pyssg' version (0.5.1.dev16, for example)
   debug: True/False # depending if --debug was used when executing
-  force: True/False # depending if --force was used when executing
 rss_run_date: # date the program was run, formatted with 'fmt.rss_date'
 sitemap_run_date: # date the program was run, formatted with 'fmt.sitemap_date'
 ...
 ```
 
-You can add any other option/section that you can later use in the Jinja templates via the exposed config object. URL's shouldn't have the trailing slash `/`
+You can add any other option/section that you can later use in the Jinja templates via the exposed config object.
+
 
 ## Available Jinja variables
 
 These variables are exposed to use within the templates. The below list is displayed in the form of *variable (type) (available from): description*. `field1/field2/field3/...` describe config file section from the YAML file and option and `object.attribute` corresponding object and it's attribute.
 
-- `config` (`dict`) (all): parsed config file plus the added options internally (as described in [config file](#config-file)).
-- `dir_config` (`dict`) (all*): parsed dir_config file plus the added options internally (as described in [config file](#config-file)). *This is for all of the specific "dir_path" files, as per configured in the YAML file `dirs.dir_path.cfg` (for exmaple `dirs./.cfg` for the required dir_path).
+- `config` (`dict[str, Any]`) (all): parsed config file plus the added options internally (as described in [config file](#config-file)).
+- `dir_config` (`dict[str, Any]`) (all*): parsed dir_config file plus the added options internally (as described in [config file](#config-file)). *This is for all of the specific "dir_path" files, as per configured in the YAML file `dirs.dir_path.cfg` (for exmaple `dirs./.cfg` for the required dir_path).
 - `all_pages` (`list(Page)`) (all): list of all the pages, sorted by creation time, reversed.
 - `page` (`Page`) (`page.html`): contains the following attributes (genarally these are parsed from the metadata in the `*.md` files):
 	- `title` (`str`): title of the page.
 	- `author` (`list[str]`): list of authors of the page.
 	- `lang` (`str`): page language, used for the general `html` tag `lang` attribute.
 	- `summary` (`str`): summary of the page, as specified in the `*.md` file.
 	- `content` (`str`): actual content of the page, this is the `html`.
+    - `toc` (`str`): table of contents as taken from `md.toc`.
+    - `toc_tokens` (`list[dict[str, Any]]`): table of contents tokens as taken from `md.toc_tokens`.
 	- `cdatetime` (`datetime.datetime`): creation datetime object of the page.
-	- `cdate` (`method`): method thtat takes the name of the `fmt.FMT` and applies it to the `cdatetime` object.
+	- `cdate` (`method(FMT: str)`): takes the name of the `fmt.FMT` and applies it to the `cdatetime` object.
 	- `cdate_rss` (`str`): formatted `cdatetime` as required by rss.
 	- `cdate_sitemap` (`str`): formatted `cdatetime` as required by sitemap.
 	- `mdatetime` (`datetime.datetime`): modification datetime object of the page. Defaults to `None`.
-	- `mdate` (`method`): method thtat takes the name of the `fmt.FMT` and applies it to the `mdatetime` object.
+	- `mdate` (`method(FMT: str)`): takes the name of the `fmt.FMT` and applies it to the `mdatetime` object.
 	- `mdate_rss` (`str`): formatted `mdatetime` as required by rss.
 	- `mdate_sitemap` (`str`): formatted `mdatetime` as required by sitemap.
-	- `tags` (`list(tuple(str))`): list of tuple of tags of the page, containing the name and the url of the tag, in that order. Defaults to empty list.
+	- `tags` (`list[tuple[str]]`): list of tuple of tags of the page, containing the name and the url of the tag, respectively. Defaults to empty list.
 	- `url` (`str`): url of the page, this already includes the `url/main` from config file.
-	- `image_url` (`str`): image url of the page, this already includes the `url/static`. Defaults to the `url/default_image` config option.
 	- `next/previous` (`Page`): reference to the next or previous page object (containing all these attributes). Defaults to `None`.
-	- `og` (`dict(str, str)`): dict for object graph metadata.
-	- `meta` (`dict(str, list(str))`): meta dict as obtained from python-markdown, in case you use a meta tag not yet supported, it will be available there.
-- `tag` (`tuple(str)`) (`tag.html`): tuple of name and url of the current tag.
-- `tag_pages` (`list(Page)`) (`tag.html`): similar to `all_pages` but contains all the pages for the current tag.
-- `all_tags` (`list(tuple(str))`) (all): similar to `page.tags` but contains all the tags.
-
+	- `meta` (`dict[str, list[str]]`): meta dict as obtained from `python-markdown`, in case you use a meta tag not directly supported, it will be available there.
+- `tag` (`tuple[str]`) (`tag.html`): tuple of name and url of the current tag.
+- `tag_pages` (`list[Page]`) (`tag.html`): similar to `all_pages` but contains all the pages for the current tag.
+- `all_tags` (`list[tuple[str]]`) (all): similar to `page.tags` but contains all the tags.
```

### Comparing `pyssg-0.8.3/README.md` & `pyssg-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,75 @@
+Metadata-Version: 2.1
+Name: pyssg
+Version: 0.9.0
+Summary: A Static Site Generator using markdown files.
+Home-page: https://github.com/luevano/pyssg
+Author: David Luevano Alvarado
+Author-email: david@luevano.xyz
+License: GPLv3
+Keywords: python,static,site,generator,markdown,website
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications :: Email :: Filters
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Filters
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyssg - Static Site Generator written in Python
 
 Generates HTML files from MD files for a static site, personally using it for a blog-like site.
 
 Initially inspired by Roman Zolotarev's [`ssg5`](https://rgz.ee/bin/ssg5) and [`rssg`](https://rgz.ee/bin/rssg), Luke Smith's [`lb` and `sup`](https://github.com/LukeSmithxyz/lb) and, pedantic.software's [`blogit`](https://pedantic.software/git/blogit/).
 
 ## Features and to-do
 
-**NOTE:** WIP, there will be changes that will break the setup.
+**NOTE:** WIP, there will be changes that will break `pyssg` generations/config setup.
 
 - [x] Build static site parsing `markdown` files ( `*.md` -> `*.html`)
 	- [x] Uses [`jinja`](https://jinja.palletsprojects.com/en/3.0.x/) for templating.
 	- [x] Preserves hand-made `*.html` files.
 	- [x] Tag functionality, useful for blog-style sites.
-	- [ ] Open Graph (and similar) support.
-		- Technically, this works if you add the correct metadata to the `*.md` files and use the variables available for Jinja.
 - [x] Build `sitemap.xml` file.
 	- [ ] Include manually added `*.html` files.
 - [x] Build `rss.xml` file.
-	- [ ] Join the `static_url` to all relative URLs found to comply with the [RSS 2.0 spec](https://validator.w3.org/feed/docs/rss2.html).
-		- This would be added to the parsed HTML text extracted from the MD files, so it would be available to the created `*.html` and `*.xml` files. Note that depending on the reader, it will append the URL specified in the RSS file or use the [`xml:base`](https://www.rssboard.org/news/151/relative-links) specified (for example, [newsboat](https://newsboat.org/) parses `xml:base`).
 	- [ ] Include manually added `*.html` files.
 - [x] YAML for configuration file, uses [`PyYAML`](https://pyyaml.org/).
-	- [ ] Handle multiple "documents".
-	- [ ] More complex directory structure to support multiple subdomains and different types of pages.
+	- [x] Support for multiple "documents". `PyYAML` supports this. In `pyssg` context, it means it can generate multiple websites (I personally use it for subdomains).
+	- [x] Support for more complex directory structure to support configuration on a per directory basis.
+- [x] File checksum checking for modification of files.
 - [ ] Option/change to using an SQL database instead of the custom solution.
-- [x] Checksum checking because the timestamp of the file is not enough.
 - [ ] Use external markdown extensions.
+  - [x] So far only extension configuration is for my own extension [pymdvar](https://github.com/luevano/pymdvar).
 
 ### Markdown features
 
 This program uses the base [`markdown` syntax](https://daringfireball.net/projects/markdown/syntax) plus additional syntax, all thanks to [`python-markdown`](https://python-markdown.github.io/) that provides [extensions](https://python-markdown.github.io/extensions/). The following extensions are used:
 
 - Extra (collection of QoL extensions).
 - Meta-Data.
 - Sane Lists.
 - SmartyPants.
 - Table of Contents.
+  - With `permalink=True` and `baselevel=2`, for more: [python-markdown toc](https://python-markdown.github.io/extensions/toc/).
 - WikiLinks.
+- [pymdvar](https://github.com/luevano/pymdvar) (made by me).
 - [yafg - Yet Another Figure Generator](https://git.sr.ht/~ferruck/yafg)
 - [Markdown Checklist](https://github.com/FND/markdown-checklist)
 - [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/)
 	- [Caret](https://facelessuser.github.io/pymdown-extensions/extensions/caret/)
 	- [Tilde](https://facelessuser.github.io/pymdown-extensions/extensions/tilde/)
 	- [Mark](https://facelessuser.github.io/pymdown-extensions/extensions/mark/)
 
@@ -74,15 +103,15 @@
 pyssg -i
 ```
 
 - You can modify the basic templates as needed (see [variables available for Jinja](#available-jinja-variables)).
 
 - Strongly recommended to edit the `rss.xml` template.
 
-4. Place your `*.md` files somewhere inside the source directory. It accepts sub-directories.
+4. Place your `*.md` files somewhere inside the source directory. It accepts sub-directories. Optionally configure for subdirectories if they are to be treated a bit different.
 
 - Recommended (no longer mandatory) metadata keys that can be added to the top of `.md` files:
 
 ```
 title: the title of your blog entry or whatever
 author: your name or online handle
 	another name maybe for multiple authors?
@@ -90,34 +119,36 @@
 summary: a summary of the entry
 tags: english
 	short
 	tutorial
 	etc
 ```
 
-- You can add more meta-data keys as long as it is [Python-Markdown compliant](https://python-markdown.github.io/extensions/meta_data/), and these will ve [available as Jinja variables](#available-jinja-variables).
+- You can add more meta-data keys as long as it is [Python-Markdown compliant](https://python-markdown.github.io/extensions/meta_data/), and these will ve [available as Jinja variables](#available-jinja-variables) in the `meta` object (`dict[str, Any]`).
 
 5. Build the `*.html` with:
 
 ```sh
 pyssg -b
 ```
 
-- After this, you have ready to deploy `*.html` files.
+- After this, you have ready to deploy `*.html` files from the `dst` directory.
 
 ## Config file
 
 All sections/options need to be compliant with [`PyYAML`](https://pyyaml.org/) which should be compliant with [`YAML 1.2`](https://yaml.org/spec/1.2.2/). Additionaly, I've added the custom tag `!join` which concatenates strings from an array, which an be used as follows:
 
 ```yaml
 variable: &variable_reference_name "value"
 other_variable: !join [*variable_reference_name, "other_value", 1]
 ```
 
-Which would produce `other_variable: "valueother_value1"`. Also environment variables will be expanded internally.
+Which would produce `other_variable: "valueother_value1"`. Also **environment variables will be expanded internally**.
+
+**Note**: URL's shouldn't have the trailing slash `/`.
 
 The following is a list of config items that need to be present in the config unless stated otherwise:
 
 ```yaml
 %YAML 1.2
 ---
 # not needed, shown here as an example of the !join tag
@@ -127,86 +158,115 @@
 path:
   src: !join [*root, "src"] # $HOME/path/to/src
   dst: "$HOME/some/other/path/to/dst"
   plt: "plt"
   db: !join [*root, "src/", "db.psv"]
 url:
   main: "https://example.com"
+  # I personally use a "static" url for images/scripts/css/etc, not necessary
+  static: "https://static.example.com"
 fmt:
   date: "%a, %b %d, %Y @ %H:%M %Z"
-  list_date: "%b %d"
-  list_sep_date: "%B %Y"
+  list_date: "%b %d" # not necessary
+  list_sep_date: "%B %Y" # not necessary
 dirs:
   /: # root "dir_path", whatever is sitting directly under "src"
-	cfg:
-	  plt: "page.html"
-	  # the template can be specified instead of just True/False, a default template will used
-	  tags: False
-	  index: True
-	  rss: True
-	  sitemap: True
-	  exclude_dirs: ["articles", "blog"] # optional; list of subdirectories to exclude when parsing the / dir_path
-# below are other example "dir_paths", can be named anything, only the / (above) is mandatory
-  articles:
     cfg:
-	  plt: "page.html"
-	  tags: True
-	  index: True
-	  rss: True
-	  sitemap: True
-  blog:
-    cfg:
-	  # ...
+      plt: "page.html" # each page template, relative to path/plt
+      tags: False
+      index: True
+      rss: True
+      sitemap: True
+      exclude_dirs: ["articles", "blog"] # optional; list of subdirs to exclude when parsing this "dir_path"
 ...
 ```
 
-The config under `dirs` are just per-subdirectory configuration of directories under `src`. Only the `/` "dir_path" is required as it is the config for the root `src` path files.
+So far only [pymdvar](https://github.com/luevano/pymdvar) can be configured by including the following to the config:
+
+```yaml
+exts:
+  pymdvar:
+    variables:
+      SOME_VAR: "some value"
+      some_other_variable: 123
+    enable_env: True # to read environment variables
+```
+
+The config under `dirs` are just per-subdirectory configuration of directories under `src`, which I called "dir_paths" for lack of creativity. Only the `/` "dir_path" is required as it is the config for the root `src` path files. Mandatory config items for each "dir_path":
+
+```yaml
+cfg:
+  plt: "template.html"
+  tags: True
+  index: True
+  rss: True
+  sitemap: True
+  exclude: [] # not necessary
+```
+
+So that extra "dir_paths" can be added under `dirs`:
 
-The following will be added on runtime:
+```yaml
+dirs:
+  /:
+    cfg:
+      ...
+  articles:
+    cfg:
+      ...
+  gallery:
+    cfg:
+      ...
+  etc:
+    ...
+```
+
+The following will be added on runtime to the configuration:
 
 ```yaml
 %YAML 1.2
 ---
 fmt:
   rss_date: "%a, %d %b %Y %H:%M:%S GMT" # fixed
   sitemap_date: "%Y-%m-%d" # fixed
 info:
   version: "x.y.z" # current 'pyssg' version (0.5.1.dev16, for example)
   debug: True/False # depending if --debug was used when executing
-  force: True/False # depending if --force was used when executing
 rss_run_date: # date the program was run, formatted with 'fmt.rss_date'
 sitemap_run_date: # date the program was run, formatted with 'fmt.sitemap_date'
 ...
 ```
 
-You can add any other option/section that you can later use in the Jinja templates via the exposed config object. URL's shouldn't have the trailing slash `/`
+You can add any other option/section that you can later use in the Jinja templates via the exposed config object.
+
 
 ## Available Jinja variables
 
 These variables are exposed to use within the templates. The below list is displayed in the form of *variable (type) (available from): description*. `field1/field2/field3/...` describe config file section from the YAML file and option and `object.attribute` corresponding object and it's attribute.
 
-- `config` (`dict`) (all): parsed config file plus the added options internally (as described in [config file](#config-file)).
-- `dir_config` (`dict`) (all*): parsed dir_config file plus the added options internally (as described in [config file](#config-file)). *This is for all of the specific "dir_path" files, as per configured in the YAML file `dirs.dir_path.cfg` (for exmaple `dirs./.cfg` for the required dir_path).
+- `config` (`dict[str, Any]`) (all): parsed config file plus the added options internally (as described in [config file](#config-file)).
+- `dir_config` (`dict[str, Any]`) (all*): parsed dir_config file plus the added options internally (as described in [config file](#config-file)). *This is for all of the specific "dir_path" files, as per configured in the YAML file `dirs.dir_path.cfg` (for exmaple `dirs./.cfg` for the required dir_path).
 - `all_pages` (`list(Page)`) (all): list of all the pages, sorted by creation time, reversed.
 - `page` (`Page`) (`page.html`): contains the following attributes (genarally these are parsed from the metadata in the `*.md` files):
 	- `title` (`str`): title of the page.
 	- `author` (`list[str]`): list of authors of the page.
 	- `lang` (`str`): page language, used for the general `html` tag `lang` attribute.
 	- `summary` (`str`): summary of the page, as specified in the `*.md` file.
 	- `content` (`str`): actual content of the page, this is the `html`.
+    - `toc` (`str`): table of contents as taken from `md.toc`.
+    - `toc_tokens` (`list[dict[str, Any]]`): table of contents tokens as taken from `md.toc_tokens`.
 	- `cdatetime` (`datetime.datetime`): creation datetime object of the page.
-	- `cdate` (`method`): method thtat takes the name of the `fmt.FMT` and applies it to the `cdatetime` object.
+	- `cdate` (`method(FMT: str)`): takes the name of the `fmt.FMT` and applies it to the `cdatetime` object.
 	- `cdate_rss` (`str`): formatted `cdatetime` as required by rss.
 	- `cdate_sitemap` (`str`): formatted `cdatetime` as required by sitemap.
 	- `mdatetime` (`datetime.datetime`): modification datetime object of the page. Defaults to `None`.
-	- `mdate` (`method`): method thtat takes the name of the `fmt.FMT` and applies it to the `mdatetime` object.
+	- `mdate` (`method(FMT: str)`): takes the name of the `fmt.FMT` and applies it to the `mdatetime` object.
 	- `mdate_rss` (`str`): formatted `mdatetime` as required by rss.
 	- `mdate_sitemap` (`str`): formatted `mdatetime` as required by sitemap.
-	- `tags` (`list(tuple(str))`): list of tuple of tags of the page, containing the name and the url of the tag, in that order. Defaults to empty list.
+	- `tags` (`list[tuple[str]]`): list of tuple of tags of the page, containing the name and the url of the tag, respectively. Defaults to empty list.
 	- `url` (`str`): url of the page, this already includes the `url/main` from config file.
-	- `image_url` (`str`): image url of the page, this already includes the `url/static`. Defaults to the `url/default_image` config option.
 	- `next/previous` (`Page`): reference to the next or previous page object (containing all these attributes). Defaults to `None`.
-	- `og` (`dict(str, str)`): dict for object graph metadata.
-	- `meta` (`dict(str, list(str))`): meta dict as obtained from python-markdown, in case you use a meta tag not yet supported, it will be available there.
-- `tag` (`tuple(str)`) (`tag.html`): tuple of name and url of the current tag.
-- `tag_pages` (`list(Page)`) (`tag.html`): similar to `all_pages` but contains all the pages for the current tag.
-- `all_tags` (`list(tuple(str))`) (all): similar to `page.tags` but contains all the tags.
+	- `meta` (`dict[str, list[str]]`): meta dict as obtained from `python-markdown`, in case you use a meta tag not directly supported, it will be available there.
+- `tag` (`tuple[str]`) (`tag.html`): tuple of name and url of the current tag.
+- `tag_pages` (`list[Page]`) (`tag.html`): similar to `all_pages` but contains all the pages for the current tag.
+- `all_tags` (`list[tuple[str]]`) (all): similar to `page.tags` but contains all the tags.
+
```

### Comparing `pyssg-0.8.3/pyssg.xyz/config.yaml` & `pyssg-0.9.0/pyssg.xyz/config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 path:
   src: !join [*root_path, "src/pyssg.xyz"]
   dst: !join [*root_path, "live/pyssg.xyz"]
   plt: !join [*root_path, "plt"]
   db: !join [*root_path, "db.psv"]
 url:
   main: "https://pyssg.xyz"
-  static: "https://static.pyssg.xyz"
+  static: "https://static.luevano.xyz"
   default_image: "images/default.png"
 fmt:
   date: "%a, %b %d, %Y @ %H:%M %Z"
   list_date: "%b %d"
   list_sep_date: "%B %Y"
 dirs:
   /:
     cfg:
       plt: "root_page.html"
       tags: False
       index: False
       rss: False
       sitemap: True
       exclude_dirs: []
+exts:
+  pymdvar:
+    variables:
+      SURL: "https://static.luevano.xyz"
+    enable_env: False
 ...
 ---
 define: &root_path "$HOME/pyssg/pyssg.xyz/"
 
 title: "pyssg blog"
 author: "David Luévano Alvarado"
 author_email: "david@luevano.xyz"
@@ -41,23 +46,28 @@
 path:
   src: !join [*root_path, "src/blog"]
   dst: !join [*root_path, "live/blog"]
   plt: !join [*root_path, "plt"]
   db: !join [*root_path, "db_blog.psv"]
 url:
   main: "https://blog.pyssg.xyz"
-  static: "https://static.pyssg.xyz"
+  static: "https://static.luevano.xyz"
   default_image: "images/default.png"
 fmt:
   date: "%a, %b %d, %Y @ %H:%M %Z"
   list_date: "%b %d"
   list_sep_date: "%B %Y"
 dirs:
   /:
     cfg:
       plt: "blog/page.html"
       tags: "blog/tag.html"
       index: "blog/index.html"
       rss: True
       sitemap: True
       exclude_dirs: []
+exts:
+  pymdvar:
+    variables:
+      SURL: "https://static.luevano.xyz"
+    enable_env: False
 ...
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/a/second.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/first.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
-<title>Second blog post for testing purposes -- pyssg blog</title>
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
+<title>First blog post for testing purposes -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
-  <meta property="og:url" content="https://blog.pyssg.xyz/a/second.md"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:url" content="https://blog.pyssg.xyz/first.md"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -53,26 +52,23 @@
 </nav>
 
 <button class="theme-switcher" onclick="toggleTheme()"><i class="fas fa-moon"></i><i class="fas fa-sun"></i></button>
 
     </header>
 
     <main>
-  <h1>Second blog post for testing purposes</h1>
+  <h1>First blog post for testing purposes</h1>
 
-  <p>By David Luévano, Someone Else</p>
-  <p>Created: Thu, Dec 15, 2022 @ 04:17 UTC</p>
-    <p>Modified: Thu, Dec 15, 2022 @ 04:34 UTC</p>
+  <p>By David Luévano</p>
+  <p>Created: Thu, Dec 15, 2022 @ 03:51 UTC</p>
 
-  <p>A second &ldquo;blog entry&rdquo; for testing purposes which uses multiple authors and is inside a subdirectory.</p>
-<p>Added a modification here after first submission.</p>
+  <p>Even though I have this &ldquo;blog&rdquo; subdomain and page setup, doesn&rsquo;t mean I&rsquo;ll be blogging for pyssg, this is just to serve as an example for the types of sites that pyssg can be used for.</p>
 
 <p>Tags: 
   <a href="https://blog.pyssg.xyz/tag/@english.html">english</a>, 
-  <a href="https://blog.pyssg.xyz/tag/@multiple-author.html">multiple-author</a>, 
   <a href="https://blog.pyssg.xyz/tag/@short.html">short</a>, 
   <a href="https://blog.pyssg.xyz/tag/@test.html">test</a>, 
   <a href="https://blog.pyssg.xyz/tag/@update.html">update</a>
 </p>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,23 +10,21 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
-****** Second blog post for testing purposes ******
-By David LuÃ©vano, Someone Else
-Created: Thu, Dec 15, 2022 @ 04:17 UTC
-Modified: Thu, Dec 15, 2022 @ 04:34 UTC
-A second “blog entry” for testing purposes which uses multiple authors and is
-inside a subdirectory.
-Added a modification here after first submission.
-Tags: english, multiple-author, short, test, update
+****** First blog post for testing purposes ******
+By David LuÃ©vano
+Created: Thu, Dec 15, 2022 @ 03:51 UTC
+Even though I have this “blog” subdomain and page setup, doesn’t mean I’ll be
+blogging for pyssg, this is just to serve as an example for the types of sites
+that pyssg can be used for.
+Tags: english, short, test, update
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/first.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/a/second.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
-<title>First blog post for testing purposes -- pyssg blog</title>
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
+<title>Second blog post for testing purposes -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
-  <meta property="og:url" content="https://blog.pyssg.xyz/first.md"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:url" content="https://blog.pyssg.xyz/a/second.md"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -53,23 +52,26 @@
 </nav>
 
 <button class="theme-switcher" onclick="toggleTheme()"><i class="fas fa-moon"></i><i class="fas fa-sun"></i></button>
 
     </header>
 
     <main>
-  <h1>First blog post for testing purposes</h1>
+  <h1>Second blog post for testing purposes</h1>
 
-  <p>By David Luévano</p>
-  <p>Created: Thu, Dec 15, 2022 @ 03:51 UTC</p>
+  <p>By David Luévano, Someone Else</p>
+  <p>Created: Thu, Dec 15, 2022 @ 04:17 UTC</p>
+    <p>Modified: Thu, Dec 15, 2022 @ 04:34 UTC</p>
 
-  <p>Even though I have this &ldquo;blog&rdquo; subdomain and page setup, doesn&rsquo;t mean I&rsquo;ll be blogging for pyssg, this is just to serve as an example for the types of sites that pyssg can be used for.</p>
+  <p>A second &ldquo;blog entry&rdquo; for testing purposes which uses multiple authors and is inside a subdirectory.</p>
+<p>Added a modification here after first submission.</p>
 
 <p>Tags: 
   <a href="https://blog.pyssg.xyz/tag/@english.html">english</a>, 
+  <a href="https://blog.pyssg.xyz/tag/@multiple-author.html">multiple-author</a>, 
   <a href="https://blog.pyssg.xyz/tag/@short.html">short</a>, 
   <a href="https://blog.pyssg.xyz/tag/@test.html">test</a>, 
   <a href="https://blog.pyssg.xyz/tag/@update.html">update</a>
 </p>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,22 +10,22 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
-****** First blog post for testing purposes ******
-By David LuÃ©vano
-Created: Thu, Dec 15, 2022 @ 03:51 UTC
-Even though I have this “blog” subdomain and page setup, doesn’t mean I’ll be
-blogging for pyssg, this is just to serve as an example for the types of sites
-that pyssg can be used for.
-Tags: english, short, test, update
+****** Second blog post for testing purposes ******
+By David LuÃ©vano, Someone Else
+Created: Thu, Dec 15, 2022 @ 04:17 UTC
+Modified: Thu, Dec 15, 2022 @ 04:34 UTC
+A second “blog entry” for testing purposes which uses multiple authors and is
+inside a subdirectory.
+Added a modification here after first submission.
+Tags: english, multiple-author, short, test, update
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/index.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
 <title>Index -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
   <meta property="og:url" content="https://blog.pyssg.xyz/index.html"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -66,14 +65,16 @@
   <a href="https://blog.pyssg.xyz/tag/@short.html">short</a>, 
   <a href="https://blog.pyssg.xyz/tag/@test.html">test</a>, 
   <a href="https://blog.pyssg.xyz/tag/@update.html">update</a>
 </p>
 
 <h2>Articles</h2>
 <ul>
+      <h3>February 2023</h3>
+  <li>Feb 18 - <a href="https://blog.pyssg.xyz/toc_test.html">Table of contents test</a></li>
       <h3>December 2022</h3>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/a/second.html">Second blog post for testing purposes</a></li>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/first.html">First blog post for testing purposes</a></li>
 </ul>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,22 +10,23 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
 ****** Index -- pyssg blog ******
 Some text here.
 Tags: english, multiple-author, short, test, update
 ***** Articles *****
+**** February 2023 ****
+Feb 18 - Table_of_contents_test
 **** December 2022 ****
 Dec 15 - Second_blog_post_for_testing_purposes
 Dec 15 - First_blog_post_for_testing_purposes
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/sitemap.xml` & `pyssg-0.9.0/pyssg.xyz/live/blog/sitemap.xml`

 * *Files 2% similar despite different names*

#### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/sitemap.xml` & `pyssg-0.9.0/pyssg.xyz/live/blog/sitemap.xml`

```diff
@@ -1,10 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.sitemaps.org/schemas/sitemap/0.9 http://www.sitemaps.org/schemas/sitemap/0.9/sitemap.xsd">
   <url>
+    <loc>https://blog.pyssg.xyz/toc_test.html</loc>
+    <lastmod>2023-05-01</lastmod>
+    <changefreq>weekly</changefreq>
+    <priority>1.0</priority>
+  </url>
+  <url>
     <loc>https://blog.pyssg.xyz/a/second.html</loc>
     <lastmod>2022-12-15</lastmod>
     <changefreq>weekly</changefreq>
     <priority>1.0</priority>
   </url>
   <url>
     <loc>https://blog.pyssg.xyz/first.html</loc>
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/tag/@english.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/tag/@english.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
 <title>Posts filtered by english -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
   <meta property="og:url" content="https://blog.pyssg.xyz/tag/@english.html"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -58,14 +57,16 @@
 
     <main>
 <h1>Posts filtered by english</h1>
 <p>Some text here.</p>
 
 <h2>Articles</h2>
 <ul>
+      <h3>February 2023</h3>
+  <li>Feb 18 - <a href="https://blog.pyssg.xyz/toc_test.html">Table of contents test</a></li>
       <h3>December 2022</h3>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/a/second.html">Second blog post for testing purposes</a></li>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/first.html">First blog post for testing purposes</a></li>
 </ul>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,21 +10,22 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
 ****** Posts filtered by english ******
 Some text here.
 ***** Articles *****
+**** February 2023 ****
+Feb 18 - Table_of_contents_test
 **** December 2022 ****
 Dec 15 - Second_blog_post_for_testing_purposes
 Dec 15 - First_blog_post_for_testing_purposes
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/tag/@multiple-author.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/tag/@multiple-author.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
 <title>Posts filtered by multiple-author -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
   <meta property="og:url" content="https://blog.pyssg.xyz/tag/@multiple-author.html"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
```

#### html2text {}

```diff
@@ -10,15 +10,14 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
 ****** Posts filtered by multiple-author ******
 Some text here.
 ***** Articles *****
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/tag/@short.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/tag/@test.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
-<title>Posts filtered by short -- pyssg blog</title>
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
+<title>Posts filtered by test -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
-  <meta property="og:url" content="https://blog.pyssg.xyz/tag/@short.html"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:url" content="https://blog.pyssg.xyz/tag/@test.html"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -53,19 +52,21 @@
 </nav>
 
 <button class="theme-switcher" onclick="toggleTheme()"><i class="fas fa-moon"></i><i class="fas fa-sun"></i></button>
 
     </header>
 
     <main>
-<h1>Posts filtered by short</h1>
+<h1>Posts filtered by test</h1>
 <p>Some text here.</p>
 
 <h2>Articles</h2>
 <ul>
+      <h3>February 2023</h3>
+  <li>Feb 18 - <a href="https://blog.pyssg.xyz/toc_test.html">Table of contents test</a></li>
       <h3>December 2022</h3>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/a/second.html">Second blog post for testing purposes</a></li>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/first.html">First blog post for testing purposes</a></li>
 </ul>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,21 +10,22 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
-****** Posts filtered by short ******
+****** Posts filtered by test ******
 Some text here.
 ***** Articles *****
+**** February 2023 ****
+Feb 18 - Table_of_contents_test
 **** December 2022 ****
 Dec 15 - Second_blog_post_for_testing_purposes
 Dec 15 - First_blog_post_for_testing_purposes
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/tag/@test.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/tag/@short.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
-<title>Posts filtered by test -- pyssg blog</title>
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
+<title>Posts filtered by short -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
-  <meta property="og:url" content="https://blog.pyssg.xyz/tag/@test.html"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:url" content="https://blog.pyssg.xyz/tag/@short.html"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -53,19 +52,21 @@
 </nav>
 
 <button class="theme-switcher" onclick="toggleTheme()"><i class="fas fa-moon"></i><i class="fas fa-sun"></i></button>
 
     </header>
 
     <main>
-<h1>Posts filtered by test</h1>
+<h1>Posts filtered by short</h1>
 <p>Some text here.</p>
 
 <h2>Articles</h2>
 <ul>
+      <h3>February 2023</h3>
+  <li>Feb 18 - <a href="https://blog.pyssg.xyz/toc_test.html">Table of contents test</a></li>
       <h3>December 2022</h3>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/a/second.html">Second blog post for testing purposes</a></li>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/first.html">First blog post for testing purposes</a></li>
 </ul>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,21 +10,22 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
-****** Posts filtered by test ******
+****** Posts filtered by short ******
 Some text here.
 ***** Articles *****
+**** February 2023 ****
+Feb 18 - Table_of_contents_test
 **** December 2022 ****
 Dec 15 - Second_blog_post_for_testing_purposes
 Dec 15 - First_blog_post_for_testing_purposes
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/blog/tag/@update.html` & `pyssg-0.9.0/pyssg.xyz/live/blog/tag/@update.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
 <title>Posts filtered by update -- pyssg blog</title>
 <meta name="description" content="PySSG blog, the python static site generator official blog."/>
 <link rel="alternate" type="application/rss+xml" href="https://blog.pyssg.xyz/rss.xml" title="pyssg blog RSS">
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg blog"/>
   <meta property="og:type" content="article"/>
   <meta property="og:url" content="https://blog.pyssg.xyz/tag/@update.html"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG blog, the python static site generator official blog."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg blog"/>
   </head>
 
   <body>
     <header>
@@ -58,14 +57,16 @@
 
     <main>
 <h1>Posts filtered by update</h1>
 <p>Some text here.</p>
 
 <h2>Articles</h2>
 <ul>
+      <h3>February 2023</h3>
+  <li>Feb 18 - <a href="https://blog.pyssg.xyz/toc_test.html">Table of contents test</a></li>
       <h3>December 2022</h3>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/a/second.html">Second blog post for testing purposes</a></li>
   <li>Dec 15 - <a href="https://blog.pyssg.xyz/first.html">First blog post for testing purposes</a></li>
 </ul>
     </main>
 
     <footer>
```

#### html2text {}

```diff
@@ -10,21 +10,22 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
 ****** Posts filtered by update ******
 Some text here.
 ***** Articles *****
+**** February 2023 ****
+Feb 18 - Table_of_contents_test
 **** December 2022 ****
 Dec 15 - Second_blog_post_for_testing_purposes
 Dec 15 - First_blog_post_for_testing_purposes
     Contact    Donate    RSS
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/404.html` & `pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/404.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
 <title>pyssg</title>
 <meta name="description" content="PySSG, the python static site generator official website."/>
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg"/>
   <meta property="og:type" content="article"/>
   <meta property="og:url" content="https://pyssg.xyz/404.md"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG, the python static site generator official website."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg"/>
   </head>
 
   <body>
     <header>
```

#### html2text {}

```diff
@@ -9,15 +9,14 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
 ****** 404 Not found ******
 The requested URL doesn’t exist. Remove any “www.” at the beginning of the URL.
     Contact    Donate
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/index.html` & `pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/index.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="en
 "
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="https://static.pyssg.xyz">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="https://static.luevano.xyz/images/icons/favicon.ico">
 <title>pyssg</title>
 <meta name="description" content="PySSG, the python static site generator official website."/>
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/style.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="https://static.luevano.xyz/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="https://static.luevano.xyz/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="https://static.luevano.xyz/css/theme.css">
     <!-- extra -->
     <!-- og meta -->
   <meta property="og:title" content="pyssg"/>
   <meta property="og:type" content="article"/>
   <meta property="og:url" content="https://pyssg.xyz/index.md"/>
-  <meta property="og:image" content="https://static.pyssg.xyz/images/default.png"/>
+  <meta property="og:image" content="https://static.luevano.xyz/images/default.png"/>
   <meta property="og:description" content="PySSG, the python static site generator official website."/>
   <meta property="og:locale" content="en"/>
   <meta property="og:site_name" content="pyssg"/>
   </head>
 
   <body>
     <header>
@@ -54,18 +53,22 @@
 <button class="theme-switcher" onclick="toggleTheme()"><i class="fas fa-moon"></i><i class="fas fa-sun"></i></button>
 
     </header>
 
     <main>
   <h1>pyssg</h1>
 
-  <p>Welcome to the official pyssg website. This is as of now serving as a testing ground when I&rsquo;m making changes to it.</p>
-<h2 id="blog">Blog</h2>
-<p>You can find the blog (actually just a mock) <a href="https://blog.pyssg.xyz">here</a>.</p>
-<p>Get the RSS feed: <a href="https://blog.pyssg.xyz/rss.xml">https://blog.pyssg.xyz/rss.xml</a></p>
+  <p>Welcome to the official pyssg website. For now this is just used as testing grounds for pyssg changes.</p>
+<h3 id="blog">Blog<a class="headerlink" href="#blog" title="Permanent link">&para;</a></h3>
+<ul>
+<li>Mock blog where I test some features: <a href="https://blog.pyssg.xyz">pyssg blog</a>
+RSS: <a href="https://blog.pyssg.xyz/rss.xml">https://blog.pyssg.xyz/rss.xml</a></li>
+<li>Personal blog that I normally use: <a href="https://blog.luevano.xyz">Luévano&rsquo;s blog</a>
+RSS: <a href="https://blog.luevano.xyz/rss.xml">https://blog.luevano.xyz/rss.xml</a></li>
+</ul>
     </main>
 
     <footer>
 <span>
   <i class="fas fa-address-card" alt="Contact"></i>
   <a href="https://pyssg.xyz/contact.html">Contact</a>
 </span>
```

#### html2text {}

```diff
@@ -9,21 +9,22 @@
 
 
 
 
 
 
 
-
     * Home
     * Blog
     * Git
 
 ****** pyssg ******
-Welcome to the official pyssg website. This is as of now serving as a testing
-ground when I’m making changes to it.
-***** Blog *****
-You can find the blog (actually just a mock) here.
-Get the RSS feed: https://blog.pyssg.xyz/rss.xml
+Welcome to the official pyssg website. For now this is just used as testing
+grounds for pyssg changes.
+**** Blog¶ ****
+    * Mock blog where I test some features: pyssg_blog RSS: https://
+      blog.pyssg.xyz/rss.xml
+    * Personal blog that I normally use: LuÃ©vano’s_blog RSS: https://
+      blog.luevano.xyz/rss.xml
     Contact    Donate
   Created with pyssg
  Copyright  2023 David LuÃ©vano Alvarado
```

### Comparing `pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/sitemap.xml` & `pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/sitemap.xml`

 * *Files 1% similar despite different names*

#### Comparing `pyssg-0.8.3/pyssg.xyz/live/pyssg.xyz/sitemap.xml` & `pyssg-0.9.0/pyssg.xyz/live/pyssg.xyz/sitemap.xml`

```diff
@@ -4,12 +4,12 @@
     <loc>https://pyssg.xyz/404.html</loc>
     <lastmod>2022-12-14</lastmod>
     <changefreq>weekly</changefreq>
     <priority>1.0</priority>
   </url>
   <url>
     <loc>https://pyssg.xyz/index.html</loc>
-    <lastmod>2022-12-27</lastmod>
+    <lastmod>2023-05-01</lastmod>
     <changefreq>weekly</changefreq>
     <priority>1.0</priority>
   </url>
 </urlset>
```

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/base.html` & `pyssg-0.9.0/pyssg.xyz/plt/base.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 <!DOCTYPE html>
 <html class="theme-dark" lang="{%block html_lang%}{%endblock html_lang%}"
   prefix="og: https://ogp.me/ns#">
   <head>
-    <base href="{{config['url']['static']}}">
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="icon" href="images/icons/favicon.ico">
+    <link rel="icon" href="{{config['url']['static']}}/images/icons/favicon.ico">
     {%block head_title%}{%endblock head_title%}
     {%block head_description%}{%endblock head_description%}
     {%block head_rss%}{%endblock head_rss%}
     <!-- general style -->
-    <link rel="stylesheet" type="text/css" href="css/style.css">
-    <link rel="stylesheet" type="text/css" href="fork-awesome/css/fork-awesome.min.css">
-    <link rel="stylesheet" type="text/css" href="font-awesome/css/all.min.css">
+    <link rel="stylesheet" type="text/css" href="{{config['url']['static']}}/css/style.css">
+    <link rel="stylesheet" type="text/css" href="{{config['url']['static']}}/fork-awesome/css/fork-awesome.min.css">
+    <link rel="stylesheet" type="text/css" href="{{config['url']['static']}}/font-awesome/css/all.min.css">
     <!-- theme related -->
-    <script type="text/javascript" src="scripts/theme.js"></script>
-    <link id="theme-css" rel="stylesheet" type="text/css" href="css/theme.css">
+    <script type="text/javascript" src="{{config['url']['static']}}/scripts/theme.js"></script>
+    <link id="theme-css" rel="stylesheet" type="text/css" href="{{config['url']['static']}}/css/theme.css">
     <!-- extra -->
     {%block head_extra%}{%endblock head_extra%}
     <!-- og meta -->
     {%block head_og%}{%endblock head_og%}
   </head>
 
   <body>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 
 
-
  {%block head_title%}{%endblock head_title%} {%block head_description%}
 {%endblock head_description%} {%block head_rss%}{%endblock head_rss%}
 
 
 
 
   {%block head_extra%}{%endblock head_extra%}  {%block head_og%}{%endblock
```

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/blog/index.html` & `pyssg-0.9.0/pyssg.xyz/plt/blog/index.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/blog/page.html` & `pyssg-0.9.0/pyssg.xyz/plt/blog/page.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/blog/tag.html` & `pyssg-0.9.0/pyssg.xyz/plt/blog/tag.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/body/footer.html` & `pyssg-0.9.0/pyssg.xyz/plt/body/footer.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/body/header.html` & `pyssg-0.9.0/pyssg.xyz/plt/body/header.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/root_page.html` & `pyssg-0.9.0/pyssg.xyz/plt/root_page.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/rss.xml` & `pyssg-0.9.0/pyssg.xyz/plt/rss.xml`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/pyssg.xyz/plt/sitemap.xml` & `pyssg-0.9.0/pyssg.xyz/plt/sitemap.xml`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/arg_parser.py` & `pyssg-0.9.0/src/pyssg/arg_parser.py`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/builder.py` & `pyssg-0.9.0/src/pyssg/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-import pprint
 from copy import deepcopy
 from operator import itemgetter
 from logging import Logger, getLogger
 
 from jinja2 import Environment, Template, FileSystemLoader as FSLoader
 
 from .utils import get_file_list, get_dir_structure, create_dir, copy_file
```

### Comparing `pyssg-0.8.3/src/pyssg/configuration.py` & `pyssg-0.9.0/src/pyssg/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,91 @@
 import sys
 from importlib.metadata import version
-from importlib.resources import path as rpath
 from datetime import datetime, timezone
 from logging import Logger, getLogger
+from typing import Any
 
 from .utils import get_expanded_path
 from .yaml_parser import get_parsed_yaml
 
 log: Logger = getLogger(__name__)
 DEFAULT_CONFIG_PATH: str = '$XDG_CONFIG_HOME/pyssg/config.yaml'
 VERSION: str = version('pyssg')
 
 
-def __check_well_formed_config(config: dict,
-                               config_base: list[dict],
+# TODO: add checking for extensions config (such as pymdvar)
+def __check_well_formed_config(config: dict[str, Any],
+                               config_base: list[dict[str, Any]],
                                prefix_key: str = '') -> None:
     for key in config_base[0].keys():
+        new_config_base: list[dict[str, Any]] = []
         current_key: str = f'{prefix_key}.{key}' if prefix_key != '' else key
         log.debug('checking "%s"', current_key)
         if key not in config:
             log.error('config doesn\'t have "%s"', current_key)
             log.debug('key: %s; config.keys: %s', key, config.keys())
             sys.exit(1)
         # checks for dir_paths
         if key == 'dirs':
+            try:
+                config[key].keys()
+            except AttributeError:
+                log.error('config doesn\'t have any dirs (dirs.*)')
+                sys.exit(1)
             if '/' not in config[key]:
-                log.error('config doesn\'t have "%s./"', current_key)
                 log.debug('key: %s; config.keys: %s', key, config[key].keys())
+                log.error('config doesn\'t have "%s./"', current_key)
                 sys.exit(1)
-            log.debug('checking "%s" fields for (%s) dir_paths', key, ', '.join(config[key].keys()))
+            log.debug('checking "%s" fields for (%s) dir_paths',
+                      key, ', '.join(config[key].keys()))
             for dkey in config[key].keys():
                 new_current_key: str = f'{current_key}.{dkey}'
-                new_config_base: list[dict] = [config_base[1], config_base[1]]
-                __check_well_formed_config(config[key][dkey], new_config_base, new_current_key)
+                new_config_base = [config_base[1], config_base[1]]
+                __check_well_formed_config(config[key][dkey],
+                                           new_config_base,
+                                           new_current_key)
             continue
         # the case for elements that don't have nested elements
         if not config_base[0][key]:
             log.debug('"%s" doesn\'t need nested elements', current_key)
             continue
-        new_config_base: list[dict] = [config_base[0][key], config_base[1]]
+        new_config_base = [config_base[0][key], config_base[1]]
         __check_well_formed_config(config[key], new_config_base, current_key)
 
 
-def __expand_all_paths(config: dict) -> None:
+def __expand_all_paths(config: dict[str, Any]) -> None:
     log.debug('expanding all path options: %s', config['path'].keys())
     for option in config['path'].keys():
         config['path'][option] = get_expanded_path(config['path'][option])
 
 
 # not necessary to type deeper than the first dict
-def get_parsed_config(path: str) -> list[dict]:
+def get_parsed_config(path: str,
+                      mc_package: str = 'mandatory_config.yaml',
+                      plt_resource: str = 'pyssg.plt') -> list[dict[str, Any]]:
     log.debug('reading config file "%s"', path)
-    config_all: list[dict] = get_parsed_yaml(path)
-    mandatory_config: list[dict] = get_parsed_yaml('mandatory_config.yaml', 'pyssg.plt')
-    log.info('found %s document(s) for configuration "%s"', len(config_all), path)
-    log.debug('checking that config file is well formed (at least contains mandatory fields')
+    config_all: list[dict[str, Any]] = get_parsed_yaml(path)
+    mandatory_config: list[dict[str, Any]] = get_parsed_yaml(mc_package,
+                                                             plt_resource)
+    log.info('found %s document(s) for config "%s"', len(config_all), path)
+    log.debug('checking that config file is well formed')
     for config in config_all:
         __check_well_formed_config(config, mandatory_config)
         __expand_all_paths(config)
     return config_all
 
 
 # not necessary to type deeper than the first dict,
 #   static config means config that shouldn't be changed by the user
-def get_static_config() -> dict[str, dict]:
+def get_static_config(sc_package: str = 'static_config.yaml',
+                      plt_resource: str = 'pyssg.plt') -> dict[str, Any]:
     log.debug('reading and setting static config')
-    config: dict = get_parsed_yaml('static_config.yaml', 'pyssg.plt')[0]
-    # do I really need a lambda function...
-    time = lambda x : datetime.now(tz=timezone.utc).strftime(config['fmt'][x])
+    config: dict[str, Any] = get_parsed_yaml(sc_package, plt_resource)[0]
+
+    # TODO: move this to utils and update the tests
+    def __time(fmt: str) -> str:
+        return datetime.now(tz=timezone.utc).strftime(config['fmt'][fmt])
+
     config['info']['version'] = VERSION
-    config['info']['rss_run_date'] = time('rss_date')
-    config['info']['sitemap_run_date'] = time('sitemap_date')
+    config['info']['rss_run_date'] = __time('rss_date')
+    config['info']['sitemap_run_date'] = __time('sitemap_date')
     return config
```

### Comparing `pyssg-0.8.3/src/pyssg/database.py` & `pyssg-0.9.0/src/pyssg/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,69 +16,69 @@
 
     def __init__(self, db_path: str) -> None:
         log.debug('initializing the page db on path "%s"', db_path)
         self.db_path: str = db_path
         self.e: dict[str, DatabaseEntry] = dict()
 
     def update_tags(self, file_name: str,
-                    new_tags: list[str]) -> None:
-        # technically, I should ensure this function can only run if self.e is populated
+                    new_tags: set[str]) -> None:
+        # technically, I should ensure this function can only run
+        #   if self.e is populated
         if file_name in self.e:
             log.debug('updating tags for entry "%s"', file_name)
             log.debug('entry "%s" old tags: %s',
-                      file_name, self.e[file_name])
+                      file_name, self.e[file_name].tags)
 
             self.e[file_name].update_tags(new_tags)
             log.debug('entry "%s" new tags: %s',
-                      file_name, self.e[file_name])
+                      file_name, self.e[file_name].tags)
         else:
             log.error('can\'t update tags for entry "%s",'
                       ' as it is not present in db', file_name)
             sys.exit(1)
 
     def update(self, file_name: str,
-               remove: str='') -> None:
+               remove: str = '') -> None:
         log.debug('updating entry for file "%s"', file_name)
         f: str = file_name
-        tags: list[str] = []
+        tags: set[str] = set()
         if remove != '':
             f = file_name.replace(remove, '')
             log.debug('removed "%s" from "%s": "%s"', remove, file_name, f)
 
         # get current time, needs actual file name
         time: float = os.stat(file_name).st_mtime
         log.debug('time for "%s": %s', file_name, time)
 
         # calculate current checksum, also needs actual file name
-        checksum: str = get_checksum(file_name)
-        log.debug('checksum for "%s": "%s"', file_name, checksum)
+        cksm: str = get_checksum(file_name)
+        log.debug('checksum for "%s": "%s"', file_name, cksm)
 
         # three cases, 1) entry didn't exist,
         # 2) entry has been mod and,
         # 3) entry hasn't been mod
-        #1)
+        # 1)
         if f not in self.e:
             log.debug('entry "%s" didn\'t exist, adding with defaults', f)
-            self.e[f] = DatabaseEntry([f, time, 0.0, checksum, tags])
+            self.e[f] = DatabaseEntry((f, time, 0.0, cksm, tags))
             return
 
-        # old_e is old entity
-        old_e: DatabaseEntry = self.e[f]
-        log.debug('entry "%s" old content: %s', f, old_e)
+        # oe is old entity
+        oe: DatabaseEntry = self.e[f]
+        log.debug('entry "%s" old content: %s', f, oe)
 
         # 2)
-        if checksum != old_e.checksum:
-            log.debug('entry "%s" has been modified, updating', f)
-            self.e[f] = DatabaseEntry([f, old_e.ctimestamp, time, checksum, tags])
-            log.debug('entry "%s" new content: (%s, %s, %s, (%s))', f, self.e[f])
-            return
+        if cksm != oe.checksum:
+            log.debug('entry "%s" has been modified, updating; '
+                      'using old tags', f)
+            self.e[f] = DatabaseEntry((f, oe.ctimestamp, time, cksm, oe.tags))
+            log.debug('entry "%s" new content: %s', f, self.e[f])
         # 3)
         else:
             log.debug('entry "%s" hasn\'t been modified', f)
-            return
 
     def write(self) -> None:
         log.debug('writing db')
         with open(self.db_path, 'w') as file:
             csv_writer = csv.writer(file, delimiter=self.__COLUMN_DELIMITER)
             for _, v in self.e.items():
                 log.debug('writing row: %s', v)
@@ -88,39 +88,45 @@
         log.debug('checking that "%s" exists or is a file', self.db_path)
         if not os.path.exists(self.db_path):
             log.warning('"%s" doesn\'t exist, will be'
                         ' created once process finishes,'
                         ' ignore if it\'s the first run', self.db_path)
             return False
         if not os.path.isfile(self.db_path):
-            log.error('"%s" is not a file"', self.db_path)
+            log.error('"%s" is not a file', self.db_path)
             sys.exit(1)
         return True
 
-    def _get_csv_rows(self) -> list[list[str]]:
+    def _get_raw_csv_rows(self) -> list[list[str]]:
         rows: list[list[str]]
         with open(self.db_path, 'r') as f:
             csv_reader = csv.reader(f, delimiter=self.__COLUMN_DELIMITER)
             rows = list(csv_reader)
         log.debug('db contains %d rows', len(rows))
         return rows
 
     # TODO: don't include files that are not in the db anymore
     def read(self) -> None:
         log.debug('reading db')
         if not self._db_path_exists():
             return
 
-        rows: list[list[str]] = self._get_csv_rows()
+        rows: list[list[str]] = self._get_raw_csv_rows()
         # l=list of values in entry
         log.debug('parsing rows from db')
         for it, row in enumerate(rows):
             i: int = it + 1
             col_num: int = len(row)
             log.debug('row %d content: "%s"', i, row)
             if col_num != self.__COLUMN_NUM:
                 log.critical('row %d doesn\'t contain %s columns, contains %d'
                              ' columns: "%s"',
                              i, self.__COLUMN_NUM, col_num, row)
                 sys.exit(1)
-            entry: DatabaseEntry = DatabaseEntry(row)
+            # actual value types
+            r: tuple[str, float, float, str, str] = (str(row[0]),
+                                                     float(row[1]),
+                                                     float(row[2]),
+                                                     str(row[3]),
+                                                     str(row[4]))
+            entry: DatabaseEntry = DatabaseEntry(r)
             self.e[entry.fname] = entry
```

### Comparing `pyssg-0.8.3/src/pyssg/md_parser.py` & `pyssg-0.9.0/src/pyssg/md_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import os
 from operator import itemgetter
-from markdown import Markdown
 from logging import Logger, getLogger
+from typing import Any
 
 from markdown import Markdown
 from yafg import YafgExtension
+from pymdvar import VariableExtension
 from markdown_checklist.extension import ChecklistExtension
+from markdown.extensions.toc import TocExtension
 
 from .database import Database
 from .page import Page
 
 log: Logger = getLogger(__name__)
 
 
-def _get_md_obj() -> Markdown:
+# TODO: add configuration testing for extensions config (pymdvar for ex)
+def get_md_obj(variables: dict[str, str],
+               enable_env: bool) -> Markdown:
     exts: list = ['extra',
                   'meta',
                   'sane_lists',
                   'smarty',
-                  'toc',
                   'wikilinks',
+                  TocExtension(permalink=True,
+                               baselevel=2),
+                  VariableExtension(variables=variables,
+                                    enable_env=enable_env),
                   # stripTitle generates an error when True,
                   # if there is no title attr
                   YafgExtension(stripTitle=False,
                                 figureClass="",
                                 figcaptionClass="",
                                 figureNumbering=False,
                                 figureNumberClass="number",
@@ -47,45 +54,60 @@
                  dir_config: dict,
                  db: Database):
         log.debug('initializing the md parser with %d files', len(files))
         self.files: list[str] = files
         self.config: dict = config
         self.dir_config: dict = dir_config
         self.db: Database = db
-        self.md: Markdown = _get_md_obj()
+        # TODO: actually add extensions support, for now only pymdvar is configured
+        self.pymdvar_vars: dict[str, str] = dict()
+        self.pymdvar_enable_env: bool = False
+        if 'exts' in config and 'pymdvar' in config['exts']:
+            pymdvar: dict[str, Any] = config['exts']['pymdvar']
+            if 'variables' in pymdvar and type(pymdvar['variables']) == dict:
+                self.pymdvar_vars = pymdvar['variables']
+            if 'enable_env' in pymdvar and type(pymdvar['enable_env']) == bool:
+                self.pymdvar_enable_env = pymdvar['enable_env']
+        log.debug('pymdvar_variables: %s', self.pymdvar_vars)
+        log.debug('pymdvar_enable_env: %s', self.pymdvar_enable_env)
+
+        self.md: Markdown = get_md_obj(self.pymdvar_vars, self.pymdvar_enable_env)
 
         self.all_files: list[Page] = []
         self.all_tags: list[tuple[str, str]] = []
 
     def parse_files(self) -> None:
         log.debug('parsing all files')
         for i, f in enumerate(self.files):
             log.debug('parsing file "%s"', f)
             src_file: str = os.path.join(self.dir_config['src'], f)
             log.debug('path "%s"', src_file)
             self.db.update(src_file, remove=f'{self.dir_config["src"]}/')
 
             log.debug('parsing md into html')
             content: str = self.md.reset().convert(open(src_file).read())
-            # ignoring md.Meta type as it is not yet defined (because it is from an extension)
+            # ignoring md.Meta type as it is not yet defined
+            #   (because it is from an extension)
             page: Page = Page(f,
                               self.db.e[f].ctimestamp,
                               self.db.e[f].mtimestamp,
                               content,
+                              self.md.toc,  # type: ignore
+                              self.md.toc_tokens,  # type: ignore
                               self.md.Meta,  # type: ignore
                               self.config,
                               self.dir_config)
             page.parse_metadata()
 
             log.debug('adding to file list')
             self.all_files.append(page)
 
             if self.dir_config['tags'] and page.tags is not None:
                 log.debug('parsing tags for "%s"', f)
-                self.db.update_tags(f, list(map(itemgetter(0), page.tags)))
+                self.db.update_tags(f, set(map(itemgetter(0), page.tags)))
 
                 log.debug('add all tags to tag list')
                 for t in page.tags:
                     if t[0] not in list(map(itemgetter(0), self.all_tags)):
                         log.debug('adding tag "%s"', t[0])
                         self.all_tags.append(t)
                     else:
```

### Comparing `pyssg-0.8.3/src/pyssg/page.py` & `pyssg-0.9.0/src/pyssg/page.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,124 @@
-import os
-import sys
 from datetime import datetime, timezone
 from logging import Logger, getLogger
+from typing import Any
 
 log: Logger = getLogger(__name__)
 
 
 class Page:
-    def __init__(self,
-                 name: str,
+    def __init__(self, name: str,
                  ctime: float,
                  mtime: float,
                  html: str,
-                 meta: dict,
-                 config: dict,
-                 dir_config: dict) -> None:
-        log.debug('initializing the page object with name "%s"', name)
+                 toc: str,
+                 toc_tokens: list[str],
+                 meta: dict[str, Any],
+                 config: dict[str, Any],
+                 dir_config: dict[str, Any]) -> None:
+        log.debug('initializing a page object with name "%s"', name)
         # initial data
         self.name: str = name
         self.ctimestamp: float = ctime
         self.mtimestamp: float = mtime
         self.content: str = html
-        self.meta: dict = meta
-        self.config: dict = config
-        self.dir_config: dict = dir_config
+        self.toc: str = toc
+        self.toc_tokens: list[str] = toc_tokens
+        self.meta: dict[str, Any] = meta
+        self.config: dict[str, Any] = config
+        self.dir_config: dict[str, Any] = dir_config
 
         # data from self.meta
         self.title: str
         self.author: list[str]
         self.summary: str
         self.lang: str
         self.cdatetime: datetime
         self.mdatetime: datetime | None = None
         self.tags: list[tuple[str, str]] = []
 
         # constructed
         self.url: str
-        self.image_url: str
         self.cdate_rss: str
         self.cdate_sitemap: str
         self.mdate_rss: str | None = None
         self.mdate_sitemap: str | None = None
 
         self.next: Page | None = None
         self.previous: Page | None = None
 
-        # also from self.meta, but for og metadata
-        self.og: dict[str, str] = dict()
-
     def __lt__(self, other):
         return self.ctimestamp < other.ctimestamp
 
-    def __get_meta(self, var: str, or_else: str | list[str]) -> str | list[str]:
+    def __get_meta(self, var: str,
+                   or_else: str | list[str] = ['']) -> str | list[str] | Any:
         if var in self.meta:
             log.debug('getting metadata "%s"', var)
             return self.meta[var]
         else:
-            log.debug('getting metadata "%s" failed, using optional value "%s"', var, or_else)
+            log.debug('getting metadata "%s" failed, using optional value "%s"',
+                      var, or_else)
             return or_else
 
-    def cdate(self, format: str) -> str:
+    # these date/cdate/mdate might be a bit overcomplicated
+
+    def __date(self, dt: datetime, format: str) -> str:
         if format in self.config['fmt']:
-            return self.cdatetime.strftime(self.config['fmt'][format])
+            return dt.strftime(self.config['fmt'][format])
         else:
-            log.warning('format "%s" not found in config["fmt"], returning empty string', format)
+            log.warning('format "%s" not found in config, returning '
+                        'empty string', format)
             return ''
 
+    def cdate(self, format: str) -> str:
+        return self.__date(self.cdatetime, format)
+
     def mdate(self, format: str) -> str:
         if self.mdatetime is None:
             log.warning('no mdatetime found, can\'t return a formatted string')
             return ''
-        if format in self.config['fmt']:
-            return self.mdatetime.strftime(self.config['fmt'][format]) # type: ignore
-        else:
-            log.warning('format "%s" not found in config["fmt"], returning empty string', format)
-            return ''
+        return self.__date(self.mdatetime, format)
 
-    # parses meta from self.meta, for og, it prioritizes,
-    #   the actual og meta
+    def from_timestamp(self, timestamp: float) -> datetime:
+        return datetime.fromtimestamp(timestamp, tz=timezone.utc)
+
+    # parses meta from self.meta
     def parse_metadata(self):
         log.debug('parsing metadata for file "%s"', self.name)
-        self.title = self.__get_meta('title', [''])[0]
-        self.author = list(self.__get_meta('author', ['']))
-        self.summary = self.__get_meta('summary', [''])[0]
-        self.lang = self.__get_meta('lang', ['en'])[0]
+        self.title = str(self.__get_meta('title')[0])
+        self.author = list(self.__get_meta('author'))
+        self.summary = str(self.__get_meta('summary')[0])
+        self.lang = str(self.__get_meta('lang', ['en'])[0])
 
         log.debug('parsing timestamp')
-        self.cdatetime = datetime.fromtimestamp(self.ctimestamp, tz=timezone.utc)
+        self.cdatetime = self.from_timestamp(self.ctimestamp)
         self.cdate_rss = self.cdate('rss_date')
         self.cdate_sitemap = self.cdate('sitemap_date')
 
         if self.mtimestamp != 0.0:
             log.debug('parsing modified timestamp')
-            self.mdatetime = datetime.fromtimestamp(self.mtimestamp, tz=timezone.utc)
+            self.mdatetime = self.from_timestamp(self.mtimestamp)
             self.mdate_rss = self.mdate('rss_date')
             self.mdate_sitemap = self.mdate('sitemap_date')
         else:
             log.debug('not parsing modified timestamp, hasn\'t been modified')
 
         if self.dir_config['tags']:
             log.debug('parsing tags')
             tags_only: list[str] = list(self.__get_meta('tags', []))
             if tags_only:
                 tags_only.sort()
 
                 for t in tags_only:
-                    # need to specify dir_config['url'] as it is a hardcoded tag url
-                    self.tags.append((t, f'{self.dir_config["url"]}/tag/@{t}.html'))
+                    # need to specify dir_config['url'] as it is
+                    #   a hardcoded tag url
+                    tag_url: str = f'{self.dir_config["url"]}/tag/@{t}.html'
+                    self.tags.append((t, tag_url))
             else:
                 log.debug('no tags to parse')
 
-        log.debug('parsing url')
-        # no need to specify dir_config['url'] as self.name already contains the relative url
-        self.url = f'{self.config["url"]["main"]}/{self.name.replace(".md", ".html")}'
+        log.debug('parsing page url')
+        # no need to specify dir_config['url'] as self.name already
+        #   contains the relative url
+        name_html: str = self.name.replace(".md", ".html")
+        self.url = f'{self.config["url"]["main"]}/{name_html}'
         log.debug('final url "%s"', self.url)
-
-        log.debug('parsing image url')
-        default_image_url: str = ''
-        if 'default_image' in self.config['url']:
-            log.debug('"default_image" url found, will use if no "image_url" is found')
-            default_image_url = self.config['url']['default_image']
-
-        image_url: str
-        image_url = self.__get_meta('image_url', [default_image_url])[0]
-
-        if image_url != '':
-            if 'static' in self.config['url']:
-                self.image_url = f'{self.config["url"]["static"]}/{image_url}'
-            else:
-                log.debug('no static url set, using main url, this could cause problems')
-                self.image_url = f'{self.config["url"]["main"]}/{image_url}'
-            log.debug('final image url "%s"', self.image_url)
-        else:
-            self.image_url = ''
-            log.debug('no image url set for the page, could be because no'
-                      ' "image_url" was found in the metadata and/or no '
-                      ' "default_image" set in the config file')
-
-        # if contains open graph elements
-        # TODO: better handle this part
-        # og_e = object graph entry
-        og_elements: list[str] = list(self.__get_meta('og', []))
-        if og_elements:
-            log.debug('parsing og metadata')
-            for og_e in og_elements:
-                kv: list[str] = og_e.split(',', 1)
-                if len(kv) != 2:
-                    log.error('invalid og syntax for "%s", needs to be "k, v"', og_e)
-                    sys.exit(1)
-
-                k: str = kv[0].strip()
-                v: str = kv[1].strip()
-
-                log.debug('og element: ("%s", "%s")', k, v)
-                self.og[k] = v
-
-        else:
-            log.debug('no tags to parse')
```

### Comparing `pyssg-0.8.3/src/pyssg/per_level_formatter.py` & `pyssg-0.9.0/src/pyssg/custom_logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-from logging import Formatter, LogRecord, DEBUG, INFO, WARNING, ERROR, CRITICAL
+import sys
+from logging import (Logger, StreamHandler, Formatter, LogRecord,
+                     DEBUG, INFO, WARNING, ERROR, CRITICAL,
+                     getLogger)
+from typing import TextIO
+
+LOG_LEVEL: int = INFO
+# 'pyssg' es the name of the root logger
+LOGGER_NAME: str = 'pyssg'
+
 
 # only reason for this class is to get info formatting as normal text
 #   and everything else with more info and with colors
 class PerLevelFormatter(Formatter):
     # colors for the terminal in ansi
     __YELLOW: str = '\x1b[33m'
     __RED: str = '\x1b[31m'
@@ -22,7 +31,16 @@
     def format(self, record: LogRecord) -> str:
         # this should never fail, as __FORMATS is defined above,
         #   so no issue of just converting to str
         fmt: str = str(self.__FORMATS.get(record.levelno))
         formatter: Formatter = Formatter(
             fmt=fmt, datefmt=self.__DATE_FMT, style='%')
         return formatter.format(record)
+
+
+def setup_logger(name: str = LOGGER_NAME, level: int = LOG_LEVEL) -> None:
+    logger: Logger = getLogger(name)
+    handler: StreamHandler[TextIO] = StreamHandler(sys.stdout)
+    logger.setLevel(level)
+    handler.setLevel(level)
+    handler.setFormatter(PerLevelFormatter())
+    logger.addHandler(handler)
```

### Comparing `pyssg-0.8.3/src/pyssg/plt/index.html` & `pyssg-0.9.0/src/pyssg/plt/index.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/plt/page.html` & `pyssg-0.9.0/src/pyssg/plt/page.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/plt/rss.xml` & `pyssg-0.9.0/src/pyssg/plt/rss.xml`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/plt/sitemap.xml` & `pyssg-0.9.0/src/pyssg/plt/sitemap.xml`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/plt/tag.html` & `pyssg-0.9.0/src/pyssg/plt/tag.html`

 * *Files identical despite different names*

### Comparing `pyssg-0.8.3/src/pyssg/pyssg.py` & `pyssg-0.9.0/src/pyssg/pyssg.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     # too messy to place at utils.py, don't want to be
     #   passing the arg parser around
     def _log_perror(message: str) -> None:
         arg_parser.print_usage()
         # even if it's an error, print it as info
         #   as it is not critical, only config related
-        log.info(message)
+        log.info(f'pyssg: error: {message}, --help for more')
         sys.exit(1)
 
     # -1 as first argument is program path
     num_args = len(sys.argv) - 1
     if num_args == 2 and args['config']:
-        _log_perror('pyssg: error: only config argument passed, --help for more')
+        _log_perror('only config argument passed')
     elif not num_args > 0 or (num_args == 1 and args['debug']):
-        _log_perror('pyssg: error: no arguments passed, --help for more')
+        _log_perror('no arguments passed')
     elif num_args == 3 and (args['debug'] and args['config']):
-        _log_perror("pyssg: error: no arguments passed other than 'debug' and 'config', --help for more")
+        _log_perror('no arguments passed other than "debug" and "config"')
 
     if args['version']:
         log.info('pyssg v%s', VERSION)
         sys.exit(0)
 
     if args['debug']:
         # need to modify the root logger specifically,
@@ -97,15 +97,14 @@
             for f in files:
                 plt_file: str = os.path.join(config['path']['plt'], f)
                 with rpath('pyssg.plt', f) as p:
                     copy_file(str(p), plt_file)
         log.info('finished initialization')
         sys.exit(0)
 
-
     if args['build']:
         log.info('building the html files')
         for config in config_all:
             log.info('building html for "%s"', config['title'])
             db: Database = Database(config['path']['db'])
             db.read()
```

### Comparing `pyssg-0.8.3/src/pyssg/utils.py` & `pyssg-0.9.0/src/pyssg/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     file_list: list[str] = []
     for root, dirs, files in os.walk(path):
         if exclude_dirs != []:
             log.debug('removing excludes from list')
             dirs[:] = [d for d in dirs if d not in exclude_dirs]
         for file in files:
             if file.endswith(exts):
-                # [1:] is required to remove the '/' at the beginning after replacing
+                # [1:] is required to remove the '/'
+                #   at the beginning after replacing
                 file_name: str = os.path.join(root, file).replace(path, '')[1:]
                 file_list.append(file_name)
                 log.debug('added file "%s" without "%s" part: "%s"',
                           file, path, file_name)
             else:
                 log.debug('ignoring file "%s" as it doesn\'t contain'
                           ' any of the extensions %s', file, exts)
@@ -40,36 +41,47 @@
         if exclude != []:
             log.debug('removing excludes from list')
             dirs[:] = [d for d in dirs if d not in exclude]
         for d in dirs:
             if root in dir_list:
                 dir_list.remove(root)
                 log.debug('removed dir "%s" as it already is in the list', root)
-            # not removing the 'path' part here, as comparisons with 'root' would fail
+            # not removing the 'path' part here,
+            #   as comparisons with 'root' would fail
             joined_dir: str = os.path.join(root, d)
             dir_list.append(joined_dir)
             log.debug('added dir "%s" to the list', joined_dir)
     log.debug('removing "%s" from all dirs in list', path)
     # [1:] is required to remove the '/' at the beginning after replacing
     return [d.replace(path, '')[1:] for d in dir_list]
 
 
+# TODO: probably change it so it returns a bool, easier to check
 def create_dir(path: str, p: bool = False, silent=False) -> None:
+    log_msg: str = ''
     try:
         if p:
             os.makedirs(path)
         else:
             os.mkdir(path)
+        log_msg = f'created directory "{path}"'
         if not silent:
-            log.info('created directory "%s"', path)
+            log.info(log_msg)
+        log.debug(log_msg)
     except FileExistsError:
+        log_msg = f'directory "{path}" exists, ignoring'
         if not silent:
-            log.info('directory "%s" already exists, ignoring', path)
+            log.info(log_msg)
+        log.debug(log_msg)
 
 
+# TODO: change this as it doesn't take directories into account,
+#   a file can be copied into a directory, need to get the filename
+#   and use it when copying
+# TODO: probably change it so it returns a bool, easier to check
 def copy_file(src: str, dst: str) -> None:
     if not os.path.exists(dst):
         shutil.copy2(src, dst)
         log.info('copied file "%s" to "%s"', src, dst)
     else:
         log.info('file "%s" already exists, ignoring', dst)
```

### Comparing `pyssg-0.8.3/src/pyssg/yaml_parser.py` & `pyssg-0.9.0/src/pyssg/yaml_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import yaml
 from yaml import SafeLoader
 from yaml.nodes import SequenceNode
-from io import TextIOWrapper
 from importlib.resources import path as rpath
 from logging import Logger, getLogger
+from typing import Any
 
 log: Logger = getLogger(__name__)
 
 
 # required to concat values in yaml using !join [value, value, ...]
 def __join_constructor(loader: SafeLoader, node: SequenceNode) -> str:
     seq = loader.construct_sequence(node)
     return ''.join([str(i) for i in seq])
 
 
-def __read_raw_yaml(path: str) -> list[dict]:
-    all_docs: list[dict] = []
+def setup_custom_yaml() -> None:
+    SafeLoader.add_constructor('!join', __join_constructor)
+
+
+def __read_raw_yaml(path: str) -> list[dict[str, Any]]:
+    all_docs: list[dict[str, Any]] = []
     with open(path, 'r') as f:
         for doc in yaml.safe_load_all(f):
             all_docs.append(doc)
     return all_docs
 
 
-def get_parsed_yaml(resource: str, package: str='') -> list[dict]:
+def get_parsed_yaml(resource: str, package: str = '') -> list[dict[str, Any]]:
     if package == '':
         log.debug('parsing yaml; reading "%s"', resource)
         return __read_raw_yaml(resource)
     log.debug('parsing yaml; reading "%s.%s"', package, resource)
     with rpath(package, resource) as p:
         return __read_raw_yaml(str(p))
-
-
-SafeLoader.add_constructor('!join', __join_constructor)
```

### Comparing `pyssg-0.8.3/src/pyssg.egg-info/PKG-INFO` & `pyssg-0.9.0/src/pyssg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,75 @@
 Metadata-Version: 2.1
 Name: pyssg
-Version: 0.8.3
-Summary: A Static Site Generator using markdown files
+Version: 0.9.0
+Summary: A Static Site Generator using markdown files.
 Home-page: https://github.com/luevano/pyssg
 Author: David Luevano Alvarado
 Author-email: david@luevano.xyz
 License: GPLv3
-Keywords: python,static,site,generator,markdown
-Classifier: Programming Language :: Python :: 3
+Keywords: python,static,site,generator,markdown,website
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications :: Email :: Filters
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS
 
 # pyssg - Static Site Generator written in Python
 
 Generates HTML files from MD files for a static site, personally using it for a blog-like site.
 
 Initially inspired by Roman Zolotarev's [`ssg5`](https://rgz.ee/bin/ssg5) and [`rssg`](https://rgz.ee/bin/rssg), Luke Smith's [`lb` and `sup`](https://github.com/LukeSmithxyz/lb) and, pedantic.software's [`blogit`](https://pedantic.software/git/blogit/).
 
 ## Features and to-do
 
-**NOTE:** WIP, there will be changes that will break the setup.
+**NOTE:** WIP, there will be changes that will break `pyssg` generations/config setup.
 
 - [x] Build static site parsing `markdown` files ( `*.md` -> `*.html`)
 	- [x] Uses [`jinja`](https://jinja.palletsprojects.com/en/3.0.x/) for templating.
 	- [x] Preserves hand-made `*.html` files.
 	- [x] Tag functionality, useful for blog-style sites.
-	- [ ] Open Graph (and similar) support.
-		- Technically, this works if you add the correct metadata to the `*.md` files and use the variables available for Jinja.
 - [x] Build `sitemap.xml` file.
 	- [ ] Include manually added `*.html` files.
 - [x] Build `rss.xml` file.
-	- [ ] Join the `static_url` to all relative URLs found to comply with the [RSS 2.0 spec](https://validator.w3.org/feed/docs/rss2.html).
-		- This would be added to the parsed HTML text extracted from the MD files, so it would be available to the created `*.html` and `*.xml` files. Note that depending on the reader, it will append the URL specified in the RSS file or use the [`xml:base`](https://www.rssboard.org/news/151/relative-links) specified (for example, [newsboat](https://newsboat.org/) parses `xml:base`).
 	- [ ] Include manually added `*.html` files.
 - [x] YAML for configuration file, uses [`PyYAML`](https://pyyaml.org/).
-	- [ ] Handle multiple "documents".
-	- [ ] More complex directory structure to support multiple subdomains and different types of pages.
+	- [x] Support for multiple "documents". `PyYAML` supports this. In `pyssg` context, it means it can generate multiple websites (I personally use it for subdomains).
+	- [x] Support for more complex directory structure to support configuration on a per directory basis.
+- [x] File checksum checking for modification of files.
 - [ ] Option/change to using an SQL database instead of the custom solution.
-- [x] Checksum checking because the timestamp of the file is not enough.
 - [ ] Use external markdown extensions.
+  - [x] So far only extension configuration is for my own extension [pymdvar](https://github.com/luevano/pymdvar).
 
 ### Markdown features
 
 This program uses the base [`markdown` syntax](https://daringfireball.net/projects/markdown/syntax) plus additional syntax, all thanks to [`python-markdown`](https://python-markdown.github.io/) that provides [extensions](https://python-markdown.github.io/extensions/). The following extensions are used:
 
 - Extra (collection of QoL extensions).
 - Meta-Data.
 - Sane Lists.
 - SmartyPants.
 - Table of Contents.
+  - With `permalink=True` and `baselevel=2`, for more: [python-markdown toc](https://python-markdown.github.io/extensions/toc/).
 - WikiLinks.
+- [pymdvar](https://github.com/luevano/pymdvar) (made by me).
 - [yafg - Yet Another Figure Generator](https://git.sr.ht/~ferruck/yafg)
 - [Markdown Checklist](https://github.com/FND/markdown-checklist)
 - [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/)
 	- [Caret](https://facelessuser.github.io/pymdown-extensions/extensions/caret/)
 	- [Tilde](https://facelessuser.github.io/pymdown-extensions/extensions/tilde/)
 	- [Mark](https://facelessuser.github.io/pymdown-extensions/extensions/mark/)
 
@@ -92,15 +103,15 @@
 pyssg -i
 ```
 
 - You can modify the basic templates as needed (see [variables available for Jinja](#available-jinja-variables)).
 
 - Strongly recommended to edit the `rss.xml` template.
 
-4. Place your `*.md` files somewhere inside the source directory. It accepts sub-directories.
+4. Place your `*.md` files somewhere inside the source directory. It accepts sub-directories. Optionally configure for subdirectories if they are to be treated a bit different.
 
 - Recommended (no longer mandatory) metadata keys that can be added to the top of `.md` files:
 
 ```
 title: the title of your blog entry or whatever
 author: your name or online handle
 	another name maybe for multiple authors?
@@ -108,34 +119,36 @@
 summary: a summary of the entry
 tags: english
 	short
 	tutorial
 	etc
 ```
 
-- You can add more meta-data keys as long as it is [Python-Markdown compliant](https://python-markdown.github.io/extensions/meta_data/), and these will ve [available as Jinja variables](#available-jinja-variables).
+- You can add more meta-data keys as long as it is [Python-Markdown compliant](https://python-markdown.github.io/extensions/meta_data/), and these will ve [available as Jinja variables](#available-jinja-variables) in the `meta` object (`dict[str, Any]`).
 
 5. Build the `*.html` with:
 
 ```sh
 pyssg -b
 ```
 
-- After this, you have ready to deploy `*.html` files.
+- After this, you have ready to deploy `*.html` files from the `dst` directory.
 
 ## Config file
 
 All sections/options need to be compliant with [`PyYAML`](https://pyyaml.org/) which should be compliant with [`YAML 1.2`](https://yaml.org/spec/1.2.2/). Additionaly, I've added the custom tag `!join` which concatenates strings from an array, which an be used as follows:
 
 ```yaml
 variable: &variable_reference_name "value"
 other_variable: !join [*variable_reference_name, "other_value", 1]
 ```
 
-Which would produce `other_variable: "valueother_value1"`. Also environment variables will be expanded internally.
+Which would produce `other_variable: "valueother_value1"`. Also **environment variables will be expanded internally**.
+
+**Note**: URL's shouldn't have the trailing slash `/`.
 
 The following is a list of config items that need to be present in the config unless stated otherwise:
 
 ```yaml
 %YAML 1.2
 ---
 # not needed, shown here as an example of the !join tag
@@ -145,87 +158,115 @@
 path:
   src: !join [*root, "src"] # $HOME/path/to/src
   dst: "$HOME/some/other/path/to/dst"
   plt: "plt"
   db: !join [*root, "src/", "db.psv"]
 url:
   main: "https://example.com"
+  # I personally use a "static" url for images/scripts/css/etc, not necessary
+  static: "https://static.example.com"
 fmt:
   date: "%a, %b %d, %Y @ %H:%M %Z"
-  list_date: "%b %d"
-  list_sep_date: "%B %Y"
+  list_date: "%b %d" # not necessary
+  list_sep_date: "%B %Y" # not necessary
 dirs:
   /: # root "dir_path", whatever is sitting directly under "src"
-	cfg:
-	  plt: "page.html"
-	  # the template can be specified instead of just True/False, a default template will used
-	  tags: False
-	  index: True
-	  rss: True
-	  sitemap: True
-	  exclude_dirs: ["articles", "blog"] # optional; list of subdirectories to exclude when parsing the / dir_path
-# below are other example "dir_paths", can be named anything, only the / (above) is mandatory
-  articles:
-    cfg:
-	  plt: "page.html"
-	  tags: True
-	  index: True
-	  rss: True
-	  sitemap: True
-  blog:
     cfg:
-	  # ...
+      plt: "page.html" # each page template, relative to path/plt
+      tags: False
+      index: True
+      rss: True
+      sitemap: True
+      exclude_dirs: ["articles", "blog"] # optional; list of subdirs to exclude when parsing this "dir_path"
 ...
 ```
 
-The config under `dirs` are just per-subdirectory configuration of directories under `src`. Only the `/` "dir_path" is required as it is the config for the root `src` path files.
+So far only [pymdvar](https://github.com/luevano/pymdvar) can be configured by including the following to the config:
+
+```yaml
+exts:
+  pymdvar:
+    variables:
+      SOME_VAR: "some value"
+      some_other_variable: 123
+    enable_env: True # to read environment variables
+```
+
+The config under `dirs` are just per-subdirectory configuration of directories under `src`, which I called "dir_paths" for lack of creativity. Only the `/` "dir_path" is required as it is the config for the root `src` path files. Mandatory config items for each "dir_path":
+
+```yaml
+cfg:
+  plt: "template.html"
+  tags: True
+  index: True
+  rss: True
+  sitemap: True
+  exclude: [] # not necessary
+```
+
+So that extra "dir_paths" can be added under `dirs`:
 
-The following will be added on runtime:
+```yaml
+dirs:
+  /:
+    cfg:
+      ...
+  articles:
+    cfg:
+      ...
+  gallery:
+    cfg:
+      ...
+  etc:
+    ...
+```
+
+The following will be added on runtime to the configuration:
 
 ```yaml
 %YAML 1.2
 ---
 fmt:
   rss_date: "%a, %d %b %Y %H:%M:%S GMT" # fixed
   sitemap_date: "%Y-%m-%d" # fixed
 info:
   version: "x.y.z" # current 'pyssg' version (0.5.1.dev16, for example)
   debug: True/False # depending if --debug was used when executing
-  force: True/False # depending if --force was used when executing
 rss_run_date: # date the program was run, formatted with 'fmt.rss_date'
 sitemap_run_date: # date the program was run, formatted with 'fmt.sitemap_date'
 ...
 ```
 
-You can add any other option/section that you can later use in the Jinja templates via the exposed config object. URL's shouldn't have the trailing slash `/`
+You can add any other option/section that you can later use in the Jinja templates via the exposed config object.
+
 
 ## Available Jinja variables
 
 These variables are exposed to use within the templates. The below list is displayed in the form of *variable (type) (available from): description*. `field1/field2/field3/...` describe config file section from the YAML file and option and `object.attribute` corresponding object and it's attribute.
 
-- `config` (`dict`) (all): parsed config file plus the added options internally (as described in [config file](#config-file)).
-- `dir_config` (`dict`) (all*): parsed dir_config file plus the added options internally (as described in [config file](#config-file)). *This is for all of the specific "dir_path" files, as per configured in the YAML file `dirs.dir_path.cfg` (for exmaple `dirs./.cfg` for the required dir_path).
+- `config` (`dict[str, Any]`) (all): parsed config file plus the added options internally (as described in [config file](#config-file)).
+- `dir_config` (`dict[str, Any]`) (all*): parsed dir_config file plus the added options internally (as described in [config file](#config-file)). *This is for all of the specific "dir_path" files, as per configured in the YAML file `dirs.dir_path.cfg` (for exmaple `dirs./.cfg` for the required dir_path).
 - `all_pages` (`list(Page)`) (all): list of all the pages, sorted by creation time, reversed.
 - `page` (`Page`) (`page.html`): contains the following attributes (genarally these are parsed from the metadata in the `*.md` files):
 	- `title` (`str`): title of the page.
 	- `author` (`list[str]`): list of authors of the page.
 	- `lang` (`str`): page language, used for the general `html` tag `lang` attribute.
 	- `summary` (`str`): summary of the page, as specified in the `*.md` file.
 	- `content` (`str`): actual content of the page, this is the `html`.
+    - `toc` (`str`): table of contents as taken from `md.toc`.
+    - `toc_tokens` (`list[dict[str, Any]]`): table of contents tokens as taken from `md.toc_tokens`.
 	- `cdatetime` (`datetime.datetime`): creation datetime object of the page.
-	- `cdate` (`method`): method thtat takes the name of the `fmt.FMT` and applies it to the `cdatetime` object.
+	- `cdate` (`method(FMT: str)`): takes the name of the `fmt.FMT` and applies it to the `cdatetime` object.
 	- `cdate_rss` (`str`): formatted `cdatetime` as required by rss.
 	- `cdate_sitemap` (`str`): formatted `cdatetime` as required by sitemap.
 	- `mdatetime` (`datetime.datetime`): modification datetime object of the page. Defaults to `None`.
-	- `mdate` (`method`): method thtat takes the name of the `fmt.FMT` and applies it to the `mdatetime` object.
+	- `mdate` (`method(FMT: str)`): takes the name of the `fmt.FMT` and applies it to the `mdatetime` object.
 	- `mdate_rss` (`str`): formatted `mdatetime` as required by rss.
 	- `mdate_sitemap` (`str`): formatted `mdatetime` as required by sitemap.
-	- `tags` (`list(tuple(str))`): list of tuple of tags of the page, containing the name and the url of the tag, in that order. Defaults to empty list.
+	- `tags` (`list[tuple[str]]`): list of tuple of tags of the page, containing the name and the url of the tag, respectively. Defaults to empty list.
 	- `url` (`str`): url of the page, this already includes the `url/main` from config file.
-	- `image_url` (`str`): image url of the page, this already includes the `url/static`. Defaults to the `url/default_image` config option.
 	- `next/previous` (`Page`): reference to the next or previous page object (containing all these attributes). Defaults to `None`.
-	- `og` (`dict(str, str)`): dict for object graph metadata.
-	- `meta` (`dict(str, list(str))`): meta dict as obtained from python-markdown, in case you use a meta tag not yet supported, it will be available there.
-- `tag` (`tuple(str)`) (`tag.html`): tuple of name and url of the current tag.
-- `tag_pages` (`list(Page)`) (`tag.html`): similar to `all_pages` but contains all the pages for the current tag.
-- `all_tags` (`list(tuple(str))`) (all): similar to `page.tags` but contains all the tags.
+	- `meta` (`dict[str, list[str]]`): meta dict as obtained from `python-markdown`, in case you use a meta tag not directly supported, it will be available there.
+- `tag` (`tuple[str]`) (`tag.html`): tuple of name and url of the current tag.
+- `tag_pages` (`list[Page]`) (`tag.html`): similar to `all_pages` but contains all the pages for the current tag.
+- `all_tags` (`list[tuple[str]]`) (all): similar to `page.tags` but contains all the tags.
```

