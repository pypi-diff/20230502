# Comparing `tmp/Flask-OpenAPI3-UI-1.5.1.tar.gz` & `tmp/Flask-OpenAPI3-UI-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-OpenAPI3-UI-1.5.1.tar", last modified: Fri Mar  3 16:10:34 2023, max compression
+gzip compressed data, was "Flask-OpenAPI3-UI-1.6.0.tar", last modified: Tue May  2 11:42:25 2023, max compression
```

## Comparing `Flask-OpenAPI3-UI-1.5.1.tar` & `Flask-OpenAPI3-UI-1.6.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.148783 Flask-OpenAPI3-UI-1.5.1/
--rw-r--r--   0 root         (0) root         (0)     1083 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3644 2023-03-03 16:10:34.148783 Flask-OpenAPI3-UI-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1648 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1548 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-03 16:10:34.148783 Flask-OpenAPI3-UI-1.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.104782 Flask-OpenAPI3-UI-1.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.112782 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3644 2023-03-03 16:10:34.000000 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4857 2023-03-03 16:10:34.000000 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 16:10:34.000000 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-03-03 16:10:34.000000 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-03 16:10:34.000000 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-03 16:10:34.000000 Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.112782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/
--rw-r--r--   0 root         (0) root         (0)      530 2023-03-03 16:10:28.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35467 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/base.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/commands.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/constants.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/marshmallow_apispec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.108782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.116783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.120782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/
--rw-r--r--   0 root         (0) root         (0)    41666 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/print.css
--rw-r--r--   0 root         (0) root         (0)      773 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/reset.css
--rw-r--r--   0 root         (0) root         (0)    43644 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/screen.css
--rw-r--r--   0 root         (0) root         (0)     3488 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/style.css
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/typography.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.124782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/
--rw-r--r--   0 root         (0) root         (0)    42480 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/DroidSans-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)    41028 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/DroidSans.ttf
--rw-r--r--   0 root         (0) root         (0)    22922 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.eot
--rw-r--r--   0 root         (0) root         (0)    73575 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.svg
--rw-r--r--   0 root         (0) root         (0)    40513 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.ttf
--rw-r--r--   0 root         (0) root         (0)    25992 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff
--rw-r--r--   0 root         (0) root         (0)    11480 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff2
--rw-r--r--   0 root         (0) root         (0)    22008 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.eot
--rw-r--r--   0 root         (0) root         (0)    72148 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.svg
--rw-r--r--   0 root         (0) root         (0)    39069 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.ttf
--rw-r--r--   0 root         (0) root         (0)    24868 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff
--rw-r--r--   0 root         (0) root         (0)    11304 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.128782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/
--rw-r--r--   0 root         (0) root         (0)       69 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/collapse.gif
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/expand.gif
--rw-r--r--   0 root         (0) root         (0)     5115 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/explorer_icons.png
--rwxr-xr-x   0 root         (0) root         (0)      445 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/favicon-16x16.png
--rwxr-xr-x   0 root         (0) root         (0)     1141 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/favicon-32x32.png
--rwxr-xr-x   0 root         (0) root         (0)     5430 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      455 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/logo_small.png
--rw-r--r--   0 root         (0) root         (0)      631 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/pet_store_api.png
--rw-r--r--   0 root         (0) root         (0)     9257 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/throbber.gif
--rw-r--r--   0 root         (0) root         (0)      670 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/wordnik_api.png
--rw-r--r--   0 root         (0) root         (0)     4335 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.132783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/
--rw-r--r--   0 root         (0) root         (0)     2395 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ca.js
--rw-r--r--   0 root         (0) root         (0)     3470 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/el.js
--rw-r--r--   0 root         (0) root         (0)     2342 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/en.js
--rw-r--r--   0 root         (0) root         (0)     2464 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/es.js
--rw-r--r--   0 root         (0) root         (0)     2503 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/fr.js
--rw-r--r--   0 root         (0) root         (0)     3856 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/geo.js
--rw-r--r--   0 root         (0) root         (0)     2432 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/it.js
--rwxr-xr-x   0 root         (0) root         (0)     2721 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ja.js
--rw-r--r--   0 root         (0) root         (0)     2320 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ko-kr.js
--rw-r--r--   0 root         (0) root         (0)     2298 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/pl.js
--rw-r--r--   0 root         (0) root         (0)     2314 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/pt.js
--rw-r--r--   0 root         (0) root         (0)     3100 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ru.js
--rw-r--r--   0 root         (0) root         (0)     2286 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/tr.js
--rw-r--r--   0 root         (0) root         (0)     1421 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/translator.js
--rw-r--r--   0 root         (0) root         (0)     2203 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/zh-cn.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.136783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/
--rw-r--r--   0 root         (0) root         (0)    19371 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/backbone-min.js
--rw-r--r--   0 root         (0) root         (0)    22724 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/es5-shim.js
--rw-r--r--   0 root         (0) root         (0)    71504 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/handlebars-4.0.5.js
--rw-r--r--   0 root         (0) root         (0)    10962 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/highlight.9.1.0.pack.js
--rw-r--r--   0 root         (0) root         (0)      310 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/highlight.9.1.0.pack_extended.js
--rw-r--r--   0 root         (0) root         (0)    92032 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery-1.8.0.min.js
--rw-r--r--   0 root         (0) root         (0)     3518 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery.ba-bbq.min.js
--rw-r--r--   0 root         (0) root         (0)      365 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery.slideto.min.js
--rw-r--r--   0 root         (0) root         (0)      536 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery.wiggle.min.js
--rw-r--r--   0 root         (0) root         (0)    43510 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/js-yaml.min.js
--rw-r--r--   0 root         (0) root         (0)   129835 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jsoneditor.min.js
--rw-r--r--   0 root         (0) root         (0)    51894 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/lodash.min.js
--rw-r--r--   0 root         (0) root         (0)    15724 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/marked.js
--rw-r--r--   0 root         (0) root         (0)      349 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/object-assign-pollyfill.js
--rw-r--r--   0 root         (0) root         (0)   130418 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/sanitize-html.min.js
--rw-r--r--   0 root         (0) root         (0)     7061 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/swagger-oauth.js
--rw-r--r--   0 root         (0) root         (0)      479 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/o2c.html
--rw-r--r--   0 root         (0) root         (0)  2708212 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/swagger-ui.js
--rw-r--r--   0 root         (0) root         (0)   453854 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/swagger-ui.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.108782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.136783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/flask_openapi/
--rw-r--r--   0 root         (0) root         (0)     7396 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/flask_openapi/index.html
--rw-r--r--   0 root         (0) root         (0)     6253 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/flask_openapi/index_old.html
--rw-r--r--   0 root         (0) root         (0)      479 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/flask_openapi/o2c.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.108782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.148783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/
--rw-r--r--   0 root         (0) root         (0)      665 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/favicon-16x16.png
--rw-r--r--   0 root         (0) root         (0)      628 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/favicon-32x32.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.148783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/lib/
--rw-r--r--   0 root         (0) root         (0)    85578 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/lib/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)   129572 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/lib/jquery.min.map
--rw-r--r--   0 root         (0) root         (0)  1002172 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-bundle.js
--rw-r--r--   0 root         (0) root         (0)  4277142 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-bundle.js.map
--rw-r--r--   0 root         (0) root         (0)   310590 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js
--rw-r--r--   0 root         (0) root         (0)  1381697 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 root         (0) root         (0)   142690 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.css
--rw-r--r--   0 root         (0) root         (0)   280799 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.css.map
--rw-r--r--   0 root         (0) root         (0)   399813 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.js
--rw-r--r--   0 root         (0) root         (0)  1322743 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.108782 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 16:10:34.148783 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/
--rw-r--r--   0 root         (0) root         (0)      176 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/body_scripts.html
--rw-r--r--   0 root         (0) root         (0)      108 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/custom_head.html
--rw-r--r--   0 root         (0) root         (0)      402 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/footer.html
--rw-r--r--   0 root         (0) root         (0)      659 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/head.html
--rw-r--r--   0 root         (0) root         (0)     1182 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/index.html
--rw-r--r--   0 root         (0) root         (0)     2388 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/oauth2-redirect.html
--rw-r--r--   0 root         (0) root         (0)     2674 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/swagger.html
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/top.html
--rw-r--r--   0 root         (0) root         (0)    36834 2023-03-03 16:09:19.000000 Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/utils.py
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.813829 Flask-OpenAPI3-UI-1.6.0/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     1083 2023-02-07 09:53:28.000000 Flask-OpenAPI3-UI-1.6.0/LICENSE
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3644 2023-05-02 11:42:25.813678 Flask-OpenAPI3-UI-1.6.0/PKG-INFO
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     1648 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/README.md
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     1548 2023-05-02 11:39:12.000000 Flask-OpenAPI3-UI-1.6.0/pyproject.toml
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)       38 2023-05-02 11:42:25.813869 Flask-OpenAPI3-UI-1.6.0/setup.cfg
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.791908 Flask-OpenAPI3-UI-1.6.0/src/
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.793959 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3644 2023-05-02 11:42:25.000000 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/PKG-INFO
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     4857 2023-05-02 11:42:25.000000 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/SOURCES.txt
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)        1 2023-05-02 11:42:25.000000 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/dependency_links.txt
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)       82 2023-05-02 11:42:25.000000 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/entry_points.txt
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)       71 2023-05-02 11:42:25.000000 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/requires.txt
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)       14 2023-05-02 11:42:25.000000 Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/top_level.txt
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.794810 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      538 2023-05-02 11:42:20.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/__init__.py
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    35191 2023-05-02 11:39:12.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/base.py
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     1222 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/commands.py
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      699 2023-05-02 11:39:12.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/constants.py
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     4829 2023-05-02 11:39:12.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/marshmallow_apispec.py
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.792474 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.796517 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.797516 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    41666 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/print.css
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      773 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/reset.css
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    43644 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/screen.css
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3488 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/style.css
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/typography.css
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.799257 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    42480 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/DroidSans-Bold.ttf
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    41028 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/DroidSans.ttf
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    22922 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.eot
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    73575 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.svg
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    40513 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.ttf
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    25992 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    11480 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff2
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    22008 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.eot
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    72148 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.svg
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    39069 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.ttf
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    24868 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    11304 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff2
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.800556 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)       69 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/collapse.gif
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)       73 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/expand.gif
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     5115 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/explorer_icons.png
+-rwxr-xr-x   0 jthompson-lindley   (503) staff       (20)      445 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/favicon-16x16.png
+-rwxr-xr-x   0 jthompson-lindley   (503) staff       (20)     1141 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/favicon-32x32.png
+-rwxr-xr-x   0 jthompson-lindley   (503) staff       (20)     5430 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/favicon.ico
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      455 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/logo_small.png
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      631 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/pet_store_api.png
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     9257 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/throbber.gif
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      670 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/wordnik_api.png
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     4335 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/index.html
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.802537 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2395 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ca.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3470 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/el.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2342 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/en.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2464 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/es.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2503 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/fr.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3856 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/geo.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2432 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/it.js
+-rwxr-xr-x   0 jthompson-lindley   (503) staff       (20)     2721 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ja.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2320 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ko-kr.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2298 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/pl.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2314 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/pt.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3100 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ru.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2286 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/tr.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     1421 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/translator.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2203 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/zh-cn.js
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.805115 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    19371 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/backbone-min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    22724 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/es5-shim.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    71504 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/handlebars-4.0.5.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    10962 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/highlight.9.1.0.pack.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      310 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/highlight.9.1.0.pack_extended.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    92032 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery-1.8.0.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     3518 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery.ba-bbq.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      365 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery.slideto.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      536 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery.wiggle.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    43510 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/js-yaml.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   129835 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jsoneditor.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    51894 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/lodash.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    15724 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/marked.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      349 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/object-assign-pollyfill.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   130418 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/sanitize-html.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     7061 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/swagger-oauth.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      479 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/o2c.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)  2708212 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/swagger-ui.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   453854 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/swagger-ui.min.js
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.792524 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.805533 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/flask_openapi/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     7396 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/flask_openapi/index.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     6253 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/flask_openapi/index_old.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      479 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/flask_openapi/o2c.html
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.792790 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.811273 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      665 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/favicon-16x16.png
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      628 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/favicon-32x32.png
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.812227 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/lib/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    85578 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/lib/jquery.min.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   129572 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/lib/jquery.min.map
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)  1002172 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-bundle.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)  4277142 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-bundle.js.map
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   310590 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)  1381697 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   142690 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.css
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   280799 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.css.map
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)   399813 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.js
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)  1322743 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.js.map
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.792848 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/
+drwxr-xr-x   0 jthompson-lindley   (503) staff       (20)        0 2023-05-02 11:42:25.813461 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      176 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/body_scripts.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      108 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/custom_head.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      402 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/footer.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      659 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/head.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     1182 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/index.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2388 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/oauth2-redirect.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)     2674 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/swagger.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)      168 2023-05-02 11:39:10.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/top.html
+-rw-r--r--   0 jthompson-lindley   (503) staff       (20)    36693 2023-05-02 11:39:12.000000 Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/utils.py
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/LICENSE` & `Flask-OpenAPI3-UI-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/PKG-INFO` & `Flask-OpenAPI3-UI-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-OpenAPI3-UI
-Version: 1.5.1
+Version: 1.6.0
 Summary: Next generation OpenAPI v3 Integration for Flask based APIs. Based on Flasgger.
 Author-email: Overflow Digital <team@overflow.digital>
 Maintainer-email: Katerina Tiddy <katerina@overflow.digital>, Joshua Thompson-Lindley <joshua@overflow.digital>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Overflow Digital
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/README.md` & `Flask-OpenAPI3-UI-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/pyproject.toml` & `Flask-OpenAPI3-UI-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6"
 ]
 keywords = ['flask', 'swagger', 'openapi', 'python', 'api', 'rest', 'openapi3']
 dependencies = [
-    "Flask>=2.1.2",
+    "Flask>=2.3.1",
     "PyYAML==6.0",
     "jsonschema==4.17.3",
     "mistune==2.0.4",
     "six==1.16.0"
 ]
 
 [project.urls]
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/PKG-INFO` & `Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-OpenAPI3-UI
-Version: 1.5.1
+Version: 1.6.0
 Summary: Next generation OpenAPI v3 Integration for Flask based APIs. Based on Flasgger.
 Author-email: Overflow Digital <team@overflow.digital>
 Maintainer-email: Katerina Tiddy <katerina@overflow.digital>, Joshua Thompson-Lindley <joshua@overflow.digital>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Overflow Digital
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/Flask_OpenAPI3_UI.egg-info/SOURCES.txt` & `Flask-OpenAPI3-UI-1.6.0/src/Flask_OpenAPI3_UI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/__init__.py` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # DO NOT CHANGE MANUALLY THIS IS CHANGED IN THE PIPELINES
-__version__ = '1.5.1'
+__version__ = "1.6.0"
 # Based on works of Bruno Rocha and the Flasgger open source community
 
 
 from jsonschema import ValidationError  # noqa
 
-from .base import (BR_SANITIZER, Flasgger, LazyJSONEncoder,  # noqa
-                   MK_SANITIZER, NO_SANITIZER, Swagger)
+from .base import (
+    BR_SANITIZER,
+    Flasgger,
+    LazyJSONEncoder,  # noqa
+    MK_SANITIZER,
+    NO_SANITIZER,
+    Swagger,
+)
 from .constants import OPTIONAL_FIELDS  # noqa
 from .marshmallow_apispec import APISpec, fields, Schema, SwaggerView  # noqa
 from .utils import apispec_to_template, LazyString, swag_from, validate  # noqa
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/base.py` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Markup,
     redirect,
     render_template,
     request,
     Response,
     url_for,
 )
-from flask.json import JSONEncoder
+from json import JSONEncoder
 from flask.views import MethodView
 from werkzeug.datastructures import Authorization
 
 try:
     from flask_restful.reqparse import RequestParser
 except ImportError:
     RequestParser = None
@@ -58,138 +58,141 @@
 
 
 def NO_SANITIZER(text):
     return text
 
 
 def BR_SANITIZER(text):
-    return text.replace('\n', '<br/>') if text else text
+    return text.replace("\n", "<br/>") if text else text
 
 
 def MK_SANITIZER(text):
     return Markup(markdown(text)) if text else text
 
 
 class APIDocsView(MethodView):
     """
     The /apidocs
     """
 
     def __init__(self, *args, **kwargs):
-        view_args = kwargs.pop('view_args', {})
-        self.config = view_args.get('config')
+        view_args = kwargs.pop("view_args", {})
+        self.config = view_args.get("config")
         super(APIDocsView, self).__init__(*args, **kwargs)
 
     def get(self):
         """
         The data under /apidocs
         json or Swagger UI
         """
 
-        do_auth: bool = self.config.get('pageProtection', False)
+        do_auth: bool = self.config.get("pageProtection", False)
         is_auth: bool = True
 
         if do_auth:
             request_auth: Optional[Authorization] = request.authorization
-            username: str = self.config.get('pageUsername', '')
-            password: str = self.config.get('pagePassword', '')
-            is_auth = (request_auth and request_auth.type == 'basic' and request_auth.username == username and request_auth.password == password)  # noqa
+            username: str = self.config.get("pageUsername", "")
+            password: str = self.config.get("pagePassword", "")
+            is_auth = (
+                request_auth
+                and request_auth.type == "basic"
+                and request_auth.username == username
+                and request_auth.password == password
+            )  # noqa
 
         if is_auth:
-            base_endpoint = self.config.get('endpoint', 'flask_openapi')
+            base_endpoint = self.config.get("endpoint", "flask_openapi")
             specs = [
                 {
-                    "url": url_for(".".join((base_endpoint, spec['endpoint']))),
-                    "title": spec.get('title', 'API Spec 1'),
-                    "name": spec.get('name', None),
-                    "version": spec.get("version", '0.0.1'),
-                    "endpoint": spec.get('endpoint')
+                    "url": url_for(".".join((base_endpoint, spec["endpoint"]))),
+                    "title": spec.get("title", "API Spec 1"),
+                    "name": spec.get("name", None),
+                    "version": spec.get("version", "0.0.1"),
+                    "endpoint": spec.get("endpoint"),
                 }
-                for spec in self.config.get('specs', [])
+                for spec in self.config.get("specs", [])
             ]
             urls = [
-                {
-                    "name": spec["name"],
-                    "url": spec["url"]
-                }
-                for spec in specs if spec["name"]
+                {"name": spec["name"], "url": spec["url"]}
+                for spec in specs
+                if spec["name"]
             ]
             data = {
                 "specs": specs,
                 "urls": urls,
-                "title": self.config.get('title', 'API Docs')
+                "title": self.config.get("title", "API Docs"),
             }
-            if request.args.get('json'):
+            if request.args.get("json"):
                 # calling with ?json returns specs
                 return jsonify(data)
             else:  # pragma: no cover
-                data['flasgger_config'] = self.config
-                data['json'] = json
-                data['flasgger_version'] = __version__
-                data['favicon'] = self.config.get(
-                    'favicon',
-                    url_for('flask_openapi.static',
-                            filename='favicon-32x32.png')
-                )
-                data['swagger_ui_bundle_js'] = self.config.get(
-                    'swagger_ui_bundle_js',
-                    url_for('flask_openapi.static',
-                            filename='swagger-ui-bundle.js')
+                data["flasgger_config"] = self.config
+                data["json"] = json
+                data["flasgger_version"] = __version__
+                data["favicon"] = self.config.get(
+                    "favicon",
+                    url_for("flask_openapi.static", filename="favicon-32x32.png"),
                 )
-                data['swagger_ui_standalone_preset_js'] = self.config.get(
-                    'swagger_ui_standalone_preset_js',
-                    url_for('flask_openapi.static',
-                            filename='swagger-ui-standalone-preset.js')
+                data["swagger_ui_bundle_js"] = self.config.get(
+                    "swagger_ui_bundle_js",
+                    url_for("flask_openapi.static", filename="swagger-ui-bundle.js"),
                 )
-                data['jquery_js'] = self.config.get(
-                    'jquery_js',
-                    url_for('flask_openapi.static',
-                            filename='lib/jquery.min.js')
+                data["swagger_ui_standalone_preset_js"] = self.config.get(
+                    "swagger_ui_standalone_preset_js",
+                    url_for(
+                        "flask_openapi.static",
+                        filename="swagger-ui-standalone-preset.js",
+                    ),
                 )
-                data['swagger_ui_css'] = self.config.get(
-                    'swagger_ui_css',
-                    url_for('flask_openapi.static', filename='swagger-ui.css')
+                data["jquery_js"] = self.config.get(
+                    "jquery_js",
+                    url_for("flask_openapi.static", filename="lib/jquery.min.js"),
                 )
-                return render_template(
-                    'flask_openapi/index.html',
-                    **data
+                data["swagger_ui_css"] = self.config.get(
+                    "swagger_ui_css",
+                    url_for("flask_openapi.static", filename="swagger-ui.css"),
                 )
+                return render_template("flask_openapi/index.html", **data)
         else:
-            return ('Unauthorized', 401, {'WWW-Authenticate': 'Basic realm="OpenAPI Documentation"'})
+            return (
+                "Unauthorized",
+                401,
+                {"WWW-Authenticate": 'Basic realm="OpenAPI Documentation"'},
+            )
 
 
 class OAuthRedirect(MethodView):
     """
     The OAuth2 redirect HTML for Swagger UI standard/implicit flow
     """
 
     def get(self):
         return render_template(
-            ['flask_openapi/oauth2-redirect.html', 'flask_openapi/o2c.html'],
+            ["flask_openapi/oauth2-redirect.html", "flask_openapi/o2c.html"],
         )
 
 
 class APISpecsView(MethodView):
     """
     The /apispec_1.json and other specs
     """
 
     def __init__(self, *args, **kwargs):
-        self.loader = kwargs.pop('loader')
+        self.loader = kwargs.pop("loader")
         super(APISpecsView, self).__init__(*args, **kwargs)
 
     def get(self):
         """
         The Swagger view get method outputs to /apispecs_1.json
         """
         try:
             return jsonify(self.loader())
         except Exception:
             specs = json.dumps(self.loader())
-            return Response(specs, mimetype='application/json')
+            return Response(specs, mimetype="application/json")
 
 
 class SwaggerDefinition(object):
     """
     Class based definition
     """
 
@@ -197,55 +200,66 @@
         self.name = name
         self.obj = obj
         self.tags = tags or []
 
 
 class Swagger(object):
 
-    DEFAULT_ENDPOINT = 'apispec_1'
+    DEFAULT_ENDPOINT = "apispec_1"
     DEFAULT_CONFIG = {
-        "headers": [
-        ],
+        "headers": [],
         "specs": [
             {
                 "endpoint": DEFAULT_ENDPOINT,
-                "route": '/{}.json'.format(DEFAULT_ENDPOINT),
+                "route": "/{}.json".format(DEFAULT_ENDPOINT),
                 "rule_filter": lambda rule: True,  # all in
                 "model_filter": lambda tag: True,  # all in
             }
         ],
         "static_url_path": "/flask_openapi_static",
         # "static_folder": "static",  # must be set by user
         "swagger_ui": True,
-        "specs_route": "/apidocs/"
+        "specs_route": "/apidocs/",
     }
 
-    SCHEMA_TYPES = {'string': str, 'integer': int, 'number': float,
-                    'boolean': bool}
-    SCHEMA_LOCATIONS = {'query': 'args', 'header': 'headers',
-                        'formData': 'form', 'body': 'json', 'path': 'path'}
+    SCHEMA_TYPES = {"string": str, "integer": int, "number": float, "boolean": bool}
+    SCHEMA_LOCATIONS = {
+        "query": "args",
+        "header": "headers",
+        "formData": "form",
+        "body": "json",
+        "path": "path",
+    }
 
     def _init_config(self, config, merge):
-        """ Initializes self.config. If merge is set to true, then
+        """Initializes self.config. If merge is set to true, then
         self.config will be set to with config + DEFAULT_CONFIG.
         """
         if config and merge:
             self.config = dict(self.DEFAULT_CONFIG.copy(), **config)
         elif config and not merge:
             self.config = config
         elif not config:
             self.config = self.DEFAULT_CONFIG.copy()
         else:  # The above branches must be exhaustive
             raise ValueError
 
     def __init__(
-            self, app=None, config=None, sanitizer=None, template=None,
-            template_file=None, decorators=None, validation_function=None,
-            validation_error_handler=None, parse=False, format_checker=None,
-            merge=False
+        self,
+        app=None,
+        config=None,
+        sanitizer=None,
+        template=None,
+        template_file=None,
+        decorators=None,
+        validation_function=None,
+        validation_error_handler=None,
+        parse=False,
+        format_checker=None,
+        merge=False,
     ):
         self._configured = False
         self.endpoints = []
         self.definition_models = []  # not in app, so track here
         self.sanitizer = sanitizer or BR_SANITIZER
 
         self._init_config(config, merge)
@@ -253,25 +267,27 @@
         self.template = template
         self.template_file = template_file
         self.decorators = decorators
         self.format_checker = format_checker or jsonschema.FormatChecker()
 
         def default_validation_function(data, schema):
             return jsonschema.validate(
-                data, schema, format_checker=self.format_checker,
+                data,
+                schema,
+                format_checker=self.format_checker,
             )
 
         def default_error_handler(e, _, __):
             return abort(400, e.message)
 
-        self.validation_function = validation_function\
-            or default_validation_function
+        self.validation_function = validation_function or default_validation_function
 
-        self.validation_error_handler = validation_error_handler\
-            or default_error_handler
+        self.validation_error_handler = (
+            validation_error_handler or default_error_handler
+        )
         self.apispecs = {}  # cached apispecs
         self.parse = parse
         if app:
             self.init_app(app)
 
     def init_app(self, app, decorators=None):
         """
@@ -287,45 +303,45 @@
         if self.template_file is not None:
             self.template = self.load_swagger_file(self.template_file)
         self.register_views(app)
         self.add_headers(app)
 
         if self.parse:
             if RequestParser is None:
-                raise RuntimeError('Please install flask_restful')
+                raise RuntimeError("Please install flask_restful")
             self.parsers = {}
             self.schemas = {}
             self.parse_request(app)
 
         self._configured = True
         app.swag = self
 
     def load_swagger_file(self, filename):
-        if not filename.startswith('/'):
-            filename = os.path.join(
-                self.app.root_path,
-                filename
-            )
+        if not filename.startswith("/"):
+            filename = os.path.join(self.app.root_path, filename)
 
-        if filename.endswith('.json'):
+        if filename.endswith(".json"):
             loader = json.load
-        elif filename.endswith('.yml') or filename.endswith('.yaml'):
+        elif filename.endswith(".yml") or filename.endswith(".yaml"):
+
             def loader(stream):
                 return yaml.safe_load(parse_imports(stream.read(), filename))
+
         else:
-            with codecs.open(filename, 'r', 'utf-8') as f:
+            with codecs.open(filename, "r", "utf-8") as f:
                 contents = f.read()
                 contents = contents.strip()
-                if contents[0] in ['{', '[']:
+                if contents[0] in ["{", "["]:
                     loader = json.load
                 else:
+
                     def loader(stream):
-                        return yaml.safe_load(
-                            parse_imports(stream.read(), filename))
-        with codecs.open(filename, 'r', 'utf-8') as f:
+                        return yaml.safe_load(parse_imports(stream.read(), filename))
+
+        with codecs.open(filename, "r", "utf-8") as f:
             return loader(f)
 
     @property
     def configured(self):
         """
         Return if `init_app` is configured
         """
@@ -333,309 +349,309 @@
 
     def get_url_mappings(self, rule_filter=None):
         """
         Returns all werkzeug rules
         """
         rule_filter = rule_filter or (lambda rule: True)
         app_rules = [
-            rule for rule in current_app.url_map.iter_rules()
-            if rule_filter(rule)
+            rule for rule in current_app.url_map.iter_rules() if rule_filter(rule)
         ]
         return app_rules
 
     def get_def_models(self, definition_filter=None):
         """
         Used for class based definitions
         """
         model_filter = definition_filter or (lambda tag: True)
         return {
             definition.name: definition.obj
             for definition in self.definition_models
             if model_filter(definition)
         }
 
-    def get_apispecs(self, endpoint='apispec_1'):
+    def get_apispecs(self, endpoint="apispec_1"):
         if not self.app.debug and endpoint in self.apispecs:
             return self.apispecs[endpoint]
 
         spec = None
-        for _spec in self.config['specs']:
-            if _spec['endpoint'] == endpoint:
+        for _spec in self.config["specs"]:
+            if _spec["endpoint"] == endpoint:
                 spec = _spec
                 break
         if not spec:
             raise RuntimeError(
-                'Can`t find specs by endpoint {},'
-                ' check your flasgger`s config'.format(endpoint))
+                "Can`t find specs by endpoint {},"
+                " check your flasgger`s config".format(endpoint)
+            )
 
         data = {
             # try to get from config['SWAGGER']['info']
             # then config['SWAGGER']['specs'][x]
             # then config['SWAGGER']
             # then default
-            "info": self.config.get('info') or {
-                "version": spec.get(
-                    'version', self.config.get('version', "0.0.1")
-                ),
-                "title": spec.get(
-                    'title', self.config.get('title', "A swagger API")
-                ),
+            "info": self.config.get("info")
+            or {
+                "version": spec.get("version", self.config.get("version", "0.0.1")),
+                "title": spec.get("title", self.config.get("title", "A swagger API")),
                 "description": spec.get(
-                    'description', self.config.get('description',
-                                                   "powered by Flasgger")
+                    "description", self.config.get("description", "powered by Flasgger")
                 ),
                 "termsOfService": spec.get(
-                    'termsOfService', self.config.get('termsOfService',
-                                                      "/tos")
+                    "termsOfService", self.config.get("termsOfService", "/tos")
                 ),
             },
-            "paths": self.config.get('paths') or defaultdict(dict),
-            "definitions": self.config.get('definitions') or defaultdict(dict)
+            "paths": self.config.get("paths") or defaultdict(dict),
+            "definitions": self.config.get("definitions") or defaultdict(dict),
         }
 
-        openapi_version = self.config.get('openapi')
+        openapi_version = self.config.get("openapi")
 
         # If it's openapi3, #/components/schemas replaces #/definitions
         if is_openapi3(openapi_version):
-            data.setdefault('components', {})['schemas'] = data['definitions']
+            data.setdefault("components", {})["schemas"] = data["definitions"]
 
         if openapi_version:
             data["openapi"] = openapi_version
         else:
-            data["swagger"] = self.config.get('swagger') or self.config.get(
-                'swagger_version', "2.0"
+            data["swagger"] = self.config.get("swagger") or self.config.get(
+                "swagger_version", "2.0"
             )
 
         # Support extension properties in the top level config
         top_level_extension_options = get_vendor_extension_fields(self.config)
         if top_level_extension_options:
             data.update(top_level_extension_options)
 
         # if True schemaa ids will be prefized by function_method_{id}
         # for backwards compatibility with <= 0.5.14
-        prefix_ids = self.config.get('prefix_ids')
+        prefix_ids = self.config.get("prefix_ids")
 
-        if self.config.get('host'):
-            data['host'] = self.config.get('host')
+        if self.config.get("host"):
+            data["host"] = self.config.get("host")
         if self.config.get("basePath"):
-            data["basePath"] = self.config.get('basePath')
-        if self.config.get('schemes'):
-            data['schemes'] = self.config.get('schemes')
+            data["basePath"] = self.config.get("basePath")
+        if self.config.get("schemes"):
+            data["schemes"] = self.config.get("schemes")
         if self.config.get("securityDefinitions"):
-            data["securityDefinitions"] = self.config.get(
-                'securityDefinitions'
-            )
+            data["securityDefinitions"] = self.config.get("securityDefinitions")
 
         if is_openapi3(openapi_version):
             # enable oas3 fields when openapi_version is 3.*.*
-            optional_oas3_fields = self.config.get(
-                'optional_oas3_fields') or OPTIONAL_OAS3_FIELDS
+            optional_oas3_fields = (
+                self.config.get("optional_oas3_fields") or OPTIONAL_OAS3_FIELDS
+            )
             for key in optional_oas3_fields:
                 if self.config.get(key):
                     data[key] = self.config.get(key)
 
         # set defaults from template
         if self.template is not None:
             data.update(self.template)
 
-        paths = data['paths']
+        paths = data["paths"]
         definitions = extract_schema(data)
-        ignore_verbs = set(
-            self.config.get('ignore_verbs', ("HEAD", "OPTIONS"))
-        )
+        ignore_verbs = set(self.config.get("ignore_verbs", ("HEAD", "OPTIONS")))
 
         # technically only responses is non-optional
-        optional_fields = self.config.get('optional_fields') or OPTIONAL_FIELDS
+        optional_fields = self.config.get("optional_fields") or OPTIONAL_FIELDS
 
         specs = get_specs(
-            self.get_url_mappings(spec.get('rule_filter')), ignore_verbs,
-            optional_fields, self.sanitizer,
+            self.get_url_mappings(spec.get("rule_filter")),
+            ignore_verbs,
+            optional_fields,
+            self.sanitizer,
             openapi_version=openapi_version,
-            doc_dir=self.config.get('doc_dir'))
+            doc_dir=self.config.get("doc_dir"),
+        )
 
         for name, def_model in self.get_def_models(
-                spec.get('definition_filter')).items():
-            description, swag = parse_definition_docstring(
-                def_model, self.sanitizer)
+            spec.get("definition_filter")
+        ).items():
+            description, swag = parse_definition_docstring(def_model, self.sanitizer)
             if name and swag:
                 if description:
-                    swag.update({'description': description})
+                    swag.update({"description": description})
                 definitions[name].update(swag)
 
         def merge_sub_component(dest, key, source):
             if len(source) > 0 and dest.get(key) is None:
                 dest[key] = {}
             if len(source) > 0 and len(dest[key]) >= 0:
                 dest[key].update(source)
 
         def get_operations(swag, path_verb=None):
 
             if is_openapi3(openapi_version):
-                source_components = swag.get('components', {})
-                update_schemas = source_components.get('schemas', {})
+                source_components = swag.get("components", {})
+                update_schemas = source_components.get("schemas", {})
                 # clone list so we can modify
                 active_sub_components = OAS3_SUB_COMPONENTS[:]
                 # schemas are handled separately, so remove them here
                 active_sub_components.remove("schemas")
                 for subcomponent in OAS3_SUB_COMPONENTS:
-                    merge_sub_component(data['components'], subcomponent,
-                                        source_components.get(subcomponent,
-                                        {}))
+                    merge_sub_component(
+                        data["components"],
+                        subcomponent,
+                        source_components.get(subcomponent, {}),
+                    )
             else:  # openapi2
-                update_schemas = swag.get('definitions', {})
+                update_schemas = swag.get("definitions", {})
 
             if type(update_schemas) == list and type(update_schemas[0]) == dict:
                 # pop, assert single element
-                update_schemas, = update_schemas
+                (update_schemas,) = update_schemas
             definitions.update(update_schemas)
             defs = []  # swag.get('definitions', [])
             defs += extract_definitions(
-                defs, endpoint=rule.endpoint, verb=verb,
+                defs,
+                endpoint=rule.endpoint,
+                verb=verb,
                 prefix_ids=prefix_ids,
-                openapi_version=openapi_version
+                openapi_version=openapi_version,
             )
 
-            params = swag.get('parameters', [])
+            params = swag.get("parameters", [])
             if verb in swag.keys():
                 verb_swag = swag.get(verb)
                 if len(params) == 0 and verb.lower() in http_methods:
-                    params = verb_swag.get('parameters', [])
+                    params = verb_swag.get("parameters", [])
 
-            defs += extract_definitions(params,
-                                        endpoint=rule.endpoint,
-                                        verb=verb,
-                                        prefix_ids=prefix_ids,
-                                        openapi_version=openapi_version)
+            defs += extract_definitions(
+                params,
+                endpoint=rule.endpoint,
+                verb=verb,
+                prefix_ids=prefix_ids,
+                openapi_version=openapi_version,
+            )
 
-            request_body = swag.get('requestBody')
+            request_body = swag.get("requestBody")
             if request_body:
                 content = request_body.get("content", {})
                 extract_definitions(
                     list(content.values()),
                     endpoint=rule.endpoint,
                     verb=verb,
                     prefix_ids=prefix_ids,
-                    openapi_version=openapi_version
+                    openapi_version=openapi_version,
                 )
 
             callbacks = swag.get("callbacks", {})
             if callbacks:
-                callbacks = {
-                    str(key): value
-                    for key, value in callbacks.items()
-                }
+                callbacks = {str(key): value for key, value in callbacks.items()}
                 extract_definitions(
                     list(callbacks.values()),
                     endpoint=rule.endpoint,
                     verb=verb,
                     prefix_ids=prefix_ids,
-                    openapi_version=openapi_version
+                    openapi_version=openapi_version,
                 )
 
             responses = None
-            if 'responses' in swag:
-                responses = swag.get('responses', {})
-                responses = {
-                    str(key): value
-                    for key, value in responses.items()
-                }
+            if "responses" in swag:
+                responses = swag.get("responses", {})
+                responses = {str(key): value for key, value in responses.items()}
                 if responses is not None:
                     defs = defs + extract_definitions(
                         responses.values(),
                         endpoint=rule.endpoint,
                         verb=verb,
                         prefix_ids=prefix_ids,
-                        openapi_version=openapi_version
+                        openapi_version=openapi_version,
                     )
                 for definition in defs:
-                    if 'id' not in definition:
+                    if "id" not in definition:
                         definitions.update(definition)
                         continue
-                    def_id = definition.pop('id')
+                    def_id = definition.pop("id")
                     if def_id is not None:
                         definitions[def_id].update(definition)
 
             operation = {}
-            if swag.get('summary'):
-                operation['summary'] = swag.get('summary')
-            if swag.get('description'):
-                operation['description'] = swag.get('description')
+            if swag.get("summary"):
+                operation["summary"] = swag.get("summary")
+            if swag.get("description"):
+                operation["description"] = swag.get("description")
             if request_body:
-                operation['requestBody'] = request_body
+                operation["requestBody"] = request_body
             if callbacks:
-                operation['callbacks'] = callbacks
+                operation["callbacks"] = callbacks
             # parameters - swagger ui dislikes empty parameter lists
             if len(params) > 0:
-                operation['parameters'] = params
+                operation["parameters"] = params
 
-            media_types = ['application/json']
+            media_types = ["application/json"]
             # other optionals
             for key in optional_fields:
                 if key in swag:
                     value = swag.get(key)
-                    if key in ('produces', 'consumes'):
+                    if key in ("produces", "consumes"):
                         if not isinstance(value, (list, tuple)):
                             value = [value]
-                        if key == 'produces':
+                        if key == "produces":
                             media_types = value
 
                     operation[key] = value
 
                 if responses:
                     if is_openapi3(openapi_version):
                         convert_responses_to_openapi3(responses, media_types)
 
-                    operation['responses'] = responses
+                    operation["responses"] = responses
 
             if path_verb:
                 operations[path_verb] = operation
             else:
                 operations[verb] = operation
 
-        http_methods = ['get', 'post', 'put', 'delete', 'patch']
+        http_methods = ["get", "post", "put", "delete", "patch"]
         for rule, verbs in specs:
             operations = dict()
             for verb, swag in verbs:
-                if swag.get('paths'):
+                if swag.get("paths"):
                     try:
-                        for path in swag.get('paths'):  # /projects/{project_id}/alarms:
-                            for path_verb in swag.get('paths').get(path):  # get:
+                        for path in swag.get("paths"):  # /projects/{project_id}/alarms:
+                            for path_verb in swag.get("paths").get(path):  # get:
                                 if path_verb == verb:
-                                    get_operations(swag.get('paths').get(path).get(path_verb), path_verb)
+                                    get_operations(
+                                        swag.get("paths").get(path).get(path_verb),
+                                        path_verb,
+                                    )
                     except AttributeError:
-                        logging.exception(f'Swagger doc not in the correct format. {swag}')
+                        logging.exception(
+                            f"Swagger doc not in the correct format. {swag}"
+                        )
                 else:
                     get_operations(swag)
 
             if len(operations):
                 try:
                     # Add reverse proxy prefix to route
-                    prefix = self.template['swaggerUiPrefix']
+                    prefix = self.template["swaggerUiPrefix"]
                 except (KeyError, TypeError):
-                    prefix = ''
-                srule = '{0}{1}'.format(prefix, rule)
+                    prefix = ""
+                srule = "{0}{1}".format(prefix, rule)
 
                 try:
                     # handle basePath
-                    base_path = self.template['basePath']
+                    base_path = self.template["basePath"]
 
                     if base_path:
-                        if base_path.endswith('/'):
+                        if base_path.endswith("/"):
                             base_path = base_path[:-1]
                         if base_path:
                             # suppress base_path from srule if needed.
                             # Otherwise we will get definitions twice...
                             if srule.startswith(base_path):
-                                srule = srule[len(base_path):]
+                                srule = srule[len(base_path) :]
                 except (KeyError, TypeError):
                     pass
 
                 # old regex '(<(.*?\:)?(.*?)>)'
-                for arg in re.findall('(<([^<>]*:)?([^<>]*)>)', srule):
-                    srule = srule.replace(arg[0], '{%s}' % arg[2])
+                for arg in re.findall("(<([^<>]*:)?([^<>]*)>)", srule):
+                    srule = srule.replace(arg[0], "{%s}" % arg[2])
 
                 for key, val in operations.items():
                     if srule not in paths:
                         paths[srule] = {}
                     if key in paths[srule]:
                         paths[srule][key].update(val)
                     else:
@@ -643,250 +659,248 @@
         self.apispecs[endpoint] = data
 
         # if is_openapi3(openapi_version):
         #     del data['definitions']
         if is_openapi3(openapi_version):
             # Copy definitions to components/schemas
             if definitions:
-                data.setdefault('components', {}).setdefault('schemas', {}).update(definitions)
+                data.setdefault("components", {}).setdefault("schemas", {}).update(
+                    definitions
+                )
 
         return data
 
     def definition(self, name, tags=None):
         """
         Decorator to add class based definitions
         """
+
         def wrapper(obj):
-            self.definition_models.append(SwaggerDefinition(name, obj,
-                                                            tags=tags))
+            self.definition_models.append(SwaggerDefinition(name, obj, tags=tags))
             return obj
+
         return wrapper
 
     def load_config(self, app):
         """
         Copy config from app
         """
-        self.config.update(app.config.get('SWAGGER', {}))
+        self.config.update(app.config.get("SWAGGER", {}))
 
     def register_views(self, app):
         """
         Register Flasgger views
         """
 
         # Wrap the views in an arbitrary number of decorators.
         def wrap_view(view):
             if self.decorators:
                 for decorator in self.decorators:
                     view = decorator(view)
             return view
 
-        if self.config.get('swagger_ui', True):
-            uiversion = self.config.get('uiversion', 3)
+        if self.config.get("swagger_ui", True):
+            uiversion = self.config.get("uiversion", 3)
             blueprint = Blueprint(
-                self.config.get('endpoint', 'flask_openapi'),
+                self.config.get("endpoint", "flask_openapi"),
                 __name__,
-                url_prefix=self.config.get('url_prefix', None),
-                subdomain=self.config.get('subdomain', None),
+                url_prefix=self.config.get("url_prefix", None),
+                subdomain=self.config.get("subdomain", None),
                 template_folder=self.config.get(
-                    'template_folder', 'ui{0}/templates'.format(uiversion)
+                    "template_folder", "ui{0}/templates".format(uiversion)
                 ),
                 static_folder=self.config.get(
-                    'static_folder', 'ui{0}/static'.format(uiversion)
+                    "static_folder", "ui{0}/static".format(uiversion)
                 ),
-                static_url_path=self.config.get('static_url_path', None)
+                static_url_path=self.config.get("static_url_path", None),
             )
 
-            specs_route = self.config.get('specs_route', '/apidocs/')
+            specs_route = self.config.get("specs_route", "/apidocs/")
             blueprint.add_url_rule(
                 specs_route,
-                'apidocs',
-                view_func=wrap_view(APIDocsView().as_view(
-                    'apidocs',
-                    view_args=dict(config=self.config)
-                ))
+                "apidocs",
+                view_func=wrap_view(
+                    APIDocsView().as_view("apidocs", view_args=dict(config=self.config))
+                ),
             )
 
             if uiversion < 3:
-                redirect_default = specs_route + '/o2c.html'
+                redirect_default = specs_route + "/o2c.html"
             else:
                 redirect_default = "/oauth2-redirect.html"
 
             blueprint.add_url_rule(
-                self.config.get('oauth_redirect', redirect_default),
-                'oauth_redirect',
-                view_func=wrap_view(OAuthRedirect().as_view(
-                    'oauth_redirect'
-                ))
+                self.config.get("oauth_redirect", redirect_default),
+                "oauth_redirect",
+                view_func=wrap_view(OAuthRedirect().as_view("oauth_redirect")),
             )
 
             # backwards compatibility with old url style
             blueprint.add_url_rule(
-                '/apidocs/index.html',
-                view_func=lambda: redirect(url_for('flask_openapi.apidocs'))
+                "/apidocs/index.html",
+                view_func=lambda: redirect(url_for("flask_openapi.apidocs")),
             )
         else:
             blueprint = Blueprint(
-                self.config.get('endpoint', 'flask_openapi'),
-                __name__
+                self.config.get("endpoint", "flask_openapi"), __name__
             )
 
-        for spec in self.config['specs']:
-            self.endpoints.append(spec['endpoint'])
+        for spec in self.config["specs"]:
+            self.endpoints.append(spec["endpoint"])
             blueprint.add_url_rule(
-                spec['route'],
-                spec['endpoint'],
-                view_func=wrap_view(APISpecsView.as_view(
-                    spec['endpoint'],
-                    loader=partial(
-                        self.get_apispecs, endpoint=spec['endpoint'])
-                ))
+                spec["route"],
+                spec["endpoint"],
+                view_func=wrap_view(
+                    APISpecsView.as_view(
+                        spec["endpoint"],
+                        loader=partial(self.get_apispecs, endpoint=spec["endpoint"]),
+                    )
+                ),
             )
         app.register_blueprint(blueprint)
 
     def add_headers(self, app):
         """
         Inject headers after request
         """
+
         @app.after_request
         def after_request(response):  # noqa
-            for header, value in self.config.get('headers'):
+            for header, value in self.config.get("headers"):
                 response.headers[header] = value
             return response
 
     def parse_request(self, app):
         @app.before_request
         def before_request():  # noqa
             """
             Parse and validate request data(query, form, header and body),
             set data to `request.parsed_data`
             """
             # convert "/api/items/<int:id>/" to "/api/items/{id}/"
             subs = []
-            for sub in str(request.url_rule).split('/'):
-                if '<' in sub:
-                    if ':' in sub:
-                        start = sub.index(':') + 1
+            for sub in str(request.url_rule).split("/"):
+                if "<" in sub:
+                    if ":" in sub:
+                        start = sub.index(":") + 1
                     else:
                         start = 1
-                    subs.append('{{{:s}}}'.format(sub[start:-1]))
+                    subs.append("{{{:s}}}".format(sub[start:-1]))
                 else:
                     subs.append(sub)
-            path = '/'.join(subs)
+            path = "/".join(subs)
             path_key = path + request.method.lower()
 
             if not self.app.debug and path_key in self.parsers:
                 parsers = self.parsers[path_key]
                 schemas = self.schemas[path_key]
             else:
                 doc = None
                 definitions = None
-                for spec in self.config['specs']:
-                    apispec = self.get_apispecs(endpoint=spec['endpoint'])
-                    if path in apispec['paths']:
-                        if request.method.lower() in apispec['paths'][path]:
-                            doc = apispec['paths'][path][
-                                request.method.lower()]
+                for spec in self.config["specs"]:
+                    apispec = self.get_apispecs(endpoint=spec["endpoint"])
+                    if path in apispec["paths"]:
+                        if request.method.lower() in apispec["paths"][path]:
+                            doc = apispec["paths"][path][request.method.lower()]
                             definitions = extract_schema(apispec)
                             break
                 if not doc:
                     return
 
                 parsers = defaultdict(RequestParser)
                 schemas = defaultdict(
-                    lambda: {'type': 'object', 'properties': defaultdict(dict)}
+                    lambda: {"type": "object", "properties": defaultdict(dict)}
                 )
                 self.update_schemas_parsers(doc, schemas, parsers, definitions)
                 self.schemas[path_key] = schemas
                 self.parsers[path_key] = parsers
 
-            parsed_data = {'path': request.view_args}
+            parsed_data = {"path": request.view_args}
             for location in parsers.keys():
                 parsed_data[location] = parsers[location].parse_args()
-            if 'json' in schemas:
-                parsed_data['json'] = request.json or {}
+            if "json" in schemas:
+                parsed_data["json"] = request.json or {}
             for location, data in parsed_data.items():
                 try:
                     ret = self.validation_function(data, schemas[location])
                     print(ret)
                 except jsonschema.ValidationError as e:
                     self.validation_error_handler(e, data, schemas[location])
 
-            setattr(request, 'parsed_data', parsed_data)
+            setattr(request, "parsed_data", parsed_data)
 
     def update_schemas_parsers(self, doc, schemas, parsers, definitions):
-        '''
+        """
         Schemas and parsers would be updated here from doc
-        '''
-        if is_openapi3(self.config.get('openapi')):
+        """
+        if is_openapi3(self.config.get("openapi")):
             # 'json' to comply with self.SCHEMA_LOCATIONS's {'body':'json'}
-            location = 'json'
+            location = "json"
             json_schema = None
 
             # For openapi3, currently only support single schema
-            for name, value in doc.get('requestBody', {}).get('content', {})\
-                    .items():
-                if 'application/json' in name:
+            for name, value in doc.get("requestBody", {}).get("content", {}).items():
+                if "application/json" in name:
                     # `$ref` to json, lookup in #/components/schema
-                    json_schema = value.get('schema', {})
+                    json_schema = value.get("schema", {})
                 else:  # schema set in requesty body
                     # Since osa3 might changed, repeat openapi2's code
                     parsers[location].add_argument(
                         name,
                         type=self.SCHEMA_TYPES[
-                            value['schema'].get('type', None)
-                            if 'schema' in value
-                            else value.get('type', None)],
-                        required=value.get('required', False),
-
+                            value["schema"].get("type", None)
+                            if "schema" in value
+                            else value.get("type", None)
+                        ],
+                        required=value.get("required", False),
                         # Parsed in body
-                        location=self.SCHEMA_LOCATIONS['body'],
-                        store_missing=False
+                        location=self.SCHEMA_LOCATIONS["body"],
+                        store_missing=False,
                     )
 
             # TODO support anyOf and oneOf in the future
             if (json_schema is not None) and type(json_schema) == dict:
 
                 schemas[location] = json_schema
                 self.set_schemas(schemas, location, definitions)
 
         else:  # openapi2
-            for param in doc.get('parameters', []):
-                location = self.SCHEMA_LOCATIONS[param['in']]
-                if location == 'json':  # load data from 'request.json'
-                    schemas[location] = param['schema']
+            for param in doc.get("parameters", []):
+                location = self.SCHEMA_LOCATIONS[param["in"]]
+                if location == "json":  # load data from 'request.json'
+                    schemas[location] = param["schema"]
                     self.set_schemas(schemas, location, definitions)
                 else:
-                    name = param['name']
-                    if location != 'path':
+                    name = param["name"]
+                    if location != "path":
                         parsers[location].add_argument(
                             name,
                             type=self.SCHEMA_TYPES[
-                                param['schema'].get('type', None)
-                                if 'schema' in param
-                                else param.get('type', None)],
-                            required=param.get('required', False),
-                            location=self.SCHEMA_LOCATIONS[
-                                param['in']],
-                            store_missing=False)
+                                param["schema"].get("type", None)
+                                if "schema" in param
+                                else param.get("type", None)
+                            ],
+                            required=param.get("required", False),
+                            location=self.SCHEMA_LOCATIONS[param["in"]],
+                            store_missing=False,
+                        )
 
                     for k in param:
-                        if k != 'required':
-                            schemas[
-                                location]['properties'][name][k] = param[k]
-
-    def set_schemas(self, schemas: dict, location: str,
-                    definitions: dict):
-        if is_openapi3(self.config.get('openapi')):
-            schemas[location]['components'] = {'schemas': dict(definitions)}
+                        if k != "required":
+                            schemas[location]["properties"][name][k] = param[k]
+
+    def set_schemas(self, schemas: dict, location: str, definitions: dict):
+        if is_openapi3(self.config.get("openapi")):
+            schemas[location]["components"] = {"schemas": dict(definitions)}
         else:
-            schemas[location]['definitions'] = dict(definitions)
+            schemas[location]["definitions"] = dict(definitions)
 
     def validate(
-            self, schema_id, validation_function=None,
-            validation_error_handler=None):
+        self, schema_id, validation_function=None, validation_error_handler=None
+    ):
         """
         A decorator that is used to validate incoming requests data
         against a schema
 
             swagger = Swagger(app)
 
             @app.route('/pets', methods=['POST'])
@@ -922,18 +936,19 @@
             validation_error_handler = self.validation_error_handler
 
         def decorator(func):
             @wraps(func)
             def wrapper(*args, **kwargs):
                 specs = get_schema_specs(schema_id, self)
                 validate(
-                    schema_id=schema_id, specs=specs,
+                    schema_id=schema_id,
+                    specs=specs,
                     validation_function=validation_function,
                     validation_error_handler=validation_error_handler,
-                    openapi_version=self.config.get('openapi')
+                    openapi_version=self.config.get("openapi"),
                 )
                 return func(*args, **kwargs)
 
             return wrapper
 
         return decorator
 
@@ -945,25 +960,24 @@
         found by Flasgger
 
         :param schema_id: the id of the desired schema
         """
         schema_specs = get_schema_specs(schema_id, self)
 
         if schema_specs is None:
-            raise KeyError(
-                'Specified schema_id \'{0}\' not found'.format(schema_id))
+            raise KeyError("Specified schema_id '{0}' not found".format(schema_id))
 
         for schema in (
-                parameter.get('schema') for parameter in
-                schema_specs['parameters']):
-            if schema is not None and schema.get('id').lower() == schema_id:
+            parameter.get("schema") for parameter in schema_specs["parameters"]
+        ):
+            if schema is not None and schema.get("id").lower() == schema_id:
                 return schema
 
     def is_openapi3(self):
-        return is_openapi3(self.config.get('openapi'))
+        return is_openapi3(self.config.get("openapi"))
 
 
 # backwards compatibility
 Flasgger = Swagger  # noqa
 
 
 class LazyJSONEncoder(JSONEncoder):
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/commands.py` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/commands.py`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/marshmallow_apispec.py` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/marshmallow_apispec.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,33 +11,33 @@
     from marshmallow import fields
 
     # Note that openapi_converter is initialized with trivial
     #   schema_name_resolver. Resolving circular reference is not
     #   supported for now. See issue #314 .
     # Also see: https://github.com/marshmallow-code/apispec/pull/447
     openapi_converter = openapi.OpenAPIConverter(
-        openapi_version='2.0',
+        openapi_version="2.0",
         schema_name_resolver=lambda schema: None,
-        spec=BaseAPISpec
+        spec=BaseAPISpec,
     )
     schema2jsonschema = openapi_converter.schema2jsonschema
     schema2parameters = openapi_converter.schema2parameters
 
     class Schema(marshmallow.Schema):
         swag_in = "body"
         swag_validate = True
         swag_validation_function = None
         swag_validation_error_handler = None
         swag_require_data = True
 
         def to_specs_dict(self):
-            specs = {'parameters': self.__class__}
+            specs = {"parameters": self.__class__}
             definitions: dict = {}
             specs.update(convert_schemas(specs, definitions))
-            specs['definitions'] = definitions
+            specs["definitions"] = definitions
             return specs
 
 except ImportError:
     Schema = None
     fields = None
     schema2jsonschema = lambda schema: {}  # noqa
     schema2parameters = lambda schema, location: []  # noqa
@@ -51,34 +51,32 @@
 
     def to_flasgger(self, app=None, definitions=None, paths=None):
         """
         Converts APISpec dict to flasgger suitable dict
         also adds definitions and paths (optional)
         """
         if Schema is None:
-            raise RuntimeError('Please install marshmallow and apispec')
+            raise RuntimeError("Please install marshmallow and apispec")
 
         return flask_openapi.utils.apispec_to_template(
-            app,
-            self,
-            definitions=definitions,
-            paths=paths
+            app, self, definitions=definitions, paths=paths
         )
 
 
 class SwaggerView(MethodView):
     """
     A Swagger view
     """
+
     parameters = []
     responses = {}
     definitions = {}
     tags = []
-    consumes = ['application/json']
-    produces = ['application/json']
+    consumes = ["application/json"]
+    produces = ["application/json"]
     schemes = []
     security = []
     deprecated = False
     operationId = None
     externalDocs = {}
     summary = None
     description = None
@@ -89,39 +87,43 @@
     def dispatch_request(self, *args, **kwargs):
         """
         If validation=True perform validation
         """
         if self.validation:
             specs = {}
             attrs = flask_openapi.constants.OPTIONAL_FIELDS + [
-                'parameters', 'definitions', 'responses',
-                'summary', 'description'
+                "parameters",
+                "definitions",
+                "responses",
+                "summary",
+                "description",
             ]
             for attr in attrs:
                 specs[attr] = getattr(self, attr)
             definitions = {}
             specs.update(convert_schemas(specs, definitions))
-            specs['definitions'] = definitions
+            specs["definitions"] = definitions
             flask_openapi.utils.validate(
-                specs=specs, validation_function=self.validation_function,
-                validation_error_handler=self.validation_error_handler
+                specs=specs,
+                validation_function=self.validation_function,
+                validation_error_handler=self.validation_error_handler,
             )
         return super(SwaggerView, self).dispatch_request(*args, **kwargs)
 
 
 def convert_schemas(d, definitions=None):
     """
     Convert Marshmallow schemas to dict definitions
 
     Also updates the optional definitions argument with any definitions
     entries contained within the schema.
     """
     if definitions is None:
         definitions = {}
-    definitions.update(d.get('definitions', {}))
+    definitions.update(d.get("definitions", {}))
 
     new = {}
     for k, v in d.items():
         if isinstance(v, dict):
             v = convert_schemas(v, definitions)
         if isinstance(v, (list, tuple)):
             new_v = []
@@ -130,28 +132,26 @@
                     new_v.append(convert_schemas(item, definitions))
                 else:
                     new_v.append(item)
             v = new_v
         if inspect.isclass(v) and issubclass(v, Schema):
 
             if Schema is None:
-                raise RuntimeError('Please install marshmallow and apispec')
+                raise RuntimeError("Please install marshmallow and apispec")
 
             definitions[v.__name__] = schema2jsonschema(v)
-            ref = {
-                "$ref": "#/definitions/{0}".format(v.__name__)
-            }
-            if k == 'parameters':
+            ref = {"$ref": "#/definitions/{0}".format(v.__name__)}
+            if k == "parameters":
                 new[k] = schema2parameters(v, location=v.swag_in)
-                new[k][0]['schema'] = ref
-                if len(definitions[v.__name__]['required']) != 0:
-                    new[k][0]['required'] = True
+                new[k][0]["schema"] = ref
+                if len(definitions[v.__name__]["required"]) != 0:
+                    new[k][0]["required"] = True
             else:
                 new[k] = ref
         else:
             new[k] = v
 
     # This key is not permitted anywhere except the very top level.
-    if 'definitions' in new:
-        del new['definitions']
+    if "definitions" in new:
+        del new["definitions"]
 
     return new
```

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/print.css` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/print.css`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/reset.css` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/reset.css`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/screen.css` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/screen.css`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/css/style.css` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/css/style.css`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/DroidSans-Bold.ttf` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/DroidSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/DroidSans.ttf` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.eot` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.eot`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.svg` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.svg`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.ttf` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff2` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.eot` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.svg` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.ttf` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff2` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/fonts/droid-sans-v6-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/explorer_icons.png` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/explorer_icons.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/favicon-32x32.png` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/favicon.ico` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/pet_store_api.png` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/pet_store_api.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/throbber.gif` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/throbber.gif`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/images/wordnik_api.png` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/images/wordnik_api.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/index.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/index.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ca.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ca.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/el.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/el.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/en.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/en.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/es.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/es.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/fr.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/geo.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/geo.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/it.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/it.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ja.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ko-kr.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ko-kr.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/pl.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/pt.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/ru.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/tr.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/translator.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/translator.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lang/zh-cn.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/backbone-min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/backbone-min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/es5-shim.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/es5-shim.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/handlebars-4.0.5.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/handlebars-4.0.5.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/highlight.9.1.0.pack.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/highlight.9.1.0.pack.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery-1.8.0.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery-1.8.0.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery.ba-bbq.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jquery.wiggle.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jquery.wiggle.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/js-yaml.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/js-yaml.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/jsoneditor.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/lodash.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/lodash.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/marked.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/marked.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/sanitize-html.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/sanitize-html.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/lib/swagger-oauth.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/lib/swagger-oauth.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/swagger-ui.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/static/swagger-ui.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/static/swagger-ui.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/flask_openapi/index.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/flask_openapi/index.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui2/templates/flask_openapi/index_old.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui2/templates/flask_openapi/index_old.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/favicon-16x16.png` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/favicon-32x32.png` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/lib/jquery.min.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/lib/jquery.min.map` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/lib/jquery.min.map`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-bundle.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-bundle.js.map` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js.map` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.css` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.css.map` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.js` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/static/swagger-ui.js.map` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/head.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/head.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/index.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/index.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/oauth2-redirect.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/ui3/templates/flask_openapi/swagger.html` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/ui3/templates/flask_openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenAPI3-UI-1.5.1/src/flask_openapi/utils.py` & `Flask-OpenAPI3-UI-1.6.0/src/flask_openapi/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,165 +41,174 @@
             node = target.setdefault(key, [])
             node.extend(value)
         else:
             target[key] = value
 
 
 def get_schema_specs(schema_id, swagger):
-    ignore_verbs = set(
-        swagger.config.get('ignore_verbs', ("HEAD", "OPTIONS")))
+    ignore_verbs = set(swagger.config.get("ignore_verbs", ("HEAD", "OPTIONS")))
 
     # technically only responses is non-optional
-    optional_fields \
-        = swagger.config.get('optional_fields') or OPTIONAL_FIELDS
+    optional_fields = swagger.config.get("optional_fields") or OPTIONAL_FIELDS
 
-    openapi_version = swagger.config.get('openapi')
+    openapi_version = swagger.config.get("openapi")
 
     with swagger.app.app_context():
         specs = get_specs(
-            current_app.url_map.iter_rules(), ignore_verbs,
-            optional_fields, swagger.sanitizer, openapi_version)
+            current_app.url_map.iter_rules(),
+            ignore_verbs,
+            optional_fields,
+            swagger.sanitizer,
+            openapi_version,
+        )
 
-        swags = (swag for _, verbs in specs for _, swag in verbs
-                 if swag is not None)
+        swags = (swag for _, verbs in specs for _, swag in verbs if swag is not None)
 
     for swag in swags:
-        for d in swag.get('parameters', []):
-            d_schema_id = d.get('schema', {}).get('id')
-            if d_schema_id is not None \
-                    and d_schema_id.lower() == schema_id.lower():
+        for d in swag.get("parameters", []):
+            d_schema_id = d.get("schema", {}).get("id")
+            if d_schema_id is not None and d_schema_id.lower() == schema_id.lower():
                 return swag
 
 
-def get_specs(rules, ignore_verbs, optional_fields, sanitizer,
-              openapi_version, doc_dir=None):
+def get_specs(
+    rules, ignore_verbs, optional_fields, sanitizer, openapi_version, doc_dir=None
+):
 
     specs = []
     for rule in rules:
         endpoint = current_app.view_functions[rule.endpoint]
         methods = dict()
         is_mv = is_valid_method_view(endpoint)
 
         for verb in rule.methods.difference(ignore_verbs):
             if not is_mv and has_valid_dispatch_view_docs(endpoint):
-                endpoint.methods = endpoint.methods or ['GET']
+                endpoint.methods = endpoint.methods or ["GET"]
                 if verb in endpoint.methods:
                     methods[verb.lower()] = endpoint
-            elif getattr(endpoint, 'methods', None) is not None:
+            elif getattr(endpoint, "methods", None) is not None:
                 if isinstance(endpoint.methods, set):
                     if verb in endpoint.methods:
                         verb = verb.lower()
                         methods[verb] = getattr(endpoint.view_class, verb)
                 elif fmr_methods is not None:  # flask-mongorest
                     endpoint_methods = set(m.method for m in endpoint.methods)
                     if verb in endpoint_methods:
-                        proxy_verb = rule.endpoint.replace(
-                            endpoint.__name__, ''
-                        )
+                        proxy_verb = rule.endpoint.replace(endpoint.__name__, "")
                         if proxy_verb:
-                            methods[verb.lower()] = getattr(
-                                fmr_methods, proxy_verb
-                            )
+                            methods[verb.lower()] = getattr(fmr_methods, proxy_verb)
                 else:
                     raise TypeError
             else:
                 methods[verb.lower()] = endpoint
 
         verbs = []
         for verb, method in methods.items():
 
-            klass = method.__dict__.get('view_class', None)
-            if not is_mv and klass and hasattr(klass, 'verb'):
-                method = getattr(klass, 'verb', None)
-            elif klass and hasattr(klass, 'dispatch_request'):
-                method = getattr(klass, 'dispatch_request', None)
+            klass = method.__dict__.get("view_class", None)
+            if not is_mv and klass and hasattr(klass, "verb"):
+                method = getattr(klass, "verb", None)
+            elif klass and hasattr(klass, "dispatch_request"):
+                method = getattr(klass, "dispatch_request", None)
             if method is None:  # for MethodView
                 method = getattr(klass, verb, None)
 
             if method is None:
                 if is_mv:  # #76 Empty MethodViews
                     continue
-                raise RuntimeError(
-                    'Cannot detect view_func for rule {0}'.format(rule)
-                )
+                raise RuntimeError("Cannot detect view_func for rule {0}".format(rule))
 
             swag = {}
             swag_def = {}
 
             swagged = False
 
-            if getattr(method, 'specs_dict', None):
+            if getattr(method, "specs_dict", None):
                 definition = {}
                 merge_specs(
-                    swag,
-                    convert_schemas(deepcopy(method.specs_dict), definition)
+                    swag, convert_schemas(deepcopy(method.specs_dict), definition)
                 )
                 swag_def = definition
                 swagged = True
 
-            view_class = getattr(endpoint, 'view_class', None)
+            view_class = getattr(endpoint, "view_class", None)
             if view_class and issubclass(view_class, SwaggerView):
                 apispec_swag = {}
 
                 # Don't need to alter definitions here
                 # Since it only stays in apispec_attrs
                 apispec_attrs = optional_fields + [
-                    'parameters', 'definitions', 'responses',
-                    'summary', 'description'
+                    "parameters",
+                    "definitions",
+                    "responses",
+                    "summary",
+                    "description",
                 ]
                 for attr in apispec_attrs:
                     value = getattr(view_class, attr)
                     if value:
                         apispec_swag[attr] = value
                 # Don't need to change 'definitions' here
                 # Since it would be appended later according to openapi
-                apispec_definitions = apispec_swag.get('definitions', {})
-                swag.update(
-                    convert_schemas(apispec_swag, apispec_definitions)
-                )
+                apispec_definitions = apispec_swag.get("definitions", {})
+                swag.update(convert_schemas(apispec_swag, apispec_definitions))
                 swag_def = apispec_definitions
 
                 swagged = True
 
             swag_path = None
             if doc_dir:
                 swag_path = get_swag_path_from_doc_dir(
-                    method, view_class, doc_dir, endpoint)
+                    method, view_class, doc_dir, endpoint
+                )
 
             doc_summary, doc_description, doc_swag = parse_docstring(
-                method, sanitizer, endpoint=rule.endpoint, verb=verb, swag_path=swag_path)
+                method,
+                sanitizer,
+                endpoint=rule.endpoint,
+                verb=verb,
+                swag_path=swag_path,
+            )
 
             if is_openapi3(openapi_version):
-                swag.setdefault('components', {})['schemas'] = swag_def
+                swag.setdefault("components", {})["schemas"] = swag_def
             else:  # openapi2
-                swag['definitions'] = swag_def
+                swag["definitions"] = swag_def
 
             if doc_swag:
                 merge_specs(swag, doc_swag)
                 swagged = True
 
             if swagged:
                 if doc_summary:
-                    swag['summary'] = doc_summary
+                    swag["summary"] = doc_summary
 
                 if doc_description:
-                    swag['description'] = doc_description
+                    swag["description"] = doc_description
 
                 verbs.append((verb, swag))
 
         if verbs:
             specs.append((rule, verbs))
 
     return specs
 
 
 def swag_from(
-        specs=None, filetype=None, endpoint=None, methods=None,
-        validation=False, schema_id=None, data=None, definition=None,
-        validation_function=None, validation_error_handler=None):
+    specs=None,
+    filetype=None,
+    endpoint=None,
+    methods=None,
+    validation=False,
+    schema_id=None,
+    data=None,
+    definition=None,
+    validation_function=None,
+    validation_error_handler=None,
+):
     """
     Takes a filename.yml, a dictionary or object and loads swagger specs.
 
     :param specs: a filepath, a dictionary or an object
     :param filetype: yml or yaml (json and py to be implemented)
     :param endpoint: endpoint to build definition name
     :param methods: method to build method based specs
@@ -216,31 +225,32 @@
         thrown as the first, the data being validated as the second and
         the schema being used to validate as the third argument
     """
 
     def resolve_path(function, filepath):
         try:
             from pathlib import Path
+
             if isinstance(filepath, Path):
                 filepath = str(filepath)
         except ImportError:
             pass
-        if not filepath.startswith('/'):
-            if not hasattr(function, 'root_path'):
+        if not filepath.startswith("/"):
+            if not hasattr(function, "root_path"):
                 function.root_path = get_root_path(function)
             res = os.path.join(function.root_path, filepath)
             return res
         return filepath
 
     def set_from_filepath(function):
         final_filepath = resolve_path(function, specs)
-        function.swag_type = filetype or final_filepath.split('.')[-1]
+        function.swag_type = filetype or final_filepath.split(".")[-1]
 
         if endpoint or methods:
-            if not hasattr(function, 'swag_paths'):
+            if not hasattr(function, "swag_paths"):
                 function.swag_paths = {}
 
         if not endpoint and not methods:
             function.swag_path = final_filepath
         elif endpoint and methods:
             for verb in methods:
                 key = "{}_{}".format(endpoint, verb.lower())
@@ -251,103 +261,115 @@
             for verb in methods:
                 function.swag_paths[verb.lower()] = final_filepath
 
     def set_from_specs_dict(function):
         function.specs_dict = specs
 
     def is_path(specs):
-        """ Returns True if specs is a string or pathlib.Path
-        """
+        """Returns True if specs is a string or pathlib.Path"""
         is_str_path = isinstance(specs, string_types)
         try:
             from pathlib import Path
+
             is_py3_path = isinstance(specs, Path)
             return is_str_path or is_py3_path
         except ImportError:
             return is_str_path
 
     def decorator(function):
 
         if is_path(specs):
             set_from_filepath(function)
             # function must have or a single swag_path or a list of them
-            swag_path = getattr(function, 'swag_path', None)
-            swag_paths = getattr(function, 'swag_paths', None)
+            swag_path = getattr(function, "swag_path", None)
+            swag_paths = getattr(function, "swag_paths", None)
             validate_args = {
-                'filepath': swag_path or swag_paths,
-                'root': getattr(function, 'root_path', None)
+                "filepath": swag_path or swag_paths,
+                "root": getattr(function, "root_path", None),
             }
         if isinstance(specs, dict):
             set_from_specs_dict(function)
-            validate_args = {'specs': specs}
+            validate_args = {"specs": specs}
 
         @wraps(function)
         def wrapper(*args, **kwargs):
             if validation is True:
                 validate(
                     data,
                     schema_id or definition,
                     validation_function=validation_function,
                     validation_error_handler=validation_error_handler,
-                    **validate_args
+                    **validate_args,
                 )
             return function(*args, **kwargs)
+
         return wrapper
 
     return decorator
 
 
 def __replace_ref(schema, relative_path, swag):
-    """ TODO: add dev docs
+    """TODO: add dev docs
 
     :param schema:
     :param relative_path:
     :param swag:
     :return:
     """
     absolute_path = os.path.dirname(sys.argv[0])
     new_value = {}
     for key, value in schema.items():
         if isinstance(value, dict):
             new_value[key] = __replace_ref(value, relative_path, swag)
-        elif key == '$ref':
+        elif key == "$ref":
             # see:
             # https://swagger.io/docs/specification/describing-request-body/
-            if len(value) > 2 and value.startswith('#/'):  # $ref is local
+            if len(value) > 2 and value.startswith("#/"):  # $ref is local
                 content = swag
-                for id in value.split('/')[1:]:
+                for id in value.split("/")[1:]:
                     content = content[id]
-                return __replace_ref(content, relative_path, swag) \
-                    if isinstance(content, dict) else content
+                return (
+                    __replace_ref(content, relative_path, swag)
+                    if isinstance(content, dict)
+                    else content
+                )
 
-            if len(value) > 0 and value[0] == '/':
+            if len(value) > 0 and value[0] == "/":
                 file_ref_path = absolute_path + value
             else:
-                file_ref_path = relative_path + '/' + value
+                file_ref_path = relative_path + "/" + value
             relative_path = os.path.dirname(file_ref_path)
             with open(file_ref_path) as file:
                 file_content = file.read()
-                comment_index = file_content.rfind('---')
+                comment_index = file_content.rfind("---")
                 if comment_index > 0:
                     comment_index = comment_index + 3
                 else:
                     comment_index = 0
                 content = yaml.safe_load((file_content[comment_index:]))
                 new_value = content
                 if isinstance(content, dict):
                     new_value = __replace_ref(content, relative_path, swag)
         else:
             new_value[key] = value
     return new_value
 
 
 def validate(
-        data=None, schema_id=None, filepath=None, root=None, definition=None,
-        specs=None, validation_function=None, validation_error_handler=None,
-        require_data=True, openapi_version=None):
+    data=None,
+    schema_id=None,
+    filepath=None,
+    root=None,
+    definition=None,
+    specs=None,
+    validation_function=None,
+    validation_error_handler=None,
+    require_data=True,
+    openapi_version=None,
+):
     """
     This method is available to use YAML swagger definitions file
     or specs (dict or object) to validate data against its jsonschema.
 
     example:
         validate({"item": 1}, 'item_schema', 'defs.yml', root=__file__)
         validate(request.json, 'User', specs={'definitions': {'User': ...}})
@@ -370,89 +392,87 @@
         the schema being used to validate as the third argument
     :param require_data: is the data param required?
     """
     schema_id = schema_id or definition
 
     # for backwards compatibility with function signature
     if filepath is None and specs is None:
-        abort(Response('Filepath or specs is needed to validate', status=500))
+        abort(Response("Filepath or specs is needed to validate", status=500))
 
     if data is None:
         data = request.json  # defaults
     elif callable(data):
         # data=lambda: request.json
         data = data()
 
     if not data and require_data:
-        abort(Response('No data to validate', status=400))
+        abort(Response("No data to validate", status=400))
 
     # not used anymore but kept to reuse with marshmallow
-    endpoint = request.endpoint.lower().replace('.', '_')
+    endpoint = request.endpoint.lower().replace(".", "_")
     verb = request.method.lower()
 
     if filepath is not None:
         if not root:
             try:
                 frame_info = inspect.stack()[1]
                 root = os.path.dirname(os.path.abspath(frame_info[1]))
             except Exception:
                 root = None
         else:
             root = os.path.dirname(root)
 
-        if not filepath.startswith('/'):
+        if not filepath.startswith("/"):
             final_filepath = os.path.join(root, filepath)
         else:
             final_filepath = filepath
         full_doc = load_from_file(final_filepath)
-        yaml_start = full_doc.find('---')
-        swag = yaml.safe_load(full_doc[yaml_start if yaml_start >= 0 else 0:])
+        yaml_start = full_doc.find("---")
+        swag = yaml.safe_load(full_doc[yaml_start if yaml_start >= 0 else 0 :])
     else:
         swag = copy.deepcopy(specs)
 
-    params = [
-        item for item in swag.get('parameters', [])
-        if item.get('schema')
-    ]
+    params = [item for item in swag.get("parameters", []) if item.get("schema")]
 
     definitions = {}
     main_def = {}
-    raw_definitions = extract_definitions(params, endpoint=endpoint, verb=verb,
-                                          openapi_version=openapi_version)
+    raw_definitions = extract_definitions(
+        params, endpoint=endpoint, verb=verb, openapi_version=openapi_version
+    )
 
     if schema_id is None:
         for param in params:
-            if param.get('in') == 'body':
-                schema_id = param.get('schema', {}).get('$ref')
+            if param.get("in") == "body":
+                schema_id = param.get("schema", {}).get("$ref")
                 if schema_id:
-                    schema_id = schema_id.split('/')[-1]
+                    schema_id = schema_id.split("/")[-1]
                     break  # consider only the first
 
     if schema_id is None:
         # if it is still none use first raw_definition extracted
         if raw_definitions:
-            schema_id = raw_definitions[0].get('id')
+            schema_id = raw_definitions[0].get("id")
 
     for defi in raw_definitions:
-        if defi['id'].lower() == schema_id.lower():
+        if defi["id"].lower() == schema_id.lower():
             main_def = defi.copy()
         else:
-            definitions[defi['id']] = defi
+            definitions[defi["id"]] = defi
 
     # support definitions informed in dict
     if schema_id in extract_schema(swag):
         main_def = extract_schema(swag).get(schema_id)
 
     # Doensn't need to alter 'definitions' according to open api
     # Since it main_def exists only in this function
-    main_def['definitions'] = definitions
+    main_def["definitions"] = definitions
 
     for key, value in definitions.items():
-        if 'id' in value:
-            del value['id']
+        if "id" in value:
+            del value["id"]
 
     if validation_function is None:
         validation_function = jsonschema.validate
 
     absolute_path = os.path.dirname(sys.argv[0])
     if filepath is None:
         relative_path = absolute_path
@@ -482,15 +502,15 @@
 
     with app.app_context():
         for definition in definitions:
             if isinstance(definition, (tuple, list)):
                 name, schema = definition
             else:
                 schema = definition
-                name = schema.__name__.replace('Schema', '')
+                name = schema.__name__.replace("Schema", "")
 
             spec.components.schema(name, schema=schema)
 
         for path in paths:
             spec.path(view=path)
 
     spec_dict = spec.to_dict()
@@ -518,98 +538,100 @@
     return os.path.splitext(fpath)[0]
 
 
 def is_python_file(fpath):  # pragma: no cover
     """Naive Python module filterer"""
     return fpath.endswith(".py") and "__" not in fpath
 
+
 def get_path_from_doc(full_doc):
     """
     If `file:` is provided import the file.
     """
-    swag_path = full_doc.replace('file:', '').strip()
-    swag_type = swag_path.split('.')[-1]
+    swag_path = full_doc.replace("file:", "").strip()
+    swag_type = swag_path.split(".")[-1]
     return swag_path, swag_type
 
 
 def json_to_yaml(content):
     """
     TODO: convert json to yaml
     """
     return content
 
 
-def load_from_file(swag_path, swag_type='yml', root_path=None):
+def load_from_file(swag_path, swag_type="yml", root_path=None):
     """
     Load specs from YAML file
     """
-    if swag_type not in ('yaml', 'yml'):
+    if swag_type not in ("yaml", "yml"):
         raise AttributeError("Currently only yaml or yml supported")
         # TODO: support JSON
 
     try:
         enc = detect_by_bom(swag_path)
         with codecs.open(swag_path, encoding=enc) as yaml_file:
             return yaml_file.read()
     except IOError:
         # not in the same dir, add dirname
-        swag_path = os.path.join(
-            root_path or os.path.dirname(__file__), swag_path
-        )
+        swag_path = os.path.join(root_path or os.path.dirname(__file__), swag_path)
         try:
             enc = detect_by_bom(swag_path)
             with codecs.open(swag_path, encoding=enc) as yaml_file:
                 return yaml_file.read()
         except IOError:  # pragma: no cover
             # if package dir
             # see https://github.com/rochacbruno/flasgger/pull/104
             # Still not able to reproduce this case
             # test are in examples/package_example
             # need more detail on how to reproduce IOError here
             swag_path = swag_path.replace("/", os.sep).replace("\\", os.sep)
             path = swag_path.replace(
-                (root_path or os.path.dirname(__file__)), ''
+                (root_path or os.path.dirname(__file__)), ""
             ).split(os.sep)[1:]
             package_spec = importlib.util.find_spec(path[0])
             if package_spec.has_location:
                 # Improvement idea: Use package_spec.submodule_search_locations
                 # if we're sure there's only going to be one search location.
-                site_package = package_spec.origin.replace('/__init__.py', '')
+                site_package = package_spec.origin.replace("/__init__.py", "")
             else:
                 raise RuntimeError("Package does not have origin")
             swag_path = os.path.join(site_package, os.sep.join(path[1:]))
             with open(swag_path) as yaml_file:
                 return yaml_file.read()
     except TypeError:
-        logging.warning(f"File path {swag_path} is either doesnt exist or is in the wrong type")
+        logging.warning(
+            f"File path {swag_path} is either doesnt exist or is in the wrong type"
+        )
 
 
-def detect_by_bom(path, default='utf-8'):
-    with open(path, 'rb') as f:
+def detect_by_bom(path, default="utf-8"):
+    with open(path, "rb") as f:
         raw = f.read(4)  # will read less if the file is smaller
-    for enc, boms in \
-            ('utf-8-sig', (codecs.BOM_UTF8,)),\
-            ('utf-16', (codecs.BOM_UTF16_LE, codecs.BOM_UTF16_BE)),\
-            ('utf-32', (codecs.BOM_UTF32_LE, codecs.BOM_UTF32_BE)):
+    for enc, boms in (
+        ("utf-8-sig", (codecs.BOM_UTF8,)),
+        ("utf-16", (codecs.BOM_UTF16_LE, codecs.BOM_UTF16_BE)),
+        ("utf-32", (codecs.BOM_UTF32_LE, codecs.BOM_UTF32_BE)),
+    ):
         if any(raw.startswith(bom) for bom in boms):
             return enc
     return default
 
 
 def parse_docstring(obj, process_doc, endpoint=None, verb=None, swag_path=None):
     """
     Gets swag data for method/view docstring
     """
     first_line, other_lines, swag = None, None, None
 
     full_doc = None
     if not swag_path:
-        swag_path = getattr(obj, 'swag_path', None)
-    swag_type = getattr(obj, 'swag_type', 'yml')
-    swag_paths = getattr(obj, 'swag_paths', None)
+        swag_path = getattr(obj, "swag_path", None)
+    swag_type = getattr(obj, "swag_type", "yml")
+    swag_paths = getattr(obj, "swag_paths", None)
     root_path = get_root_path(obj)
     from_file = False
 
     if swag_path is not None:
         full_doc = load_from_file(swag_path, swag_type)
         from_file = True
     elif swag_paths is not None:
@@ -621,86 +643,82 @@
         # TODO: handle multiple root_paths
         # to support `import: ` from multiple places
     else:
         full_doc = inspect.getdoc(obj)
 
     if full_doc:
 
-        if full_doc.startswith('file:'):
-            if not hasattr(obj, 'root_path'):
+        if full_doc.startswith("file:"):
+            if not hasattr(obj, "root_path"):
                 obj.root_path = root_path
             swag_path, swag_type = get_path_from_doc(full_doc)
             doc_filepath = os.path.join(obj.root_path, swag_path)
             full_doc = load_from_file(doc_filepath, swag_type)
             from_file = True
 
         full_doc = parse_imports(full_doc, root_path)
 
-        yaml_sep = full_doc.find('---')
+        yaml_sep = full_doc.find("---")
 
         if yaml_sep != -1:
-            line_feed = full_doc.find('\n')
+            line_feed = full_doc.find("\n")
             if line_feed != -1:
                 first_line = process_doc(full_doc[:line_feed])
-                other_lines = process_doc(
-                    full_doc[line_feed + 1: yaml_sep]
-                )
-                swag = yaml.safe_load(full_doc[yaml_sep + 4:])
+                other_lines = process_doc(full_doc[line_feed + 1 : yaml_sep])
+                swag = yaml.safe_load(full_doc[yaml_sep + 4 :])
         else:
             if from_file:
                 swag = yaml.safe_load(full_doc)
             else:
                 first_line = full_doc
 
     return first_line, other_lines, swag
 
 
 def get_root_path(obj):
     """
     Get file path for object and returns its dirname
     """
     try:
-        filename = os.path.abspath(obj.__globals__['__file__'])
+        filename = os.path.abspath(obj.__globals__["__file__"])
     except (KeyError, AttributeError):
-        if getattr(obj, '__wrapped__', None):
+        if getattr(obj, "__wrapped__", None):
             # decorator package has been used in view
             return get_root_path(obj.__wrapped__)
         filename = inspect.getfile(obj)
     return os.path.dirname(filename)
 
 
 def parse_definition_docstring(obj, process_doc, doc_dir=None):
     """
     Gets swag data from docstring for class based definitions
     """
     doc_lines, swag = None, None
 
     full_doc = None
-    swag_path = getattr(obj, 'swag_path', None)
-    swag_type = getattr(obj, 'swag_type', 'yml')
+    swag_path = getattr(obj, "swag_path", None)
+    swag_type = getattr(obj, "swag_type", "yml")
 
     if swag_path is not None:
         full_doc = load_from_file(swag_path, swag_type)
     else:
         full_doc = inspect.getdoc(obj)
 
     if full_doc:
 
-        if full_doc.startswith('file:'):
-            if not hasattr(obj, 'root_path'):
+        if full_doc.startswith("file:"):
+            if not hasattr(obj, "root_path"):
                 obj.root_path = get_root_path(obj)
             swag_path, swag_type = get_path_from_doc(full_doc)
             doc_filepath = os.path.join(obj.root_path, swag_path)
             full_doc = load_from_file(doc_filepath, swag_type)
 
-        yaml_sep = full_doc.find('---')
+        yaml_sep = full_doc.find("---")
         if yaml_sep != -1:
-            doc_lines = process_doc(
-                full_doc[:yaml_sep - 1]
-            ) if yaml_sep else None
+            doc_lines = process_doc(full_doc[: yaml_sep - 1]) if yaml_sep else None
             swag = yaml.safe_load(full_doc[yaml_sep:])
         else:
             doc_lines = process_doc(full_doc)
 
     return doc_lines, swag
 
 
@@ -708,69 +726,68 @@
     """
     Supports `import: otherfile.yml` in docstring specs
     """
     regex = re.compile('import: "(.*)"')
     import_prop = regex.search(full_doc)
     if import_prop:
         start = import_prop.start()
-        spaces_num = start - full_doc.rfind('\n', 0, start) - 1
+        spaces_num = start - full_doc.rfind("\n", 0, start) - 1
         filepath = import_prop.group(1)
-        if filepath.startswith('/'):
+        if filepath.startswith("/"):
             imported_doc = load_from_file(filepath)
         else:
             imported_doc = load_from_file(filepath, root_path=root_path)
-        indented_imported_doc = imported_doc.replace(
-            '\n', '\n' + ' ' * spaces_num
-        )
+        indented_imported_doc = imported_doc.replace("\n", "\n" + " " * spaces_num)
         full_doc = regex.sub(indented_imported_doc, full_doc, count=1)
         return parse_imports(full_doc)
     return full_doc
 
 
-def extract_definitions(alist, level=None, endpoint=None, verb=None,
-                        prefix_ids=False, openapi_version=None):
+def extract_definitions(
+    alist, level=None, endpoint=None, verb=None, prefix_ids=False, openapi_version=None
+):
     """
     Since we couldn't be bothered to register models elsewhere
     our definitions need to be extracted from the parameters.
     We require an 'id' field for the schema to be correctly
     added to the definitions list.
     """
     endpoint = endpoint or request.endpoint.lower()
     verb = verb or request.method.lower()
-    endpoint = endpoint.replace('.', '_')
+    endpoint = endpoint.replace(".", "_")
 
     def _extract_array_defs(source):
         """
         Extracts definitions identified by `id`
         """
         # extract any definitions that are within arrays
         # this occurs recursively
         ret = []
-        items = source.get('items')
-        if items is not None and 'schema' in items:
+        items = source.get("items")
+        if items is not None and "schema" in items:
             ret += extract_definitions(
-                [items], level + 1, endpoint, verb, prefix_ids,
-                openapi_version)
+                [items], level + 1, endpoint, verb, prefix_ids, openapi_version
+            )
         return ret
 
     # for tracking level of recursion
     if level is None:
         level = 0
 
     defs = list()
     for item in alist:
-        if not getattr(item, 'get'):
-            raise RuntimeError('definitions must be a list of dicts')
+        if not getattr(item, "get"):
+            raise RuntimeError("definitions must be a list of dicts")
         schema = item.get("schema")
         if schema is not None:
             schema_id = schema.get("id")
             if schema_id is not None:
                 # add endpoint_verb to schema id to avoid conflicts
                 if prefix_ids:
-                    schema['id'] = schema_id = "{}_{}_{}".format(
+                    schema["id"] = schema_id = "{}_{}_{}".format(
                         endpoint, verb, schema_id
                     )
                 # ^ api['SWAGGER']['prefix_ids'] = True
                 # ... for backwards compatibility with <= 0.5.14
 
                 defs.append(schema)
 
@@ -782,49 +799,57 @@
                 ref = {"$ref": "{}{}".format(ref_path, schema_id)}
 
                 # only add the reference as a schema if we are in a
                 # response or a parameter i.e. at the top level
                 # directly ref if a definition is used within another
                 # definition
                 if level == 0:
-                    item['schema'] = ref
+                    item["schema"] = ref
                 else:
                     item.update(ref)
-                    del item['schema']
+                    del item["schema"]
 
             # extract any definitions that are within properties
             # this occurs recursively
-            properties = schema.get('properties')
+            properties = schema.get("properties")
             if properties is not None:
                 defs += extract_definitions(
-                    properties.values(), level + 1, endpoint, verb, prefix_ids,
-                    openapi_version)
+                    properties.values(),
+                    level + 1,
+                    endpoint,
+                    verb,
+                    prefix_ids,
+                    openapi_version,
+                )
 
             defs += _extract_array_defs(schema)
 
         defs += _extract_array_defs(item)
 
     return defs
 
 
 def has_valid_dispatch_view_docs(endpoint):
     """
     Return True if dispatch_request is swaggable
     """
-    klass = endpoint.__dict__.get('view_class', None)
-    return klass and hasattr(klass, 'dispatch_request') \
-        and hasattr(endpoint, 'methods') \
-        and getattr(klass, 'dispatch_request').__doc__
+    klass = endpoint.__dict__.get("view_class", None)
+    return (
+        klass
+        and hasattr(klass, "dispatch_request")
+        and hasattr(endpoint, "methods")
+        and getattr(klass, "dispatch_request").__doc__
+    )
 
 
 def is_valid_method_view(endpoint):
     """
     Return True if obj is MethodView
     """
-    klass = endpoint.__dict__.get('view_class', None)
+    klass = endpoint.__dict__.get("view_class", None)
     try:
         return issubclass(klass, MethodView)
     except TypeError:
         return False
 
 
 def get_vendor_extension_fields(mapping):
@@ -832,15 +857,15 @@
     Identify vendor extension fields and extract them into a new dictionary.
     Examples:
         >>> get_vendor_extension_fields({'test': 1})
         {}
         >>> get_vendor_extension_fields({'test': 1, 'x-test': 2})
         {'x-test': 2}
     """
-    return {k: v for k, v in mapping.items() if k.startswith('x-')}
+    return {k: v for k, v in mapping.items() if k.startswith("x-")}
 
 
 class StringLike(object):
     """
     Class to mimic the behavior of a regular string. Classes that inherit (or
     mixin) this class must implement the `__str__` magic method. Whatever that
     method returns is used by the various string-like methods.
@@ -966,34 +991,36 @@
                 for row in data["parameters"]:
                     specs["parameters"].append(row)
                 specs["definitions"].update(data["definitions"])
 
                 function = validate_annotation(annotation, variable)(function)
 
             elif issubclass(annotation, int):
-                m = {"name": variable,
-                     "in": "path",
-                     "type": "integer",
-                     "required": True}
+                m = {
+                    "name": variable,
+                    "in": "path",
+                    "type": "integer",
+                    "required": True,
+                }
                 if ("int(signed=True):" + variable) in args[0]:
-                    m['minimum'] = 0
+                    m["minimum"] = 0
                 specs["parameters"].append(m)
 
             elif issubclass(annotation, str):
-                specs["parameters"].append({"name": variable,
-                                            "in": "path",
-                                            "type": "string",
-                                            "required": True})
+                specs["parameters"].append(
+                    {"name": variable, "in": "path", "type": "string", "required": True}
+                )
 
         function.specs_dict = specs
         args = list(args)
         args[2] = function
         args = tuple(args)
 
         return f(*args, **kwargs)
+
     return wrapper
 
 
 def validate_annotation(an, var):
     def decorator(f):
         @wraps(f)
         def wrapper(*args, **kwargs):
@@ -1014,81 +1041,82 @@
                     validation_function=an.swag_validation_function,
                     validation_error_handler=an.swag_validation_error_handler,
                     require_data=an.swag_require_data
                     # handle openapiversion later
                 )
 
             return f(*args, **kwargs, **{var: payload})
+
         return wrapper
+
     return decorator
 
 
 def is_openapi3(openapi_version):
     """
     Returns True if openapi_version is 3
     """
-    return openapi_version and str(openapi_version).split('.')[0] == '3'
+    return openapi_version and str(openapi_version).split(".")[0] == "3"
 
 
 def extract_schema(spec: dict) -> defaultdict:
     """
     Returns schema resources according to openapi version
     """
-    openapi_version = spec.get('openapi', None)
+    openapi_version = spec.get("openapi", None)
     if is_openapi3(openapi_version):
-        return spec.get('components', {}
-                        ).get('schemas', defaultdict(dict))
+        return spec.get("components", {}).get("schemas", defaultdict(dict))
     else:  # openapi2
-        return spec.get('definitions', defaultdict(dict))
+        return spec.get("definitions", defaultdict(dict))
 
 
-def get_swag_path_from_doc_dir(method: any, view_class: any, doc_dir: str, endpoint: any):
-    file_path = ''
-    func = method.__func__ \
-        if hasattr(method, '__func__') else method
+def get_swag_path_from_doc_dir(
+    method: any, view_class: any, doc_dir: str, endpoint: any
+):
+    file_path = ""
+    func = method.__func__ if hasattr(method, "__func__") else method
     if view_class:
-        file_path = os.path.join(
-            doc_dir, endpoint.__name__, method.__name__ + '.yml')
+        file_path = os.path.join(doc_dir, endpoint.__name__, method.__name__ + ".yml")
     else:
-        file_path = os.path.join(
-            doc_dir, endpoint.__name__ + '.yml')
+        file_path = os.path.join(doc_dir, endpoint.__name__ + ".yml")
     if file_path and os.path.isfile(file_path):
-        setattr(func, 'swag_type', 'yml')
-        setattr(func, 'swag_path', file_path)
+        setattr(func, "swag_type", "yml")
+        setattr(func, "swag_path", file_path)
     else:
         # HACK: If the doc_dir doesn't quite match the filepath we take the doc_dir
         # and the current filepath without the /tmp
-        file_path = getattr(func, 'swag_path', None)
+        file_path = getattr(func, "swag_path", None)
         if file_path and not os.path.isfile(file_path):
             regex = re.compile(r"(api.+)")
             try:
                 file_path = doc_dir + regex.search(file_path)[0]
                 if os.path.isfile(file_path):
-                    setattr(func, 'swag_type', 'yml')
-                    setattr(func, 'swag_path', file_path)
+                    setattr(func, "swag_type", "yml")
+                    setattr(func, "swag_path", file_path)
             except Exception:
                 logging.exception(f"{file_path} is not a file")
 
     return file_path
 
+
 def convert_references_to_openapi3(obj):
     for key, val in obj.items():
-        if key == '$ref':
-            obj[key] = val.replace('definitions', 'components/schemas')
+        if key == "$ref":
+            obj[key] = val.replace("definitions", "components/schemas")
 
         if isinstance(val, dict):
             convert_references_to_openapi3(val)
 
 
 def convert_response_definitions_to_openapi3(response, media_types):
-    if 'schema' in response:
-        convert_references_to_openapi3(response['schema'])
-        if 'content' not in response:
-            response['content'] = {}
+    if "schema" in response:
+        convert_references_to_openapi3(response["schema"])
+        if "content" not in response:
+            response["content"] = {}
             for media_type in media_types:
-                response['content'][media_type] = {'schema': dict(response['schema'])}
-        del response['schema']
+                response["content"][media_type] = {"schema": dict(response["schema"])}
+        del response["schema"]
 
 
 def convert_responses_to_openapi3(responses, media_types):
     for val in responses.values():
-        convert_response_definitions_to_openapi3(val, media_types)
+        convert_response_definitions_to_openapi3(val, media_types)
```

