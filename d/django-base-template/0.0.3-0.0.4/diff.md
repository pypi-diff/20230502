# Comparing `tmp/django_base_template-0.0.3.tar.gz` & `tmp/django_base_template-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_base_template-0.0.3.tar", last modified: Sun Mar 19 21:55:58 2023, max compression
+gzip compressed data, was "django_base_template-0.0.4.tar", last modified: Tue May  2 21:15:10 2023, max compression
```

## Comparing `django_base_template-0.0.3.tar` & `django_base_template-0.0.4.tar`

### file list

```diff
@@ -1,142 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.732586 django_base_template-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.680585 django_base_template-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.696586 django_base_template-0.0.3/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-03-19 21:55:50.000000 django_base_template-0.0.3/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.696586 django_base_template-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-19 21:55:50.000000 django_base_template-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-19 21:55:50.000000 django_base_template-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-03-19 21:55:50.000000 django_base_template-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-19 21:55:50.000000 django_base_template-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-19 21:55:50.000000 django_base_template-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-19 21:55:58.732586 django_base_template-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.696586 django_base_template-0.0.3/base_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.700586 django_base_template-0.0.3/base_template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/__pycache__/sidebars.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/__pycache__/wsgi.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/sidebars.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-19 21:55:50.000000 django_base_template-0.0.3/base_template/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/db.sqlite3
--rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-03-19 21:55:50.000000 django_base_template-0.0.3/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-19 21:55:50.000000 django_base_template-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-19 21:55:58.732586 django_base_template-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 21:55:50.000000 django_base_template-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.692586 django_base_template-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.700586 django_base_template-0.0.3/src/base_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.704586 django_base_template-0.0.3/src/base_template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/__pycache__/context_processors.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.684586 django_base_template-0.0.3/src/base_template/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.684586 django_base_template-0.0.3/src/base_template/static/base_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.704586 django_base_template-0.0.3/src/base_template/static/base_template/css/
--rw-r--r--   0 runner    (1001) docker     (123)  1316039 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/css/style.bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)  1379283 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/css/style.bundle.rtl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.708586 django_base_template-0.0.3/src/base_template/static/base_template/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/smartphone-2-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/smartphone-2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68122 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/images/user.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.708586 django_base_template-0.0.3/src/base_template/static/base_template/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.684586 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.684586 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.708586 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/reset-password/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/reset-password/new-password.js
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/reset-password/reset-password.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.712586 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/general.js
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/i18n.js
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/two-steps.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.712586 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/coming-soon.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/free-trial.js
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/general.js
--rw-r--r--   0 runner    (1001) docker     (123)    95345 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/js/scripts.bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.684586 django_base_template-0.0.3/src/base_template/static/base_template/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.716586 django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/
--rw-r--r--   0 runner    (1001) docker     (123)   504225 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)  2158667 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   198052 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.684586 django_base_template-0.0.3/src/base_template/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.716586 django_base_template-0.0.3/src/base_template/templates/base_template/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.716586 django_base_template-0.0.3/src/base_template/templates/base_template/layout/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/_localization.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.716586 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/_sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.716586 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/footer/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/footer/__footer_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/footer/_footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.720586 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/header/_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/header/_left_menus.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/header/_right_menus.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.720586 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.720586 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/toolbar/_toolbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.720586 django_base_template-0.0.3/src/base_template/templates/base_template/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/_scrolltop.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.720586 django_base_template-0.0.3/src/base_template/templates/base_template/partials/general/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/general/_button-indicator.html
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/general/_notice.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.724586 django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/__langauage_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/_user-account-menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.724586 django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/__menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/_init.html
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/_main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.692586 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.724586 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-17.html
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-18.html
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-20.html
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-7.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.728587 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-24.html
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-31.html
--rw-r--r--   0 runner    (1001) docker     (123)    26465 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-35.html
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-36.html
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-8.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.728587 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/engage/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/engage/_widget-10.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.728587 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/lists/
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/lists/_widget-26.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.728587 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/tables/
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/tables/_widget-14.html
--rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/tables/_widget-16.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.728587 django_base_template-0.0.3/src/base_template/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templatetags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.732586 django_base_template-0.0.3/src/base_template/templatetags/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/templatetags/base_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-19 21:55:50.000000 django_base_template-0.0.3/src/base_template/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:55:58.732586 django_base_template-0.0.3/src/django_base_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-19 21:55:58.000000 django_base_template-0.0.3/src/django_base_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-03-19 21:55:58.000000 django_base_template-0.0.3/src/django_base_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 21:55:58.000000 django_base_template-0.0.3/src/django_base_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-19 21:55:58.000000 django_base_template-0.0.3/src/django_base_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.481857 django_base_template-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.idea/base_template.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-02 21:14:58.000000 django_base_template-0.0.4/.idea/workspace.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 21:14:58.000000 django_base_template-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:14:58.000000 django_base_template-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 21:15:10.501857 django_base_template-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.489857 django_base_template-0.0.4/base_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.489857 django_base_template-0.0.4/base_template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/__pycache__/sidebars.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/__pycache__/wsgi.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/sidebars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 21:14:58.000000 django_base_template-0.0.4/base_template/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/db.sqlite3
+-rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-05-02 21:14:58.000000 django_base_template-0.0.4/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 21:14:58.000000 django_base_template-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-02 21:15:10.505857 django_base_template-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:14:58.000000 django_base_template-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.489857 django_base_template-0.0.4/src/base_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.489857 django_base_template-0.0.4/src/base_template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/__pycache__/context_processors.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.481857 django_base_template-0.0.4/src/base_template/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/src/base_template/static/base_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.489857 django_base_template-0.0.4/src/base_template/static/base_template/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1316039 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/css/style.bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1379283 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/css/style.bundle.rtl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.493857 django_base_template-0.0.4/src/base_template/static/base_template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/smartphone-2-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/smartphone-2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68122 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/images/user.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.493857 django_base_template-0.0.4/src/base_template/static/base_template/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.481857 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.493857 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/reset-password/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/reset-password/new-password.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/reset-password/reset-password.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.493857 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/general.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/i18n.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/two-steps.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.493857 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/coming-soon.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/free-trial.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/general.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95345 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/js/scripts.bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/src/base_template/static/base_template/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/
+-rw-r--r--   0 runner    (1001) docker     (123)   504225 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/plugins.bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)  2158667 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/plugins.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198052 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/src/base_template/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/_localization.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/_sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/footer/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/footer/__footer_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/footer/_footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/header/_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/header/_left_menus.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/header/_right_menus.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.497857 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/toolbar/_toolbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/_scrolltop.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/general/_button-indicator.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/general/_notice.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/__langauage_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/_user-account-menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/__menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/_init.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/_main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.485857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-17.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-18.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-20.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-7.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-24.html
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-31.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26465 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-35.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-36.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-8.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/engage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/engage/_widget-10.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/lists/_widget-26.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/tables/_widget-14.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65841 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/tables/_widget-16.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templatetags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/base_template/templatetags/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/templatetags/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-02 21:14:58.000000 django_base_template-0.0.4/src/base_template/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:10.501857 django_base_template-0.0.4/src/django_base_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 21:15:10.000000 django_base_template-0.0.4/src/django_base_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-02 21:15:10.000000 django_base_template-0.0.4/src/django_base_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:15:10.000000 django_base_template-0.0.4/src/django_base_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 21:15:10.000000 django_base_template-0.0.4/src/django_base_template.egg-info/top_level.txt
```

### Comparing `django_base_template-0.0.3/.github/scripts/release.py` & `django_base_template-0.0.4/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/.gitignore` & `django_base_template-0.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,9 +154,9 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
```

### Comparing `django_base_template-0.0.3/LICENSE` & `django_base_template-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/PKG-INFO` & `django_base_template-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_base_template
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django package provides easy configuration admin template
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django_base_template-0.0.3/base_template/__pycache__/settings.cpython-38.pyc` & `django_base_template-0.0.4/base_template/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/base_template/__pycache__/urls.cpython-38.pyc` & `django_base_template-0.0.4/base_template/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/base_template/__pycache__/wsgi.cpython-38.pyc` & `django_base_template-0.0.4/base_template/__pycache__/wsgi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/base_template/settings.py` & `django_base_template-0.0.4/base_template/settings.py`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/manage.py` & `django_base_template-0.0.4/manage.py`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/setup.cfg` & `django_base_template-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/__pycache__/context_processors.cpython-38.pyc` & `django_base_template-0.0.4/src/base_template/__pycache__/context_processors.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/__pycache__/settings.cpython-38.pyc` & `django_base_template-0.0.4/src/base_template/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/__pycache__/utils.cpython-38.pyc` & `django_base_template-0.0.4/src/base_template/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/context_processors.py` & `django_base_template-0.0.4/src/base_template/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/settings.py` & `django_base_template-0.0.4/src/base_template/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Package Settings
 # localization
 from django.utils.translation import gettext_lazy as _
 
 BASE_TEMPLATE_MULTIPLE_LANGUAGES = True
 
-# Logo
-
+BASE_TEMPLATE_APP_NAME = _("Base Template")
 
 # Sidebar
 BASE_TEMPLATE_GET_SIDEBAR_METHOD = 'base_template.sidebars.get_sidebar'
 BASE_TEMPLATE_SIDEBAR_FOOTER_TEMPLATE = "base_template/layout/partials/sidebar/_footer.html"
 BASE_TEMPLATE_SIDEBAR_LOGO = "base_template/images/logo-white.svg"
 BASE_TEMPLATE_SIDEBAR_LOGO_ICON = "base_template/images/icon.svg"
```

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/css/style.bundle.css` & `django_base_template-0.0.4/src/base_template/static/base_template/css/style.bundle.css`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/css/style.bundle.rtl.css` & `django_base_template-0.0.4/src/base_template/static/base_template/css/style.bundle.rtl.css`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/icon.ico` & `django_base_template-0.0.4/src/base_template/static/base_template/images/icon.ico`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/icon.svg` & `django_base_template-0.0.4/src/base_template/static/base_template/images/icon.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/logo-dark.svg` & `django_base_template-0.0.4/src/base_template/static/base_template/images/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/logo-white.svg` & `django_base_template-0.0.4/src/base_template/static/base_template/images/logo-white.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/logo.png` & `django_base_template-0.0.4/src/base_template/static/base_template/images/logo.png`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/smartphone-2-dark.svg` & `django_base_template-0.0.4/src/base_template/static/base_template/images/smartphone-2-dark.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/smartphone-2.svg` & `django_base_template-0.0.4/src/base_template/static/base_template/images/smartphone-2.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/images/user.jpg` & `django_base_template-0.0.4/src/base_template/static/base_template/images/user.jpg`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/reset-password/new-password.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/reset-password/new-password.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/reset-password/reset-password.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/reset-password/reset-password.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/general.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/general.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/i18n.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/i18n.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-in/two-steps.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-in/two-steps.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/coming-soon.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/coming-soon.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/free-trial.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/free-trial.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/custom/authentication/sign-up/general.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/custom/authentication/sign-up/general.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/js/scripts.bundle.js` & `django_base_template-0.0.4/src/base_template/static/base_template/js/scripts.bundle.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.css` & `django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/plugins.bundle.css`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.js` & `django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/plugins.bundle.js`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css` & `django_base_template-0.0.4/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/base.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-{% load static i18n %}
+{% load static i18n base_template %}
 {% get_current_language as LANGUAGE_CODE %}
 {% get_current_language_bidi as LANGUAGE_BIDI %}
 <!DOCTYPE html>
 <html {% include "base_template/layout/_localization.html" %}>
 <head>
-  <title></title>
+  <title>{% get_base_template_setting "BASE_TEMPLATE_APP_NAME" %} | {% block title %}{% endblock %}</title>
   <meta charset="utf-8"/>
   <meta name="description" content=""/>
   <meta name="keywords" content=""/>
   <meta name="viewport" content="width=device-width, initial-scale=1"/>
   <meta property="og:locale" content=""/>
   <meta property="og:type" content=""/>
   <meta property="og:title" content=""/>
@@ -20,15 +20,15 @@
   {% if LANGUAGE_BIDI %}
     <link href="{% static "base_template/plugins/global/plugins.bundle.rtl.css" %}" rel="stylesheet" type="text/css"/>
     <link href="{% static "base_template/css/style.bundle.rtl.css" %}" rel="stylesheet" type="text/css"/>
   {% else %}
     <link href="{% static "base_template/plugins/global/plugins.bundle.css" %}" rel="stylesheet" type="text/css"/>
     <link href="{% static "base_template/css/style.bundle.css" %}" rel="stylesheet" type="text/css"/>
   {% endif %}
-  {% block base_styles %}{% endblock %}
+  {% block styles %}{% endblock %}
 </head>
 <body id="kt_app_body"
       class="app-default"
       data-kt-app-layout="dark-sidebar"
       data-kt-app-header-fixed="true"
       data-kt-app-sidebar-enabled="true"
       data-kt-app-sidebar-fixed="true"
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% load static i18n %} {% get_current_language as LANGUAGE_CODE %} {%
-get_current_language_bidi as LANGUAGE_BIDI %}
+{% load static i18n base_template %} {% get_current_language as LANGUAGE_CODE
+%} {% get_current_language_bidi as LANGUAGE_BIDI %}
 
 % include "base_template/layout/_localization.html" %}>
 
 
 
 
 
@@ -14,15 +14,15 @@
 
 mages/icon.ico" %}"/>
  {% if LANGUAGE_BIDI %}
 lugins/global/plugins.bundle.rtl.css" %}" rel="stylesheet" type="text/css"/>
 ss/style.bundle.rtl.css" %}" rel="stylesheet" type="text/css"/> {% else %}
 lugins/global/plugins.bundle.css" %}" rel="stylesheet" type="text/css"/>
 ss/style.bundle.css" %}" rel="stylesheet" type="text/css"/> {% endif %} {%
-block base_styles %}{% endblock %}
+block styles %}{% endblock %}
 {% include "base_template/partials/theme-mode/_init.html" %}
 {% include "base_template/layout/partials/header/_header.html" %}
 {% include "base_template/layout/partials/_sidebar.html" %}
 {% block toolbar %} {% include "base_template/layout/partials/toolbar/
 _toolbar.html" %} {% endblock %}
 {% block content %}{% endblock %}
 {% include "base_template/layout/partials/footer/_footer.html" %}
```

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/_sidebar.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/footer/_footer.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/footer/_footer.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/header/_header.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/header/_header.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/header/_left_menus.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/header/_left_menus.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/_scrolltop.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/_scrolltop.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/general/_notice.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/general/_notice.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/__langauage_menu.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/__langauage_menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/menus/_user-account-menu.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/menus/_user-account-menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/__menu.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/__menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/_init.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/_init.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/theme-mode/_main.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/theme-mode/_main.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-17.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-17.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-18.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-18.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-20.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-20.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/cards/_widget-7.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/cards/_widget-7.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-24.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-24.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-31.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-31.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-35.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-35.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-36.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-36.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/charts/_widget-8.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/charts/_widget-8.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/engage/_widget-10.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/engage/_widget-10.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/lists/_widget-26.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/lists/_widget-26.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/tables/_widget-14.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/tables/_widget-14.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templates/base_template/partials/widgets/tables/_widget-16.html` & `django_base_template-0.0.4/src/base_template/templates/base_template/partials/widgets/tables/_widget-16.html`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc` & `django_base_template-0.0.4/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/base_template/utils.py` & `django_base_template-0.0.4/src/base_template/utils.py`

 * *Files identical despite different names*

### Comparing `django_base_template-0.0.3/src/django_base_template.egg-info/PKG-INFO` & `django_base_template-0.0.4/src/django_base_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-base-template
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django package provides easy configuration admin template
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django_base_template-0.0.3/src/django_base_template.egg-info/SOURCES.txt` & `django_base_template-0.0.4/src/django_base_template.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 manage.py
 pyproject.toml
 setup.cfg
 setup.py
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
+.idea/base_template.iml
+.idea/misc.xml
+.idea/vcs.xml
+.idea/workspace.xml
+.idea/inspectionProfiles/Project_Default.xml
+.idea/inspectionProfiles/profiles_settings.xml
 base_template/__init__.py
 base_template/asgi.py
 base_template/settings.py
 base_template/sidebars.py
 base_template/urls.py
 base_template/wsgi.py
 base_template/__pycache__/__init__.cpython-38.pyc
```

