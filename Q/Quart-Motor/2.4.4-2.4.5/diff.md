# Comparing `tmp/Quart-Motor-2.4.4.tar.gz` & `tmp/Quart-Motor-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Quart-Motor-2.4.4.tar", last modified: Wed Jul  8 15:43:52 2020, max compression
+gzip compressed data, was "Quart-Motor-2.4.5.tar", last modified: Tue May  2 02:27:23 2023, max compression
```

## Comparing `Quart-Motor-2.4.4.tar` & `Quart-Motor-2.4.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2020-07-08 15:43:52.700531 Quart-Motor-2.4.4/
--rw-r--r--   0 sgp        (501) staff       (20)     9450 2020-07-08 15:43:52.700707 Quart-Motor-2.4.4/PKG-INFO
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2020-07-08 15:43:52.696547 Quart-Motor-2.4.4/Quart_Motor.egg-info/
--rw-r--r--   0 sgp        (501) staff       (20)     9450 2020-07-08 15:43:52.000000 Quart-Motor-2.4.4/Quart_Motor.egg-info/PKG-INFO
--rw-r--r--   0 sgp        (501) staff       (20)      445 2020-07-08 15:43:52.000000 Quart-Motor-2.4.4/Quart_Motor.egg-info/SOURCES.txt
--rw-r--r--   0 sgp        (501) staff       (20)        1 2020-07-08 15:43:52.000000 Quart-Motor-2.4.4/Quart_Motor.egg-info/dependency_links.txt
--rw-r--r--   0 sgp        (501) staff       (20)        1 2020-07-08 15:43:52.000000 Quart-Motor-2.4.4/Quart_Motor.egg-info/not-zip-safe
--rw-r--r--   0 sgp        (501) staff       (20)       45 2020-07-08 15:43:52.000000 Quart-Motor-2.4.4/Quart_Motor.egg-info/requires.txt
--rw-r--r--   0 sgp        (501) staff       (20)       18 2020-07-08 15:43:52.000000 Quart-Motor-2.4.4/Quart_Motor.egg-info/top_level.txt
--rw-r--r--   0 sgp        (501) staff       (20)     6746 2020-07-08 15:39:18.000000 Quart-Motor-2.4.4/README.md
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2020-07-08 15:43:52.697866 Quart-Motor-2.4.4/quart_motor/
--rw-r--r--   0 sgp        (501) staff       (20)     7171 2020-07-08 15:37:12.000000 Quart-Motor-2.4.4/quart_motor/__init__.py
--rw-r--r--   0 sgp        (501) staff       (20)     4393 2020-07-08 12:54:27.000000 Quart-Motor-2.4.4/quart_motor/helpers.py
--rw-r--r--   0 sgp        (501) staff       (20)     3181 2020-07-08 12:56:01.000000 Quart-Motor-2.4.4/quart_motor/wrappers.py
--rw-r--r--   0 sgp        (501) staff       (20)      162 2020-07-08 15:43:52.701098 Quart-Motor-2.4.4/setup.cfg
--rw-r--r--   0 sgp        (501) staff       (20)     1931 2020-07-08 15:38:04.000000 Quart-Motor-2.4.4/setup.py
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2020-07-08 15:43:52.698440 Quart-Motor-2.4.4/tests/
--rw-r--r--   0 sgp        (501) staff       (20)      156 2020-07-08 12:25:06.000000 Quart-Motor-2.4.4/tests/__init__.py
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2020-07-08 15:43:52.700063 Quart-Motor-2.4.4/tests/quart_motor_tests/
--rw-r--r--   0 sgp        (501) staff       (20)      144 2020-07-08 12:22:06.000000 Quart-Motor-2.4.4/tests/quart_motor_tests/__init__.py
--rw-r--r--   0 sgp        (501) staff       (20)     2866 2020-07-08 15:33:59.000000 Quart-Motor-2.4.4/tests/quart_motor_tests/test_connection.py
--rw-r--r--   0 sgp        (501) staff       (20)      912 2020-07-08 15:34:34.000000 Quart-Motor-2.4.4/tests/quart_motor_tests/test_wrappers.py
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.059043 Quart-Motor-2.4.5/
+-rw-r--r--   0 sgp        (501) staff       (20)     1389 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/LICENSE
+-rw-r--r--   0 sgp        (501) staff       (20)     7907 2023-05-02 02:27:23.059095 Quart-Motor-2.4.5/PKG-INFO
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058152 Quart-Motor-2.4.5/Quart_Motor.egg-info/
+-rw-r--r--   0 sgp        (501) staff       (20)     7907 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/PKG-INFO
+-rw-r--r--   0 sgp        (501) staff       (20)      453 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/SOURCES.txt
+-rw-r--r--   0 sgp        (501) staff       (20)        1 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/dependency_links.txt
+-rw-r--r--   0 sgp        (501) staff       (20)        1 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/not-zip-safe
+-rw-r--r--   0 sgp        (501) staff       (20)       54 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/requires.txt
+-rw-r--r--   0 sgp        (501) staff       (20)       18 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/top_level.txt
+-rw-r--r--   0 sgp        (501) staff       (20)     6940 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/README.md
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058479 Quart-Motor-2.4.5/quart_motor/
+-rw-r--r--   0 sgp        (501) staff       (20)     7189 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/quart_motor/__init__.py
+-rw-r--r--   0 sgp        (501) staff       (20)     4438 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/quart_motor/helpers.py
+-rw-r--r--   0 sgp        (501) staff       (20)     3181 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/quart_motor/wrappers.py
+-rw-r--r--   0 sgp        (501) staff       (20)      162 2023-05-02 02:27:23.059263 Quart-Motor-2.4.5/setup.cfg
+-rw-r--r--   0 sgp        (501) staff       (20)     2003 2023-05-02 02:25:03.000000 Quart-Motor-2.4.5/setup.py
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058597 Quart-Motor-2.4.5/tests/
+-rw-r--r--   0 sgp        (501) staff       (20)      158 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/__init__.py
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058933 Quart-Motor-2.4.5/tests/quart_motor_tests/
+-rw-r--r--   0 sgp        (501) staff       (20)      144 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/quart_motor_tests/__init__.py
+-rw-r--r--   0 sgp        (501) staff       (20)     2866 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/quart_motor_tests/test_connection.py
+-rw-r--r--   0 sgp        (501) staff       (20)      915 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/quart_motor_tests/test_wrappers.py
```

### Comparing `Quart-Motor-2.4.4/PKG-INFO` & `Quart-Motor-2.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,241 +1,243 @@
 Metadata-Version: 2.1
 Name: Quart-Motor
-Version: 2.4.4
+Version: 2.4.5
 Summary: Motor support for Quart applications
 Home-page: https://www.github.com/marirs/quart-motor/
+Download-URL: https://www.github.com/marirs/quart-motor/tags
 Author: Sriram G
 Author-email: marirs@gmail.com
 License: BSD
-Download-URL: https://www.github.com/marirs/quart-motor/tags
-Description: Quart-Motor
-        =============
-        [![Build Status](https://travis-ci.org/marirs/quart-motor.svg?branch=master)](https://travis-ci.org/marirs/quart-motor)
-        [![GitHub license](https://img.shields.io/badge/license-BSD%202-brightgreen)](https://github.com/marirs/quart-motor/blob/master/LICENSE)
-        
-        `MongoDB <http://www.mongodb.org/>` is an open source database that stores
-        flexible JSON-like "documents," which can have any number, name, or
-        hierarchy of fields within, instead of rows of data as in a relational
-        database. Python developers can think of MongoDB as a persistent, searchable
-        repository of Python dictionaries (and, in fact, this is how `PyMongo
-        <http://api.mongodb.org/python/current/>` represents MongoDB documents).
-        
-        Quart-Motor bridges Quart and Motor and provides some convenience
-        helpers.
-        
-        
-        Quickstart
-        ----------
-        
-        First, install Quart-Motor:
-        
-        ```bash
-        $ pip install Quart-Motor
-        ```
-        
-        Next, add a :class:`~quart_motor.Motor` to your code:
-        
-        ```python
-            from quart import Quart
-            from quart_motor import Motor
-        
-            app = Quart(__name__)
-            app.config["MONGO_URI"] = "mongodb://localhost:27017/myDatabase"
-            mongo = Motor(app)
-        ```
-        :class:`~quart_motor.Motor` connects to the MongoDB server running on
-        port 27017 on localhost, to the database named ``myDatabase``. This database
-        is exposed as the :attr:`~quart_motor.Motor.db` attribute.
-        
-        You can use :attr:`~quart_motor.Motor.db` directly in views:
-        
-        ```python
-        
-            @app.route("/")
-            def home_page():
-                online_users = mongo.db.users.find({"online": True})
-                return render_template("index.html",
-                    online_users=online_users)
-        ```
-        
-        Compatibility
-        -------------
-        
-        Quart-Motor depends on recent versions of Quart, Motor and PyMongo, where "recent"
-        is defined to mean "was released in the last 3 years". Quart-Motor *may*
-        work with older versions, but compatibility fixes for older versions will
-        not be accepted, and future changes may break compatibility in older
-        versions.
-        
-        Quart-Motor is tested against `supported versions
-        <https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
-        
-        Quart-Motor works very well with 
-        - `uvicorn` asgi 
-        - `hypercorn` asgi
-        
-        Quart-Motor is tested against `Python 3.7+` versions.
-        
-        Helpers
-        -------
-        
-        Quart-Motor provides helpers for some common tasks:
-        
-        .. automethod:: quart_motor.wrappers.Collection.find_one_or_404
-        
-        .. automethod:: quart_motor.Motor.send_file
-        
-        .. automethod:: quart_motor.Motor.save_file
-        
-        .. autoclass:: quart_motor.helpers.BSONObjectIdConverter
-        
-        .. autoclass:: quart_motor.helpers.JSONEncoder
-        
-        Configuration
-        -------------
-        
-        You can configure Quart-Motor either by passing a `MongoDB URI
-        <https://docs.mongodb.com/manual/reference/connection-string/>`_ to the
-        :class:`~quart_motor.Motor` constructor, or assigning it to the
-        ``MONGO_URI`` `Quart configuration variable
-        <https://pgjones.gitlab.io/quart/how_to_guides/configuration.html>`_
-        
-        The :class:`~quart_motor.Motor` instnace also accepts these additional
-        customization options:
-        
-        * ``json_options``, a :class:`~bson.json_util.JSONOptions` instance which
-          controls the JSON serialization of MongoDB objects when used with
-          :func:`~quart.json.jsonify`.
-        
-        You may also pass additional keyword arguments to the ``Motor``
-        constructor. These are passed directly through to the underlying
-        :class:`~motor.motor_asyncio.AsyncIOMotorClient` object.
-        
-        Note:
-        
-            By default, Quart-Motor sets the ``connect`` keyword argument to
-            ``False``, to prevent Motor from connecting immediately. Motor
-            itself `is not fork-safe
-            <http://api.mongodb.com/python/current/faq.html#is-pymongo-fork-safe>`_,
-            and delaying connection until the app is actually used is necessary to
-            avoid issues. If you wish to change this default behavior, pass
-            ``connect=True`` as a keyword argument to ``Motor``.
-        
-        You can create multiple ``Motor`` instances, to connect to multiple
-        databases or database servers:
-        
-        ```python
-        
-            app = Quart(__name__)
-        
-            # connect to MongoDB with the defaults
-            mongo1 = Motor(app, uri="mongodb://localhost:27017/databaseOne")
-        
-            # connect to another MongoDB database on the same host
-            mongo2 = Motor(app, uri="mongodb://localhost:27017/databaseTwo")
-        
-            # connect to another MongoDB server altogether
-            mongo3 = Motor(app, uri="mongodb://another.host:27017/databaseThree")
-        ```
-        Each instance is independent of the others and shares no state.
-        
-        
-        API
-        ===
-        
-        Classes
-        -------
-        
-        .. autoclass:: quart_motor.Motor
-           :members:
-        
-           .. attribute:: cx
-        
-              The :class:`~quart_motor.wrappers.AsyncIOMotorClient` connected to the
-              MongoDB server.
-        
-           .. attribute:: db
-        
-              The :class:`~quart_motor.wrappers.AsyncIOMotorDatabase` if the URI used
-              named a database, and ``None`` otherwise.
-        
-        
-        Wrappers
-        --------
-        
-        Quart-Motor wraps Motor's :class:`~motor.motor_asyncio.AsyncIOMotorClient`,
-        :class:`~motor.motor_asyncio.AsyncIOMotorDatabase`, and
-        :class:`~motor.motor_asyncio.AsyncIOMotorCollection` classes, and overrides their
-        attribute and item accessors. Wrapping the Motor classes in this way lets
-        Quart-Motor add methods to ``AsyncIOMotorCollection`` while allowing user code to use
-        MongoDB-style dotted expressions.
-        
-        ```python
-        
-            >>> type(mongo.cx)
-            <type 'quart_motor.wrappers.AsyncIOMotorClient'>
-            >>> type(mongo.db)
-            <type 'quart_motor.wrappers.AsyncIOMotorDatabase'>
-            >>> type(mongo.db.some_collection)
-            <type 'quart_motor.wrappers.AsyncIOMotorCollection'>
-        ```
-        .. autoclass:: quart_motor.wrappers.AsyncIOMotorCollection(...)
-           :members:
-        
-        
-        History and Contributors
-        ------------------------
-        
-        Changes:
-        
-        - 2.4.0: Unreleased
-        
-          - Flask-PyMongo port as released of Flask-PyMongo.
-        
-        Flask-PyMongo:
-        
-        - <https://github.com/dcrosta/flask-pymongo> 
-        
-        
-        Contributors of Flask-PyMongo:
-        
-        - `jeverling <https://github.com/jeverling>`
-        - `tang0th <https://github.com/tang0th>`
-        - `Fabrice Aneche <https://github.com/akhenakh>`
-        - `Thor Adam <https://github.com/thoradam>`
-        - `Christoph Herr <https://github.com/jarus>`
-        - `Mark Unsworth <https://github.com/markunsworth>`
-        - `Kevin Funk <https://github.com/k-funk>`
-        - `Ben Jeffrey <https://github.com/jeffbr13>`
-        - `Emmanuel Valette <https://github.com/karec>`
-        - `David Awad <https://github.com/DavidAwad>`
-        - `Robson Roberto Souza Peixoto <https://github.com/robsonpeixoto>`
-        - `juliascript <https://github.com/juliascript>`
-        - `Henrik Blidh <https://github.com/hbldh>`
-        - `jobou <https://github.com/jbouzekri>`
-        - `Craig Davis <https://github.com/blade2005>`
-        - `ratson <https://github.com/ratson>`
-        - `Abraham Toriz Cruz <https://github.com/categulario>`
-        - `MinJae Kwon <https://github.com/mingrammer>`
-        - `yarobob <https://github.com/yarobob>`
-        - `Andrew C. Hawkins <https://github.com/achawkins>`
-        
-        Contributors of Quart-Motor
-        
-        - `Sriram <https://github.com/marirs>`
-        - `Kiran <https://github.com/kirantambe>`
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Quart-Motor
+=============
+[![Build Status](https://travis-ci.org/marirs/quart-motor.svg?branch=master)](https://travis-ci.org/marirs/quart-motor)
+[![codecov](https://codecov.io/gh/marirs/quart-motor/branch/master/graph/badge.svg)](https://codecov.io/gh/marirs/quart-motor)
+[![GitHub license](https://img.shields.io/badge/license-BSD%203-brightgreen)](https://github.com/marirs/quart-motor/blob/master/LICENSE)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/Quart-Motor)
+
+`MongoDB <http://www.mongodb.org/>` is an open source database that stores
+flexible JSON-like "documents," which can have any number, name, or
+hierarchy of fields within, instead of rows of data as in a relational
+database. Python developers can think of MongoDB as a persistent, searchable
+repository of Python dictionaries (and, in fact, this is how `PyMongo
+<http://api.mongodb.org/python/current/>` represents MongoDB documents).
+
+Quart-Motor bridges Quart and Motor and provides some convenience
+helpers.
+
+
+Quickstart
+----------
+
+First, install Quart-Motor:
+
+```bash
+$ pip install Quart-Motor
+```
+
+Next, add a :class:`~quart_motor.Motor` to your code:
+
+```python
+    from quart import Quart
+    from quart_motor import Motor
+
+    app = Quart(__name__)
+    app.config["MONGO_URI"] = "mongodb://localhost:27017/myDatabase"
+    mongo = Motor(app)
+```
+:class:`~quart_motor.Motor` connects to the MongoDB server running on
+port 27017 on localhost, to the database named ``myDatabase``. This database
+is exposed as the :attr:`~quart_motor.Motor.db` attribute.
+
+You can use :attr:`~quart_motor.Motor.db` directly in views:
+
+```python
+
+    @app.route("/")
+    def home_page():
+        online_users = mongo.db.users.find({"online": True})
+        return render_template("index.html",
+            online_users=online_users)
+```
+
+Compatibility
+-------------
+
+Quart-Motor depends on recent versions of Quart, Motor and PyMongo, where "recent"
+is defined to mean "was released in the last 3 years". Quart-Motor *may*
+work with older versions, but compatibility fixes for older versions will
+not be accepted, and future changes may break compatibility in older
+versions.
+
+Quart-Motor is tested against `supported versions
+<https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
+
+Quart-Motor works very well with 
+- `uvicorn` asgi 
+- `hypercorn` asgi
+
+Quart-Motor is tested against `Python 3.7+` versions.
+
+Helpers
+-------
+
+Quart-Motor provides helpers for some common tasks:
+
+.. automethod:: quart_motor.wrappers.Collection.find_one_or_404
+
+.. automethod:: quart_motor.Motor.send_file
+
+.. automethod:: quart_motor.Motor.save_file
+
+.. autoclass:: quart_motor.helpers.BSONObjectIdConverter
+
+.. autoclass:: quart_motor.helpers.JSONEncoder
+
+Configuration
+-------------
+
+You can configure Quart-Motor either by passing a `MongoDB URI
+<https://docs.mongodb.com/manual/reference/connection-string/>`_ to the
+:class:`~quart_motor.Motor` constructor, or assigning it to the
+``MONGO_URI`` `Quart configuration variable
+<https://pgjones.gitlab.io/quart/how_to_guides/configuration.html>`_
+
+The :class:`~quart_motor.Motor` instnace also accepts these additional
+customization options:
+
+* ``json_options``, a :class:`~bson.json_util.JSONOptions` instance which
+  controls the JSON serialization of MongoDB objects when used with
+  :func:`~quart.json.jsonify`.
+
+You may also pass additional keyword arguments to the ``Motor``
+constructor. These are passed directly through to the underlying
+:class:`~motor.motor_asyncio.AsyncIOMotorClient` object.
+
+Note:
+
+    By default, Quart-Motor sets the ``connect`` keyword argument to
+    ``False``, to prevent Motor from connecting immediately. Motor
+    itself `is not fork-safe
+    <https://pymongo.readthedocs.io/en/stable/faq.html#is-pymongo-fork-safe>`_,
+    and delaying connection until the app is actually used is necessary to
+    avoid issues. If you wish to change this default behavior, pass
+    ``connect=True`` as a keyword argument to ``Motor``.
+
+You can create multiple ``Motor`` instances, to connect to multiple
+databases or database servers:
+
+```python
+
+    app = Quart(__name__)
+
+    # connect to MongoDB with the defaults
+    mongo1 = Motor(app, uri="mongodb://localhost:27017/databaseOne")
+
+    # connect to another MongoDB database on the same host
+    mongo2 = Motor(app, uri="mongodb://localhost:27017/databaseTwo")
+
+    # connect to another MongoDB server altogether
+    mongo3 = Motor(app, uri="mongodb://another.host:27017/databaseThree")
+```
+Each instance is independent of the others and shares no state.
+
+
+API
+===
+
+Classes
+-------
+
+.. autoclass:: quart_motor.Motor
+   :members:
+
+   .. attribute:: cx
+
+      The :class:`~quart_motor.wrappers.AsyncIOMotorClient` connected to the
+      MongoDB server.
+
+   .. attribute:: db
+
+      The :class:`~quart_motor.wrappers.AsyncIOMotorDatabase` if the URI used
+      named a database, and ``None`` otherwise.
+
+
+Wrappers
+--------
+
+Quart-Motor wraps Motor's :class:`~motor.motor_asyncio.AsyncIOMotorClient`,
+:class:`~motor.motor_asyncio.AsyncIOMotorDatabase`, and
+:class:`~motor.motor_asyncio.AsyncIOMotorCollection` classes, and overrides their
+attribute and item accessors. Wrapping the Motor classes in this way lets
+Quart-Motor add methods to ``AsyncIOMotorCollection`` while allowing user code to use
+MongoDB-style dotted expressions.
+
+```python
+
+    >>> type(mongo.cx)
+    <type 'quart_motor.wrappers.AsyncIOMotorClient'>
+    >>> type(mongo.db)
+    <type 'quart_motor.wrappers.AsyncIOMotorDatabase'>
+    >>> type(mongo.db.some_collection)
+    <type 'quart_motor.wrappers.AsyncIOMotorCollection'>
+```
+.. autoclass:: quart_motor.wrappers.AsyncIOMotorCollection(...)
+   :members:
+
+
+History and Contributors
+------------------------
+
+Changes:
+
+- 2.4.0: Unreleased
+
+  - Flask-PyMongo port as released of Flask-PyMongo.
+
+Flask-PyMongo:
+
+- <https://github.com/dcrosta/flask-pymongo> 
+
+
+Contributors of Flask-PyMongo:
+
+- `jeverling <https://github.com/jeverling>`
+- `tang0th <https://github.com/tang0th>`
+- `Fabrice Aneche <https://github.com/akhenakh>`
+- `Thor Adam <https://github.com/thoradam>`
+- `Christoph Herr <https://github.com/jarus>`
+- `Mark Unsworth <https://github.com/markunsworth>`
+- `Kevin Funk <https://github.com/k-funk>`
+- `Ben Jeffrey <https://github.com/jeffbr13>`
+- `Emmanuel Valette <https://github.com/karec>`
+- `David Awad <https://github.com/DavidAwad>`
+- `Robson Roberto Souza Peixoto <https://github.com/robsonpeixoto>`
+- `juliascript <https://github.com/juliascript>`
+- `Henrik Blidh <https://github.com/hbldh>`
+- `jobou <https://github.com/jbouzekri>`
+- `Craig Davis <https://github.com/blade2005>`
+- `ratson <https://github.com/ratson>`
+- `Abraham Toriz Cruz <https://github.com/categulario>`
+- `MinJae Kwon <https://github.com/mingrammer>`
+- `yarobob <https://github.com/yarobob>`
+- `Andrew C. Hawkins <https://github.com/achawkins>`
+
+Contributors of Quart-Motor
+
+- `Sriram <https://github.com/marirs>`
+- `Kiran <https://github.com/kirantambe>`
```

### Comparing `Quart-Motor-2.4.4/Quart_Motor.egg-info/PKG-INFO` & `Quart-Motor-2.4.5/Quart_Motor.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,241 +1,243 @@
 Metadata-Version: 2.1
 Name: Quart-Motor
-Version: 2.4.4
+Version: 2.4.5
 Summary: Motor support for Quart applications
 Home-page: https://www.github.com/marirs/quart-motor/
+Download-URL: https://www.github.com/marirs/quart-motor/tags
 Author: Sriram G
 Author-email: marirs@gmail.com
 License: BSD
-Download-URL: https://www.github.com/marirs/quart-motor/tags
-Description: Quart-Motor
-        =============
-        [![Build Status](https://travis-ci.org/marirs/quart-motor.svg?branch=master)](https://travis-ci.org/marirs/quart-motor)
-        [![GitHub license](https://img.shields.io/badge/license-BSD%202-brightgreen)](https://github.com/marirs/quart-motor/blob/master/LICENSE)
-        
-        `MongoDB <http://www.mongodb.org/>` is an open source database that stores
-        flexible JSON-like "documents," which can have any number, name, or
-        hierarchy of fields within, instead of rows of data as in a relational
-        database. Python developers can think of MongoDB as a persistent, searchable
-        repository of Python dictionaries (and, in fact, this is how `PyMongo
-        <http://api.mongodb.org/python/current/>` represents MongoDB documents).
-        
-        Quart-Motor bridges Quart and Motor and provides some convenience
-        helpers.
-        
-        
-        Quickstart
-        ----------
-        
-        First, install Quart-Motor:
-        
-        ```bash
-        $ pip install Quart-Motor
-        ```
-        
-        Next, add a :class:`~quart_motor.Motor` to your code:
-        
-        ```python
-            from quart import Quart
-            from quart_motor import Motor
-        
-            app = Quart(__name__)
-            app.config["MONGO_URI"] = "mongodb://localhost:27017/myDatabase"
-            mongo = Motor(app)
-        ```
-        :class:`~quart_motor.Motor` connects to the MongoDB server running on
-        port 27017 on localhost, to the database named ``myDatabase``. This database
-        is exposed as the :attr:`~quart_motor.Motor.db` attribute.
-        
-        You can use :attr:`~quart_motor.Motor.db` directly in views:
-        
-        ```python
-        
-            @app.route("/")
-            def home_page():
-                online_users = mongo.db.users.find({"online": True})
-                return render_template("index.html",
-                    online_users=online_users)
-        ```
-        
-        Compatibility
-        -------------
-        
-        Quart-Motor depends on recent versions of Quart, Motor and PyMongo, where "recent"
-        is defined to mean "was released in the last 3 years". Quart-Motor *may*
-        work with older versions, but compatibility fixes for older versions will
-        not be accepted, and future changes may break compatibility in older
-        versions.
-        
-        Quart-Motor is tested against `supported versions
-        <https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
-        
-        Quart-Motor works very well with 
-        - `uvicorn` asgi 
-        - `hypercorn` asgi
-        
-        Quart-Motor is tested against `Python 3.7+` versions.
-        
-        Helpers
-        -------
-        
-        Quart-Motor provides helpers for some common tasks:
-        
-        .. automethod:: quart_motor.wrappers.Collection.find_one_or_404
-        
-        .. automethod:: quart_motor.Motor.send_file
-        
-        .. automethod:: quart_motor.Motor.save_file
-        
-        .. autoclass:: quart_motor.helpers.BSONObjectIdConverter
-        
-        .. autoclass:: quart_motor.helpers.JSONEncoder
-        
-        Configuration
-        -------------
-        
-        You can configure Quart-Motor either by passing a `MongoDB URI
-        <https://docs.mongodb.com/manual/reference/connection-string/>`_ to the
-        :class:`~quart_motor.Motor` constructor, or assigning it to the
-        ``MONGO_URI`` `Quart configuration variable
-        <https://pgjones.gitlab.io/quart/how_to_guides/configuration.html>`_
-        
-        The :class:`~quart_motor.Motor` instnace also accepts these additional
-        customization options:
-        
-        * ``json_options``, a :class:`~bson.json_util.JSONOptions` instance which
-          controls the JSON serialization of MongoDB objects when used with
-          :func:`~quart.json.jsonify`.
-        
-        You may also pass additional keyword arguments to the ``Motor``
-        constructor. These are passed directly through to the underlying
-        :class:`~motor.motor_asyncio.AsyncIOMotorClient` object.
-        
-        Note:
-        
-            By default, Quart-Motor sets the ``connect`` keyword argument to
-            ``False``, to prevent Motor from connecting immediately. Motor
-            itself `is not fork-safe
-            <http://api.mongodb.com/python/current/faq.html#is-pymongo-fork-safe>`_,
-            and delaying connection until the app is actually used is necessary to
-            avoid issues. If you wish to change this default behavior, pass
-            ``connect=True`` as a keyword argument to ``Motor``.
-        
-        You can create multiple ``Motor`` instances, to connect to multiple
-        databases or database servers:
-        
-        ```python
-        
-            app = Quart(__name__)
-        
-            # connect to MongoDB with the defaults
-            mongo1 = Motor(app, uri="mongodb://localhost:27017/databaseOne")
-        
-            # connect to another MongoDB database on the same host
-            mongo2 = Motor(app, uri="mongodb://localhost:27017/databaseTwo")
-        
-            # connect to another MongoDB server altogether
-            mongo3 = Motor(app, uri="mongodb://another.host:27017/databaseThree")
-        ```
-        Each instance is independent of the others and shares no state.
-        
-        
-        API
-        ===
-        
-        Classes
-        -------
-        
-        .. autoclass:: quart_motor.Motor
-           :members:
-        
-           .. attribute:: cx
-        
-              The :class:`~quart_motor.wrappers.AsyncIOMotorClient` connected to the
-              MongoDB server.
-        
-           .. attribute:: db
-        
-              The :class:`~quart_motor.wrappers.AsyncIOMotorDatabase` if the URI used
-              named a database, and ``None`` otherwise.
-        
-        
-        Wrappers
-        --------
-        
-        Quart-Motor wraps Motor's :class:`~motor.motor_asyncio.AsyncIOMotorClient`,
-        :class:`~motor.motor_asyncio.AsyncIOMotorDatabase`, and
-        :class:`~motor.motor_asyncio.AsyncIOMotorCollection` classes, and overrides their
-        attribute and item accessors. Wrapping the Motor classes in this way lets
-        Quart-Motor add methods to ``AsyncIOMotorCollection`` while allowing user code to use
-        MongoDB-style dotted expressions.
-        
-        ```python
-        
-            >>> type(mongo.cx)
-            <type 'quart_motor.wrappers.AsyncIOMotorClient'>
-            >>> type(mongo.db)
-            <type 'quart_motor.wrappers.AsyncIOMotorDatabase'>
-            >>> type(mongo.db.some_collection)
-            <type 'quart_motor.wrappers.AsyncIOMotorCollection'>
-        ```
-        .. autoclass:: quart_motor.wrappers.AsyncIOMotorCollection(...)
-           :members:
-        
-        
-        History and Contributors
-        ------------------------
-        
-        Changes:
-        
-        - 2.4.0: Unreleased
-        
-          - Flask-PyMongo port as released of Flask-PyMongo.
-        
-        Flask-PyMongo:
-        
-        - <https://github.com/dcrosta/flask-pymongo> 
-        
-        
-        Contributors of Flask-PyMongo:
-        
-        - `jeverling <https://github.com/jeverling>`
-        - `tang0th <https://github.com/tang0th>`
-        - `Fabrice Aneche <https://github.com/akhenakh>`
-        - `Thor Adam <https://github.com/thoradam>`
-        - `Christoph Herr <https://github.com/jarus>`
-        - `Mark Unsworth <https://github.com/markunsworth>`
-        - `Kevin Funk <https://github.com/k-funk>`
-        - `Ben Jeffrey <https://github.com/jeffbr13>`
-        - `Emmanuel Valette <https://github.com/karec>`
-        - `David Awad <https://github.com/DavidAwad>`
-        - `Robson Roberto Souza Peixoto <https://github.com/robsonpeixoto>`
-        - `juliascript <https://github.com/juliascript>`
-        - `Henrik Blidh <https://github.com/hbldh>`
-        - `jobou <https://github.com/jbouzekri>`
-        - `Craig Davis <https://github.com/blade2005>`
-        - `ratson <https://github.com/ratson>`
-        - `Abraham Toriz Cruz <https://github.com/categulario>`
-        - `MinJae Kwon <https://github.com/mingrammer>`
-        - `yarobob <https://github.com/yarobob>`
-        - `Andrew C. Hawkins <https://github.com/achawkins>`
-        
-        Contributors of Quart-Motor
-        
-        - `Sriram <https://github.com/marirs>`
-        - `Kiran <https://github.com/kirantambe>`
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Quart-Motor
+=============
+[![Build Status](https://travis-ci.org/marirs/quart-motor.svg?branch=master)](https://travis-ci.org/marirs/quart-motor)
+[![codecov](https://codecov.io/gh/marirs/quart-motor/branch/master/graph/badge.svg)](https://codecov.io/gh/marirs/quart-motor)
+[![GitHub license](https://img.shields.io/badge/license-BSD%203-brightgreen)](https://github.com/marirs/quart-motor/blob/master/LICENSE)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/Quart-Motor)
+
+`MongoDB <http://www.mongodb.org/>` is an open source database that stores
+flexible JSON-like "documents," which can have any number, name, or
+hierarchy of fields within, instead of rows of data as in a relational
+database. Python developers can think of MongoDB as a persistent, searchable
+repository of Python dictionaries (and, in fact, this is how `PyMongo
+<http://api.mongodb.org/python/current/>` represents MongoDB documents).
+
+Quart-Motor bridges Quart and Motor and provides some convenience
+helpers.
+
+
+Quickstart
+----------
+
+First, install Quart-Motor:
+
+```bash
+$ pip install Quart-Motor
+```
+
+Next, add a :class:`~quart_motor.Motor` to your code:
+
+```python
+    from quart import Quart
+    from quart_motor import Motor
+
+    app = Quart(__name__)
+    app.config["MONGO_URI"] = "mongodb://localhost:27017/myDatabase"
+    mongo = Motor(app)
+```
+:class:`~quart_motor.Motor` connects to the MongoDB server running on
+port 27017 on localhost, to the database named ``myDatabase``. This database
+is exposed as the :attr:`~quart_motor.Motor.db` attribute.
+
+You can use :attr:`~quart_motor.Motor.db` directly in views:
+
+```python
+
+    @app.route("/")
+    def home_page():
+        online_users = mongo.db.users.find({"online": True})
+        return render_template("index.html",
+            online_users=online_users)
+```
+
+Compatibility
+-------------
+
+Quart-Motor depends on recent versions of Quart, Motor and PyMongo, where "recent"
+is defined to mean "was released in the last 3 years". Quart-Motor *may*
+work with older versions, but compatibility fixes for older versions will
+not be accepted, and future changes may break compatibility in older
+versions.
+
+Quart-Motor is tested against `supported versions
+<https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
+
+Quart-Motor works very well with 
+- `uvicorn` asgi 
+- `hypercorn` asgi
+
+Quart-Motor is tested against `Python 3.7+` versions.
+
+Helpers
+-------
+
+Quart-Motor provides helpers for some common tasks:
+
+.. automethod:: quart_motor.wrappers.Collection.find_one_or_404
+
+.. automethod:: quart_motor.Motor.send_file
+
+.. automethod:: quart_motor.Motor.save_file
+
+.. autoclass:: quart_motor.helpers.BSONObjectIdConverter
+
+.. autoclass:: quart_motor.helpers.JSONEncoder
+
+Configuration
+-------------
+
+You can configure Quart-Motor either by passing a `MongoDB URI
+<https://docs.mongodb.com/manual/reference/connection-string/>`_ to the
+:class:`~quart_motor.Motor` constructor, or assigning it to the
+``MONGO_URI`` `Quart configuration variable
+<https://pgjones.gitlab.io/quart/how_to_guides/configuration.html>`_
+
+The :class:`~quart_motor.Motor` instnace also accepts these additional
+customization options:
+
+* ``json_options``, a :class:`~bson.json_util.JSONOptions` instance which
+  controls the JSON serialization of MongoDB objects when used with
+  :func:`~quart.json.jsonify`.
+
+You may also pass additional keyword arguments to the ``Motor``
+constructor. These are passed directly through to the underlying
+:class:`~motor.motor_asyncio.AsyncIOMotorClient` object.
+
+Note:
+
+    By default, Quart-Motor sets the ``connect`` keyword argument to
+    ``False``, to prevent Motor from connecting immediately. Motor
+    itself `is not fork-safe
+    <https://pymongo.readthedocs.io/en/stable/faq.html#is-pymongo-fork-safe>`_,
+    and delaying connection until the app is actually used is necessary to
+    avoid issues. If you wish to change this default behavior, pass
+    ``connect=True`` as a keyword argument to ``Motor``.
+
+You can create multiple ``Motor`` instances, to connect to multiple
+databases or database servers:
+
+```python
+
+    app = Quart(__name__)
+
+    # connect to MongoDB with the defaults
+    mongo1 = Motor(app, uri="mongodb://localhost:27017/databaseOne")
+
+    # connect to another MongoDB database on the same host
+    mongo2 = Motor(app, uri="mongodb://localhost:27017/databaseTwo")
+
+    # connect to another MongoDB server altogether
+    mongo3 = Motor(app, uri="mongodb://another.host:27017/databaseThree")
+```
+Each instance is independent of the others and shares no state.
+
+
+API
+===
+
+Classes
+-------
+
+.. autoclass:: quart_motor.Motor
+   :members:
+
+   .. attribute:: cx
+
+      The :class:`~quart_motor.wrappers.AsyncIOMotorClient` connected to the
+      MongoDB server.
+
+   .. attribute:: db
+
+      The :class:`~quart_motor.wrappers.AsyncIOMotorDatabase` if the URI used
+      named a database, and ``None`` otherwise.
+
+
+Wrappers
+--------
+
+Quart-Motor wraps Motor's :class:`~motor.motor_asyncio.AsyncIOMotorClient`,
+:class:`~motor.motor_asyncio.AsyncIOMotorDatabase`, and
+:class:`~motor.motor_asyncio.AsyncIOMotorCollection` classes, and overrides their
+attribute and item accessors. Wrapping the Motor classes in this way lets
+Quart-Motor add methods to ``AsyncIOMotorCollection`` while allowing user code to use
+MongoDB-style dotted expressions.
+
+```python
+
+    >>> type(mongo.cx)
+    <type 'quart_motor.wrappers.AsyncIOMotorClient'>
+    >>> type(mongo.db)
+    <type 'quart_motor.wrappers.AsyncIOMotorDatabase'>
+    >>> type(mongo.db.some_collection)
+    <type 'quart_motor.wrappers.AsyncIOMotorCollection'>
+```
+.. autoclass:: quart_motor.wrappers.AsyncIOMotorCollection(...)
+   :members:
+
+
+History and Contributors
+------------------------
+
+Changes:
+
+- 2.4.0: Unreleased
+
+  - Flask-PyMongo port as released of Flask-PyMongo.
+
+Flask-PyMongo:
+
+- <https://github.com/dcrosta/flask-pymongo> 
+
+
+Contributors of Flask-PyMongo:
+
+- `jeverling <https://github.com/jeverling>`
+- `tang0th <https://github.com/tang0th>`
+- `Fabrice Aneche <https://github.com/akhenakh>`
+- `Thor Adam <https://github.com/thoradam>`
+- `Christoph Herr <https://github.com/jarus>`
+- `Mark Unsworth <https://github.com/markunsworth>`
+- `Kevin Funk <https://github.com/k-funk>`
+- `Ben Jeffrey <https://github.com/jeffbr13>`
+- `Emmanuel Valette <https://github.com/karec>`
+- `David Awad <https://github.com/DavidAwad>`
+- `Robson Roberto Souza Peixoto <https://github.com/robsonpeixoto>`
+- `juliascript <https://github.com/juliascript>`
+- `Henrik Blidh <https://github.com/hbldh>`
+- `jobou <https://github.com/jbouzekri>`
+- `Craig Davis <https://github.com/blade2005>`
+- `ratson <https://github.com/ratson>`
+- `Abraham Toriz Cruz <https://github.com/categulario>`
+- `MinJae Kwon <https://github.com/mingrammer>`
+- `yarobob <https://github.com/yarobob>`
+- `Andrew C. Hawkins <https://github.com/achawkins>`
+
+Contributors of Quart-Motor
+
+- `Sriram <https://github.com/marirs>`
+- `Kiran <https://github.com/kirantambe>`
```

### Comparing `Quart-Motor-2.4.4/README.md` & `Quart-Motor-2.4.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Quart-Motor
 =============
 [![Build Status](https://travis-ci.org/marirs/quart-motor.svg?branch=master)](https://travis-ci.org/marirs/quart-motor)
-[![GitHub license](https://img.shields.io/badge/license-BSD%202-brightgreen)](https://github.com/marirs/quart-motor/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/marirs/quart-motor/branch/master/graph/badge.svg)](https://codecov.io/gh/marirs/quart-motor)
+[![GitHub license](https://img.shields.io/badge/license-BSD%203-brightgreen)](https://github.com/marirs/quart-motor/blob/master/LICENSE)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/Quart-Motor)
 
 `MongoDB <http://www.mongodb.org/>` is an open source database that stores
 flexible JSON-like "documents," which can have any number, name, or
 hierarchy of fields within, instead of rows of data as in a relational
 database. Python developers can think of MongoDB as a persistent, searchable
 repository of Python dictionaries (and, in fact, this is how `PyMongo
 <http://api.mongodb.org/python/current/>` represents MongoDB documents).
@@ -102,15 +104,15 @@
 :class:`~motor.motor_asyncio.AsyncIOMotorClient` object.
 
 Note:
 
     By default, Quart-Motor sets the ``connect`` keyword argument to
     ``False``, to prevent Motor from connecting immediately. Motor
     itself `is not fork-safe
-    <http://api.mongodb.com/python/current/faq.html#is-pymongo-fork-safe>`_,
+    <https://pymongo.readthedocs.io/en/stable/faq.html#is-pymongo-fork-safe>`_,
     and delaying connection until the app is actually used is necessary to
     avoid issues. If you wish to change this default behavior, pass
     ``connect=True`` as a keyword argument to ``Motor``.
 
 You can create multiple ``Motor`` instances, to connect to multiple
 databases or database servers:
```

### Comparing `Quart-Motor-2.4.4/quart_motor/__init__.py` & `Quart-Motor-2.4.5/quart_motor/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import asyncio
 
 import pymongo
 from functools import partial
 from mimetypes import guess_type
 import sys
 
-from quart import abort, current_app, request
+from quart import abort, current_app, request, Quart
 from gridfs import GridFS, NoFile
 from pymongo import uri_parser
 from werkzeug.wsgi import wrap_file
 
 from quart_motor.helpers import BSONObjectIdConverter, JSONEncoder
 from quart_motor.wrappers import AsyncIOMotorClient
 
@@ -55,15 +55,15 @@
         self.cx = None
         self.db = None
         self._json_encoder = partial(JSONEncoder, json_options=json_options)
 
         if app is not None:
             self.init_app(app, uri, *args, **kwargs)
 
-    def init_app(self, app, uri=None, *args, **kwargs):
+    def init_app(self, app: Quart, uri=None, *args, **kwargs):
         """Initialize this :class:`Motor` for use.
 
         Configure a :class:`~motor_async.AsyncIOMotorClient`
         in the following scenarios:
         1. If ``uri`` is not ``None``, pass the ``uri`` and any positional
            or keyword arguments to :class:`~motor_async.AsyncIOMotorClient`
         2. If ``uri`` is ``None``, and a Quart config variable named
@@ -92,21 +92,21 @@
                 "You must specify a URI or set the MONGO_URI Quart config variable",
             )
 
         parsed_uri = uri_parser.parse_uri(uri)
         database_name = parsed_uri["database"]
 
         # Try to delay connecting, in case the app is loaded before forking, per
-        # http://api.mongodb.com/python/current/faq.html#is-pymongo-fork-safe
+        # https://pymongo.readthedocs.io/en/stable/faq.html#is-pymongo-fork-safe
         kwargs.setdefault("connect", False)
 
         app.before_serving(_before_serving)
 
         app.url_map.converters["ObjectId"] = BSONObjectIdConverter
-        app.json_encoder = self._json_encoder
+        app.json = self._json_encoder(app=app)
 
     # view helpers
     def send_file(self, filename, base="fs", version=-1, cache_for=31536000):
         """Respond with a file from GridFS.
 
         Returns an instance of the :attr:`~quart.Quart.response_class`
         containing the named file, and implement conditional GET semantics
```

### Comparing `Quart-Motor-2.4.4/quart_motor/helpers.py` & `Quart-Motor-2.4.5/quart_motor/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Helpers."""
 from bson import json_util, SON
 from bson.errors import InvalidId
 from bson.objectid import ObjectId
-from quart import abort, json as quart_json
+from quart import abort, json as quart_json, Quart
 from six import iteritems, string_types
 from werkzeug.routing import BaseConverter
 import pymongo
 
 __all__ = ["BSONObjectIdConverter", "JSONEncoder"]
 
 
@@ -52,15 +52,15 @@
             raise abort(404)
 
     def to_url(self, value):
         """to_url."""
         return str(value)
 
 
-class JSONEncoder(quart_json.JSONEncoder):
+class JSONEncoder(quart_json.provider.DefaultJSONProvider):
     """A JSON encoder that uses :mod:`bson.json_util` for MongoDB documents.
 
     .. code-block:: python
         @app.route("/cart/<ObjectId:cart_id>")
         def json_route(cart_id):
             results = mongo.db.carts.find({"_id": cart_id})
             return jsonify(results)
@@ -80,24 +80,24 @@
         :class:`~bson.json_util.JSONOptions` is only supported as of
         PyMongo version 3.4. For older versions of PyMongo, you will
         have less control over the JSON format that results from calls
         to :func:`~Quart.json.jsonify`.
     .. versionadded:: 2.4.0
     """
 
-    def __init__(self, json_options, *args, **kwargs):
+    def __init__(self, app: Quart, json_options, *args, **kwargs):
         """__init__."""
         if json_options is None:
             json_options = DEFAULT_JSON_OPTIONS
         if json_options is not None:
             self._default_kwargs = {"json_options": json_options}
         else:
             self._default_kwargs = {}
 
-        super(JSONEncoder, self).__init__(*args, **kwargs)
+        super(JSONEncoder, self).__init__(app=app, *args, **kwargs)
 
     def default(self, obj):
         """Serialize MongoDB object types using :mod:`bson.json_util`.
 
         Falls back to Quart's default JSON serialization for all other types.
         This may raise ``TypeError`` for object types not recognized.
         .. version-added:: 2.4.0
```

### Comparing `Quart-Motor-2.4.4/quart_motor/wrappers.py` & `Quart-Motor-2.4.5/quart_motor/wrappers.py`

 * *Files identical despite different names*

### Comparing `Quart-Motor-2.4.4/setup.py` & `Quart-Motor-2.4.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 """
 
 from setuptools import find_packages, setup
 
 tests_require = [
     'coverage>=4.5',
     'coveralls>=1.8',
+    'codecov>=2.1.7',
     'pytest>=5.2',
     'pytest-cov>=2.8',
+    'pytest-asyncio>=0.14.0',
     'pytest-pep8>=1.0',
     'pydocstyle>=4.0',
 ]
 
 extras_require = {
     'tests': tests_require,
 }
@@ -32,30 +34,31 @@
 ]
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="Quart-Motor",
-    version='2.4.4',
+    version='2.4.5',
     url="https://www.github.com/marirs/quart-motor/",
     download_url="https://www.github.com/marirs/quart-motor/tags",
     license="BSD",
     author="Sriram G",
     author_email="marirs@gmail.com",
     description="Motor support for Quart applications",
     long_description=long_description,
     long_description_content_type='text/markdown',
     zip_safe=False,
     packages=find_packages(),
     install_requires=[
         "PyMongo>=3.10",
-        "Quart>=0.12.0",
+        "Quart>=0.18.0",
         "motor>=2.1.0",
         "six",
+        "werkzeug"
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
@@ -64,8 +67,8 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
     python_requires='>=3.6',
-)
+)
```

### Comparing `Quart-Motor-2.4.4/tests/quart_motor_tests/test_connection.py` & `Quart-Motor-2.4.5/tests/quart_motor_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `Quart-Motor-2.4.4/tests/quart_motor_tests/test_wrappers.py` & `Quart-Motor-2.4.5/tests/quart_motor_tests/test_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from quart import Quart
-from quart.exceptions import NotFound
+from werkzeug.exceptions import NotFound
 
 from quart_motor import Motor
 
 
 class TestCollection:
     uri = f"mongodb://localhost:27017/test"
```

