# Comparing `tmp/Flask-2.3.1.tar.gz` & `tmp/Flask-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-2.3.1.tar", last modified: Tue Apr 25 20:15:30 2023, max compression
+gzip compressed data, was "Flask-2.3.2.tar", last modified: Mon May  1 15:36:10 2023, max compression
```

## Comparing `Flask-2.3.1.tar` & `Flask-2.3.2.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.831820 Flask-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    66956 2023-04-25 20:15:19.000000 Flask-2.3.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-25 20:15:19.000000 Flask-2.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 20:15:19.000000 Flask-2.3.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-25 20:15:19.000000 Flask-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-25 20:15:30.831820 Flask-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-25 20:15:19.000000 Flask-2.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.807820 Flask-2.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.807820 Flask-2.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   207889 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/_static/debugger.png
--rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/_static/flask-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/_static/flask-vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    99654 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/_static/pycharm-run-config.png
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/_static/shortcut-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    21833 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/appcontext.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/async-await.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/blueprints.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/debugging.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.807820 Flask-2.3.1/docs/deploying/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/apache-httpd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/asgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/eventlet.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/gevent.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/gunicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/mod_wsgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/nginx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/proxy_fix.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/uwsgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/deploying/waitress.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/errorhandling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/extensiondev.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.811820 Flask-2.3.1/docs/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/appdispatch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/appfactories.rst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/caching.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/celery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/deferredcallbacks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/favicon.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/fileuploads.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/flashing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/javascript.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/jquery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/lazyloading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/methodoverrides.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/mongoengine.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/packages.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/requestchecksum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/singlepageapplications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/sqlalchemy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/sqlite3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/streaming.rst
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/subclassing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/templateinheritance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/urlprocessors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/viewdecorators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/patterns/wtforms.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32281 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/reqcontext.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/security.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/shell.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/templating.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.811820 Flask-2.3.1/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/blog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/flaskr_edit.png
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/flaskr_index.png
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/flaskr_login.png
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/next.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/static.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18265 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/tutorial/views.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-04-25 20:15:19.000000 Flask-2.3.1/docs/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.799820 Flask-2.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/celery/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/make_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.799820 Flask-2.3.1/examples/celery/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/celery/src/task_app/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/src/task_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/src/task_app/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/celery/src/task_app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/src/task_app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/celery/src/task_app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/javascript/js_example/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/js_example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/javascript/js_example/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/js_example/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/js_example/templates/fetch.html
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/js_example/templates/jquery.html
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/js_example/templates/xhr.html
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/js_example/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/javascript/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/javascript/tests/test_js_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/tutorial/flaskr/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/tutorial/flaskr/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/tutorial/flaskr/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.815820 Flask-2.3.1/examples/tutorial/flaskr/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/templates/auth/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/templates/auth/register.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.819820 Flask-2.3.1/examples/tutorial/flaskr/templates/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/templates/blog/create.html
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/templates/blog/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/flaskr/templates/blog/update.html
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.819820 Flask-2.3.1/examples/tutorial/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/tests/data.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 20:15:19.000000 Flask-2.3.1/examples/tutorial/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-25 20:15:19.000000 Flask-2.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.819820 Flask-2.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 20:15:19.000000 Flask-2.3.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-25 20:15:19.000000 Flask-2.3.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-25 20:15:19.000000 Flask-2.3.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 20:15:19.000000 Flask-2.3.1/requirements/tests-pallets-min.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 20:15:19.000000 Flask-2.3.1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 20:15:19.000000 Flask-2.3.1/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 20:15:30.831820 Flask-2.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.799820 Flask-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.819820 Flask-2.3.1/src/Flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-25 20:15:30.000000 Flask-2.3.1/src/Flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-25 20:15:30.000000 Flask-2.3.1/src/Flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 20:15:30.000000 Flask-2.3.1/src/Flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 20:15:30.000000 Flask-2.3.1/src/Flask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-25 20:15:30.000000 Flask-2.3.1/src/Flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 20:15:30.000000 Flask-2.3.1/src/Flask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.823820 Flask-2.3.1/src/flask/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87594 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    33720 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/debughelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    24957 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.823820 Flask-2.3.1/src/flask/json/
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/json/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/json/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-25 20:15:19.000000 Flask-2.3.1/src/flask/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.823820 Flask-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/static/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/static/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/_macro.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/context_template.html
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/escaping_template.html
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/mail.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/templates/nested/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/nested/nested.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/non_escaping_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/simple_template.html
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/template_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/templates/template_test.html
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_appctx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/.env
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/.flaskenv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/static/css/test.css
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/static/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.799820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/admin/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/frontend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.799820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/blueprintapp/apps/frontend/templates/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/blueprintapp/apps/frontend/templates/frontend/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/cliapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/importerrorapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/cliapp/inner1/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/inner1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/cliapp/inner1/inner2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/inner1/inner2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/inner1/inner2/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/message.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/cliapp/multiapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/helloworld/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/helloworld/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/subdomaintestmodule/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/subdomaintestmodule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.827820 Flask-2.3.1/tests/test_apps/subdomaintestmodule/static/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_apps/subdomaintestmodule/static/hello.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    51152 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_instance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_json_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_reqctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_session_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_subclassing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_templating.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_user_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:15:30.831820 Flask-2.3.1/tests/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/typing/typing_app_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/typing/typing_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-25 20:15:19.000000 Flask-2.3.1/tests/typing/typing_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-25 20:15:19.000000 Flask-2.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.293284 Flask-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    67164 2023-05-01 15:35:58.000000 Flask-2.3.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-01 15:35:58.000000 Flask-2.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 15:35:58.000000 Flask-2.3.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-01 15:35:58.000000 Flask-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-01 15:36:10.293284 Flask-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-01 15:35:58.000000 Flask-2.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.269284 Flask-2.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.269284 Flask-2.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   207889 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/_static/debugger.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/_static/flask-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/_static/flask-vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99654 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/_static/pycharm-run-config.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/_static/shortcut-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21833 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/appcontext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/async-await.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/blueprints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/debugging.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.269284 Flask-2.3.2/docs/deploying/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/apache-httpd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/asgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/eventlet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/gevent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/gunicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/mod_wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/nginx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/proxy_fix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/uwsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/deploying/waitress.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/errorhandling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/extensiondev.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.273284 Flask-2.3.2/docs/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/appdispatch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/appfactories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/deferredcallbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/favicon.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/fileuploads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/flashing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/javascript.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/jquery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/lazyloading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/methodoverrides.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/mongoengine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/packages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/requestchecksum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/singlepageapplications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/sqlalchemy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/sqlite3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/streaming.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/subclassing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/templateinheritance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/urlprocessors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/viewdecorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/patterns/wtforms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32281 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/reqcontext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/shell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/templating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/blog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/flaskr_edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/flaskr_index.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/flaskr_login.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/next.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/static.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18265 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/tutorial/views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-05-01 15:35:58.000000 Flask-2.3.2/docs/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.261284 Flask-2.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/make_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.261284 Flask-2.3.2/examples/celery/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/celery/src/task_app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/src/task_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/src/task_app/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/celery/src/task_app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/src/task_app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/celery/src/task_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/javascript/js_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/js_example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/javascript/js_example/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/js_example/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/js_example/templates/fetch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/js_example/templates/jquery.html
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/js_example/templates/xhr.html
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/js_example/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/javascript/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/javascript/tests/test_js_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/tutorial/flaskr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/tutorial/flaskr/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/tutorial/flaskr/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.277284 Flask-2.3.2/examples/tutorial/flaskr/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/templates/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/templates/auth/register.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.281284 Flask-2.3.2/examples/tutorial/flaskr/templates/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/templates/blog/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/templates/blog/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/flaskr/templates/blog/update.html
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.281284 Flask-2.3.2/examples/tutorial/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/tests/data.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 15:35:58.000000 Flask-2.3.2/examples/tutorial/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-01 15:35:58.000000 Flask-2.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.281284 Flask-2.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 15:35:58.000000 Flask-2.3.2/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-01 15:35:58.000000 Flask-2.3.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-01 15:35:58.000000 Flask-2.3.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-01 15:35:58.000000 Flask-2.3.2/requirements/tests-pallets-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 15:35:58.000000 Flask-2.3.2/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 15:35:58.000000 Flask-2.3.2/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:36:10.293284 Flask-2.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.261284 Flask-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.281284 Flask-2.3.2/src/Flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-01 15:36:10.000000 Flask-2.3.2/src/Flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-01 15:36:10.000000 Flask-2.3.2/src/Flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:36:10.000000 Flask-2.3.2/src/Flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 15:36:10.000000 Flask-2.3.2/src/Flask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 15:36:10.000000 Flask-2.3.2/src/Flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 15:36:10.000000 Flask-2.3.2/src/Flask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.285284 Flask-2.3.2/src/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87620 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33720 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/debughelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24957 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.285284 Flask-2.3.2/src/flask/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/json/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/json/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14169 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-01 15:35:58.000000 Flask-2.3.2/src/flask/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.285284 Flask-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/static/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/static/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/_macro.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/context_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/escaping_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/mail.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/templates/nested/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/nested/nested.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/non_escaping_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/simple_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/template_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/templates/template_test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_appctx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/.env
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/.flaskenv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/static/css/test.css
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/static/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.261284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/admin/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/frontend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.261284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/blueprintapp/apps/frontend/templates/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/blueprintapp/apps/frontend/templates/frontend/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/cliapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/importerrorapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/cliapp/inner1/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/inner1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/cliapp/inner1/inner2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/inner1/inner2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/inner1/inner2/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/message.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/cliapp/multiapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/helloworld/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/helloworld/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/subdomaintestmodule/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/subdomaintestmodule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.289284 Flask-2.3.2/tests/test_apps/subdomaintestmodule/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_apps/subdomaintestmodule/static/hello.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51654 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_instance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_json_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_reqctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_session_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_subclassing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_user_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:36:10.293284 Flask-2.3.2/tests/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/typing/typing_app_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/typing/typing_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-01 15:35:58.000000 Flask-2.3.2/tests/typing/typing_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-01 15:35:58.000000 Flask-2.3.2/tox.ini
```

### Comparing `Flask-2.3.1/CHANGES.rst` & `Flask-2.3.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 2.3.2
+-------------
+
+Released 2022-05-01
+
+-   Set ``Vary: Cookie`` header when the session is accessed, modified, or refreshed.
+-   Update Werkzeug requirement to >=2.3.3 to apply recent bug fixes.
+
+
 Version 2.3.1
 -------------
 
 Released 2023-04-25
 
 -   Restore deprecated ``from flask import Markup``. :issue:`5084`
```

### Comparing `Flask-2.3.1/CONTRIBUTING.rst` & `Flask-2.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/LICENSE.rst` & `Flask-2.3.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/PKG-INFO` & `Flask-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple framework for building complex web applications.
 Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 Maintainer-email: Pallets <contact@palletsprojects.com>
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Changes, https://flask.palletsprojects.com/changes/
```

### Comparing `Flask-2.3.1/README.rst` & `Flask-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/Makefile` & `Flask-2.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/_static/debugger.png` & `Flask-2.3.2/docs/_static/debugger.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/_static/flask-horizontal.png` & `Flask-2.3.2/docs/_static/flask-horizontal.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/_static/flask-vertical.png` & `Flask-2.3.2/docs/_static/flask-vertical.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/_static/pycharm-run-config.png` & `Flask-2.3.2/docs/_static/pycharm-run-config.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/_static/shortcut-icon.png` & `Flask-2.3.2/docs/_static/shortcut-icon.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/api.rst` & `Flask-2.3.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/appcontext.rst` & `Flask-2.3.2/docs/appcontext.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/async-await.rst` & `Flask-2.3.2/docs/async-await.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/blueprints.rst` & `Flask-2.3.2/docs/blueprints.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/cli.rst` & `Flask-2.3.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/conf.py` & `Flask-2.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/config.rst` & `Flask-2.3.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/debugging.rst` & `Flask-2.3.2/docs/debugging.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/apache-httpd.rst` & `Flask-2.3.2/docs/deploying/apache-httpd.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/asgi.rst` & `Flask-2.3.2/docs/deploying/asgi.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/eventlet.rst` & `Flask-2.3.2/docs/deploying/eventlet.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/gevent.rst` & `Flask-2.3.2/docs/deploying/gevent.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/gunicorn.rst` & `Flask-2.3.2/docs/deploying/gunicorn.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/index.rst` & `Flask-2.3.2/docs/deploying/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/mod_wsgi.rst` & `Flask-2.3.2/docs/deploying/mod_wsgi.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/nginx.rst` & `Flask-2.3.2/docs/deploying/nginx.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/proxy_fix.rst` & `Flask-2.3.2/docs/deploying/proxy_fix.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/uwsgi.rst` & `Flask-2.3.2/docs/deploying/uwsgi.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/deploying/waitress.rst` & `Flask-2.3.2/docs/deploying/waitress.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/design.rst` & `Flask-2.3.2/docs/design.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/errorhandling.rst` & `Flask-2.3.2/docs/errorhandling.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/extensiondev.rst` & `Flask-2.3.2/docs/extensiondev.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/extensions.rst` & `Flask-2.3.2/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/index.rst` & `Flask-2.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/installation.rst` & `Flask-2.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/lifecycle.rst` & `Flask-2.3.2/docs/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/logging.rst` & `Flask-2.3.2/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/make.bat` & `Flask-2.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/appdispatch.rst` & `Flask-2.3.2/docs/patterns/appdispatch.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/appfactories.rst` & `Flask-2.3.2/docs/patterns/appfactories.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/caching.rst` & `Flask-2.3.2/docs/patterns/caching.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/celery.rst` & `Flask-2.3.2/docs/patterns/celery.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/deferredcallbacks.rst` & `Flask-2.3.2/docs/patterns/deferredcallbacks.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/favicon.rst` & `Flask-2.3.2/docs/patterns/favicon.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/fileuploads.rst` & `Flask-2.3.2/docs/patterns/fileuploads.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/flashing.rst` & `Flask-2.3.2/docs/patterns/flashing.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/index.rst` & `Flask-2.3.2/docs/patterns/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/javascript.rst` & `Flask-2.3.2/docs/patterns/javascript.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/lazyloading.rst` & `Flask-2.3.2/docs/patterns/lazyloading.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/methodoverrides.rst` & `Flask-2.3.2/docs/patterns/methodoverrides.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/mongoengine.rst` & `Flask-2.3.2/docs/patterns/mongoengine.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/packages.rst` & `Flask-2.3.2/docs/patterns/packages.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/requestchecksum.rst` & `Flask-2.3.2/docs/patterns/requestchecksum.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/singlepageapplications.rst` & `Flask-2.3.2/docs/patterns/singlepageapplications.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/sqlalchemy.rst` & `Flask-2.3.2/docs/patterns/sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/sqlite3.rst` & `Flask-2.3.2/docs/patterns/sqlite3.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/streaming.rst` & `Flask-2.3.2/docs/patterns/streaming.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/subclassing.rst` & `Flask-2.3.2/docs/patterns/subclassing.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/templateinheritance.rst` & `Flask-2.3.2/docs/patterns/templateinheritance.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/urlprocessors.rst` & `Flask-2.3.2/docs/patterns/urlprocessors.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/viewdecorators.rst` & `Flask-2.3.2/docs/patterns/viewdecorators.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/patterns/wtforms.rst` & `Flask-2.3.2/docs/patterns/wtforms.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/quickstart.rst` & `Flask-2.3.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/reqcontext.rst` & `Flask-2.3.2/docs/reqcontext.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/security.rst` & `Flask-2.3.2/docs/security.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/server.rst` & `Flask-2.3.2/docs/server.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/shell.rst` & `Flask-2.3.2/docs/shell.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/signals.rst` & `Flask-2.3.2/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/templating.rst` & `Flask-2.3.2/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/testing.rst` & `Flask-2.3.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/blog.rst` & `Flask-2.3.2/docs/tutorial/blog.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/database.rst` & `Flask-2.3.2/docs/tutorial/database.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/deploy.rst` & `Flask-2.3.2/docs/tutorial/deploy.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/factory.rst` & `Flask-2.3.2/docs/tutorial/factory.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/flaskr_edit.png` & `Flask-2.3.2/docs/tutorial/flaskr_edit.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/flaskr_index.png` & `Flask-2.3.2/docs/tutorial/flaskr_index.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/flaskr_login.png` & `Flask-2.3.2/docs/tutorial/flaskr_login.png`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/index.rst` & `Flask-2.3.2/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/install.rst` & `Flask-2.3.2/docs/tutorial/install.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/layout.rst` & `Flask-2.3.2/docs/tutorial/layout.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/next.rst` & `Flask-2.3.2/docs/tutorial/next.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/static.rst` & `Flask-2.3.2/docs/tutorial/static.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/templates.rst` & `Flask-2.3.2/docs/tutorial/templates.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/tests.rst` & `Flask-2.3.2/docs/tutorial/tests.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/tutorial/views.rst` & `Flask-2.3.2/docs/tutorial/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/docs/views.rst` & `Flask-2.3.2/docs/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/celery/README.md` & `Flask-2.3.2/examples/celery/README.md`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/celery/requirements.txt` & `Flask-2.3.2/examples/celery/requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/celery/src/task_app/__init__.py` & `Flask-2.3.2/examples/celery/src/task_app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/celery/src/task_app/templates/index.html` & `Flask-2.3.2/examples/celery/src/task_app/templates/index.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/celery/src/task_app/views.py` & `Flask-2.3.2/examples/celery/src/task_app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/LICENSE.rst` & `Flask-2.3.2/examples/javascript/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/README.rst` & `Flask-2.3.2/examples/javascript/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/js_example/templates/base.html` & `Flask-2.3.2/examples/javascript/js_example/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/js_example/templates/fetch.html` & `Flask-2.3.2/examples/javascript/js_example/templates/fetch.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/js_example/templates/jquery.html` & `Flask-2.3.2/examples/javascript/js_example/templates/jquery.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/js_example/templates/xhr.html` & `Flask-2.3.2/examples/javascript/js_example/templates/xhr.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/pyproject.toml` & `Flask-2.3.2/examples/javascript/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/javascript/tests/test_js_example.py` & `Flask-2.3.2/examples/javascript/tests/test_js_example.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/LICENSE.rst` & `Flask-2.3.2/examples/tutorial/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/README.rst` & `Flask-2.3.2/examples/tutorial/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/__init__.py` & `Flask-2.3.2/examples/tutorial/flaskr/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/auth.py` & `Flask-2.3.2/examples/tutorial/flaskr/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/blog.py` & `Flask-2.3.2/examples/tutorial/flaskr/blog.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/db.py` & `Flask-2.3.2/examples/tutorial/flaskr/db.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/static/style.css` & `Flask-2.3.2/examples/tutorial/flaskr/static/style.css`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/templates/base.html` & `Flask-2.3.2/examples/tutorial/flaskr/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/templates/blog/index.html` & `Flask-2.3.2/examples/tutorial/flaskr/templates/blog/index.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/flaskr/templates/blog/update.html` & `Flask-2.3.2/examples/tutorial/flaskr/templates/blog/update.html`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/pyproject.toml` & `Flask-2.3.2/examples/tutorial/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/tests/conftest.py` & `Flask-2.3.2/examples/tutorial/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/tests/test_auth.py` & `Flask-2.3.2/examples/tutorial/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/tests/test_blog.py` & `Flask-2.3.2/examples/tutorial/tests/test_blog.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/examples/tutorial/tests/test_db.py` & `Flask-2.3.2/examples/tutorial/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/pyproject.toml` & `Flask-2.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Internet :: WWW/HTTP :: WSGI",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "Werkzeug>=2.3.0",
+    "Werkzeug>=2.3.3",
     "Jinja2>=3.1.2",
     "itsdangerous>=2.1.2",
     "click>=8.1.3",
     "blinker>=1.6.2",
     "importlib-metadata>=3.6.0; python_version < '3.10'",
 ]
 dynamic = ["version"]
```

### Comparing `Flask-2.3.1/requirements/dev.txt` & `Flask-2.3.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/requirements/docs.txt` & `Flask-2.3.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/requirements/tests-pallets-min.txt` & `Flask-2.3.2/requirements/tests-pallets-min.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SHA1:93a20a0c3518e8617dd501183caffc1364455d8d
+# SHA1:0b58503b99aabc227b7f39357216d676d9987a12
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 blinker==1.6.2
@@ -14,9 +14,9 @@
 jinja2==3.1.2
     # via -r requirements/tests-pallets-min.in
 markupsafe==2.1.1
     # via
     #   -r requirements/tests-pallets-min.in
     #   jinja2
     #   werkzeug
-werkzeug==2.3.0
+werkzeug==2.3.3
     # via -r requirements/tests-pallets-min.in
```

### Comparing `Flask-2.3.1/requirements/typing.txt` & `Flask-2.3.2/requirements/typing.txt`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/Flask.egg-info/PKG-INFO` & `Flask-2.3.2/src/Flask.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple framework for building complex web applications.
 Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 Maintainer-email: Pallets <contact@palletsprojects.com>
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Changes, https://flask.palletsprojects.com/changes/
```

### Comparing `Flask-2.3.1/src/Flask.egg-info/SOURCES.txt` & `Flask-2.3.2/src/Flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/__init__.py` & `Flask-2.3.2/src/flask/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .signals import request_tearing_down as request_tearing_down
 from .signals import template_rendered as template_rendered
 from .templating import render_template as render_template
 from .templating import render_template_string as render_template_string
 from .templating import stream_template as stream_template
 from .templating import stream_template_string as stream_template_string
 
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 
 
 def __getattr__(name):
     if name == "_app_ctx_stack":
         import warnings
         from .globals import __app_ctx_stack
```

### Comparing `Flask-2.3.1/src/flask/app.py` & `Flask-2.3.2/src/flask/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1848,15 +1848,15 @@
             if isinstance(status, (str, bytes, bytearray)):
                 rv.status = status
             else:
                 rv.status_code = status
 
         # extend existing headers with provided headers
         if headers:
-            rv.headers.update(headers)
+            rv.headers.update(headers)  # type: ignore[arg-type]
 
         return rv
 
     def create_url_adapter(self, request: Request | None) -> MapAdapter | None:
         """Creates a URL adapter for the given request. The URL adapter
         is created at a point where the request context is not yet set
         up so the request is passed explicitly.
```

### Comparing `Flask-2.3.1/src/flask/blueprints.py` & `Flask-2.3.2/src/flask/blueprints.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/cli.py` & `Flask-2.3.2/src/flask/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/config.py` & `Flask-2.3.2/src/flask/config.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/ctx.py` & `Flask-2.3.2/src/flask/ctx.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/debughelpers.py` & `Flask-2.3.2/src/flask/debughelpers.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/globals.py` & `Flask-2.3.2/src/flask/globals.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/helpers.py` & `Flask-2.3.2/src/flask/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/json/__init__.py` & `Flask-2.3.2/src/flask/json/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/json/provider.py` & `Flask-2.3.2/src/flask/json/provider.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/json/tag.py` & `Flask-2.3.2/src/flask/json/tag.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/logging.py` & `Flask-2.3.2/src/flask/logging.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/scaffold.py` & `Flask-2.3.2/src/flask/scaffold.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/sessions.py` & `Flask-2.3.2/src/flask/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,33 +325,34 @@
         name = self.get_cookie_name(app)
         domain = self.get_cookie_domain(app)
         path = self.get_cookie_path(app)
         secure = self.get_cookie_secure(app)
         samesite = self.get_cookie_samesite(app)
         httponly = self.get_cookie_httponly(app)
 
+        # Add a "Vary: Cookie" header if the session was accessed at all.
+        if session.accessed:
+            response.vary.add("Cookie")
+
         # If the session is modified to be empty, remove the cookie.
         # If the session is empty, return without setting the cookie.
         if not session:
             if session.modified:
                 response.delete_cookie(
                     name,
                     domain=domain,
                     path=path,
                     secure=secure,
                     samesite=samesite,
                     httponly=httponly,
                 )
+                response.vary.add("Cookie")
 
             return
 
-        # Add a "Vary: Cookie" header if the session was accessed at all.
-        if session.accessed:
-            response.vary.add("Cookie")
-
         if not self.should_set_cookie(app, session):
             return
 
         expires = self.get_expiration_time(app, session)
         val = self.get_signing_serializer(app).dumps(dict(session))  # type: ignore
         response.set_cookie(
             name,
@@ -359,7 +360,8 @@
             expires=expires,
             httponly=httponly,
             domain=domain,
             path=path,
             secure=secure,
             samesite=samesite,
         )
+        response.vary.add("Cookie")
```

### Comparing `Flask-2.3.1/src/flask/signals.py` & `Flask-2.3.2/src/flask/signals.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/templating.py` & `Flask-2.3.2/src/flask/templating.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/testing.py` & `Flask-2.3.2/src/flask/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,29 +134,22 @@
 
         Internally this is implemented by going through a temporary test
         request context and since session handling could depend on
         request variables this function accepts the same arguments as
         :meth:`~flask.Flask.test_request_context` which are directly
         passed through.
         """
-        # new cookie interface for Werkzeug >= 2.3
-        cookie_storage = self._cookies if hasattr(self, "_cookies") else self.cookie_jar
-
-        if cookie_storage is None:
+        if self._cookies is None:
             raise TypeError(
                 "Cookies are disabled. Create a client with 'use_cookies=True'."
             )
 
         app = self.application
         ctx = app.test_request_context(*args, **kwargs)
-
-        if hasattr(self, "_add_cookies_to_wsgi"):
-            self._add_cookies_to_wsgi(ctx.request.environ)
-        else:
-            self.cookie_jar.inject_wsgi(ctx.request.environ)  # type: ignore[union-attr]
+        self._add_cookies_to_wsgi(ctx.request.environ)
 
         with ctx:
             sess = app.session_interface.open_session(app, ctx.request)
 
         if sess is None:
             raise RuntimeError("Session backend did not open a session.")
 
@@ -165,22 +158,19 @@
 
         if app.session_interface.is_null_session(sess):
             return
 
         with ctx:
             app.session_interface.save_session(app, sess, resp)
 
-        if hasattr(self, "_update_cookies_from_response"):
-            self._update_cookies_from_response(
-                ctx.request.host.partition(":")[0], resp.headers.getlist("Set-Cookie")
-            )
-        else:
-            self.cookie_jar.extract_wsgi(  # type: ignore[union-attr]
-                ctx.request.environ, resp.headers
-            )
+        self._update_cookies_from_response(
+            ctx.request.host.partition(":")[0],
+            ctx.request.path,
+            resp.headers.getlist("Set-Cookie"),
+        )
 
     def _copy_environ(self, other):
         out = {**self.environ_base, **other}
 
         if self.preserve_context:
             out["werkzeug.debug.preserve_context"] = self._new_contexts.append
```

### Comparing `Flask-2.3.1/src/flask/typing.py` & `Flask-2.3.2/src/flask/typing.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/views.py` & `Flask-2.3.2/src/flask/views.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/src/flask/wrappers.py` & `Flask-2.3.2/src/flask/wrappers.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/conftest.py` & `Flask-2.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_appctx.py` & `Flask-2.3.2/tests/test_appctx.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_async.py` & `Flask-2.3.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_basic.py` & `Flask-2.3.2/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,14 +497,19 @@
     def getitem():
         return flask.session["test"]
 
     @app.route("/setdefault")
     def setdefault():
         return flask.session.setdefault("test", "default")
 
+    @app.route("/clear")
+    def clear():
+        flask.session.clear()
+        return ""
+
     @app.route("/vary-cookie-header-set")
     def vary_cookie_header_set():
         response = flask.Response()
         response.vary.add("Cookie")
         flask.session["test"] = "test"
         return response
 
@@ -529,19 +534,37 @@
         else:
             assert "Vary" not in rv.headers
 
     expect("/set")
     expect("/get")
     expect("/getitem")
     expect("/setdefault")
+    expect("/clear")
     expect("/vary-cookie-header-set")
     expect("/vary-header-set", "Accept-Encoding, Accept-Language, Cookie")
     expect("/no-vary-header", None)
 
 
+def test_session_refresh_vary(app, client):
+    @app.get("/login")
+    def login():
+        flask.session["user_id"] = 1
+        flask.session.permanent = True
+        return ""
+
+    @app.get("/ignored")
+    def ignored():
+        return ""
+
+    rv = client.get("/login")
+    assert rv.headers["Vary"] == "Cookie"
+    rv = client.get("/ignored")
+    assert rv.headers["Vary"] == "Cookie"
+
+
 def test_flashes(app, req_ctx):
     assert not flask.session.modified
     flask.flash("Zap")
     flask.session.modified = False
     flask.flash("Zip")
     assert flask.session.modified
     assert list(flask.get_flashed_messages()) == ["Zap", "Zip"]
```

### Comparing `Flask-2.3.1/tests/test_blueprints.py` & `Flask-2.3.2/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_cli.py` & `Flask-2.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_config.py` & `Flask-2.3.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_converters.py` & `Flask-2.3.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_helpers.py` & `Flask-2.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_instance_config.py` & `Flask-2.3.2/tests/test_instance_config.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_json.py` & `Flask-2.3.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_json_tag.py` & `Flask-2.3.2/tests/test_json_tag.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_logging.py` & `Flask-2.3.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_regression.py` & `Flask-2.3.2/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_reqctx.py` & `Flask-2.3.2/tests/test_reqctx.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_session_interface.py` & `Flask-2.3.2/tests/test_session_interface.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_signals.py` & `Flask-2.3.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_templating.py` & `Flask-2.3.2/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_testing.py` & `Flask-2.3.2/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_user_error_handler.py` & `Flask-2.3.2/tests/test_user_error_handler.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/test_views.py` & `Flask-2.3.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/typing/typing_app_decorators.py` & `Flask-2.3.2/tests/typing/typing_app_decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/typing/typing_error_handler.py` & `Flask-2.3.2/tests/typing/typing_error_handler.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tests/typing/typing_route.py` & `Flask-2.3.2/tests/typing/typing_route.py`

 * *Files identical despite different names*

### Comparing `Flask-2.3.1/tox.ini` & `Flask-2.3.2/tox.ini`

 * *Files identical despite different names*

