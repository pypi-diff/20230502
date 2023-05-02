# Comparing `tmp/phanterpwa-13.12.8.tar.gz` & `tmp/phanterpwa-13.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\phanterpwa-13.12.8.tar", last modified: Mon Dec  5 02:55:32 2022, max compression
+gzip compressed data, was "dist\phanterpwa-13.13.0.tar", last modified: Tue May  2 02:44:47 2023, max compression
```

## Comparing `phanterpwa-13.12.8.tar` & `phanterpwa-13.13.0.tar`

### file list

```diff
@@ -1,567 +1,568 @@
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/
--rw-rw-rw-   0        0        0    19227 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1918 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/PKG-INFO
--rw-rw-rw-   0        0        0      456 2021-03-14 22:53:21.000000 phanterpwa-13.12.8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/
--rw-rw-rw-   0        0        0      397 2022-12-04 16:49:36.000000 phanterpwa-13.12.8/phanterpwa/__init__.py
--rw-rw-rw-   0        0        0     4017 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/backend/
--rw-rw-rw-   0        0        0       68 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/__init__.py
--rw-rw-rw-   0        0        0    62992 2022-11-26 15:00:34.000000 phanterpwa-13.12.8/phanterpwa/backend/dataforms.py
--rw-rw-rw-   0        0        0    55021 2022-11-26 14:46:09.000000 phanterpwa-13.12.8/phanterpwa/backend/decorators.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/
--rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/__init__.py
--rw-rw-rw-   0        0        0     8365 2022-05-09 18:31:57.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/auth.py
--rw-rw-rw-   0        0        0     1581 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/cas.py
--rw-rw-rw-   0        0        0     2234 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/credentials.py
--rw-rw-rw-   0        0        0     1919 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/extra_validations.py
--rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/gallery.py
--rw-rw-rw-   0        0        0     1379 2022-05-11 18:10:28.000000 phanterpwa-13.12.8/phanterpwa/backend/pydal/internal_messages.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/__init__.py
--rw-rw-rw-   0        0        0    59625 2022-04-29 21:46:35.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/admin.py
--rw-rw-rw-   0        0        0   166939 2022-07-06 19:17:03.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/auth.py
--rw-rw-rw-   0        0        0    24299 2022-07-06 19:20:32.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/cas.py
--rw-rw-rw-   0        0        0    46299 2022-07-06 19:14:19.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/credentials.py
--rw-rw-rw-   0        0        0     3775 2022-07-06 18:58:48.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/errors.py
--rw-rw-rw-   0        0        0     2490 2021-05-26 06:53:02.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/i18n_server.py
--rw-rw-rw-   0        0        0    15986 2022-07-06 19:19:25.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/internal_messages.py
--rw-rw-rw-   0        0        0    44555 2022-07-06 19:18:59.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/oauth.py
--rw-rw-rw-   0        0        0     5527 2022-11-23 12:46:20.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/websocket.py
--rw-rw-rw-   0        0        0      723 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/backend/request_handlers/welcome.py
--rw-rw-rw-   0        0        0     1300 2022-07-06 19:19:45.000000 phanterpwa-13.12.8/phanterpwa/backend/security.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/__init__.py
--rw-rw-rw-   0        0        0    12359 2022-07-06 19:12:56.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/captcha.py
--rw-rw-rw-   0        0        0   133091 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/captchadata.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/__init__.py
--rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/circle.recs
--rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/heart.recs
--rw-rw-rw-   0        0        0      131 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/octagon.recs
--rw-rw-rw-   0        0        0       77 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/square.recs
--rw-rw-rw-   0        0        0      191 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/recipes/star.recs
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/sass/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/sass/__init__.py
--rw-rw-rw-   0        0        0     1137 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/sass/captcha.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/
--rw-rw-rw-   0        0        0       71 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/
--rw-rw-rw-   0        0        0     1445 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/butterfly.recs
--rw-rw-rw-   0        0        0     3131 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/crab.recs
--rw-rw-rw-   0        0        0     2662 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/pig.recs
--rw-rw-rw-   0        0        0     1424 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/rabbit.recs
--rw-rw-rw-   0        0        0     2968 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/rooster.recs
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/arrow/
--rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/arrow/down.recs
--rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/arrow/left.recs
--rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/arrow/right.recs
--rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/arrow/up.recs
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/
--rw-rw-rw-   0        0        0     1570 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/a.recs
--rw-rw-rw-   0        0        0     1966 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/b.recs
--rw-rw-rw-   0        0        0     1254 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/c.recs
--rw-rw-rw-   0        0        0     1377 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/d.recs
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/
--rw-rw-rw-   0        0        0     1064 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs
--rw-rw-rw-   0        0        0     1863 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs
--rw-rw-rw-   0        0        0     2914 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs
--rw-rw-rw-   0        0        0      688 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/
--rw-rw-rw-   0        0        0     2263 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/four.recs
--rw-rw-rw-   0        0        0     1231 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/one.recs
--rw-rw-rw-   0        0        0     1940 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/three.recs
--rw-rw-rw-   0        0        0     1758 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/two.recs
--rw-rw-rw-   0        0        0    47478 2022-04-28 00:32:01.000000 phanterpwa-13.12.8/phanterpwa/compiler.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/components/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/__init__.py
--rw-rw-rw-   0        0        0    14007 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/inputs.py
--rw-rw-rw-   0        0        0     6111 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/left_bar.py
--rw-rw-rw-   0        0        0    25523 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/materialize.py
--rw-rw-rw-   0        0        0    19016 2022-02-21 15:44:58.000000 phanterpwa-13.12.8/phanterpwa/components/phanterpwagallery.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/__init__.py
--rw-rw-rw-   0        0        0     3584 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/android.py
--rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/android.sass
--rw-rw-rw-   0        0        0     1483 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/discs.py
--rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/discs.sass
--rw-rw-rw-   0        0        0     1116 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/explosion.py
--rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/explosion.sass
--rw-rw-rw-   0        0        0     1460 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/run_points.py
--rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/run_points.sass
--rw-rw-rw-   0        0        0      620 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/square.py
--rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/square.sass
--rw-rw-rw-   0        0        0      828 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/squares.py
--rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/components/preloaders/squares.sass
--rw-rw-rw-   0        0        0    26327 2022-07-06 20:17:07.000000 phanterpwa-13.12.8/phanterpwa/configer.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/frontend/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/__init__.py
--rw-rw-rw-   0        0        0    56675 2022-07-06 19:39:07.000000 phanterpwa-13.12.8/phanterpwa/frontend/application.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/__init__.py
--rw-rw-rw-   0        0        0    69689 2022-04-04 10:57:28.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/admin.py
--rw-rw-rw-   0        0        0   172575 2022-12-05 02:22:39.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/auth_user.py
--rw-rw-rw-   0        0        0    57394 2022-04-04 10:57:28.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/datetimepicker.py
--rw-rw-rw-   0        0        0     3726 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/events.py
--rw-rw-rw-   0        0        0    34075 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/gallery.py
--rw-rw-rw-   0        0        0    55112 2021-12-06 00:44:42.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/left_bar.py
--rw-rw-rw-   0        0        0     9100 2022-12-05 02:22:50.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/modal.py
--rw-rw-rw-   0        0        0      791 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/pagination.py
--rw-rw-rw-   0        0        0     4060 2021-11-21 02:57:14.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/snippets.py
--rw-rw-rw-   0        0        0     3175 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/top_slide.py
--rw-rw-rw-   0        0        0   227581 2022-12-05 02:23:16.000000 phanterpwa-13.12.8/phanterpwa/frontend/components/widgets.py
--rw-rw-rw-   0        0        0     4042 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/decorators.py
--rw-rw-rw-   0        0        0    31267 2021-08-01 05:39:42.000000 phanterpwa-13.12.8/phanterpwa/frontend/fmasks.py
--rw-rw-rw-   0        0        0    41536 2022-05-13 19:24:36.000000 phanterpwa-13.12.8/phanterpwa/frontend/forms.py
--rw-rw-rw-   0        0        0    33833 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/gallery.py
--rw-rw-rw-   0        0        0    14753 2022-04-30 16:30:51.000000 phanterpwa-13.12.8/phanterpwa/frontend/gatehandler.py
--rw-rw-rw-   0        0        0     9861 2022-06-16 23:20:19.000000 phanterpwa-13.12.8/phanterpwa/frontend/helpers.py
--rw-rw-rw-   0        0        0     4593 2022-04-04 10:57:28.000000 phanterpwa-13.12.8/phanterpwa/frontend/i18n.py
--rw-rw-rw-   0        0        0    41699 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/initializer.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/frontend/plugins/
--rw-rw-rw-   0        0        0    27481 2022-11-26 15:07:06.000000 phanterpwa-13.12.8/phanterpwa/frontend/plugins/client.py
--rw-rw-rw-   0        0        0     4927 2022-08-19 19:22:51.000000 phanterpwa-13.12.8/phanterpwa/frontend/preloaders.py
--rw-rw-rw-   0        0        0     1798 2021-11-17 18:30:18.000000 phanterpwa-13.12.8/phanterpwa/frontend/progressbar.py
--rw-rw-rw-   0        0        0     5467 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/frontend/selects.py
--rw-rw-rw-   0        0        0    20154 2022-05-21 19:29:34.000000 phanterpwa-13.12.8/phanterpwa/frontend/server.py
--rw-rw-rw-   0        0        0    10504 2021-11-30 01:36:21.000000 phanterpwa-13.12.8/phanterpwa/frontend/validations.py
--rw-rw-rw-   0        0        0     4381 2022-04-29 11:22:51.000000 phanterpwa-13.12.8/phanterpwa/frontend/websocket.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/gallery/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/gallery/__init__.py
--rw-rw-rw-   0        0        0     7220 2022-02-21 15:44:58.000000 phanterpwa-13.12.8/phanterpwa/gallery/cutter.py
--rw-rw-rw-   0        0        0     8578 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/gallery/integrationDAL.py
--rw-rw-rw-   0        0        0    12138 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/helpers.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/i18n/
--rw-rw-rw-   0        0        0     8670 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/
--rw-rw-rw-   0        0        0     1066 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/LICENSE
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/controllers/
--rw-rw-rw-   0        0        0      206 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/controllers/__init__.py
--rw-rw-rw-   0        0        0    29445 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/controllers/developer.py
--rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/controllers/welcome.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/
--rw-rw-rw-   0        0        0      682 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table
--rw-rw-rw-   0        0        0      487 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_group.table
--rw-rw-rw-   0        0        0      536 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table
--rw-rw-rw-   0        0        0     2572 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table
--rw-rw-rw-   0        0        0      793 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table
--rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table
--rw-rw-rw-   0        0        0      842 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table
--rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table
--rw-rw-rw-   0        0        0      597 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table
--rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table
--rw-rw-rw-   0        0        0      590 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table
--rw-rw-rw-   0        0        0      714 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table
--rw-rw-rw-   0        0        0      733 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table
--rw-rw-rw-   0        0        0       35 2022-04-26 23:50:37.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/readme.txt
--rw-rw-rw-   0        0        0     4285 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/sql.log
--rw-rw-rw-   0        0        0    81920 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite
--rw-rw-rw-   0        0        0     6349 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/handlers.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/admin/
--rw-rw-rw-   0        0        0      807 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json
--rw-rw-rw-   0        0        0     1541 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/
--rw-rw-rw-   0        0        0      497 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/entries.json
--rw-rw-rw-   0        0        0     1124 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/email/
--rw-rw-rw-   0        0        0     1577 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json
--rw-rw-rw-   0        0        0     3117 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json
--rw-rw-rw-   0        0        0     3108 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/entries.json
--rw-rw-rw-   0        0        0     6164 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/models/
--rw-rw-rw-   0        0        0      996 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/statics/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/statics/images/
--rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/statics/images/user.png
--rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/uploads/
--rw-rw-rw-   0        0        0       28 2022-04-27 00:31:13.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/uploads/readme.txt
--rw-rw-rw-   0        0        0     2812 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/core.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/__init__.py
--rw-rw-rw-   0        0        0     1121 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/handlers.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/languages/
--rw-rw-rw-   0        0        0     1266 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json
--rw-rw-rw-   0        0        0     2403 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/
--rw-rw-rw-   0        0        0     8390 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/
--rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass
--rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/logo.sass
--rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass
--rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/
--rw-rw-rw-   0        0        0     1177 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass
--rw-rw-rw-   0        0        0      121 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/developer.sass
--rw-rw-rw-   0        0        0      564 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/__init__.py
--rw-rw-rw-   0        0        0      785 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py
--rw-rw-rw-   0        0        0      675 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py
--rw-rw-rw-   0        0        0      747 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py
--rw-rw-rw-   0        0        0      963 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py
--rw-rw-rw-   0        0        0    38183 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py
--rw-rw-rw-   0        0        0     1272 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py
--rw-rw-rw-   0        0        0     7459 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg
--rw-rw-rw-   0        0        0      158 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/svg_logo.py
--rw-rw-rw-   0        0        0     3267 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/
--rw-rw-rw-   0        0        0    38395 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py
--rw-rw-rw-   0        0        0     1122 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py
--rw-rw-rw-   0        0        0    20765 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/
--rw-rw-rw-   0        0        0     1363 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/
--rw-rw-rw-   0        0        0      932 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/__init__.py
--rw-rw-rw-   0        0        0     2543 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py
--rw-rw-rw-   0        0        0    12805 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py
--rw-rw-rw-   0        0        0     4692 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py
--rw-rw-rw-   0        0        0    19789 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/__init__.py
--rw-rw-rw-   0        0        0    17986 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py
--rw-rw-rw-   0        0        0     9456 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py
--rw-rw-rw-   0        0        0    46491 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py
--rw-rw-rw-   0        0        0    46731 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py
--rw-rw-rw-   0        0        0     2600 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py
--rw-rw-rw-   0        0        0    16739 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py
--rw-rw-rw-   0        0        0     5783 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py
--rw-rw-rw-   0        0        0     5528 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/
--rw-rw-rw-   0        0        0     1502 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/
--rw-rw-rw-   0        0        0    57333 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css
--rw-rw-rw-   0        0        0     6138 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css
--rw-rw-rw-   0        0        0   444223 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/
--rw-rw-rw-   0        0        0    11462 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png
--rw-rw-rw-   0        0        0     7107 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    19743 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png
--rw-rw-rw-   0        0        0    19618 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     6233 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png
--rw-rw-rw-   0        0        0      246 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/browserconfig.xml
--rw-rw-rw-   0        0        0     1209 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png
--rw-rw-rw-   0        0        0     1865 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png
--rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico
--rw-rw-rw-   0        0        0      268 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/manifest.json
--rw-rw-rw-   0        0        0     5185 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png
--rw-rw-rw-   0        0        0      426 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/site.webmanifest
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/
--rw-rw-rw-   0        0        0    46822 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot
--rw-rw-rw-   0        0        0    57097 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg
--rw-rw-rw-   0        0        0    46592 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf
--rw-rw-rw-   0        0        0    30204 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff
--rw-rw-rw-   0        0        0    25040 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2
--rw-rw-rw-   0        0        0    12376 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2
--rw-rw-rw-   0        0        0    16028 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2
--rw-rw-rw-   0        0        0    21659 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot
--rw-rw-rw-   0        0        0   127584 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0    61628 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff
--rw-rw-rw-   0        0        0    48524 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2
--rw-rw-rw-   0        0        0    18004 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2
--rw-rw-rw-   0        0        0    36060 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2
--rw-rw-rw-   0        0        0    49240 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2
--rw-rw-rw-   0        0        0    17854 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot
--rw-rw-rw-   0        0        0    48974 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg
--rw-rw-rw-   0        0        0    36176 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf
--rw-rw-rw-   0        0        0    20268 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff
--rw-rw-rw-   0        0        0    15736 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/
--rw-rw-rw-   0        0        0   104800 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg
--rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png
--rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/
--rw-rw-rw-   0        0        0    45781 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js
--rw-rw-rw-   0        0        0    43028 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map
--rw-rw-rw-   0        0        0      988 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js
--rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js
--rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map
--rw-rw-rw-   0        0        0    11272 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/
--rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json
--rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/
--rw-rw-rw-   0        0        0     8705 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css
--rw-rw-rw-   0        0        0   397228 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/
--rw-rw-rw-   0        0        0     6268 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html
--rw-rw-rw-   0        0        0    14676 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js
--rw-rw-rw-   0        0        0     2014 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/
--rw-rw-rw-   0        0        0   133034 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   132728 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    89824 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76548 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34390 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0    34092 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16800 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13600 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   194078 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   193792 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0    99004 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    76120 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/logs/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/logs/api.log
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/logs/app.log
--rw-rw-rw-   0        0        0       23 2022-04-26 23:49:53.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/logs/readme.txt
--rw-rw-rw-   0        0        0      286 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/production.py
--rw-rw-rw-   0        0        0      145 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/run.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/
--rw-rw-rw-   0        0        0     9893 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass
--rw-rw-rw-   0        0        0     1228 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_admin.json
--rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_components.json
--rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json
--rw-rw-rw-   0        0        0      221 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/phanterpwa_modules_mtime.json
--rw-rw-rw-   0        0        0        0 2022-04-26 23:56:37.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/readme.txt
--rw-rw-rw-   0        0        0    11082 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_admin.json
--rw-rw-rw-   0        0        0     8222 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_components.json
--rw-rw-rw-   0        0        0     8119 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0     6140 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json
--rw-rw-rw-   0        0        0     1369 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_admin.json
--rw-rw-rw-   0        0        0      592 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_components.json
--rw-rw-rw-   0        0        0     1075 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0     3682 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json
--rw-rw-rw-   0        0        0      681 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/templates_mtime_admin.json
--rw-rw-rw-   0        0        0      338 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/templates_mtime_components.json
--rw-rw-rw-   0        0        0      474 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/templates_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0      190 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/templates_mtime_sindfa.json
--rw-rw-rw-   0        0        0     2676 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json
--rw-rw-rw-   0        0        0      810 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json
--rw-rw-rw-   0        0        0     1342 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0     1127 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/trash/
--rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.12.8/phanterpwa/interface/Admin/trash/readme.txt
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/__init__.py
--rw-rw-rw-   0        0        0     7015 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/admin_tk.py
--rw-rw-rw-   0        0        0    50861 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/cli.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/grafics/
--rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/grafics/icon.ico
--rw-rw-rw-   0        0        0      634 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/grafics/on.jpg
--rw-rw-rw-   0        0        0   140200 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/graphic.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/interface/langs/
--rw-rw-rw-   0        0        0     5309 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/langs/English.json
--rw-rw-rw-   0        0        0     5339 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/langs/Portuguese.json
--rw-rw-rw-   0        0        0     2800 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/interface/langs/entries.json
--rw-rw-rw-   0        0        0     5741 2021-09-05 00:25:27.000000 phanterpwa-13.12.8/phanterpwa/mail.py
--rw-rw-rw-   0        0        0    10764 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/reversexml.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/samples/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/__init__.py
--rw-rw-rw-   0        0        0      372 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/about_cli
--rw-rw-rw-   0        0        0      269 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/about_graphic
--rw-rw-rw-   0        0        0      533 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/art
--rw-rw-rw-   0        0        0      408 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/art_cli
--rw-rw-rw-   0        0        0     2183 2022-07-06 20:15:09.000000 phanterpwa-13.12.8/phanterpwa/samples/config.json
--rw-rw-rw-   0        0        0     4996 2022-11-26 15:08:21.000000 phanterpwa-13.12.8/phanterpwa/samples/email.sass
--rw-rw-rw-   0        0        0     6072 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/email_activation_code.py
--rw-rw-rw-   0        0        0     5840 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/samples/email_password.py
--rw-rw-rw-   0        0        0     9137 2021-09-05 04:01:49.000000 phanterpwa-13.12.8/phanterpwa/samples/email_two_factor_code.py
--rw-rw-rw-   0        0        0     1879 2022-07-06 20:14:49.000000 phanterpwa-13.12.8/phanterpwa/samples/project_config_sample.py
--rw-rw-rw-   0        0        0      236 2021-09-05 03:59:44.000000 phanterpwa-13.12.8/phanterpwa/samples/sms_activation_code.py
--rw-rw-rw-   0        0        0      245 2021-09-04 16:15:07.000000 phanterpwa-13.12.8/phanterpwa/samples/sms_password.py
--rw-rw-rw-   0        0        0      241 2021-09-04 16:33:02.000000 phanterpwa-13.12.8/phanterpwa/samples/sms_two_factor_code.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/scaffolds/
--rw-rw-rw-   0        0        0  2214300 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/scaffolds/__init__.py
--rw-rw-rw-   0        0        0    12247 2022-09-23 00:15:14.000000 phanterpwa-13.12.8/phanterpwa/server.py
--rw-rw-rw-   0        0        0     1313 2021-09-05 16:25:04.000000 phanterpwa-13.12.8/phanterpwa/sms.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/tests/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/tests/helpers_out/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/helpers_out/__init__.py
--rw-rw-rw-   0        0        0      331 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/helpers_out/my_sass.sass
--rw-rw-rw-   0        0        0      352 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/helpers_out/new_sass.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/__init__.py
--rw-rw-rw-   0        0        0      456 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/entries.json
--rw-rw-rw-   0        0        0      854 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/es.json
--rw-rw-rw-   0        0        0      852 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/fr.json
--rw-rw-rw-   0        0        0      860 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/pt-BR.json
--rw-rw-rw-   0        0        0      851 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/pt-PT.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:31.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/__init__.py
--rw-rw-rw-   0        0        0     9764 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_android.html
--rw-rw-rw-   0        0        0     3489 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_discs.html
--rw-rw-rw-   0        0        0     5956 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html
--rw-rw-rw-   0        0        0     4451 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html
--rw-rw-rw-   0        0        0     1752 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_square.html
--rw-rw-rw-   0        0        0     4231 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_squares.html
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/static/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/static/__init__.py
--rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/static/jquery.min.js
--rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/static/jquery.min.map
--rw-rw-rw-   0        0        0     2117 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/not_project/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/not_project/__init__.py
--rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/not_project/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project-invalid-name/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project-invalid-name/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project-invalid-name/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project01/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project01/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project01/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project02/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project02/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/project02/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/without_configjson/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_cli_projects/without_configjson/__init__.py
--rw-rw-rw-   0        0        0     4079 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_components_preloaders.py
--rw-rw-rw-   0        0        0    12208 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/fake_project/
--rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/fake_project/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project-invalid-name/
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project-invalid-name/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backapps/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backapps/api/
--rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backend/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backend/api/
--rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini
--rw-rw-rw-   0        0        0     2618 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontapps/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontapps/app01/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontapps/app01/app.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontapps/app02/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontapps/app02/app.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontend/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontend/app01/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontend/app01/app.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontend/app02/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/frontend/app02/app.ini
--rw-rw-rw-   0        0        0      189 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/project.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project02/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project02/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project02/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/
--rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini
--rw-rw-rw-   0        0        0     2143 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/app.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/app.ini
--rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/project.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/
--rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini
--rw-rw-rw-   0        0        0     2640 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/config.json
--rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/project.ini
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_folder/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_folder/cfg.json
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_folder/cfgij.json
--rw-rw-rw-   0        0        0       23 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_folder/config.json
--rw-rw-rw-   0        0        0    80202 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers_languages/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers_languages/__init__.py
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers_languages/en-US.json
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers_languages/entries.json
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers_languages/glingon.json
--rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/tests/test_helpers_languages/pt-BR.json
--rw-rw-rw-   0        0        0     3729 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n_languages/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n_languages/__init__.py
--rw-rw-rw-   0        0        0       65 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n_languages/en-US.json
--rw-rw-rw-   0        0        0       36 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n_languages/entries.json
--rw-rw-rw-   0        0        0       63 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n_languages/pt-BR.json
--rw-rw-rw-   0        0        0       63 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_i18n_languages/pt-PT.json
--rw-rw-rw-   0        0        0     4212 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_reversexml.py
--rw-rw-rw-   0        0        0    11521 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_tools.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/tests/test_tools_humanize_seconds/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/test_tools_humanize_seconds/entries.json
--rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.12.8/phanterpwa/tests/test_tools_humanize_seconds/pt-BR.json
--rw-rw-rw-   0        0        0     1386 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/tests/tests.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:30.000000 phanterpwa-13.12.8/phanterpwa/third_parties/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/third_parties/__init__.py
--rw-rw-rw-   0        0        0     5857 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/third_parties/xss.py
--rw-rw-rw-   0        0        0    45683 2022-04-27 18:34:47.000000 phanterpwa-13.12.8/phanterpwa/tools.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/trash/
--rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.12.8/phanterpwa/trash/readme.txt
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/
--rw-rw-rw-   0        0        0     1794 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/alert_top_activation.sass
--rw-rw-rw-   0        0        0     1551 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/breascrumbs.sass
--rw-rw-rw-   0        0        0     2741 2021-07-27 18:35:01.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/buttons.sass
--rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/capcha_preload.sass
--rw-rw-rw-   0        0        0     7323 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/captcha.sass
--rw-rw-rw-   0        0        0     5213 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass
--rw-rw-rw-   0        0        0      643 2022-11-25 21:37:56.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/card.sass
--rw-rw-rw-   0        0        0    13548 2022-04-04 10:57:28.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/cmp_auth_user.sass
--rw-rw-rw-   0        0        0     6615 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/datetimepicker.sass
--rw-rw-rw-   0        0        0     1741 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/developer.sass
--rw-rw-rw-   0        0        0     3154 2022-06-07 17:05:55.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/easy.sass
--rw-rw-rw-   0        0        0     1067 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/flash.sass
--rw-rw-rw-   0        0        0     2937 2022-04-27 17:07:49.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/forms.sass
--rw-rw-rw-   0        0        0     1888 2022-05-17 18:44:18.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/messages.sass
--rw-rw-rw-   0        0        0     3190 2022-04-04 10:57:28.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/modal.sass
--rw-rw-rw-   0        0        0     1694 2021-09-05 18:33:48.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/modal_login.sass
--rw-rw-rw-   0        0        0      649 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/phanterpwa_gallery.sass
--rw-rw-rw-   0        0        0     4103 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass
--rw-rw-rw-   0        0        0     1450 2021-08-13 03:26:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass
--rw-rw-rw-   0        0        0     2959 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/progressbar.sass
--rw-rw-rw-   0        0        0      660 2022-02-03 09:45:15.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/pseudomodal.sass
--rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/run_points.sass
--rw-rw-rw-   0        0        0     1536 2021-06-17 02:27:21.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/sections.sass
--rw-rw-rw-   0        0        0      811 2021-05-25 20:28:47.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/snippet.sass
--rw-rw-rw-   0        0        0    78485 2022-12-04 21:28:01.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/widgets.sass
--rw-rw-rw-   0        0        0     4968 2021-06-15 20:39:00.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/components/xtable.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/display/
--rw-rw-rw-   0        0        0    42388 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/display/grid.sass
--rw-rw-rw-   0        0        0     3962 2021-12-14 21:24:18.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/display/media_print.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/events/
--rw-rw-rw-   0        0        0      238 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/events/waves.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/extends/
--rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/extends/capcha_preload.sass
--rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/extends/logo.sass
--rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/extends/run_points.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/gates/
--rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/gates/componentes.sass
--rw-rw-rw-   0        0        0      631 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/gates/main.sass
--rw-rw-rw-   0        0        0     9341 2022-04-27 17:07:49.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/phanterpwa.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/plugins/
--rw-rw-rw-   0        0        0      153 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/plugins/codemirror.sass
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/
--rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/android.sass
--rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/discs.sass
--rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/explosion.sass
--rw-rw-rw-   0        0        0      954 2022-08-19 19:22:51.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/indefined_text.sass
--rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/run_points.sass
--rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/square.sass
--rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/squares.sass
--rw-rw-rw-   0        0        0     8645 2022-04-27 17:07:49.000000 phanterpwa-13.12.8/phanterpwa/usual_sass/variables.sass
--rw-rw-rw-   0        0        0   162497 2022-04-04 10:57:28.000000 phanterpwa-13.12.8/phanterpwa/xmlconstructor.py
-drwxrwxrwx   0        0        0        0 2022-12-05 02:55:29.000000 phanterpwa-13.12.8/phanterpwa.egg-info/
--rw-rw-rw-   0        0        0     1918 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    25125 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      122 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/requires.txt
--rw-rw-rw-   0        0        0     5319 2022-12-05 02:55:28.000000 phanterpwa-13.12.8/phanterpwa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-05 02:55:32.000000 phanterpwa-13.12.8/setup.cfg
--rw-rw-rw-   0        0        0     4419 2022-07-15 11:22:48.000000 phanterpwa-13.12.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.653288 phanterpwa-13.13.0/
+-rw-rw-rw-   0        0        0     1087 2021-03-14 22:53:21.000000 phanterpwa-13.13.0/LICENSE
+-rw-rw-rw-   0        0        0    19227 2023-05-02 02:44:40.000000 phanterpwa-13.13.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1712 2023-05-02 02:44:47.652286 phanterpwa-13.13.0/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2021-03-14 22:53:21.000000 phanterpwa-13.13.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.996286 phanterpwa-13.13.0/phanterpwa/
+-rw-rw-rw-   0        0        0      397 2023-05-02 02:03:50.000000 phanterpwa-13.13.0/phanterpwa/__init__.py
+-rw-rw-rw-   0        0        0     4017 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.084287 phanterpwa-13.13.0/phanterpwa/backend/
+-rw-rw-rw-   0        0        0       68 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/__init__.py
+-rw-rw-rw-   0        0        0    62992 2022-11-26 15:00:34.000000 phanterpwa-13.13.0/phanterpwa/backend/dataforms.py
+-rw-rw-rw-   0        0        0    55413 2023-03-07 19:04:12.000000 phanterpwa-13.13.0/phanterpwa/backend/decorators.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.142287 phanterpwa-13.13.0/phanterpwa/backend/pydal/
+-rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/__init__.py
+-rw-rw-rw-   0        0        0     8365 2022-05-09 18:31:57.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/auth.py
+-rw-rw-rw-   0        0        0     1581 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/cas.py
+-rw-rw-rw-   0        0        0     2234 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/credentials.py
+-rw-rw-rw-   0        0        0     1919 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/extra_validations.py
+-rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/gallery.py
+-rw-rw-rw-   0        0        0     1379 2022-05-11 18:10:28.000000 phanterpwa-13.13.0/phanterpwa/backend/pydal/internal_messages.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.247286 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/__init__.py
+-rw-rw-rw-   0        0        0    59625 2023-04-16 16:08:09.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/admin.py
+-rw-rw-rw-   0        0        0   167134 2023-05-02 02:02:59.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/auth.py
+-rw-rw-rw-   0        0        0    24299 2022-07-06 19:20:32.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/cas.py
+-rw-rw-rw-   0        0        0    46299 2022-07-06 19:14:19.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/credentials.py
+-rw-rw-rw-   0        0        0     3775 2022-07-06 18:58:48.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/errors.py
+-rw-rw-rw-   0        0        0     2490 2021-05-26 06:53:02.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/i18n_server.py
+-rw-rw-rw-   0        0        0    15986 2022-07-06 19:19:25.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/internal_messages.py
+-rw-rw-rw-   0        0        0    44555 2022-07-06 19:18:59.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/oauth.py
+-rw-rw-rw-   0        0        0     5527 2022-11-23 12:46:20.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/websocket.py
+-rw-rw-rw-   0        0        0      723 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/backend/request_handlers/welcome.py
+-rw-rw-rw-   0        0        0     1300 2022-07-06 19:19:45.000000 phanterpwa-13.13.0/phanterpwa/backend/security.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.413287 phanterpwa-13.13.0/phanterpwa/captchasvg/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/__init__.py
+-rw-rw-rw-   0        0        0    12359 2022-07-06 19:12:56.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/captcha.py
+-rw-rw-rw-   0        0        0   133091 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/captchadata.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.461285 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/__init__.py
+-rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/circle.recs
+-rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/heart.recs
+-rw-rw-rw-   0        0        0      131 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/octagon.recs
+-rw-rw-rw-   0        0        0       77 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/square.recs
+-rw-rw-rw-   0        0        0      191 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/recipes/star.recs
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.470287 phanterpwa-13.13.0/phanterpwa/captchasvg/sass/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/sass/__init__.py
+-rw-rw-rw-   0        0        0     1137 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/sass/captcha.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.271286 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/
+-rw-rw-rw-   0        0        0       71 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.515315 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/
+-rw-rw-rw-   0        0        0     1445 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/butterfly.recs
+-rw-rw-rw-   0        0        0     3131 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/crab.recs
+-rw-rw-rw-   0        0        0     2662 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/pig.recs
+-rw-rw-rw-   0        0        0     1424 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/rabbit.recs
+-rw-rw-rw-   0        0        0     2968 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/rooster.recs
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.545289 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/arrow/
+-rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/arrow/down.recs
+-rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/arrow/left.recs
+-rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/arrow/right.recs
+-rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/arrow/up.recs
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.578287 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/
+-rw-rw-rw-   0        0        0     1570 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/a.recs
+-rw-rw-rw-   0        0        0     1966 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/b.recs
+-rw-rw-rw-   0        0        0     1254 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/c.recs
+-rw-rw-rw-   0        0        0     1377 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/d.recs
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.611290 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/
+-rw-rw-rw-   0        0        0     1064 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs
+-rw-rw-rw-   0        0        0     1863 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs
+-rw-rw-rw-   0        0        0     2914 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs
+-rw-rw-rw-   0        0        0      688 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.644288 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/
+-rw-rw-rw-   0        0        0     2263 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/four.recs
+-rw-rw-rw-   0        0        0     1231 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/one.recs
+-rw-rw-rw-   0        0        0     1940 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/three.recs
+-rw-rw-rw-   0        0        0     1758 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/two.recs
+-rw-rw-rw-   0        0        0    47478 2022-04-28 00:32:01.000000 phanterpwa-13.13.0/phanterpwa/compiler.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.313286 phanterpwa-13.13.0/phanterpwa/components/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/__init__.py
+-rw-rw-rw-   0        0        0    14007 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/inputs.py
+-rw-rw-rw-   0        0        0     6111 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/left_bar.py
+-rw-rw-rw-   0        0        0    25523 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/materialize.py
+-rw-rw-rw-   0        0        0    19016 2022-02-21 15:44:58.000000 phanterpwa-13.13.0/phanterpwa/components/phanterpwagallery.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.727287 phanterpwa-13.13.0/phanterpwa/components/preloaders/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/__init__.py
+-rw-rw-rw-   0        0        0     3584 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/android.py
+-rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/android.sass
+-rw-rw-rw-   0        0        0     1483 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/discs.py
+-rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/discs.sass
+-rw-rw-rw-   0        0        0     1116 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/explosion.py
+-rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/explosion.sass
+-rw-rw-rw-   0        0        0     1460 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/run_points.py
+-rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/run_points.sass
+-rw-rw-rw-   0        0        0      620 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/square.py
+-rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/square.sass
+-rw-rw-rw-   0        0        0      828 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/squares.py
+-rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/components/preloaders/squares.sass
+-rw-rw-rw-   0        0        0    26327 2022-07-06 20:17:07.000000 phanterpwa-13.13.0/phanterpwa/configer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.561287 phanterpwa-13.13.0/phanterpwa/frontend/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/__init__.py
+-rw-rw-rw-   0        0        0    56787 2023-03-13 15:33:52.000000 phanterpwa-13.13.0/phanterpwa/frontend/application.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.691287 phanterpwa-13.13.0/phanterpwa/frontend/components/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/__init__.py
+-rw-rw-rw-   0        0        0    69794 2023-04-16 16:07:37.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/admin.py
+-rw-rw-rw-   0        0        0   172952 2023-04-14 17:18:15.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/auth_user.py
+-rw-rw-rw-   0        0        0    57394 2022-04-04 10:57:28.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/datetimepicker.py
+-rw-rw-rw-   0        0        0     3726 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/events.py
+-rw-rw-rw-   0        0        0    34075 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/gallery.py
+-rw-rw-rw-   0        0        0    55112 2021-12-06 00:44:42.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/left_bar.py
+-rw-rw-rw-   0        0        0     9100 2022-12-05 02:22:50.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/modal.py
+-rw-rw-rw-   0        0        0      791 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/pagination.py
+-rw-rw-rw-   0        0        0     4060 2021-11-21 02:57:14.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/snippets.py
+-rw-rw-rw-   0        0        0     3175 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/top_slide.py
+-rw-rw-rw-   0        0        0   231156 2023-04-14 17:13:15.000000 phanterpwa-13.13.0/phanterpwa/frontend/components/widgets.py
+-rw-rw-rw-   0        0        0     4042 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/decorators.py
+-rw-rw-rw-   0        0        0    31267 2021-08-01 05:39:42.000000 phanterpwa-13.13.0/phanterpwa/frontend/fmasks.py
+-rw-rw-rw-   0        0        0    42583 2023-04-13 14:03:07.000000 phanterpwa-13.13.0/phanterpwa/frontend/forms.py
+-rw-rw-rw-   0        0        0    33833 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/gallery.py
+-rw-rw-rw-   0        0        0    14753 2022-04-30 16:30:51.000000 phanterpwa-13.13.0/phanterpwa/frontend/gatehandler.py
+-rw-rw-rw-   0        0        0     9861 2022-06-16 23:20:19.000000 phanterpwa-13.13.0/phanterpwa/frontend/helpers.py
+-rw-rw-rw-   0        0        0     4593 2022-04-04 10:57:28.000000 phanterpwa-13.13.0/phanterpwa/frontend/i18n.py
+-rw-rw-rw-   0        0        0    41699 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/initializer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.702289 phanterpwa-13.13.0/phanterpwa/frontend/plugins/
+-rw-rw-rw-   0        0        0    27481 2022-11-26 15:07:06.000000 phanterpwa-13.13.0/phanterpwa/frontend/plugins/client.py
+-rw-rw-rw-   0        0        0     4927 2022-08-19 19:22:51.000000 phanterpwa-13.13.0/phanterpwa/frontend/preloaders.py
+-rw-rw-rw-   0        0        0     1798 2021-11-17 18:30:18.000000 phanterpwa-13.13.0/phanterpwa/frontend/progressbar.py
+-rw-rw-rw-   0        0        0     5467 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/frontend/selects.py
+-rw-rw-rw-   0        0        0    20154 2022-05-21 19:29:34.000000 phanterpwa-13.13.0/phanterpwa/frontend/server.py
+-rw-rw-rw-   0        0        0    10504 2021-11-30 01:36:21.000000 phanterpwa-13.13.0/phanterpwa/frontend/validations.py
+-rw-rw-rw-   0        0        0     4381 2022-04-29 11:22:51.000000 phanterpwa-13.13.0/phanterpwa/frontend/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.724285 phanterpwa-13.13.0/phanterpwa/gallery/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/gallery/__init__.py
+-rw-rw-rw-   0        0        0     7220 2022-02-21 15:44:58.000000 phanterpwa-13.13.0/phanterpwa/gallery/cutter.py
+-rw-rw-rw-   0        0        0     8578 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/gallery/integrationDAL.py
+-rw-rw-rw-   0        0        0    12138 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.734285 phanterpwa-13.13.0/phanterpwa/i18n/
+-rw-rw-rw-   0        0        0     8670 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.774286 phanterpwa-13.13.0/phanterpwa/interface/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.735287 phanterpwa-13.13.0/phanterpwa/interface/Admin/
+-rw-rw-rw-   0        0        0     1066 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.173408 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.849285 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.877287 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/controllers/
+-rw-rw-rw-   0        0        0      206 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/controllers/__init__.py
+-rw-rw-rw-   0        0        0    29445 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/controllers/developer.py
+-rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/controllers/welcome.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.878286 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/
+-rw-rw-rw-   0        0        0      682 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table
+-rw-rw-rw-   0        0        0      487 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_group.table
+-rw-rw-rw-   0        0        0      536 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table
+-rw-rw-rw-   0        0        0     2572 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table
+-rw-rw-rw-   0        0        0      793 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table
+-rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table
+-rw-rw-rw-   0        0        0      842 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table
+-rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table
+-rw-rw-rw-   0        0        0      597 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table
+-rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table
+-rw-rw-rw-   0        0        0      590 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table
+-rw-rw-rw-   0        0        0      714 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table
+-rw-rw-rw-   0        0        0      733 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table
+-rw-rw-rw-   0        0        0       35 2022-04-26 23:50:37.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/readme.txt
+-rw-rw-rw-   0        0        0     4285 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/sql.log
+-rw-rw-rw-   0        0        0    81920 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite
+-rw-rw-rw-   0        0        0     6349 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/handlers.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.894287 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.910287 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/admin/
+-rw-rw-rw-   0        0        0      807 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json
+-rw-rw-rw-   0        0        0     1541 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.924286 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/captcha/
+-rw-rw-rw-   0        0        0      497 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/captcha/entries.json
+-rw-rw-rw-   0        0        0     1124 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.940286 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/email/
+-rw-rw-rw-   0        0        0     1577 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json
+-rw-rw-rw-   0        0        0     3117 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json
+-rw-rw-rw-   0        0        0     3108 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/entries.json
+-rw-rw-rw-   0        0        0     6164 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.887286 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/models/
+-rw-rw-rw-   0        0        0      996 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.209402 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/statics/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.946288 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/statics/images/
+-rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/statics/images/user.png
+-rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.951286 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/uploads/
+-rw-rw-rw-   0        0        0       28 2022-04-27 00:31:13.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/uploads/readme.txt
+-rw-rw-rw-   0        0        0     2812 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/core.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.889287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.902290 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/__init__.py
+-rw-rw-rw-   0        0        0     1121 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/handlers.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.967287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/languages/
+-rw-rw-rw-   0        0        0     1266 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json
+-rw-rw-rw-   0        0        0     2403 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.211409 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.974286 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/
+-rw-rw-rw-   0        0        0     8390 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.008289 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/
+-rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass
+-rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/logo.sass
+-rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass
+-rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.030308 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/
+-rw-rw-rw-   0        0        0     1177 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass
+-rw-rw-rw-   0        0        0      121 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/developer.sass
+-rw-rw-rw-   0        0        0      564 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.915285 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.038307 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/__init__.py
+-rw-rw-rw-   0        0        0      785 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py
+-rw-rw-rw-   0        0        0      675 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py
+-rw-rw-rw-   0        0        0      747 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py
+-rw-rw-rw-   0        0        0      963 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py
+-rw-rw-rw-   0        0        0    38183 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py
+-rw-rw-rw-   0        0        0     1272 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py
+-rw-rw-rw-   0        0        0     7459 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg
+-rw-rw-rw-   0        0        0      158 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/svg_logo.py
+-rw-rw-rw-   0        0        0     3267 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.015314 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/
+-rw-rw-rw-   0        0        0    38395 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py
+-rw-rw-rw-   0        0        0     1122 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py
+-rw-rw-rw-   0        0        0    20765 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.027287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/
+-rw-rw-rw-   0        0        0     1363 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.035297 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/
+-rw-rw-rw-   0        0        0      932 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.130286 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/__init__.py
+-rw-rw-rw-   0        0        0     2543 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py
+-rw-rw-rw-   0        0        0    12805 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py
+-rw-rw-rw-   0        0        0     4692 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py
+-rw-rw-rw-   0        0        0    19789 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.163287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/__init__.py
+-rw-rw-rw-   0        0        0    17986 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py
+-rw-rw-rw-   0        0        0     9456 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py
+-rw-rw-rw-   0        0        0    46491 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py
+-rw-rw-rw-   0        0        0    46731 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py
+-rw-rw-rw-   0        0        0     2600 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py
+-rw-rw-rw-   0        0        0    16739 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py
+-rw-rw-rw-   0        0        0     5783 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py
+-rw-rw-rw-   0        0        0     5528 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.172310 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/
+-rw-rw-rw-   0        0        0     1502 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.222407 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.066287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/
+-rw-rw-rw-   0        0        0    57333 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css
+-rw-rw-rw-   0        0        0     6138 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css
+-rw-rw-rw-   0        0        0   444223 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.128286 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/
+-rw-rw-rw-   0        0        0    11462 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png
+-rw-rw-rw-   0        0        0     7107 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    19743 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png
+-rw-rw-rw-   0        0        0    19618 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     6233 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      246 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/browserconfig.xml
+-rw-rw-rw-   0        0        0     1209 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1865 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico
+-rw-rw-rw-   0        0        0      268 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/manifest.json
+-rw-rw-rw-   0        0        0     5185 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png
+-rw-rw-rw-   0        0        0      426 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/site.webmanifest
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.303286 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/
+-rw-rw-rw-   0        0        0    46822 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot
+-rw-rw-rw-   0        0        0    57097 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg
+-rw-rw-rw-   0        0        0    46592 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf
+-rw-rw-rw-   0        0        0    30204 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff
+-rw-rw-rw-   0        0        0    25040 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2
+-rw-rw-rw-   0        0        0    12376 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2
+-rw-rw-rw-   0        0        0    16028 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2
+-rw-rw-rw-   0        0        0    21659 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot
+-rw-rw-rw-   0        0        0   127584 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0    61628 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff
+-rw-rw-rw-   0        0        0    48524 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2
+-rw-rw-rw-   0        0        0    18004 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2
+-rw-rw-rw-   0        0        0    36060 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2
+-rw-rw-rw-   0        0        0    49240 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2
+-rw-rw-rw-   0        0        0    17854 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot
+-rw-rw-rw-   0        0        0    48974 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg
+-rw-rw-rw-   0        0        0    36176 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf
+-rw-rw-rw-   0        0        0    20268 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff
+-rw-rw-rw-   0        0        0    15736 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.321287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/
+-rw-rw-rw-   0        0        0   104800 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg
+-rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png
+-rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.448298 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/
+-rw-rw-rw-   0        0        0    45781 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js
+-rw-rw-rw-   0        0        0    43028 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map
+-rw-rw-rw-   0        0        0      988 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js
+-rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js
+-rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map
+-rw-rw-rw-   0        0        0    11272 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.459287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/json/
+-rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json
+-rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.541288 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/lib/
+-rw-rw-rw-   0        0        0     8705 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css
+-rw-rw-rw-   0        0        0   397228 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.221408 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.589311 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/
+-rw-rw-rw-   0        0        0     6268 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html
+-rw-rw-rw-   0        0        0    14676 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js
+-rw-rw-rw-   0        0        0     2014 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.694287 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/
+-rw-rw-rw-   0        0        0   133034 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   132728 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    89824 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76548 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34390 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0    34092 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16800 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13600 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   194078 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   193792 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0    99004 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    76120 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.706315 phanterpwa-13.13.0/phanterpwa/interface/Admin/logs/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/logs/api.log
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/logs/app.log
+-rw-rw-rw-   0        0        0       23 2022-04-26 23:49:53.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/logs/readme.txt
+-rw-rw-rw-   0        0        0      286 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/production.py
+-rw-rw-rw-   0        0        0      145 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/run.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.894285 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/
+-rw-rw-rw-   0        0        0     9893 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass
+-rw-rw-rw-   0        0        0     1228 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_admin.json
+-rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_components.json
+-rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json
+-rw-rw-rw-   0        0        0      221 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/phanterpwa_modules_mtime.json
+-rw-rw-rw-   0        0        0        0 2022-04-26 23:56:37.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/readme.txt
+-rw-rw-rw-   0        0        0    11082 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_admin.json
+-rw-rw-rw-   0        0        0     8222 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_components.json
+-rw-rw-rw-   0        0        0     8119 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0     6140 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json
+-rw-rw-rw-   0        0        0     1369 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_admin.json
+-rw-rw-rw-   0        0        0      592 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_components.json
+-rw-rw-rw-   0        0        0     1075 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0     3682 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json
+-rw-rw-rw-   0        0        0      681 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/templates_mtime_admin.json
+-rw-rw-rw-   0        0        0      338 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/templates_mtime_components.json
+-rw-rw-rw-   0        0        0      474 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/templates_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0      190 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/templates_mtime_sindfa.json
+-rw-rw-rw-   0        0        0     2676 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json
+-rw-rw-rw-   0        0        0      810 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json
+-rw-rw-rw-   0        0        0     1342 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0     1127 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.901285 phanterpwa-13.13.0/phanterpwa/interface/Admin/trash/
+-rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.13.0/phanterpwa/interface/Admin/trash/readme.txt
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/__init__.py
+-rw-rw-rw-   0        0        0     7015 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/admin_tk.py
+-rw-rw-rw-   0        0        0    50861 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.911286 phanterpwa-13.13.0/phanterpwa/interface/grafics/
+-rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/grafics/icon.ico
+-rw-rw-rw-   0        0        0      634 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/grafics/on.jpg
+-rw-rw-rw-   0        0        0   140200 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/graphic.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.935287 phanterpwa-13.13.0/phanterpwa/interface/langs/
+-rw-rw-rw-   0        0        0     5309 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/langs/English.json
+-rw-rw-rw-   0        0        0     5339 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/langs/Portuguese.json
+-rw-rw-rw-   0        0        0     2800 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/interface/langs/entries.json
+-rw-rw-rw-   0        0        0     5741 2021-09-05 00:25:27.000000 phanterpwa-13.13.0/phanterpwa/mail.py
+-rw-rw-rw-   0        0        0    10764 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/reversexml.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.978287 phanterpwa-13.13.0/phanterpwa/samples/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/__init__.py
+-rw-rw-rw-   0        0        0      372 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/about_cli
+-rw-rw-rw-   0        0        0      269 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/about_graphic
+-rw-rw-rw-   0        0        0      533 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/art
+-rw-rw-rw-   0        0        0      408 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/art_cli
+-rw-rw-rw-   0        0        0     2183 2022-07-06 20:15:09.000000 phanterpwa-13.13.0/phanterpwa/samples/config.json
+-rw-rw-rw-   0        0        0     4996 2022-11-26 15:08:21.000000 phanterpwa-13.13.0/phanterpwa/samples/email.sass
+-rw-rw-rw-   0        0        0     6072 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/email_activation_code.py
+-rw-rw-rw-   0        0        0     5840 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/samples/email_password.py
+-rw-rw-rw-   0        0        0     9137 2021-09-05 04:01:49.000000 phanterpwa-13.13.0/phanterpwa/samples/email_two_factor_code.py
+-rw-rw-rw-   0        0        0     1879 2022-07-06 20:14:49.000000 phanterpwa-13.13.0/phanterpwa/samples/project_config_sample.py
+-rw-rw-rw-   0        0        0      236 2021-09-05 03:59:44.000000 phanterpwa-13.13.0/phanterpwa/samples/sms_activation_code.py
+-rw-rw-rw-   0        0        0      245 2021-09-04 16:15:07.000000 phanterpwa-13.13.0/phanterpwa/samples/sms_password.py
+-rw-rw-rw-   0        0        0      241 2021-09-04 16:33:02.000000 phanterpwa-13.13.0/phanterpwa/samples/sms_two_factor_code.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:46.989286 phanterpwa-13.13.0/phanterpwa/scaffolds/
+-rw-rw-rw-   0        0        0  2214300 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/scaffolds/__init__.py
+-rw-rw-rw-   0        0        0    12247 2022-09-23 00:15:14.000000 phanterpwa-13.13.0/phanterpwa/server.py
+-rw-rw-rw-   0        0        0     1313 2021-09-05 16:25:04.000000 phanterpwa-13.13.0/phanterpwa/sms.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.350283 phanterpwa-13.13.0/phanterpwa/tests/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.012297 phanterpwa-13.13.0/phanterpwa/tests/helpers_out/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/helpers_out/__init__.py
+-rw-rw-rw-   0        0        0      331 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/helpers_out/my_sass.sass
+-rw-rw-rw-   0        0        0      352 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/helpers_out/new_sass.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.046287 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/__init__.py
+-rw-rw-rw-   0        0        0      456 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/entries.json
+-rw-rw-rw-   0        0        0      854 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/es.json
+-rw-rw-rw-   0        0        0      852 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/fr.json
+-rw-rw-rw-   0        0        0      860 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/pt-BR.json
+-rw-rw-rw-   0        0        0      851 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/pt-PT.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.098286 phanterpwa-13.13.0/phanterpwa/tests/preloaders/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/__init__.py
+-rw-rw-rw-   0        0        0     9764 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_android.html
+-rw-rw-rw-   0        0        0     3489 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_discs.html
+-rw-rw-rw-   0        0        0     5956 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html
+-rw-rw-rw-   0        0        0     4451 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html
+-rw-rw-rw-   0        0        0     1752 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_square.html
+-rw-rw-rw-   0        0        0     4231 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_squares.html
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.158316 phanterpwa-13.13.0/phanterpwa/tests/static/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/static/__init__.py
+-rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/static/jquery.min.js
+-rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/static/jquery.min.map
+-rw-rw-rw-   0        0        0     2117 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.361286 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.167314 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/not_project/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/not_project/__init__.py
+-rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/not_project/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.174287 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project-invalid-name/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project-invalid-name/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project-invalid-name/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.178287 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project01/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project01/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project01/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.181287 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project02/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project02/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/project02/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.373287 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/without_configjson/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_cli_projects/without_configjson/__init__.py
+-rw-rw-rw-   0        0        0     4079 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_components_preloaders.py
+-rw-rw-rw-   0        0        0    12208 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.375285 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.184287 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/fake_project/
+-rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/fake_project/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.186287 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project-invalid-name/
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project-invalid-name/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.203287 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.228408 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backapps/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.212286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backapps/api/
+-rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.231408 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backend/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.222286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backend/api/
+-rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini
+-rw-rw-rw-   0        0        0     2618 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.233408 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontapps/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.229286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontapps/app01/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontapps/app01/app.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.236286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontapps/app02/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontapps/app02/app.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.235408 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontend/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.240286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontend/app01/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontend/app01/app.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.243286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontend/app02/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/frontend/app02/app.ini
+-rw-rw-rw-   0        0        0      189 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/project.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.246286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project02/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project02/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project02/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.263286 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.236406 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.270284 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/
+-rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini
+-rw-rw-rw-   0        0        0     2143 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.238408 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.274287 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/app.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.277287 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/app.ini
+-rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/project.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.288285 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:43.239407 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/backend/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.291285 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/
+-rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini
+-rw-rw-rw-   0        0        0     2640 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/config.json
+-rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/project.ini
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.304287 phanterpwa-13.13.0/phanterpwa/tests/test_folder/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_folder/cfg.json
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_folder/cfgij.json
+-rw-rw-rw-   0        0        0       23 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_folder/config.json
+-rw-rw-rw-   0        0        0    80202 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.313285 phanterpwa-13.13.0/phanterpwa/tests/test_helpers_languages/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_helpers_languages/__init__.py
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_helpers_languages/en-US.json
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_helpers_languages/entries.json
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_helpers_languages/glingon.json
+-rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/tests/test_helpers_languages/pt-BR.json
+-rw-rw-rw-   0        0        0     3729 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_i18n.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.336285 phanterpwa-13.13.0/phanterpwa/tests/test_i18n_languages/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_i18n_languages/__init__.py
+-rw-rw-rw-   0        0        0       65 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_i18n_languages/en-US.json
+-rw-rw-rw-   0        0        0       36 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_i18n_languages/entries.json
+-rw-rw-rw-   0        0        0       63 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/tests/test_i18n_languages/pt-BR.json
+-rw-rw-rw-   0        0        0       63 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_i18n_languages/pt-PT.json
+-rw-rw-rw-   0        0        0     4212 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_reversexml.py
+-rw-rw-rw-   0        0        0    11521 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.341287 phanterpwa-13.13.0/phanterpwa/tests/test_tools_humanize_seconds/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/test_tools_humanize_seconds/entries.json
+-rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.13.0/phanterpwa/tests/test_tools_humanize_seconds/pt-BR.json
+-rw-rw-rw-   0        0        0     1386 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:45.405288 phanterpwa-13.13.0/phanterpwa/third_parties/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/third_parties/__init__.py
+-rw-rw-rw-   0        0        0     5857 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/third_parties/xss.py
+-rw-rw-rw-   0        0        0    45683 2022-04-27 18:34:47.000000 phanterpwa-13.13.0/phanterpwa/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.344287 phanterpwa-13.13.0/phanterpwa/trash/
+-rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.13.0/phanterpwa/trash/readme.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.363286 phanterpwa-13.13.0/phanterpwa/usual_sass/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.559285 phanterpwa-13.13.0/phanterpwa/usual_sass/components/
+-rw-rw-rw-   0        0        0     1794 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/alert_top_activation.sass
+-rw-rw-rw-   0        0        0     1551 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/breascrumbs.sass
+-rw-rw-rw-   0        0        0     2741 2021-07-27 18:35:01.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/buttons.sass
+-rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/capcha_preload.sass
+-rw-rw-rw-   0        0        0     7323 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/captcha.sass
+-rw-rw-rw-   0        0        0     5213 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass
+-rw-rw-rw-   0        0        0      643 2022-11-25 21:37:56.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/card.sass
+-rw-rw-rw-   0        0        0    13548 2022-04-04 10:57:28.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/cmp_auth_user.sass
+-rw-rw-rw-   0        0        0     6615 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/datetimepicker.sass
+-rw-rw-rw-   0        0        0     1741 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/developer.sass
+-rw-rw-rw-   0        0        0     3154 2022-06-07 17:05:55.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/easy.sass
+-rw-rw-rw-   0        0        0     1067 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/flash.sass
+-rw-rw-rw-   0        0        0     2937 2022-04-27 17:07:49.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/forms.sass
+-rw-rw-rw-   0        0        0     1888 2022-05-17 18:44:18.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/messages.sass
+-rw-rw-rw-   0        0        0     3190 2022-04-04 10:57:28.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/modal.sass
+-rw-rw-rw-   0        0        0     1694 2021-09-05 18:33:48.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/modal_login.sass
+-rw-rw-rw-   0        0        0      649 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/phanterpwa_gallery.sass
+-rw-rw-rw-   0        0        0     4103 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass
+-rw-rw-rw-   0        0        0     1450 2021-08-13 03:26:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass
+-rw-rw-rw-   0        0        0     2959 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/progressbar.sass
+-rw-rw-rw-   0        0        0      660 2022-02-03 09:45:15.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/pseudomodal.sass
+-rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/run_points.sass
+-rw-rw-rw-   0        0        0     1536 2021-06-17 02:27:21.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/sections.sass
+-rw-rw-rw-   0        0        0      811 2021-05-25 20:28:47.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/snippet.sass
+-rw-rw-rw-   0        0        0    79319 2023-01-26 13:45:09.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/widgets.sass
+-rw-rw-rw-   0        0        0     4968 2021-06-15 20:39:00.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/components/xtable.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.580289 phanterpwa-13.13.0/phanterpwa/usual_sass/display/
+-rw-rw-rw-   0        0        0    42388 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/display/grid.sass
+-rw-rw-rw-   0        0        0     3962 2021-12-14 21:24:18.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/display/media_print.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.588285 phanterpwa-13.13.0/phanterpwa/usual_sass/events/
+-rw-rw-rw-   0        0        0      238 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/events/waves.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.597290 phanterpwa-13.13.0/phanterpwa/usual_sass/extends/
+-rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/extends/capcha_preload.sass
+-rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/extends/logo.sass
+-rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/extends/run_points.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.614287 phanterpwa-13.13.0/phanterpwa/usual_sass/gates/
+-rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/gates/componentes.sass
+-rw-rw-rw-   0        0        0      631 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/gates/main.sass
+-rw-rw-rw-   0        0        0     9456 2023-01-22 22:50:53.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/phanterpwa.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.622293 phanterpwa-13.13.0/phanterpwa/usual_sass/plugins/
+-rw-rw-rw-   0        0        0      153 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/plugins/codemirror.sass
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:47.650287 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/
+-rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/android.sass
+-rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/discs.sass
+-rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/explosion.sass
+-rw-rw-rw-   0        0        0      954 2022-08-19 19:22:51.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/indefined_text.sass
+-rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/run_points.sass
+-rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/square.sass
+-rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/squares.sass
+-rw-rw-rw-   0        0        0     8645 2022-04-27 17:07:49.000000 phanterpwa-13.13.0/phanterpwa/usual_sass/variables.sass
+-rw-rw-rw-   0        0        0   162695 2023-02-02 15:14:57.000000 phanterpwa-13.13.0/phanterpwa/xmlconstructor.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:44:44.044285 phanterpwa-13.13.0/phanterpwa.egg-info/
+-rw-rw-rw-   0        0        0     1712 2023-05-02 02:44:41.000000 phanterpwa-13.13.0/phanterpwa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    25133 2023-05-02 02:44:43.000000 phanterpwa-13.13.0/phanterpwa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-05-02 02:44:42.000000 phanterpwa-13.13.0/phanterpwa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-02 02:44:42.000000 phanterpwa-13.13.0/phanterpwa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-02 02:44:41.000000 phanterpwa-13.13.0/phanterpwa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      122 2023-05-02 02:44:42.000000 phanterpwa-13.13.0/phanterpwa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     5319 2023-05-02 02:44:42.000000 phanterpwa-13.13.0/phanterpwa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 02:44:47.654288 phanterpwa-13.13.0/setup.cfg
+-rw-rw-rw-   0        0        0     4419 2022-07-15 11:22:48.000000 phanterpwa-13.13.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `phanterpwa-13.12.8/MANIFEST.in` & `phanterpwa-13.13.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/PKG-INFO` & `phanterpwa-13.13.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,17 @@
 Metadata-Version: 2.1
 Name: phanterpwa
-Version: 13.12.8
+Version: 13.13.0
 Summary: Tools for the phanterpwadeveloper framework
 Home-page: https://github.com/PhanterJR/phanterpwa
 Author: PhanterJR
 Author-email: phanterjr@conexaodidata.com.br
 Maintainer: PhanterJR
 Maintainer-email: phanterjr@conexaodidata.com.br
 License: MIT
-Description: # Phanterpwa
-            Tools for the phanterpwadeveloper framework
-        
-        ## Dependencies installed on setup
-        
-            psutil
-            tornado
-            libsass
-            transcrypt
-            pillow
-            itsdangerous
-            pydal
-            passlib
-            requests-oauthlib
-        
-        ## Requeriments
-            Python 3.6+
-            Python 3.7 Recommended
-        
-        ## Browser Compatibility
-        #### The browser needs compatibility with:
-            HTML5
-            ES6 (Javascript6)
-        
-        ## Web Tecnologies
-            jQuery
-            Font Awesome
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -50,7 +22,36 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Phanterpwa
+    Tools for the phanterpwadeveloper framework
+
+## Dependencies installed on setup
+
+    psutil
+    tornado
+    libsass
+    transcrypt
+    pillow
+    itsdangerous
+    pydal
+    passlib
+    requests-oauthlib
+
+## Requeriments
+    Python 3.6+
+    Python 3.7 Recommended
+
+## Browser Compatibility
+#### The browser needs compatibility with:
+    HTML5
+    ES6 (Javascript6)
+
+## Web Tecnologies
+    jQuery
+    Font Awesome
```

### Comparing `phanterpwa-13.12.8/phanterpwa/__main__.py` & `phanterpwa-13.13.0/phanterpwa/__main__.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/dataforms.py` & `phanterpwa-13.13.0/phanterpwa/backend/dataforms.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/decorators.py` & `phanterpwa-13.13.0/phanterpwa/backend/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,19 +402,21 @@
                 token_content = t.loads(self.phanterpwa_url_token)
             except BadSignature:
                 token_content = None
             if token_content:
                 if "user_agent" in token_content:
                     if ignore_user_agent:
                         self.phanterpwa_url_token_checked = token_content
+                        q_user = self.DALDatabase(self.DALDatabase.auth_user.id == token_content.get("id_user")).select().first()
+                        self.phanterpwa_current_user = q_user
                     else:
                         if token_content['user_agent'] == self.phanterpwa_user_agent:
+                            q_user = self.DALDatabase(self.DALDatabase.auth_user.id == token_content.get("id_user")).select().first()
+                            self.phanterpwa_current_user = q_user
                             self.phanterpwa_url_token_checked = token_content
-
-
             if self.phanterpwa_url_token_checked:
                 return f(self, *args, **kargs)
             else:
                 msg = "The URL token is invalid!"
                 dict_response = {
                     'status': 'Forbidden',
                     'code': 403,
```

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/pydal/auth.py` & `phanterpwa-13.13.0/phanterpwa/backend/pydal/auth.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/pydal/cas.py` & `phanterpwa-13.13.0/phanterpwa/backend/pydal/cas.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/pydal/credentials.py` & `phanterpwa-13.13.0/phanterpwa/backend/pydal/credentials.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/pydal/extra_validations.py` & `phanterpwa-13.13.0/phanterpwa/backend/pydal/extra_validations.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/pydal/gallery.py` & `phanterpwa-13.13.0/phanterpwa/backend/pydal/gallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/pydal/internal_messages.py` & `phanterpwa-13.13.0/phanterpwa/backend/pydal/internal_messages.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/admin.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/admin.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/auth.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -3379,21 +3379,21 @@
         })
 
 
 class AuthActivityNoRelational():
     def __init__(self, DALDatabase):
         self.DALDatabase = DALDatabase
 
-    def get_rows_by_user_id(self, id_user):
+    def get_rows_by_user_id(self, id_user, limit=100):
         db = self.DALDatabase
         return db(
             db.auth_activity_no_relational.id_user == int(id_user)
         ).select(
             orderby=~db.auth_activity_no_relational.id,
-            limitby=(0, 100)
+            limitby=(0, limit)
         )
 
     def set_activity(self, id_user, request, activity, date_activity=None):
         db = self.DALDatabase
         if date_activity is None:
             date_activity = datetime.now()
         db.auth_activity_no_relational.insert(
@@ -3401,22 +3401,27 @@
             request=request,
             activity=activity,
             date_activity=date_activity
         )
         db.commit()
         self.clean(id_user)
 
+    def get_last_activity(self, id_user):
+        db = self.DALDatabase
+        row = db(db.auth_activity_no_relational.id_user == id_user).select().last()
+        return row
+
     def clean(self, id_user):
         db = self.DALDatabase
         exedent_records = db(
             db.auth_activity_no_relational.id_user == int(id_user)
         )._select(
             db.auth_activity_no_relational.id,
             orderby=~db.auth_activity_no_relational.id,
-            limitby=(100, 1000)
+            limitby=(2000, 3000)
         )
         db(db.auth_activity_no_relational.id.belongs(exedent_records)).delete()
         db.commit()
 
 
 class AuthUserAutoComplete(web.RequestHandler):
     """
```

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/cas.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/cas.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/credentials.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/credentials.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/errors.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/errors.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/i18n_server.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/i18n_server.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/internal_messages.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/internal_messages.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/oauth.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/oauth.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/websocket.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/websocket.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/request_handlers/welcome.py` & `phanterpwa-13.13.0/phanterpwa/backend/request_handlers/welcome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/backend/security.py` & `phanterpwa-13.13.0/phanterpwa/backend/security.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/captcha.py` & `phanterpwa-13.13.0/phanterpwa/captchasvg/captcha.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/captchadata.json` & `phanterpwa-13.13.0/phanterpwa/captchasvg/captchadata.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/sass/captcha.sass` & `phanterpwa-13.13.0/phanterpwa/captchasvg/sass/captcha.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/butterfly.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/butterfly.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/crab.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/crab.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/pig.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/pig.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/rabbit.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/rabbit.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/animal/rooster.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/animal/rooster.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/a.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/a.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/b.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/b.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/c.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/c.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/letter/d.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/letter/d.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/four.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/four.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/one.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/one.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/three.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/three.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/captchasvg/vectors/number/two.recs` & `phanterpwa-13.13.0/phanterpwa/captchasvg/vectors/number/two.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/compiler.py` & `phanterpwa-13.13.0/phanterpwa/compiler.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/inputs.py` & `phanterpwa-13.13.0/phanterpwa/components/inputs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/left_bar.py` & `phanterpwa-13.13.0/phanterpwa/components/left_bar.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/materialize.py` & `phanterpwa-13.13.0/phanterpwa/components/materialize.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/phanterpwagallery.py` & `phanterpwa-13.13.0/phanterpwa/components/phanterpwagallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/android.py` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/android.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/android.sass` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/android.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/discs.py` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/discs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/discs.sass` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/discs.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/explosion.py` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/explosion.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/explosion.sass` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/explosion.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/run_points.py` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/run_points.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/run_points.sass` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/square.py` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/square.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/square.sass` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/square.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/squares.py` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/squares.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/components/preloaders/squares.sass` & `phanterpwa-13.13.0/phanterpwa/components/preloaders/squares.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/configer.py` & `phanterpwa-13.13.0/phanterpwa/configer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/application.py` & `phanterpwa-13.13.0/phanterpwa/frontend/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             "twitter": I(_class="fab fa-twitter")
         }
 
         # jQuery(document).ajaxComplete(
         #     lambda event, xhr, options: self._after_ajax_complete(event, xhr, options)
         # )
         window.PhanterPWA = self
+        window.onhashchange = lambda: jQuery(".phanterpwa-component-pseudomodal-container").remove()
         test_bool = __pragma__("js", "{}", "'serviceWorker' in navigator")
         if test_bool:
             caches.js_keys().then(lambda names: self._clear_cache(names))
             navigator.serviceWorker.register(
                 '/sw.js', {'scope': '/'}
             ).then(
                 lambda reg: self._swregister(reg, "register")
@@ -782,15 +783,15 @@
             callback(target)
         window.PhanterPWA.I18N.DOMTranslate(target)
 
     @staticmethod
     def get_consolided_way():
         current_way = sessionStorage.getItem("current_way")
         if current_way is None or current_way is js_undefined or current_way is "lock":
-            current_way = "home"
+            current_way = self.default_way
         return current_way
 
     def get_current_way(self):
         current_way = self._get_way_from_url_hash()
         # current_way = sessionStorage.getItem("current_way")
         if current_way is None or current_way is js_undefined or current_way is "lock":
             current_way = "home"
```

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/admin.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,27 +545,31 @@
             }
         )
         self.modal_temporary_password.open()
         jQuery("#phanterpwa-widget-form-submit_button-yes_delete").off(
             "click.yes_delete"
         ).on(
             "click.yes_delete",
-            lambda: self._request_temporary_password()
+            lambda: self._request_temporary_password(email)
         )
         jQuery("#phanterpwa-widget-form-form_button-no_delete").off(
             "click.no_delete"
         ).on(
             "click.no_delete",
             lambda: self.modal_temporary_password.close()
         )
         forms.SignForm("#form-auth_user", after_sign=lambda: forms.ValidateForm("#form-auth_user"))
 
-    def _request_temporary_password(self):
+    def _request_temporary_password(self, email):
         form_temporary_password = jQuery("#form-auth_user")[0]
         form_temporary_password = __new__(FormData(form_temporary_password))
+        form_temporary_password.append(
+            "email",
+            email
+        )
         window.PhanterPWA.POST(
             "api",
             "admin",
             "request-password",
             form_data=form_temporary_password,
             onComplete=lambda data, ajax_status: self._after_request_temporary_password(data, ajax_status)
         )
```

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/auth_user.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/auth_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1664,14 +1664,27 @@
         )
         self.element_target.find("#phanterpwa-widget-form-form_button-activation_new_code").off(
             'click.modal_submit_activation_new_code'
         ).on(
             'click.modal_submit_activation_new_code',
             lambda: self.request_new_activation_code_to_send_to_email()
         )
+        jQuery(
+            "#form-activation"
+        ).off(
+            "keydown.form-activation"
+        ).on(
+            "keydown.form-activation",
+            self._on_press_key_enter
+        )
+
+    def _on_press_key_enter(self, event):
+        if event.keyCode == 13:
+            event.preventDefault()
+            self.submit()
 
     def _process_alert_content(self):
         email = window.PhanterPWA.get_auth_user().email
         if str(email).endswith(".mobile@phanterpwa.com"):
             html = CONCATENATE(
                 DIV(
                     I18N(
@@ -2045,22 +2058,23 @@
                 I(_class="fas fa-home"),
                 **{"tag": "a",
                     "_href": "#_phanterpwa:/home",
                     "position": "top"}
             )
         )
 
+
 class MessagesMonitor(application.Component):
     def __init__(self, target_selector, **parameters):
         time = __new__(Date())
         self.initime = time.getTime()
         self.target_selector = target_selector
         self.element_target = jQuery(self.target_selector)
         message_link = parameters.get('messages_link', window.PhanterPWA.XWAY("messages", "inbox"))
-        self.interval = parameters.get('interval', 30000)
+        self.interval = parameters.get('interval', 600000)
         html = DIV(
             DIV(
                 A(I(_class="fas fa-envelope"), DIV(_class="phanterpwa-component-messages-total_messages"), _href=message_link),
                 _class="link phanterpwa-component-messages-button"
             ),
             _id="phanterpwa-component-messages-container",
             _class="phanterpwa-component-messages-container"
@@ -2867,19 +2881,14 @@
                         window.PhanterPWA.I18N.load_storage(), {
                             "year": "numeric",
                             "month": "2-digit",
                             "day": "numeric"
                         }
                     )
                     activity = x.activity
-                    activity = activity.replace(" __", " <strong>").replace("__ ", "</strong> ")
-                    if activity.endswith("__"):
-                        activity = "".join([activity[0:-2], "</strong>"])
-                    if activity.startswith("__"):
-                        activity = "".join(["<strong>", activity[2:]])
                     MyTable.append(
                         TableData(
                             "data_activity_{0}".format(x.id),
                             date_created,
                             XML(activity),
                             drag_and_drop=False
                         )
@@ -3223,14 +3232,27 @@
             "#phanterpwa-widget-form-submit_button-confirmation-code"
         ).off(
             "click.confirmation-code_button_save"
         ).on(
             "click.confirmation-code_button_save",
             self.submit
         )
+        jQuery(
+            "#form-confirmation-code"
+        ).off(
+            "keydown.form-confirmation-code"
+        ).on(
+            "keydown.form-confirmation-code",
+            self._on_press_key_enter
+        )
+
+    def _on_press_key_enter(self, event):
+        if event.keyCode == 13:
+            event.preventDefault()
+            self.submit()
 
     def reload(self):
         self.start()
 
     def start(self):
         xml_content = CONCATENATE(
             DIV(
```

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/datetimepicker.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/datetimepicker.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/events.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/events.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/gallery.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/gallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/left_bar.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/left_bar.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/modal.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/modal.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/pagination.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/pagination.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/snippets.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/snippets.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/top_slide.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/top_slide.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/components/widgets.py` & `phanterpwa-13.13.0/phanterpwa/frontend/components/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -918,23 +918,24 @@
 
 
 class Autocomplete(Widget):
     def __init__(self, identifier, **parameters):
         self.identifier = identifier
         self._alias_value = ""
         self._value = parameters.get("value", "")
+        self._editable = parameters.get("editable", False)
         self._data_set(parameters.get("data_set", []))
         self._label = parameters.get("label", None)
         self._placeholder = parameters.get("placeholder", None)
         self._name = parameters.get("name", None)
-        self._editable = parameters.get("editable", False)
         self._icon = parameters.get("icon", None)
         self._message_error = parameters.get("message_error", None)
         self._can_empty = parameters.get("can_empty", False)
         self._ajax_url = parameters.get("ajax_data_set", False)
+        self._on_modal_open = parameters.get("on_menu_open", None)
         self._validator = parameters.get("validators", None)
         self._wear = parameters.get("wear", "material")
         self._form = parameters.get("form", None)
         self._icon_option = parameters.get("icon_option", I(_class="far fa-circle"))
         self._icon_option_selected = parameters.get("icon_option_selected", I(_class="far fa-dot-circle"))
         self._icon_plus = parameters.get("icon_plus", I(_class="fas fa-plus"))
         self._icon_confirm = parameters.get("icon_confirm", I(_class="fas fa-check"))
@@ -987,15 +988,15 @@
                 "_name": self._name,
                 "_tabindex": "0"
             }),
             label,
             DIV(
                 I(_class="fab fa-sistrix"),
                 _class="phanterpwa-widget-autocomplete-caret"
-            ),
+            ) if self.icon is None else "",
             xml_icon,
             DIV(
                 I(_class="fas fa-check"),
                 _class="phanterpwa-widget-check"
             ),
             DIV(
                 self.get_message_error(),
@@ -1050,14 +1051,17 @@
             for vdata in data.keys():
                 new_data.append([vdata, data[vdata]])
                 if self._value == vdata:
                     self._alias_value = data[vdata]
             self._data = new_data
             self._data_dict = data
 
+        if self._editable and str(self._value) not in self._data_dict.keys():
+            self._alias_value = self._value
+
     def set_new_data_set(self, data):
         self._data_set(data)
 
     def _create_xml_modal(self, value):
         table = TABLE(_class="phanterpwa-widget-autocomplete-options-wrapper")
         self._value = value
         self._first_value = ""
@@ -1173,14 +1177,16 @@
                 self._xml_modal,
                 on_close=lambda: self._after_modal_close(el),
                 width="100%",
                 z_index=self._z_index,
                 recalc_on_scroll=self._recalc_on_scroll
             )
             self.modal.start()
+            if callable(self._on_modal_open):
+                self._on_modal_open(self)
             self._binds_modal_content()
         else:
             if self.modal is not js_undefined:
                 self.modal.close()
 
     def _switch_focus(self, el):
         el = jQuery(el)
@@ -1193,16 +1199,14 @@
             if stat_modal != "enabled":
                 jQuery(".phanterpwa-widget-wrapper").removeClass("focus").removeClass("pre_focus")
                 p.addClass("focus")
         else:
             p.removeClass("focus")
         self._check_value(el)
 
-
-
     def _remove_focus(self, el):
         el = jQuery(el)
         p = el.parent()
         if el.js_is(":focus"):
             p.addClass("focus")
         else:
             p.removeClass("focus")
@@ -1345,27 +1349,28 @@
     #         setTimeout(lambda: self.open_modal(el), 30)
     #     # self._check_value(el)
 
     def _open_by_keyup(self, event, el):
         code = event.keyCode or event.which
         p = jQuery(el).parent()
         p.addClass("focus")
-        if self._ajax_url is not False:
-            formdata = __new__(FormData())
-            formdata.append(
-                "startswith",
-                self.value()
-            )
-            window.PhanterPWA.POST(
-                self._ajax_url,
-                form_data=formdata,
-                onComplete=lambda data, ajax_status: self._data_set_from_ajax(data, ajax_status, el)
-            )
-        else:
-            setTimeout(lambda: self.open_modal(el), 30)
+        if code not in [9, 38, 13]:
+            if self._ajax_url is not False:
+                formdata = __new__(FormData())
+                formdata.append(
+                    "startswith",
+                    self.value()
+                )
+                window.PhanterPWA.POST(
+                    self._ajax_url,
+                    form_data=formdata,
+                    onComplete=lambda data, ajax_status: self._data_set_from_ajax(data, ajax_status, el)
+                )
+            else:
+                setTimeout(lambda: self.open_modal(el), 30)
 
     def _data_set_from_ajax(self, data, ajax_status, el):
         if ajax_status == "success":
             json = data.responseJSON
             data = json.data_set
             if data is not js_undefined:
                 data = list(data)
@@ -1375,19 +1380,26 @@
     def _open_by_keydown(self, event, el):
         code = event.keyCode or event.which
         p = jQuery(el).parent()
         if code == 9:
             self._create_xml_modal(jQuery(el).val())
             if self._first_value == "":
                 if not self._editable:
-                    jQuery(el).val("")
+                    jQuery(el).val("").focus()
             else:
                 jQuery(el).val(self._first_value)
                 if self.modal is not js_undefined:
                     self.modal.close()
+        elif code == 13:
+            if self.modal is not js_undefined:
+                self.modal.close()
+        elif code == 38:
+            self._create_xml_modal(jQuery(el).val())
+            if self.modal is not js_undefined:
+                jQuery("#{0}".format(self.modal._identifier)).find(".phanterpwa-widget-autocomplete-li-option").first().focus()
 
     def set_on_click_new_button(self, value):
         if callable(value):
             self._on_click_new = value
         else:
             console.error("The 'on_click_new_butto' value must be callable.")
 
@@ -2055,16 +2067,16 @@
 class ListString(Widget):
     def __init__(self, identifier, **parameters):
         self._label = parameters.get("label", None)
         self._identifier = identifier
         self._placeholder = parameters.get("placeholder", None)
         self._editable = parameters.get("editable", True)
         self._name = parameters.get("name", None)
-        self._value = parameters.get("value", [])
         self._data_set(parameters.get("data_set", []))
+        self._value = parameters.get("value", [])
         self._fixed = parameters.get("fixed", [])
         self._icon = parameters.get("icon", None)
         self._message_error = parameters.get("message_error", None)
         self._can_empty = parameters.get("can_empty", False)
         self._validator = parameters.get("validators", None)
         self._wear = parameters.get("wear", "material")
         self._kind = parameters.get("kind", "text")
@@ -2226,14 +2238,31 @@
                                     "_data-value": str(x[0]),
                                     "_class": "phanterpwa-widget-list_string-value-content{0}".format(
                                         "" if x[1] not in self._fixed else " widget-liststring-fixed"),
                                     "_tabindex": "0"
                                 }
                             )
                         )
+                    elif x in self._data_dict.keys():
+                        self._input_value.append(x)
+                        self._dict_input_value[str(x)] = self._data_dict[x]
+                        new_value.append([str(x), self._data_dict[x]])
+                        xml.append(
+                            DIV(
+                                self._data_dict[x],
+                                DIV(I(_class="fas fa-times"),
+                                    _class="phanterpwa-widget-list_string-value-icon_close icon_button wave_on_click") if x not in self._fixed else "",
+                                **{
+                                    "_data-value": x,
+                                    "_class": "phanterpwa-widget-list_string-value-content{0}".format(
+                                        "" if x not in self._fixed else " widget-liststring-fixed"),
+                                    "_tabindex": "0"
+                                }
+                            )
+                        )
                     else:
                         self._input_value.append(x)
                         self._dict_input_value[str(x)] = x
                         new_value.append([str(x), x])
                         xml.append(
                             DIV(
                                 x,
@@ -2793,15 +2822,16 @@
                 **{
                     "_id": "phanterpwa-widget-textarea-textarea-{0}".format(identifier),
                     "_class": "phanterpwa-widget-textarea-textarea",
                     "_name": self._name,
                     "_placeholder": self._placeholder,
                     "_data-validators": data_validators,
                     "_data-form": self._form
-            }),
+                }
+            ),
             label,
             DIV(
                 I(_class="fas fa-check"),
                 _class="phanterpwa-widget-check"
             ),
             DIV(
                 self.get_message_error(),
@@ -2944,25 +2974,42 @@
 class Inert(Widget):
     def __init__(self, identifier, **parameters):
         self._label = parameters.get("label", None)
         self._name = parameters.get("name", None)
         self._value = parameters.get("value", "")
         self._wear = parameters.get("wear", "material")
         self._form = parameters.get("form", None)
+        self._kind = parameters.get("kind", "text")
         wrapper_attr = {
             "_class": "phanterpwa-widget-wrapper its_disabled phanterpwa-widget-wear-{0} {1}".format(
                 self._wear,
                 "phanterpwa-widget-inert-wrapper"
             )
         }
         parameters["_id"] = identifier
         if "_class" in parameters:
             parameters["_class"] = "{0}{1}".format(parameters["_class"], " phanterpwa-widget-inert")
         else:
             parameters['_class'] = "phanterpwa-widget-inert"
+        n_type = ["date", "datetime", "password", "hidden"]
+        if self._kind in n_type:
+            if self._kind == "datetime":
+                self._type = "text"
+                if self._format is None:
+                    self._format = "yyyy-MM-dd HH:ss:mm"
+                self._mask = masks.date_and_datetime_to_maks(self._format)
+            elif self._kind == "date":
+                self._type = "text"
+                if self._format is None:
+                    self._format = "yyyy-MM-dd"
+                self._mask = masks.date_and_datetime_to_maks(self._format)
+            elif self._kind == "password":
+                self._type = "password"
+            elif self._kind == "hidden":
+                parameters["_class"] = "{0}{1}".format(parameters["_class"], " e-display_hidden")
         label = ""
         if self._label is not None:
             wrapper_attr["_class"] = "{0}{1}".format(wrapper_attr["_class"], " has_label")
             label = LABEL(self._label, _for="phanterpwa-widget-inert-inert-{0}".format(identifier))
         if self._value is not "":
             wrapper_attr["_class"] = "{0}{1}".format(wrapper_attr["_class"], " has_value")
 
@@ -3244,14 +3291,15 @@
     def start(self):
         self._binds()
 
 
 class MenuBox(Widget):
     def __init__(self, identifier, button, *options, **parameters):
         class_button = ""
+        self.menu_option_has_icon = False
         if button is js_undefined or button is None:
             self._button = I(_class="fas fa-ellipsis-v")
             class_button = " icon_button"
         else:
             if isinstance(button, helpers.XmlConstructor) and button.tag.upper() == "I":
                 class_button = " icon_button"
             self._button = button
@@ -3277,14 +3325,16 @@
             parameters["_class"] = "{0}{1}".format(parameters["_class"], " phanterpwa-widget-menubox")
         else:
             parameters['_class'] = "phanterpwa-widget-menubox"
         Widget.__init__(self, identifier, html, **parameters)
 
     def add_option(self, option):
         if isinstance(option, MenuOption):
+            if option.has_icon:
+                self.menu_option_has_icon = True
             self._xml_menu.append(option)
         elif isinstance(option, helpers.XmlConstructor) and option.tag.upper() == "HR":
             self._xml_menu.append(option)
         else:
             self._xml_menu.append(DIV(option, _class="phanterpwa-widget-menubox-option wave_on_click"))
 
     def _on_click(self, el):
@@ -3303,14 +3353,17 @@
             vertical=True,
             width=self._width,
             z_index=self._z_index,
             recalc_on_scroll=self._recalc_on_scroll,
             on_open=self._onopen
         )
         self.modal.start()
+        if self.menu_option_has_icon:
+            jQuery("#phanterpwa-widget-menubox-options-content-{0}".format(
+                self.identifier)).addClass("menu_option_has_icon")
         if self._close_after_click_in is True:
             jQuery("#phanterpwa-widget-menubox-options-content-{0}".format(
                 self.identifier)).find(".phanterpwa-widget-menubox-option").off(
                 "click.close_pseudo_modal"
             ).on(
                 "click.close_pseudo_modal",
                 lambda: self.modal.close()
@@ -3350,24 +3403,39 @@
 
     def start(self):
         target = jQuery(self.target_selector)
         target.off("click.open_menu_phanterpwa").on(
             "click.open_menu_phanterpwa",
             lambda: self._on_click(this)
         )
+
         if callable(self._onreload):
             self._onreload(target)
 
 
 class MenuOption(helpers.XmlConstructor):
     def __init__(self, *content, **attributes):
+        self.has_icon = False
         if "_class" in attributes:
             attributes['_class'] = "phanterpwa-widget-menubox-option {0}".format(attributes['_class'])
         else:
             attributes['_class'] = "phanterpwa-widget-menubox-option"
+        icon = attributes.get("icon")
+        if icon is None:
+            icon = ""
+        else:
+            self.has_icon = True
+            attributes['_class'] = "{0} {1}".format(attributes['_class'], "has_icon")
+        content = [
+            SPAN(
+                DIV(icon, _class="phanterpwa-widget-menubox-option-icon-content"),
+                _class="phanterpwa-widget-menubox-option-icon-wrapper"
+            ),
+            SPAN(*content, _class="phanterpwa-widget-menubox-option-content")
+        ]
         tag = "div"
         if "_href" in attributes:
             tag = "a"
         helpers.XmlConstructor.__init__(self, tag, False, *content, **attributes)
 
 
 class PseudoModal():
```

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/decorators.py` & `phanterpwa-13.13.0/phanterpwa/frontend/decorators.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/fmasks.py` & `phanterpwa-13.13.0/phanterpwa/frontend/fmasks.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/forms.py` & `phanterpwa-13.13.0/phanterpwa/frontend/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,16 @@
         self._cutter = json_widget.get("cutter", False)
         self._url = json_widget.get("url", None)
         self._ajax_data_set = json_widget.get("ajax_data_set", False)
         self._nocache = json_widget.get("no-cache", False)
         self._width = json_widget.get("width", 190)
         self._height = json_widget.get("height", 200)
         self._disabled = json_widget.get("disabled", None)
+        self._on_change = json_widget.get("on_change", None)
+        self._wear = json_widget.get("wear", None)
         if "_id" not in json_widget:
             json_widget["_id"] = "phanterpwa-widget-wrapper-{0}-{1}".format(self.table_name, self.input_name)
         if "type" not in json_widget:
             json_widget["type"] = "string"
         self._widget_type = json_widget["type"]
         if "_class" in json_widget:
             json_widget["_class"] = "{0}{1}".format(
@@ -437,15 +439,26 @@
             elif self._widget_type == "boolean":
                 w = widgets.CheckBox(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._value is True,
                     disabled=True,
-                    form=self.table_name
+                    form=self.table_name,
+                )
+            elif self._widget_type == "hidden":
+                w = widgets.Inert(
+                    "{0}-{1}".format(self.table_name, self.input_name),
+                    label=self.json_widget['label'],
+                    name=self.input_name,
+                    value=dvalue,
+                    wear="shadows",
+                    _class="data_view",
+                    kind="hidden",
+                    form=self.table_name,
                 )
 
             elif self._widget_type == "image":
 
                 w = widgets.Image(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
@@ -480,14 +493,15 @@
                         dvalue = validations.format_iso_date_datetime(dvalue, dformat, self._widget_type)
 
                 w = widgets.Input(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=dvalue,
+                    wear=self._wear,
                     format=dformat,
                     kind=self._widget_type,
                     mask=dformat,
                     form=self.table_name,
                     icon=I(_class="fas fa-calendar-alt"),
                     validators=self.validators
                 )
@@ -496,96 +510,105 @@
                 w = widgets.Select(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     editable=self._editable,
                     can_empty=self._can_empty,
                     value=self._value,
+                    wear=self._wear,
                     data_set=self.json_widget['data_set'],
                     form=self.table_name,
                     validators=self.validators
                 )
 
             elif self._widget_type == "autocomplete":
                 w = widgets.Autocomplete(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     editable=self._editable,
                     can_empty=self._can_empty,
                     ajax_data_set=self._ajax_data_set,
                     value=self._value,
+                    wear=self._wear,
                     data_set=self.json_widget['data_set'],
                     form=self.table_name,
                     validators=self.validators
                 )
 
             elif self._widget_type == "list_string":
                 ds = self.json_widget.get('data_set', [])
                 w = widgets.ListString(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     #editable=self._editable,
                     #can_empty=self._can_empty,
                     value=self._value,
+                    wear=self._wear,
                     data_set=ds,
                     form=self.table_name,
                     #validators=self.validators
                 )
             
             elif self._widget_type == "text":
                 w = widgets.Textarea(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     editable=self._editable,
                     can_empty=self._can_empty,
                     value=self._value,
+                    wear=self._wear,
                     mask=self._mask,
                     form=self.table_name,
                     validators=self.validators
                 )
 
             elif self._widget_type == "id":
                 w = widgets.Inert(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._value,
+                    wear=self._wear,
                     form=self.table_name,
                 )
 
             elif self._widget_type == "boolean":
                 w = widgets.CheckBox(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._value is True,
-                    form=self.table_name
+                    form=self.table_name,
+                    wear=self._wear,
+                    on_change=self._on_change
                 )
 
             elif self._widget_type == "password":
                 w = widgets.Input(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._value,
+                    wear=self._wear,
                     form=self.table_name,
                     validators=self.validators,
                     kind="password",
                     icon=self._icon
                 )
 
             elif self._widget_type == "hidden":
                 w = widgets.Input(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._value,
+                    wear=self._wear,
                     editable=self._editable,
                     can_empty=self._can_empty,                
                     mask=self._mask,
                     form=self.table_name,
                     kind="hidden",
                     validators=self.validators
                 )
@@ -593,27 +616,29 @@
             elif self._widget_type == "image":
 
                 w = widgets.Image(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._url,
+                    wear=self._wear,
                     form=self.table_name,
                     cutter=self._cutter,
                     nocache=self._nocache,
                     width=self._width,
                     height=self._height
                 )
 
             else:
                 w = widgets.Input(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
                     value=self._value,
+                    wear=self._wear,
                     editable=self._editable,
                     can_empty=self._can_empty,
                     disabled=self._disabled,
                     mask=self._mask,
                     form=self.table_name,
                     validators=self.validators
                 )
```

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/gallery.py` & `phanterpwa-13.13.0/phanterpwa/frontend/gallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/gatehandler.py` & `phanterpwa-13.13.0/phanterpwa/frontend/gatehandler.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/helpers.py` & `phanterpwa-13.13.0/phanterpwa/frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/i18n.py` & `phanterpwa-13.13.0/phanterpwa/frontend/i18n.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/initializer.py` & `phanterpwa-13.13.0/phanterpwa/frontend/initializer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/plugins/client.py` & `phanterpwa-13.13.0/phanterpwa/frontend/plugins/client.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/preloaders.py` & `phanterpwa-13.13.0/phanterpwa/frontend/preloaders.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/progressbar.py` & `phanterpwa-13.13.0/phanterpwa/frontend/progressbar.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/selects.py` & `phanterpwa-13.13.0/phanterpwa/frontend/selects.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/server.py` & `phanterpwa-13.13.0/phanterpwa/frontend/server.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/validations.py` & `phanterpwa-13.13.0/phanterpwa/frontend/validations.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/frontend/websocket.py` & `phanterpwa-13.13.0/phanterpwa/frontend/websocket.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/gallery/cutter.py` & `phanterpwa-13.13.0/phanterpwa/gallery/cutter.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/gallery/integrationDAL.py` & `phanterpwa-13.13.0/phanterpwa/gallery/integrationDAL.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/helpers.py` & `phanterpwa-13.13.0/phanterpwa/helpers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/i18n/__init__.py` & `phanterpwa-13.13.0/phanterpwa/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/LICENSE` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/LICENSE`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/controllers/developer.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/controllers/developer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/sql.log` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/sql.log`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/handlers.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/handlers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/entries.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/models/__init__.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/statics/images/user.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/statics/images/user.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/core.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/core.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/handlers.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/handlers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_admin.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_components.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_admin.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_components.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_admin.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_components.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/templates_mtime_admin.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/templates_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json` & `phanterpwa-13.13.0/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/admin_tk.py` & `phanterpwa-13.13.0/phanterpwa/interface/admin_tk.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/cli.py` & `phanterpwa-13.13.0/phanterpwa/interface/cli.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/grafics/icon.ico` & `phanterpwa-13.13.0/phanterpwa/interface/grafics/icon.ico`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/grafics/on.jpg` & `phanterpwa-13.13.0/phanterpwa/interface/grafics/on.jpg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/graphic.py` & `phanterpwa-13.13.0/phanterpwa/interface/graphic.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/langs/English.json` & `phanterpwa-13.13.0/phanterpwa/interface/langs/English.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/langs/Portuguese.json` & `phanterpwa-13.13.0/phanterpwa/interface/langs/Portuguese.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/interface/langs/entries.json` & `phanterpwa-13.13.0/phanterpwa/interface/langs/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/mail.py` & `phanterpwa-13.13.0/phanterpwa/mail.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/reversexml.py` & `phanterpwa-13.13.0/phanterpwa/reversexml.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/art` & `phanterpwa-13.13.0/phanterpwa/samples/art`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/config.json` & `phanterpwa-13.13.0/phanterpwa/samples/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/email.sass` & `phanterpwa-13.13.0/phanterpwa/samples/email.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/email_activation_code.py` & `phanterpwa-13.13.0/phanterpwa/samples/email_activation_code.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/email_password.py` & `phanterpwa-13.13.0/phanterpwa/samples/email_password.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/email_two_factor_code.py` & `phanterpwa-13.13.0/phanterpwa/samples/email_two_factor_code.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/samples/project_config_sample.py` & `phanterpwa-13.13.0/phanterpwa/samples/project_config_sample.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa` & `phanterpwa-13.13.0/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/server.py` & `phanterpwa-13.13.0/phanterpwa/server.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/sms.py` & `phanterpwa-13.13.0/phanterpwa/sms.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/es.json` & `phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/es.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/fr.json` & `phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/fr.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/pt-BR.json` & `phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/path_of_languages/pt-PT.json` & `phanterpwa-13.13.0/phanterpwa/tests/path_of_languages/pt-PT.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_android.html` & `phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_android.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_discs.html` & `phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_discs.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html` & `phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html` & `phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_square.html` & `phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_square.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/preloaders/test_components_preloaders_squares.html` & `phanterpwa-13.13.0/phanterpwa/tests/preloaders/test_components_preloaders_squares.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/static/jquery.min.js` & `phanterpwa-13.13.0/phanterpwa/tests/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/static/jquery.min.map` & `phanterpwa-13.13.0/phanterpwa/tests/static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_cli.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_components_preloaders.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_components_preloaders.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project01/config.json` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project01/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_configer_path/project_without_ini/config.json` & `phanterpwa-13.13.0/phanterpwa/tests/test_configer_path/project_without_ini/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_helpers.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_i18n.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_reversexml.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_reversexml.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/test_tools.py` & `phanterpwa-13.13.0/phanterpwa/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tests/tests.py` & `phanterpwa-13.13.0/phanterpwa/tests/tests.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/third_parties/xss.py` & `phanterpwa-13.13.0/phanterpwa/third_parties/xss.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/tools.py` & `phanterpwa-13.13.0/phanterpwa/tools.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/alert_top_activation.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/alert_top_activation.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/breascrumbs.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/breascrumbs.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/buttons.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/buttons.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/capcha_preload.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/capcha_preload.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/captcha.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/captcha.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/card.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/card.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/cmp_auth_user.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/cmp_auth_user.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/datetimepicker.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/datetimepicker.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/developer.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/developer.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/easy.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/easy.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/flash.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/flash.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/forms.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/forms.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/messages.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/messages.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/modal.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/modal.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/modal_login.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/modal_login.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/phanterpwa_gallery.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/phanterpwa_gallery.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/progressbar.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/progressbar.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/pseudomodal.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/pseudomodal.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/run_points.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/sections.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/sections.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/snippet.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/snippet.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/widgets.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/widgets.sass`

 * *Files 0% similar despite different names*

```diff
@@ -360,16 +360,14 @@
                     transition: width 0.3s ease
                 .phanterpwa-widget-message_error
                     height: auto
                     transition: height 0.3s ease
         &.phanterpwa-widget-wear-shadows
             position: relative
             padding-top: 5px
-            &.has_label
-                padding: 22px 5px
             input, textarea
                 border-radius: 5px
                 line-height: 1.5rem
                 width: 100%
                 padding: 5px
                 background-color: $white
                 border: 1px solid $grey07
@@ -379,34 +377,43 @@
                 top: 0px
                 position: absolute
                 color: $grey07
                 font-size: 1rem
                 transition: color 0.3s ease
             .phanterpwa-widget-check
                 position: absolute
-                top: 32px
+                top: 17px
                 right: 13px
                 font-size: 0.7rem
                 &.has_value
                 label
                     color: $components
                     transition: color 0.3s ease
+            &.has_label
+                padding: 22px 5px
+                .phanterpwa-widget-check
+                    top: 32px
             &.focus
                 input, textarea
                     box-shadow: 0px 0px 5px $components
                     border: 1px solid $components
                     transition: box-shadow 0.3s ease, border, 0.3s ease
 
                 label
                     color: $components
                     transition: color 0.3s ease
             &.has_error
                 .phanterpwa-widget-message_error
                     height: auto
                     transition: height 0.3s ease
+            &.has_icon
+                padding-right: 50px
+                .phanterpwa-widget-icon-wrapper
+                    top: 20px
+
         &.phanterpwa-widget-wear-elegant
             position: relative
             padding-top: 5px
             &.has_label
                 padding: 22px 5px
             input, textarea
                 border-radius: 5px
@@ -838,17 +845,19 @@
                 top: 12px
                 right: 30px
                 font-size: 0.7rem
             &.has_icon
                 .phanterpwa-widget-autocomplete-caret
                     right: 53px
                 .phanterpwa-widget-check
-                    right: 70px
+                    right: 50px
                 .phanterpwa-widget-autocomplete-touchpad    
                     width: calc(100% - 40px)
+                .phanterpwa-widget-icon-wrapper
+                    cursor: pointer
 
             &.has_value
                 label
                     left: 5px
                     bottom: 39px
                     position: absolute
                     color: $components
@@ -2035,14 +2044,20 @@
                             position: absolute
                             top: 0
                             right: 5px
                             width: 35px
                             transition: color 0.5s ease
 
 .phanterpwa-widget-menubox-options-content
+    .phanterpwa-widget-menubox-option-no_icon
+        margin-right: 60px
+    .phanterpwa-widget-menubox-option-icon-content
+        width: 20px
+        padding-right: 10px
+
     hr
         margin: 0
         color: $material_level05
     .phanterpwa-widget-menubox-option
         min-width: 150px
         height: 40px
         line-height: 20px
@@ -2051,14 +2066,17 @@
         color: $components
         text-align: center
         margin: 0
         padding: 10px 20px
         cursor: pointer
         &:hover
             background-color: rgb(224, 224, 224)
+        .phanterpwa-widget-menubox-option-icon-content
+            display: none
+
     a.phanterpwa-widget-menubox-option
         display: block
         text-decoration: none
     ul
         margin: 0
         padding: 0
         >li
@@ -2067,14 +2085,22 @@
             margin: 0
             padding: 10px 20px
             &::marker
                 content: ""
             cursor: pointer
             &:hover
                 background-color: rgb(224, 224, 224)
+    &.menu_option_has_icon
+        .phanterpwa-widget-menubox-option
+            text-align: left
+            .phanterpwa-widget-menubox-option-icon-content
+                display: inline-block
+                width: 25px
+                padding-right: 10px
+
 .phanterpwa-widget
     .phanterpwa-widget-inert-wrapper
         &.phanterpwa-widget-wear-material
             hr
                 &.material-widgets-animation-offfocus
                     border-bottom-color: $warning
         &.phanterpwa-widget-wear-shadows
```

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/components/xtable.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/components/xtable.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/display/grid.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/display/grid.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/display/media_print.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/display/media_print.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/extends/capcha_preload.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/extends/capcha_preload.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/extends/run_points.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/extends/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/gates/componentes.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/gates/componentes.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/gates/main.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/gates/main.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/phanterpwa.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/phanterpwa.sass`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,21 @@
         color: $components
 
 .link
     cursor: pointer
     &:hover
         color: $attention
 
+a
+    &.link
+        text-decoration: none
+        color: unset
+        &:visited
+            color: unser
+
 .phanterpwa-title
     text-align: center
     padding: 10px 0px
     font-size: 1.5rem
     color: $components
 
 .phanterpwa-subtitle
```

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/android.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/android.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/discs.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/discs.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/explosion.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/explosion.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/indefined_text.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/indefined_text.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/run_points.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/square.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/square.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/preloaders/squares.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/preloaders/squares.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/usual_sass/variables.sass` & `phanterpwa-13.13.0/phanterpwa/usual_sass/variables.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/phanterpwa/xmlconstructor.py` & `phanterpwa-13.13.0/phanterpwa/xmlconstructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3951,14 +3951,21 @@
         elif self.void:
             xml = self._tag_begin_cmp(close_void)
         else:
             xml = "".join([self._tag_begin_cmp(close_void), self.tag_end])
         xml = "".join([self.before_xml, xml, self.after_xml])
         return xml
 
+    def __format__(self, spec=None):
+        if spec == "repr":
+            return self.introspect
+        elif spec == "hash":
+            return hash(self.xml())
+        return self.xml()
+
     def __hash__(self):
         return hash(self.xml())
 
     def __str__(self):
         return self.xml()
 
     def __repr__(self):
```

### Comparing `phanterpwa-13.12.8/phanterpwa.egg-info/PKG-INFO` & `phanterpwa-13.13.0/phanterpwa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,17 @@
 Metadata-Version: 2.1
 Name: phanterpwa
-Version: 13.12.8
+Version: 13.13.0
 Summary: Tools for the phanterpwadeveloper framework
 Home-page: https://github.com/PhanterJR/phanterpwa
 Author: PhanterJR
 Author-email: phanterjr@conexaodidata.com.br
 Maintainer: PhanterJR
 Maintainer-email: phanterjr@conexaodidata.com.br
 License: MIT
-Description: # Phanterpwa
-            Tools for the phanterpwadeveloper framework
-        
-        ## Dependencies installed on setup
-        
-            psutil
-            tornado
-            libsass
-            transcrypt
-            pillow
-            itsdangerous
-            pydal
-            passlib
-            requests-oauthlib
-        
-        ## Requeriments
-            Python 3.6+
-            Python 3.7 Recommended
-        
-        ## Browser Compatibility
-        #### The browser needs compatibility with:
-            HTML5
-            ES6 (Javascript6)
-        
-        ## Web Tecnologies
-            jQuery
-            Font Awesome
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -50,7 +22,36 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Phanterpwa
+    Tools for the phanterpwadeveloper framework
+
+## Dependencies installed on setup
+
+    psutil
+    tornado
+    libsass
+    transcrypt
+    pillow
+    itsdangerous
+    pydal
+    passlib
+    requests-oauthlib
+
+## Requeriments
+    Python 3.6+
+    Python 3.7 Recommended
+
+## Browser Compatibility
+#### The browser needs compatibility with:
+    HTML5
+    ES6 (Javascript6)
+
+## Web Tecnologies
+    jQuery
+    Font Awesome
```

### Comparing `phanterpwa-13.12.8/phanterpwa.egg-info/SOURCES.txt` & `phanterpwa-13.13.0/phanterpwa.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 phanterpwa/__init__.py
 phanterpwa/__main__.py
 phanterpwa/compiler.py
 phanterpwa/configer.py
```

### Comparing `phanterpwa-13.12.8/phanterpwa.egg-info/top_level.txt` & `phanterpwa-13.13.0/phanterpwa.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.12.8/setup.py` & `phanterpwa-13.13.0/setup.py`

 * *Files identical despite different names*

