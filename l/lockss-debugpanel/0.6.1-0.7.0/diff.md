# Comparing `tmp/lockss_debugpanel-0.6.1.tar.gz` & `tmp/lockss_debugpanel-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_debugpanel-0.6.1.tar", max compression
+gzip compressed data, was "lockss_debugpanel-0.7.0.tar", max compression
```

## Comparing `lockss_debugpanel-0.6.1.tar` & `lockss_debugpanel-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      564 2023-03-16 21:33:51.679186 lockss_debugpanel-0.6.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-14 16:04:54.653141 lockss_debugpanel-0.6.1/LICENSE
--rw-r--r--   0        0        0    36004 2023-03-16 21:31:46.438886 lockss_debugpanel-0.6.1/README.rst
--rw-r--r--   0        0        0      928 2023-03-16 21:31:51.748899 lockss_debugpanel-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5673 2023-03-16 21:31:35.055525 lockss_debugpanel-0.6.1/src/lockss/debugpanel/__init__.py
--rw-r--r--   0        0        0     1639 2023-03-14 16:04:54.653141 lockss_debugpanel-0.6.1/src/lockss/debugpanel/__main__.py
--rw-r--r--   0        0        0    19111 2023-03-16 21:34:06.329221 lockss_debugpanel-0.6.1/src/lockss/debugpanel/cli.py
--rw-r--r--   0        0        0    37079 1970-01-01 00:00:00.000000 lockss_debugpanel-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-03-14 16:04:54.653141 lockss_debugpanel-0.7.0/LICENSE
+-rw-r--r--   0        0        0    37646 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/README.rst
+-rw-r--r--   0        0        0      947 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5673 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/src/lockss/debugpanel/__init__.py
+-rw-r--r--   0        0        0     1639 2023-03-14 16:04:54.653141 lockss_debugpanel-0.7.0/src/lockss/debugpanel/__main__.py
+-rw-r--r--   0        0        0    20145 2023-05-02 07:40:55.864231 lockss_debugpanel-0.7.0/src/lockss/debugpanel/cli.py
+-rw-r--r--   0        0        0    38761 1970-01-01 00:00:00.000000 lockss_debugpanel-0.7.0/PKG-INFO
```

### Comparing `lockss_debugpanel-0.6.1/LICENSE` & `lockss_debugpanel-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_debugpanel-0.6.1/README.rst` & `lockss_debugpanel-0.7.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,154 @@
 ==========
 Debugpanel
 ==========
 
+.. |RELEASE| replace:: 0.7.0
+.. |RELEASE_DATE| replace:: 2023-05-02
+
 .. |AUID| replace:: ``--auid/-a``
 .. |AUIDS| replace:: ``--auids/-A``
 .. |HELP| replace:: ``--help/-h``
 .. |NODE| replace:: ``--node/-n``
 .. |NODES| replace:: ``--nodes/-N``
 
 Debugpanel is a library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet.
 
-**Latest release:** 0.6.1 (2023-03-16)
+**Latest release:** |RELEASE| (|RELEASE_DATE|)
 
--------------
-Prerequisites
--------------
+-----------------
+Table of Contents
+-----------------
 
-*  `Python <https://www.python.org/>`_ 3.7 or greater.
+*  `Installation`_
 
-Prerequisites for development work only:
+   *  `Prerequisites`_
 
-*  `Poetry <https://python-poetry.org/>`_ 1.4 or greater.
+   *  `pip`_
 
-------------
-Installation
-------------
+*  `Overview`_
 
-Debugpanel is available from the `Python Package Index <https://pypi.org/>`_ (PyPI) as ``lockss-debugpanel``: https://pypi.org/project/lockss-debugpanel
+   * `Per-Node Operations`_
 
-You can install it with ``pip``. To install it in a virtual environment, simply use::
+   * `Per-AU Operations`_
 
-   pip3 install lockss-debugpanel
+*  `Command Line Tool`_
 
-To install it in your own non-root, non-virtual environment, use the ``--user`` option::
+   * `Synopsis`_
 
-   pip3 install --user lockss-debugpanel
+   * `Commands`_
 
-.. danger::
+      * `Top-Level Program`_
 
-   Do not run ``pip3``/``pip`` as ``root``, with ``sudo`` or otherwise.
+      *  `check-substance`_
 
-The installation process adds a ``lockss.debugpanel`` `Library`_ and a ``debugpanel`` `Command Line Tool`_. You can check at the command line that the installation is functional by running ``debugpanel version`` or ``debugpanel --help``.
+      *  `copyright`_
 
---------
-Overview
---------
+      *  `crawl`_
 
-Per-Node Operations
-===================
+      *  `crawl-plugins`_
 
-You can use Debugpanel to get LOCKSS nodes to:
+      *  `deep-crawl`_
 
-*  Reload their configuration (`reload-config`_ command, ``lockss.debugpanel.reload_config()`` function).
+      *  `disable-indexing`_
 
-*  Crawl their plugins (`crawl-plugins`_ command, ``lockss.debugpanel.crawl_plugins()`` function).
+      *  `license`_
 
-Per-AU Operations
-=================
+      *  `poll`_
 
-You can use Debugpanel to get LOCKSS nodes to perform an operation on AUs identified by AUID, namely:
+      *  `reindex-metadata`_
 
-*  Crawl (`crawl`_ command, ``lockss.debugpanel.crawl()`` function).
+      *  `reload-config`_
 
-*  Crawl with depth (`deep-crawl`_ command, ``lockss.debugpanel.deep_crawl()`` function).
+      *  `usage`_
 
-*  Poll (`poll`_ command, ``lockss.debugpanel.poll()`` function).
+      *  `validate-files`_
 
-*  Check substance (`check-substance`_ command, ``lockss.debugpanel.check_substance()`` function).
+      *  `version`_
 
-*  Validate files (`validate-files`_ command, ``lockss.debugpanel.validate_files()`` function).
+   * `Options`_
 
-*  Reindex metadata (`reindex-metadata`_ command, ``lockss.debugpanel.reindex_metadata()`` function).
+      *  `Node Arguments and Options`_
 
-*  Disable metadata indexing (`disable-indexing`_ command, ``lockss.debugpanel.disable_reindexing()`` function).
+      *  `AUID Options`_
 
--------
-Library
--------
+      *  `Output Format Control`_
 
-You can use Debugpanel as a Python library.
+      *  `Job Pool Control`_
 
-The ``lockss.debugpanel`` module's ``node()`` method can create a node object from a node reference (a string like ``host:8081``, ``http://host:8081``, ``http://host:8081/``, ``https://host:8081``, ``https://host:8081/``; no protocol defaults to ``http://``), a username, and a password.
+*  `Library`_
 
-This node object can be used as the argument to ``crawl_plugins()`` or ``reload_config()``.
+------------
+Installation
+------------
 
-It can also be used as the first argument to ``check_substance()``, ``crawl()``, ``deep_crawl()``, ``disable_indexing()``, ``poll()``, ``reindex_metadata()``, or ``validate_files``, together with an AUID string as the second argument.
+Debugpanel is available from the `Python Package Index <https://pypi.org/>`_ (PyPI) as ``lockss-debugpanel`` (https://pypi.org/project/lockss-debugpanel), and can be installed with `pip`_.
 
-The ``deep_crawl()`` method has an optional third argument, ``depth``, for the crawl depth (whch defaults to ``lockss.debugpanel.DEFAULT_DEPTH``).
+The installation process adds a ``lockss.debugpanel`` Python `Library`_ and a ``debugpanel`` `Command Line Tool`_. You can check at the command line that the installation is functional by running ``debugpanel version`` or ``debugpanel --help``.
 
-All operations return the modified ``http.client.HTTPResponse`` object from ``urllib.request.urlopen()`` (see https://docs.python.org/3.7/library/urllib.request.html#urllib.request.urlopen). A status code of 200 indicates that the request to the node was made successfully (but not much else; for example if there is no such AUID for an AUID operation, nothing happens).
+Prerequisites
+=============
 
-Use of the module is illustrated in this example::
+*  `Python <https://www.python.org/>`_ 3.7 or greater. (You can check the version of Python 3 with ``python3 --version``.)
 
-    import getpass
-    import lockss.debugpanel
+Prerequisites for development work only:
 
-    hostport = '...'
-    username = input('Username: ')
-    password = getpass.getpass('Password: ')
-    node = lockss.debugpanel.node(hostport, username, password)
-    auid = '...'
+*  `Poetry <https://python-poetry.org/>`_ 1.4 or greater. (You can check the version of Poetry with ``poetry --version``.)
 
-    try:
-        resp = lockss.debugpanel.poll(node, auid)
-        if resp.status == 200:
-            print('Poll requested (200)')
-        else:
-            print(f'{resp.reason} ({resp.status})')
-    except Exception as exc:
-        print(f'Error: {exc!s}')
+.. _pip:
+
+``pip``
+=======
+
+You can install Debugpanel with ``pip``.
+
+To install it in your own non-root, non-virtual environment, use the ``--user`` option::
+
+   pip3 install --user lockss-debugpanel
+
+To install it in a virtual environment, simply use::
+
+   pip3 install lockss-debugpanel
+
+.. danger::
+
+   Do not run ``pip3``/``pip`` as ``root``, with ``sudo`` or otherwise.
+
+--------
+Overview
+--------
+
+Per-Node Operations
+===================
+
+Some operations operate on one or more nodes.
+
+========================= ================ ========
+Operation                 Command          Function
+========================= ================ ========
+Crawl plugins             `crawl-plugins`_ ``crawl_plugins()``
+Reload node configuration `reload-config`_ ``reload_config()``
+========================= ================ ========
+
+Per-AU Operations
+=================
+
+Some operation operate on one or more AUs on one or more nodes.
+
+================================ =================== ========
+Operation                        Command             Function
+================================ =================== ========
+Check substance of AUs           `check-substance`_  ``check_substance()``
+Crawl AUs                        `crawl`_            ``crawl()``
+Crawl AUs with depth             `deep-crawl`_       ``deep_crawl()``
+Disable metadata indexing of AUs `disable-indexing`_ ``disable_indexing()``
+Poll                             `poll`_             ``poll()``
+Reindex AU metadata              `reindex-metadata`_ ``reindex_metadata()``
+Validate AU files                `validate-files`_   ``validate_files()``
+================================ =================== ========
 
 -----------------
 Command Line Tool
 -----------------
 
 Debugpanel is invoked at the command line as::
 
@@ -120,14 +156,17 @@
 
 or as a Python module::
 
    python3 -m lockss.debugpanel
 
 Help messages and this document use ``debugpanel`` throughout, but the two invocation styles are interchangeable.
 
+Synopsis
+========
+
 Debugpanel uses `Commands`_, in the style of programs like ``git``, ``dnf``/``yum``, ``apt``/``apt-get``, and the like. You can see the list of available `Commands`_ by invoking ``debugpanel --help``, and you can find a usage summary of all the `Commands`_ by invoking ``debugpanel usage``::
 
     usage: debugpanel [-h] [--debug-cli] [--verbose] COMMAND ...
 
            debugpanel check-substance [-h] [--output-format FMT]
                                       [--node HOST:PORT] [--nodes FILE]
                                       [--password PASS] [--username USER]
@@ -199,42 +238,46 @@
            debugpanel version [-h]
 
 Commands
 ========
 
 The available commands are:
 
-*  `check-substance`_ (cs):  cause nodes to check the substance of AUs
-*  `copyright`_:             show copyright and exit
-*  `crawl`_ (cr):            cause nodes to crawl AUs
-*  `crawl-plugins`_ (cp):    cause nodes to crawl plugins
-*  `deep-crawl`_ (dc):       cause nodes to crawl AUs, with depth
-*  `disable-indexing`_ (di): cause nodes to disable metadata indexing of AUs
-*  `license`_:               show license and exit
-*  `poll`_ (po):             cause nodes to poll AUs
-*  `reindex-metadata`_ (ri): cause nodes to reindex the metadata of AUs
-*  `reload-config`_ (rc):    cause nodes to reload their configuration
-*  `usage`_:                 show detailed usage and exit
-*  `validate-files`_ (vf):   cause nodes to run file validation on AUs
-*  `version`_:               show version and exit
+=================== ============ =======
+Command             Abbreviation Purpose
+=================== ============ =======
+`check-substance`_  cs           cause nodes to check the substance of AUs
+`copyright`_                     show copyright and exit
+`crawl`_            cr           cause nodes to crawl AUs
+`crawl-plugins`_    cp           cause nodes to crawl plugins
+`deep-crawl`_       dc           cause nodes to crawl AUs, with depth
+`disable-indexing`_ di           cause nodes to disable metadata indexing of AUs
+`license`_                       show license and exit
+`poll`_             po           cause nodes to poll AUs
+`reindex-metadata`_ ri           cause nodes to reindex the metadata of AUs
+`reload-config`_    rc           cause nodes to reload their configuration
+`usage`_                         show detailed usage and exit
+`validate-files`_   vf           cause nodes to run file validation on AUs
+`version`_                       show version and exit
+=================== ============ =======
 
-Top-Level Command
-=================
+Top-Level Program
+-----------------
 
 The top-level executable alone does not perform any action or default to a given command. It does define a few options, which you can see by invoking Debugpanel with the |HELP| option::
 
     usage: debugpanel [-h] [--debug-cli] [--verbose] COMMAND ...
 
     options:
       -h, --help            show this help message and exit
       --debug-cli           print the result of parsing command line arguments
       --verbose, -v         print verbose output
 
     commands:
-      Add --help to see the command's own help message
+      Add --help to see the command's own help message.
 
       COMMAND               DESCRIPTION
         check-substance (cs)
                             cause nodes to check the substance of AUs
         copyright           show copyright and exit
         crawl (cr)          cause nodes to crawl AUs
         crawl-plugins (cp)  cause nodes to crawl plugins
@@ -250,27 +293,27 @@
         validate-files (vf)
                             Cause nodes to run file validation on AUs
         version             show version and exit
 
 .. _check-substance:
 
 ``check-substance`` (``cs``)
-============================
+----------------------------
 
 The ``check-substance`` command is one of the `Per-AU Operations`_, used to cause nodes to check the substance of AUs. It has its own |HELP| option::
 
     usage: debugpanel check-substance [-h] [--output-format FMT]
                                       [--node HOST:PORT] [--nodes FILE]
                                       [--password PASS] [--username USER]
                                       [--auid AUID] [--auids FILE]
                                       [--pool-size SIZE]
                                       [--process-pool | --thread-pool]
                                       [HOST:PORT ...]
 
-    Cause nodes to check the substance of AUs
+    Cause nodes to check the substance of AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -308,32 +351,32 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _copyright:
 
 ``copyright``
-=============
+-------------
 
 The ``copyright`` command displays the copyright notice for Debugpanel and exits.
 
 .. _crawl:
 
 ``crawl`` (``cr``)
-==================
+------------------
 
 The ``crawl`` command is one of the `Per-AU Operations`_, used to cause nodes to crawl AUs. It has its own |HELP| option::
 
     usage: debugpanel crawl-plugins [-h] [--output-format FMT] [--node HOST:PORT]
                                     [--nodes FILE] [--password PASS]
                                     [--username USER] [--pool-size SIZE]
                                     [--process-pool | --thread-pool]
                                     [HOST:PORT ...]
 
-    Cause nodes to crawl plugins
+    Cause nodes to crawl plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -366,25 +409,25 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _crawl-plugins:
 
 ``crawl-plugins`` (``cp``)
-==========================
+--------------------------
 
 The ``crawl-plugins`` command is one of the `Per-Node Operations`_, used to cause nodes to crawl their plugins. It has its own |HELP| option::
 
     usage: debugpanel crawl-plugins [-h] [--output-format FMT] [--node HOST:PORT]
                                     [--nodes FILE] [--password PASS]
                                     [--username USER] [--pool-size SIZE]
                                     [--process-pool | --thread-pool]
                                     [HOST:PORT ...]
 
-    Cause nodes to crawl plugins
+    Cause nodes to crawl plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -415,26 +458,26 @@
 *  One or more nodes, from the `Node Arguments and Options`_ (bare arguments, |NODE| options, |NODES| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _deep-crawl:
 
 ``deep-crawl`` (``dc``)
-=======================
+-----------------------
 
 The ``deep-crawl`` command is one of the `Per-AU Operations`_, used to cause nodes to crawl AUs with depth. It has its own |HELP| option::
 
     usage: debugpanel deep-crawl [-h] [--output-format FMT] [--node HOST:PORT]
                                  [--nodes FILE] [--password PASS]
                                  [--username USER] [--auid AUID] [--auids FILE]
                                  [--pool-size SIZE]
                                  [--process-pool | --thread-pool] [--depth DEPTH]
                                  [HOST:PORT ...]
 
-    Cause nodes to crawl AUs, with depth
+    Cause nodes to crawl AUs, with depth.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -477,27 +520,27 @@
 It has a unique option, ``--depth/-d``, which is an integer specifying the desired crawl depth.
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _disable-indexing:
 
 ``disable-indexing`` (``di``)
-=============================
+-----------------------------
 
 The ``disable-indexing`` command is one of the `Per-AU Operations`_, used to cause nodes to disable metadata indexing of AUs. It has its own |HELP| option::
 
     usage: debugpanel disable-indexing [-h] [--output-format FMT]
                                        [--node HOST:PORT] [--nodes FILE]
                                        [--password PASS] [--username USER]
                                        [--auid AUID] [--auids FILE]
                                        [--pool-size SIZE]
                                        [--process-pool | --thread-pool]
                                        [HOST:PORT ...]
 
-    Cause nodes to disable metadata indexing of AUs
+    Cause nodes to disable metadata indexing of AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -535,32 +578,32 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _license:
 
 ``license``
-=============
+-----------
 
 The ``license`` command displays the license terms for Debugpanel and exits.
 
 .. _poll:
 
 ``poll`` (``po``)
-=================
+-----------------
 
 The ``poll`` command is one of the `Per-AU Operations`_, used to cause nodes to poll AUs. It has its own |HELP| option::
 
     usage: debugpanel poll [-h] [--output-format FMT] [--node HOST:PORT]
                            [--nodes FILE] [--password PASS] [--username USER]
                            [--auid AUID] [--auids FILE] [--pool-size SIZE]
                            [--process-pool | --thread-pool]
                            [HOST:PORT ...]
 
-    Cause nodes to poll AUs
+    Cause nodes to poll AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -598,27 +641,27 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _reindex-metadata:
 
 ``reindex-metadata`` (``ri``)
-=============================
+-----------------------------
 
 The ``reindex-metadata`` command is one of the `Per-AU Operations`_, used to cause nodes to reindex the metadata of AUs. It has its own |HELP| option::
 
     usage: debugpanel reindex-metadata [-h] [--output-format FMT]
                                        [--node HOST:PORT] [--nodes FILE]
                                        [--password PASS] [--username USER]
                                        [--auid AUID] [--auids FILE]
                                        [--pool-size SIZE]
                                        [--process-pool | --thread-pool]
                                        [HOST:PORT ...]
 
-    Cause nodes to reindex the metadata of AUs
+    Cause nodes to reindex the metadata of AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -656,25 +699,25 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _reload-config:
 
 ``reload-config`` (``rc``)
-==========================
+--------------------------
 
 The ``reload-config`` command is one of the `Per-Node Operations`_, used to cause nodes to reload their configuration. It has its own |HELP| option::
 
     usage: debugpanel reload-config [-h] [--output-format FMT] [--node HOST:PORT]
                                     [--nodes FILE] [--password PASS]
                                     [--username USER] [--pool-size SIZE]
                                     [--process-pool | --thread-pool]
                                     [HOST:PORT ...]
 
-    Cause nodes to reload their configuration
+    Cause nodes to reload their configuration.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -705,33 +748,33 @@
 *  One or more nodes, from the `Node Arguments and Options`_ (bare arguments, |NODE| options, |NODES| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _usage:
 
 ``usage``
-=========
+---------
 
 The ``usage`` command displays the usage message of all the Debugpanel `Commands`_.
 
 .. _validate-files:
 
 ``validate-files`` (``vf``)
-=============================
+---------------------------
 
 The ``validate-files`` command is one of the `Per-AU Operations`_, used to cause nodes to reindex the metadata of AUs. It has its own |HELP| option::
 
     usage: debugpanel validate-files [-h] [--output-format FMT] [--node HOST:PORT]
                                      [--nodes FILE] [--password PASS]
                                      [--username USER] [--auid AUID]
                                      [--auids FILE] [--pool-size SIZE]
                                      [--process-pool | --thread-pool]
                                      [HOST:PORT ...]
 
-    Cause nodes to run file validation on AUs
+    Cause nodes to run file validation on AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -769,44 +812,91 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _version:
 
 ``version``
-===========
+-----------
 
 The ``version`` command displays the version number of Debugpanel and exits.
 
--------
 Options
--------
+=======
 
 Node Arguments and Options
-==========================
+--------------------------
 
 `Commands`_ for `Per-Node Operations`_ expect one or more node references in ``HOST:PORT`` format, for instance ``lockss.myuniversity.edu:8081``. The list of nodes to process is derived from:
 
 *  The nodes listed as bare arguments to the command.
 
 *  The nodes listed as |NODE| options.
 
 *  The nodes found in the files listed as |NODES| options.
 
 AUID Options
-============
+------------
 
 In addition to `Node Arguments and Options`_, `Commands`_ for `Per-AU Operations`_ expect one or more AUIDs. The list of AUIDs to target is derived from:
 
 *  The AUIDs listed as |AUID| options.
 
 *  The AUIDs found in the files listed as |AUIDS| options.
 
 Output Format Control
-=====================
+---------------------
 
 Debugpanel's tabular output is performed by the `tabulate <https://pypi.org/project/tabulate>`_ library through the ``--output-format`` option. See its PyPI page for a visual reference of the various output formats available. The **default** is ``simple``.
 
 Job Pool Control
-================
+----------------
 
 Debugpanel performs multiple operations (contacting multiple nodes and/or working on multiple AU requests per node) in parallel using a thread pool (``--thread-pool``, the default) or a process pool (``--process-pool``). You can change the size of the job pool with the ``--pool-size`` option, which accepts a nonzero integer. Note that the underlying implementation may limit the number of threads or processes despite a larger number at the command line. The default value depends on the system's CPU characteristics (represented in this document as "N"). Using ``--thread-pool --pool-size=1`` approximates no parallel processing.
+
+.. _check_substance():
+.. _crawl():
+.. _crawl_plugins():
+.. _deep_crawl():
+.. _disable_indexing():
+.. _node():
+.. _poll():
+.. _reindex_metadata():
+.. _reload_config():
+.. _validate_files():
+
+-------
+Library
+-------
+
+You can use Debugpanel as a Python library.
+
+The ``lockss.debugpanel`` module's `node()`_ method can create a node object from a node reference (a string like ``host:8081``, ``http://host:8081``, ``http://host:8081/``, ``https://host:8081``, ``https://host:8081/``; no protocol defaults to ``http://``), a username, and a password.
+
+This node object can be used as the argument to `crawl_plugins()`_ or `reload_config()`_.
+
+It can also be used as the first argument to `check_substance()`_, `crawl()`_, `deep_crawl()`_, `disable_indexing()`_, `poll()`_, `reindex_metadata()`_, or `validate_files()`_, together with an AUID string as the second argument.
+
+The `deep_crawl()`_ method has an optional third argument, ``depth``, for the crawl depth (whch defaults to ``lockss.debugpanel.DEFAULT_DEPTH``).
+
+All operations return the modified ``http.client.HTTPResponse`` object from ``urllib.request.urlopen()`` (see https://docs.python.org/3.7/library/urllib.request.html#urllib.request.urlopen). A status code of 200 indicates that the request to the node was made successfully (but not much else; for example if there is no such AUID for an AUID operation, nothing happens).
+
+Use of the module is illustrated in this example::
+
+    import getpass
+    import lockss.debugpanel
+
+    hostport = '...'
+    username = input('Username: ')
+    password = getpass.getpass('Password: ')
+    node = lockss.debugpanel.node(hostport, username, password)
+    auid = '...'
+
+    try:
+        resp = lockss.debugpanel.poll(node, auid)
+        if resp.status == 200:
+            print('Poll requested (200)')
+        else:
+            print(f'{resp.reason} ({resp.status})')
+    except Exception as exc:
+        print(f'Error: {exc!s}')
+
```

### Comparing `lockss_debugpanel-0.6.1/pyproject.toml` & `lockss_debugpanel-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "lockss-debugpanel"
-version = "0.6.1"
+version = "0.7.0"
 description = "Library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
-repository = "https://code.stanford.edu/lockss/tools/debugpanel"
+repository = "https://github.com/lockss/lockss-debugpanel"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Operating System :: POSIX :: Linux",
     "Topic :: Utilities"
@@ -22,14 +22,15 @@
 ]
 include = [
     "CHANGELOG.rst"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
+rich-argparse = "^1.1.0"
 tabulate = "^0.9.0"
 
 [tool.poetry.scripts]
 debugpanel = 'lockss.debugpanel.cli:main'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lockss_debugpanel-0.6.1/src/lockss/debugpanel/__init__.py` & `lockss_debugpanel-0.7.0/src/lockss/debugpanel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.6.1'
+__version__ = '0.7.0'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
```

### Comparing `lockss_debugpanel-0.6.1/src/lockss/debugpanel/__main__.py` & `lockss_debugpanel-0.7.0/src/lockss/debugpanel/__main__.py`

 * *Files identical despite different names*

### Comparing `lockss_debugpanel-0.6.1/src/lockss/debugpanel/cli.py` & `lockss_debugpanel-0.7.0/src/lockss/debugpanel/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import os
 from pathlib import Path, PurePath
 import sys
 import traceback
 import urllib.error
 import urllib.request
 
+import rich_argparse
 import tabulate
 
 import lockss.debugpanel
 
 
 def _path(purepath_or_string):
     if not issubclass(type(purepath_or_string), PurePath):
@@ -158,14 +159,21 @@
 
     def _make_option_depth(self, container):
         container.add_argument('--depth', '-d',
                                type=int,
                                default=DebugPanelCli.DEFAULT_DEPTH,
                                help='depth of deep crawls (default: %(default)s)')
 
+    def _make_option_output_format(self, container):
+        container.add_argument('--output-format',
+                               metavar='FMT',
+                               choices=tabulate.tabulate_formats,
+                               default='simple',
+                               help='set tabular output format to %(metavar)s (default: %(default)s; choices: %(choices)s)')
+
     def _make_option_verbose(self, container):
         container.add_argument('--verbose', '-v',
                                action='store_true',
                                help='print verbose output')
 
     def _make_options_auids(self, container):
         group = container.add_argument_group(title='AUID options')
@@ -214,25 +222,26 @@
         group.add_argument('--password', '-p',
                            metavar='PASS',
                            help='UI password (default: interactive prompt)')
         group.add_argument('--username', '-u',
                            metavar='USER',
                            help='UI username (default: interactive prompt)')
 
-    def _make_option_output_format(self, container):
-        container.add_argument('--output-format',
-                               metavar='FMT',
-                               choices=tabulate.tabulate_formats,
-                               default='simple',
-                               help='set tabular output format to %(metavar)s (default: %(default)s; choices: %(choices)s)')
-
     def _make_parser(self):
-        self._parser = argparse.ArgumentParser(prog=DebugPanelCli.PROG)
+        for cls in [rich_argparse.RichHelpFormatter]:
+            cls.styles.update({
+                'argparse.args': f'bold {cls.styles["argparse.args"]}',
+                'argparse.groups': f'bold {cls.styles["argparse.groups"]}',
+                'argparse.metavar': f'bold {cls.styles["argparse.metavar"]}',
+                'argparse.prog': f'bold {cls.styles["argparse.prog"]}',
+            })
+        self._parser = argparse.ArgumentParser(prog=DebugPanelCli.PROG,
+                                               formatter_class=rich_argparse.RichHelpFormatter)
         self._subparsers = self._parser.add_subparsers(title='commands',
-                                                       description="Add --help to see the command's own help message",
+                                                       description="Add --help to see the command's own help message.",
                                                        dest='command',
                                                        required=True,
                                                        # With subparsers, metavar is also used as the heading of the column of subcommands
                                                        metavar='COMMAND',
                                                        # With subparsers, help is used as the heading of the column of subcommand descriptions
                                                        help='DESCRIPTION')
         self._make_option_debug_cli(self._parser)
@@ -250,119 +259,125 @@
         self._make_parser_usage(self._subparsers)
         self._make_parser_validate_files(self._subparsers)
         self._make_parser_version(self._subparsers)
 
     def _make_parser_check_substance(self, container):
         self._make_parser_per_auid(container,
                                    'check-substance', ['cs'],
-                                   'Cause nodes to check the substance of AUs',
+                                   'Cause nodes to check the substance of AUs.',
                                    'cause nodes to check the substance of AUs',
                                    lockss.debugpanel.check_substance)
 
     def _make_parser_copyright(self, container):
         parser = container.add_parser('copyright',
-                                      description='Show copyright and exit',
-                                      help='show copyright and exit')
+                                      description='Show copyright and exit.',
+                                      help='show copyright and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._copyright)
 
     def _make_parser_crawl(self, container):
         self._make_parser_per_auid(container,
                                    'crawl', ['cr'],
-                                   'Cause nodes to crawl AUs',
+                                   'Cause nodes to crawl AUs.',
                                    'cause nodes to crawl AUs',
                                    lockss.debugpanel.crawl)
 
     def _make_parser_crawl_plugins(self, container):
         self._make_parser_per_node(container,
                                    'crawl-plugins', ['cp'],
-                                   'Cause nodes to crawl plugins',
+                                   'Cause nodes to crawl plugins.',
                                    'cause nodes to crawl plugins',
                                    lockss.debugpanel.crawl_plugins)
 
     def _make_parser_deep_crawl(self, container):
         parser = self._make_parser_per_auid(container,
                                             'deep-crawl', ['dc'],
-                                            'Cause nodes to crawl AUs, with depth',
+                                            'Cause nodes to crawl AUs, with depth.',
                                             'cause nodes to crawl AUs, with depth',
                                             lockss.debugpanel.deep_crawl)
         self._make_option_depth(parser)
 
     def _make_parser_disable_indexing(self, container):
         parser = self._make_parser_per_auid(container,
                                             'disable-indexing', ['di'],
-                                            'Cause nodes to disable metadata indexing of AUs',
+                                            'Cause nodes to disable metadata indexing of AUs.',
                                             'cause nodes to disable metadata indexing of AUs',
                                             lockss.debugpanel.disable_indexing)
 
     def _make_parser_license(self, container):
         parser = container.add_parser('license',
-                                      description='Show license and exit',
-                                      help='show license and exit')
+                                      description='Show license and exit.',
+                                      help='show license and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._license)
 
     def _make_parser_per_auid(self, container, option, aliases, description, help, target):
         parser = container.add_parser(option, aliases=aliases,
                                       description=description,
-                                      help=help)
+                                      help=help,
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._per_auid)
         parser.set_defaults(target=target)
         self._make_option_output_format(parser)
         self._make_options_nodes(parser)
         self._make_options_auids(parser)
         self._make_options_job_pool(parser)
         return parser
 
     def _make_parser_per_node(self, container, option, aliases, description, help, target):
         parser = container.add_parser(option, aliases=aliases,
                                       description=description,
-                                      help=help)
+                                      help=help,
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._per_node)
         parser.set_defaults(target=target)
         self._make_option_output_format(parser)
         self._make_options_nodes(parser)
         self._make_options_job_pool(parser)
 
     def _make_parser_poll(self, container):
         self._make_parser_per_auid(container,
                                    'poll', ['po'],
-                                   'Cause nodes to poll AUs',
+                                   'Cause nodes to poll AUs.',
                                    'cause nodes to poll AUs',
                                    lockss.debugpanel.poll)
 
     def _make_parser_reindex_metadata(self, container):
         parser = self._make_parser_per_auid(container,
                                             'reindex-metadata', ['ri'],
-                                            'Cause nodes to reindex the metadata of AUs',
+                                            'Cause nodes to reindex the metadata of AUs.',
                                             'cause nodes to reindex the metadata of AUs',
                                             lockss.debugpanel.reindex_metadata)
 
     def _make_parser_reload_config(self, container):
         self._make_parser_per_node(container,
                                    'reload-config', ['rc'],
-                                   'Cause nodes to reload their configuration',
+                                   'Cause nodes to reload their configuration.',
                                    'cause nodes to reload their configuration',
                                    lockss.debugpanel.reload_config)
 
     def _make_parser_usage(self, container):
         parser = container.add_parser('usage',
-                                      description='Show detailed usage and exit',
-                                      help='show detailed usage and exit')
+                                      description='Show detailed usage and exit.',
+                                      help='show detailed usage and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._usage)
 
     def _make_parser_validate_files(self, container):
         self._make_parser_per_auid(container,
                                    'validate-files', ['vf'],
-                                   'Cause nodes to run file validation on AUs',
+                                   'Cause nodes to run file validation on AUs.',
                                    'cause nodes to run file validation on AUs',
                                    lockss.debugpanel.validate_files)
 
     def _make_parser_version(self, container):
         parser = container.add_parser('version',
-                                      description='Show version and exit',
-                                      help='show version and exit')
+                                      description='Show version and exit.',
+                                      help='show version and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._version)
 
     def _per_auid(self):
         self._initialize_auth()
         self._initialize_executor()
         node_objects = [lockss.debugpanel.node(node, *self._auth) for node in self._get_nodes()]
         futures = {self._executor.submit(_do_per_auid, node_object, auid, self._args.target, pickled=True): (node, auid) for auid in self._get_auids() for node, node_object in zip(self._get_nodes(), node_objects)}
```

### Comparing `lockss_debugpanel-0.6.1/PKG-INFO` & `lockss_debugpanel-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-debugpanel
-Version: 0.6.1
+Version: 0.7.0
 Summary: Library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,129 +16,166 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Requires-Dist: rich-argparse (>=1.1.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Project-URL: Repository, https://code.stanford.edu/lockss/tools/debugpanel
+Project-URL: Repository, https://github.com/lockss/lockss-debugpanel
 Description-Content-Type: text/x-rst
 
 ==========
 Debugpanel
 ==========
 
+.. |RELEASE| replace:: 0.7.0
+.. |RELEASE_DATE| replace:: 2023-05-02
+
 .. |AUID| replace:: ``--auid/-a``
 .. |AUIDS| replace:: ``--auids/-A``
 .. |HELP| replace:: ``--help/-h``
 .. |NODE| replace:: ``--node/-n``
 .. |NODES| replace:: ``--nodes/-N``
 
 Debugpanel is a library and command line tool to interact with the LOCKSS 1.x DebugPanel servlet.
 
-**Latest release:** 0.6.1 (2023-03-16)
+**Latest release:** |RELEASE| (|RELEASE_DATE|)
 
--------------
-Prerequisites
--------------
+-----------------
+Table of Contents
+-----------------
 
-*  `Python <https://www.python.org/>`_ 3.7 or greater.
+*  `Installation`_
 
-Prerequisites for development work only:
+   *  `Prerequisites`_
 
-*  `Poetry <https://python-poetry.org/>`_ 1.4 or greater.
+   *  `pip`_
 
-------------
-Installation
-------------
+*  `Overview`_
 
-Debugpanel is available from the `Python Package Index <https://pypi.org/>`_ (PyPI) as ``lockss-debugpanel``: https://pypi.org/project/lockss-debugpanel
+   * `Per-Node Operations`_
 
-You can install it with ``pip``. To install it in a virtual environment, simply use::
+   * `Per-AU Operations`_
 
-   pip3 install lockss-debugpanel
+*  `Command Line Tool`_
 
-To install it in your own non-root, non-virtual environment, use the ``--user`` option::
+   * `Synopsis`_
 
-   pip3 install --user lockss-debugpanel
+   * `Commands`_
 
-.. danger::
+      * `Top-Level Program`_
 
-   Do not run ``pip3``/``pip`` as ``root``, with ``sudo`` or otherwise.
+      *  `check-substance`_
 
-The installation process adds a ``lockss.debugpanel`` `Library`_ and a ``debugpanel`` `Command Line Tool`_. You can check at the command line that the installation is functional by running ``debugpanel version`` or ``debugpanel --help``.
+      *  `copyright`_
 
---------
-Overview
---------
+      *  `crawl`_
 
-Per-Node Operations
-===================
+      *  `crawl-plugins`_
 
-You can use Debugpanel to get LOCKSS nodes to:
+      *  `deep-crawl`_
 
-*  Reload their configuration (`reload-config`_ command, ``lockss.debugpanel.reload_config()`` function).
+      *  `disable-indexing`_
 
-*  Crawl their plugins (`crawl-plugins`_ command, ``lockss.debugpanel.crawl_plugins()`` function).
+      *  `license`_
 
-Per-AU Operations
-=================
+      *  `poll`_
 
-You can use Debugpanel to get LOCKSS nodes to perform an operation on AUs identified by AUID, namely:
+      *  `reindex-metadata`_
 
-*  Crawl (`crawl`_ command, ``lockss.debugpanel.crawl()`` function).
+      *  `reload-config`_
 
-*  Crawl with depth (`deep-crawl`_ command, ``lockss.debugpanel.deep_crawl()`` function).
+      *  `usage`_
 
-*  Poll (`poll`_ command, ``lockss.debugpanel.poll()`` function).
+      *  `validate-files`_
 
-*  Check substance (`check-substance`_ command, ``lockss.debugpanel.check_substance()`` function).
+      *  `version`_
 
-*  Validate files (`validate-files`_ command, ``lockss.debugpanel.validate_files()`` function).
+   * `Options`_
 
-*  Reindex metadata (`reindex-metadata`_ command, ``lockss.debugpanel.reindex_metadata()`` function).
+      *  `Node Arguments and Options`_
 
-*  Disable metadata indexing (`disable-indexing`_ command, ``lockss.debugpanel.disable_reindexing()`` function).
+      *  `AUID Options`_
 
--------
-Library
--------
+      *  `Output Format Control`_
 
-You can use Debugpanel as a Python library.
+      *  `Job Pool Control`_
 
-The ``lockss.debugpanel`` module's ``node()`` method can create a node object from a node reference (a string like ``host:8081``, ``http://host:8081``, ``http://host:8081/``, ``https://host:8081``, ``https://host:8081/``; no protocol defaults to ``http://``), a username, and a password.
+*  `Library`_
 
-This node object can be used as the argument to ``crawl_plugins()`` or ``reload_config()``.
+------------
+Installation
+------------
 
-It can also be used as the first argument to ``check_substance()``, ``crawl()``, ``deep_crawl()``, ``disable_indexing()``, ``poll()``, ``reindex_metadata()``, or ``validate_files``, together with an AUID string as the second argument.
+Debugpanel is available from the `Python Package Index <https://pypi.org/>`_ (PyPI) as ``lockss-debugpanel`` (https://pypi.org/project/lockss-debugpanel), and can be installed with `pip`_.
 
-The ``deep_crawl()`` method has an optional third argument, ``depth``, for the crawl depth (whch defaults to ``lockss.debugpanel.DEFAULT_DEPTH``).
+The installation process adds a ``lockss.debugpanel`` Python `Library`_ and a ``debugpanel`` `Command Line Tool`_. You can check at the command line that the installation is functional by running ``debugpanel version`` or ``debugpanel --help``.
 
-All operations return the modified ``http.client.HTTPResponse`` object from ``urllib.request.urlopen()`` (see https://docs.python.org/3.7/library/urllib.request.html#urllib.request.urlopen). A status code of 200 indicates that the request to the node was made successfully (but not much else; for example if there is no such AUID for an AUID operation, nothing happens).
+Prerequisites
+=============
 
-Use of the module is illustrated in this example::
+*  `Python <https://www.python.org/>`_ 3.7 or greater. (You can check the version of Python 3 with ``python3 --version``.)
 
-    import getpass
-    import lockss.debugpanel
+Prerequisites for development work only:
 
-    hostport = '...'
-    username = input('Username: ')
-    password = getpass.getpass('Password: ')
-    node = lockss.debugpanel.node(hostport, username, password)
-    auid = '...'
+*  `Poetry <https://python-poetry.org/>`_ 1.4 or greater. (You can check the version of Poetry with ``poetry --version``.)
 
-    try:
-        resp = lockss.debugpanel.poll(node, auid)
-        if resp.status == 200:
-            print('Poll requested (200)')
-        else:
-            print(f'{resp.reason} ({resp.status})')
-    except Exception as exc:
-        print(f'Error: {exc!s}')
+.. _pip:
+
+``pip``
+=======
+
+You can install Debugpanel with ``pip``.
+
+To install it in your own non-root, non-virtual environment, use the ``--user`` option::
+
+   pip3 install --user lockss-debugpanel
+
+To install it in a virtual environment, simply use::
+
+   pip3 install lockss-debugpanel
+
+.. danger::
+
+   Do not run ``pip3``/``pip`` as ``root``, with ``sudo`` or otherwise.
+
+--------
+Overview
+--------
+
+Per-Node Operations
+===================
+
+Some operations operate on one or more nodes.
+
+========================= ================ ========
+Operation                 Command          Function
+========================= ================ ========
+Crawl plugins             `crawl-plugins`_ ``crawl_plugins()``
+Reload node configuration `reload-config`_ ``reload_config()``
+========================= ================ ========
+
+Per-AU Operations
+=================
+
+Some operation operate on one or more AUs on one or more nodes.
+
+================================ =================== ========
+Operation                        Command             Function
+================================ =================== ========
+Check substance of AUs           `check-substance`_  ``check_substance()``
+Crawl AUs                        `crawl`_            ``crawl()``
+Crawl AUs with depth             `deep-crawl`_       ``deep_crawl()``
+Disable metadata indexing of AUs `disable-indexing`_ ``disable_indexing()``
+Poll                             `poll`_             ``poll()``
+Reindex AU metadata              `reindex-metadata`_ ``reindex_metadata()``
+Validate AU files                `validate-files`_   ``validate_files()``
+================================ =================== ========
 
 -----------------
 Command Line Tool
 -----------------
 
 Debugpanel is invoked at the command line as::
 
@@ -146,14 +183,17 @@
 
 or as a Python module::
 
    python3 -m lockss.debugpanel
 
 Help messages and this document use ``debugpanel`` throughout, but the two invocation styles are interchangeable.
 
+Synopsis
+========
+
 Debugpanel uses `Commands`_, in the style of programs like ``git``, ``dnf``/``yum``, ``apt``/``apt-get``, and the like. You can see the list of available `Commands`_ by invoking ``debugpanel --help``, and you can find a usage summary of all the `Commands`_ by invoking ``debugpanel usage``::
 
     usage: debugpanel [-h] [--debug-cli] [--verbose] COMMAND ...
 
            debugpanel check-substance [-h] [--output-format FMT]
                                       [--node HOST:PORT] [--nodes FILE]
                                       [--password PASS] [--username USER]
@@ -225,42 +265,46 @@
            debugpanel version [-h]
 
 Commands
 ========
 
 The available commands are:
 
-*  `check-substance`_ (cs):  cause nodes to check the substance of AUs
-*  `copyright`_:             show copyright and exit
-*  `crawl`_ (cr):            cause nodes to crawl AUs
-*  `crawl-plugins`_ (cp):    cause nodes to crawl plugins
-*  `deep-crawl`_ (dc):       cause nodes to crawl AUs, with depth
-*  `disable-indexing`_ (di): cause nodes to disable metadata indexing of AUs
-*  `license`_:               show license and exit
-*  `poll`_ (po):             cause nodes to poll AUs
-*  `reindex-metadata`_ (ri): cause nodes to reindex the metadata of AUs
-*  `reload-config`_ (rc):    cause nodes to reload their configuration
-*  `usage`_:                 show detailed usage and exit
-*  `validate-files`_ (vf):   cause nodes to run file validation on AUs
-*  `version`_:               show version and exit
+=================== ============ =======
+Command             Abbreviation Purpose
+=================== ============ =======
+`check-substance`_  cs           cause nodes to check the substance of AUs
+`copyright`_                     show copyright and exit
+`crawl`_            cr           cause nodes to crawl AUs
+`crawl-plugins`_    cp           cause nodes to crawl plugins
+`deep-crawl`_       dc           cause nodes to crawl AUs, with depth
+`disable-indexing`_ di           cause nodes to disable metadata indexing of AUs
+`license`_                       show license and exit
+`poll`_             po           cause nodes to poll AUs
+`reindex-metadata`_ ri           cause nodes to reindex the metadata of AUs
+`reload-config`_    rc           cause nodes to reload their configuration
+`usage`_                         show detailed usage and exit
+`validate-files`_   vf           cause nodes to run file validation on AUs
+`version`_                       show version and exit
+=================== ============ =======
 
-Top-Level Command
-=================
+Top-Level Program
+-----------------
 
 The top-level executable alone does not perform any action or default to a given command. It does define a few options, which you can see by invoking Debugpanel with the |HELP| option::
 
     usage: debugpanel [-h] [--debug-cli] [--verbose] COMMAND ...
 
     options:
       -h, --help            show this help message and exit
       --debug-cli           print the result of parsing command line arguments
       --verbose, -v         print verbose output
 
     commands:
-      Add --help to see the command's own help message
+      Add --help to see the command's own help message.
 
       COMMAND               DESCRIPTION
         check-substance (cs)
                             cause nodes to check the substance of AUs
         copyright           show copyright and exit
         crawl (cr)          cause nodes to crawl AUs
         crawl-plugins (cp)  cause nodes to crawl plugins
@@ -276,27 +320,27 @@
         validate-files (vf)
                             Cause nodes to run file validation on AUs
         version             show version and exit
 
 .. _check-substance:
 
 ``check-substance`` (``cs``)
-============================
+----------------------------
 
 The ``check-substance`` command is one of the `Per-AU Operations`_, used to cause nodes to check the substance of AUs. It has its own |HELP| option::
 
     usage: debugpanel check-substance [-h] [--output-format FMT]
                                       [--node HOST:PORT] [--nodes FILE]
                                       [--password PASS] [--username USER]
                                       [--auid AUID] [--auids FILE]
                                       [--pool-size SIZE]
                                       [--process-pool | --thread-pool]
                                       [HOST:PORT ...]
 
-    Cause nodes to check the substance of AUs
+    Cause nodes to check the substance of AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -334,32 +378,32 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _copyright:
 
 ``copyright``
-=============
+-------------
 
 The ``copyright`` command displays the copyright notice for Debugpanel and exits.
 
 .. _crawl:
 
 ``crawl`` (``cr``)
-==================
+------------------
 
 The ``crawl`` command is one of the `Per-AU Operations`_, used to cause nodes to crawl AUs. It has its own |HELP| option::
 
     usage: debugpanel crawl-plugins [-h] [--output-format FMT] [--node HOST:PORT]
                                     [--nodes FILE] [--password PASS]
                                     [--username USER] [--pool-size SIZE]
                                     [--process-pool | --thread-pool]
                                     [HOST:PORT ...]
 
-    Cause nodes to crawl plugins
+    Cause nodes to crawl plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -392,25 +436,25 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _crawl-plugins:
 
 ``crawl-plugins`` (``cp``)
-==========================
+--------------------------
 
 The ``crawl-plugins`` command is one of the `Per-Node Operations`_, used to cause nodes to crawl their plugins. It has its own |HELP| option::
 
     usage: debugpanel crawl-plugins [-h] [--output-format FMT] [--node HOST:PORT]
                                     [--nodes FILE] [--password PASS]
                                     [--username USER] [--pool-size SIZE]
                                     [--process-pool | --thread-pool]
                                     [HOST:PORT ...]
 
-    Cause nodes to crawl plugins
+    Cause nodes to crawl plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -441,26 +485,26 @@
 *  One or more nodes, from the `Node Arguments and Options`_ (bare arguments, |NODE| options, |NODES| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _deep-crawl:
 
 ``deep-crawl`` (``dc``)
-=======================
+-----------------------
 
 The ``deep-crawl`` command is one of the `Per-AU Operations`_, used to cause nodes to crawl AUs with depth. It has its own |HELP| option::
 
     usage: debugpanel deep-crawl [-h] [--output-format FMT] [--node HOST:PORT]
                                  [--nodes FILE] [--password PASS]
                                  [--username USER] [--auid AUID] [--auids FILE]
                                  [--pool-size SIZE]
                                  [--process-pool | --thread-pool] [--depth DEPTH]
                                  [HOST:PORT ...]
 
-    Cause nodes to crawl AUs, with depth
+    Cause nodes to crawl AUs, with depth.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -503,27 +547,27 @@
 It has a unique option, ``--depth/-d``, which is an integer specifying the desired crawl depth.
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _disable-indexing:
 
 ``disable-indexing`` (``di``)
-=============================
+-----------------------------
 
 The ``disable-indexing`` command is one of the `Per-AU Operations`_, used to cause nodes to disable metadata indexing of AUs. It has its own |HELP| option::
 
     usage: debugpanel disable-indexing [-h] [--output-format FMT]
                                        [--node HOST:PORT] [--nodes FILE]
                                        [--password PASS] [--username USER]
                                        [--auid AUID] [--auids FILE]
                                        [--pool-size SIZE]
                                        [--process-pool | --thread-pool]
                                        [HOST:PORT ...]
 
-    Cause nodes to disable metadata indexing of AUs
+    Cause nodes to disable metadata indexing of AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -561,32 +605,32 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _license:
 
 ``license``
-=============
+-----------
 
 The ``license`` command displays the license terms for Debugpanel and exits.
 
 .. _poll:
 
 ``poll`` (``po``)
-=================
+-----------------
 
 The ``poll`` command is one of the `Per-AU Operations`_, used to cause nodes to poll AUs. It has its own |HELP| option::
 
     usage: debugpanel poll [-h] [--output-format FMT] [--node HOST:PORT]
                            [--nodes FILE] [--password PASS] [--username USER]
                            [--auid AUID] [--auids FILE] [--pool-size SIZE]
                            [--process-pool | --thread-pool]
                            [HOST:PORT ...]
 
-    Cause nodes to poll AUs
+    Cause nodes to poll AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -624,27 +668,27 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _reindex-metadata:
 
 ``reindex-metadata`` (``ri``)
-=============================
+-----------------------------
 
 The ``reindex-metadata`` command is one of the `Per-AU Operations`_, used to cause nodes to reindex the metadata of AUs. It has its own |HELP| option::
 
     usage: debugpanel reindex-metadata [-h] [--output-format FMT]
                                        [--node HOST:PORT] [--nodes FILE]
                                        [--password PASS] [--username USER]
                                        [--auid AUID] [--auids FILE]
                                        [--pool-size SIZE]
                                        [--process-pool | --thread-pool]
                                        [HOST:PORT ...]
 
-    Cause nodes to reindex the metadata of AUs
+    Cause nodes to reindex the metadata of AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -682,25 +726,25 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _reload-config:
 
 ``reload-config`` (``rc``)
-==========================
+--------------------------
 
 The ``reload-config`` command is one of the `Per-Node Operations`_, used to cause nodes to reload their configuration. It has its own |HELP| option::
 
     usage: debugpanel reload-config [-h] [--output-format FMT] [--node HOST:PORT]
                                     [--nodes FILE] [--password PASS]
                                     [--username USER] [--pool-size SIZE]
                                     [--process-pool | --thread-pool]
                                     [HOST:PORT ...]
 
-    Cause nodes to reload their configuration
+    Cause nodes to reload their configuration.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -731,33 +775,33 @@
 *  One or more nodes, from the `Node Arguments and Options`_ (bare arguments, |NODE| options, |NODES| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _usage:
 
 ``usage``
-=========
+---------
 
 The ``usage`` command displays the usage message of all the Debugpanel `Commands`_.
 
 .. _validate-files:
 
 ``validate-files`` (``vf``)
-=============================
+---------------------------
 
 The ``validate-files`` command is one of the `Per-AU Operations`_, used to cause nodes to reindex the metadata of AUs. It has its own |HELP| option::
 
     usage: debugpanel validate-files [-h] [--output-format FMT] [--node HOST:PORT]
                                      [--nodes FILE] [--password PASS]
                                      [--username USER] [--auid AUID]
                                      [--auids FILE] [--pool-size SIZE]
                                      [--process-pool | --thread-pool]
                                      [HOST:PORT ...]
 
-    Cause nodes to run file validation on AUs
+    Cause nodes to run file validation on AUs.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -795,45 +839,92 @@
 *  One or more AUIDs, from the `AUID Options`_ (|AUID| options, |AUIDS| options).
 
 It also accepts `Options`_ for `Output Format Control`_ and `Job Pool Control`_.
 
 .. _version:
 
 ``version``
-===========
+-----------
 
 The ``version`` command displays the version number of Debugpanel and exits.
 
--------
 Options
--------
+=======
 
 Node Arguments and Options
-==========================
+--------------------------
 
 `Commands`_ for `Per-Node Operations`_ expect one or more node references in ``HOST:PORT`` format, for instance ``lockss.myuniversity.edu:8081``. The list of nodes to process is derived from:
 
 *  The nodes listed as bare arguments to the command.
 
 *  The nodes listed as |NODE| options.
 
 *  The nodes found in the files listed as |NODES| options.
 
 AUID Options
-============
+------------
 
 In addition to `Node Arguments and Options`_, `Commands`_ for `Per-AU Operations`_ expect one or more AUIDs. The list of AUIDs to target is derived from:
 
 *  The AUIDs listed as |AUID| options.
 
 *  The AUIDs found in the files listed as |AUIDS| options.
 
 Output Format Control
-=====================
+---------------------
 
 Debugpanel's tabular output is performed by the `tabulate <https://pypi.org/project/tabulate>`_ library through the ``--output-format`` option. See its PyPI page for a visual reference of the various output formats available. The **default** is ``simple``.
 
 Job Pool Control
-================
+----------------
 
 Debugpanel performs multiple operations (contacting multiple nodes and/or working on multiple AU requests per node) in parallel using a thread pool (``--thread-pool``, the default) or a process pool (``--process-pool``). You can change the size of the job pool with the ``--pool-size`` option, which accepts a nonzero integer. Note that the underlying implementation may limit the number of threads or processes despite a larger number at the command line. The default value depends on the system's CPU characteristics (represented in this document as "N"). Using ``--thread-pool --pool-size=1`` approximates no parallel processing.
 
+.. _check_substance():
+.. _crawl():
+.. _crawl_plugins():
+.. _deep_crawl():
+.. _disable_indexing():
+.. _node():
+.. _poll():
+.. _reindex_metadata():
+.. _reload_config():
+.. _validate_files():
+
+-------
+Library
+-------
+
+You can use Debugpanel as a Python library.
+
+The ``lockss.debugpanel`` module's `node()`_ method can create a node object from a node reference (a string like ``host:8081``, ``http://host:8081``, ``http://host:8081/``, ``https://host:8081``, ``https://host:8081/``; no protocol defaults to ``http://``), a username, and a password.
+
+This node object can be used as the argument to `crawl_plugins()`_ or `reload_config()`_.
+
+It can also be used as the first argument to `check_substance()`_, `crawl()`_, `deep_crawl()`_, `disable_indexing()`_, `poll()`_, `reindex_metadata()`_, or `validate_files()`_, together with an AUID string as the second argument.
+
+The `deep_crawl()`_ method has an optional third argument, ``depth``, for the crawl depth (whch defaults to ``lockss.debugpanel.DEFAULT_DEPTH``).
+
+All operations return the modified ``http.client.HTTPResponse`` object from ``urllib.request.urlopen()`` (see https://docs.python.org/3.7/library/urllib.request.html#urllib.request.urlopen). A status code of 200 indicates that the request to the node was made successfully (but not much else; for example if there is no such AUID for an AUID operation, nothing happens).
+
+Use of the module is illustrated in this example::
+
+    import getpass
+    import lockss.debugpanel
+
+    hostport = '...'
+    username = input('Username: ')
+    password = getpass.getpass('Password: ')
+    node = lockss.debugpanel.node(hostport, username, password)
+    auid = '...'
+
+    try:
+        resp = lockss.debugpanel.poll(node, auid)
+        if resp.status == 200:
+            print('Poll requested (200)')
+        else:
+            print(f'{resp.reason} ({resp.status})')
+    except Exception as exc:
+        print(f'Error: {exc!s}')
+
+
```

