# Comparing `tmp/lockss_turtles-0.4.0.dev1.tar.gz` & `tmp/lockss_turtles-0.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_turtles-0.4.0.dev1.tar", max compression
+gzip compressed data, was "lockss_turtles-0.4.0.dev2.tar", max compression
```

## Comparing `lockss_turtles-0.4.0.dev1.tar` & `lockss_turtles-0.4.0.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3133 2023-03-28 06:13:40.936931 lockss_turtles-0.4.0.dev1/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev1/LICENSE
--rw-r--r--   0        0        0    36115 2023-03-28 06:45:00.264670 lockss_turtles-0.4.0.dev1/README.rst
--rw-r--r--   0        0        0      976 2023-03-23 07:25:17.054405 lockss_turtles-0.4.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     3201 2023-03-23 07:25:17.051072 lockss_turtles-0.4.0.dev1/src/lockss/turtles/__init__.py
--rw-r--r--   0        0        0     1633 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev1/src/lockss/turtles/__main__.py
--rw-r--r--   0        0        0     9074 2023-03-28 03:37:09.141564 lockss_turtles-0.4.0.dev1/src/lockss/turtles/app.py
--rw-r--r--   0        0        0    21367 2023-03-28 06:12:08.865314 lockss_turtles-0.4.0.dev1/src/lockss/turtles/cli.py
--rw-r--r--   0        0        0     4312 2023-03-28 04:09:36.841384 lockss_turtles-0.4.0.dev1/src/lockss/turtles/plugin.py
--rw-r--r--   0        0        0     9445 2023-03-28 04:13:05.571566 lockss_turtles-0.4.0.dev1/src/lockss/turtles/plugin_registry.py
--rw-r--r--   0        0        0    10486 2023-03-28 03:40:12.508020 lockss_turtles-0.4.0.dev1/src/lockss/turtles/plugin_set.py
--rw-r--r--   0        0        0     1579 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/__init__.py
--rw-r--r--   0        0        0      685 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-registry-catalog-schema.json
--rw-r--r--   0        0        0     2766 2023-03-28 04:02:43.557727 lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-registry-schema.json
--rw-r--r--   0        0        0      650 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-set-catalog-schema.json
--rw-r--r--   0        0        0     2338 2023-03-04 21:54:35.657031 lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-set-schema.json
--rw-r--r--   0        0        0      753 2023-03-06 06:11:17.982107 lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-signing-credentials-schema.json
--rw-r--r--   0        0        0     2430 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev1/src/lockss/turtles/util.py
--rw-r--r--   0        0        0    37326 1970-01-01 00:00:00.000000 lockss_turtles-0.4.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-04-07 16:33:57.473442 lockss_turtles-0.4.0.dev2/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/LICENSE
+-rw-r--r--   0        0        0    38149 2023-05-02 19:16:12.800240 lockss_turtles-0.4.0.dev2/README.rst
+-rw-r--r--   0        0        0     1001 2023-05-02 19:16:18.990341 lockss_turtles-0.4.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     3201 2023-05-02 19:17:04.874415 lockss_turtles-0.4.0.dev2/src/lockss/turtles/__init__.py
+-rw-r--r--   0        0        0     1633 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/__main__.py
+-rw-r--r--   0        0        0     9074 2023-03-28 03:37:09.141564 lockss_turtles-0.4.0.dev2/src/lockss/turtles/app.py
+-rw-r--r--   0        0        0    22480 2023-04-07 16:33:57.473442 lockss_turtles-0.4.0.dev2/src/lockss/turtles/cli.py
+-rw-r--r--   0        0        0     4312 2023-03-28 04:09:36.841384 lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin.py
+-rw-r--r--   0        0        0     9445 2023-03-28 04:13:05.571566 lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_registry.py
+-rw-r--r--   0        0        0    10486 2023-03-28 03:40:12.508020 lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_set.py
+-rw-r--r--   0        0        0     1579 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/__init__.py
+-rw-r--r--   0        0        0      685 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-catalog-schema.json
+-rw-r--r--   0        0        0     2766 2023-03-28 04:02:43.557727 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-schema.json
+-rw-r--r--   0        0        0      650 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-catalog-schema.json
+-rw-r--r--   0        0        0     2338 2023-03-04 21:54:35.657031 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-schema.json
+-rw-r--r--   0        0        0      753 2023-03-06 06:11:17.982107 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-signing-credentials-schema.json
+-rw-r--r--   0        0        0     2430 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/util.py
+-rw-r--r--   0        0        0    39406 1970-01-01 00:00:00.000000 lockss_turtles-0.4.0.dev2/PKG-INFO
```

### Comparing `lockss_turtles-0.4.0.dev1/CHANGELOG.rst` & `lockss_turtles-0.4.0.dev2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 *  **Features**
 
    *  ``directory`` plugin registry layout now has the same file naming convention option as ``rcs``.
 
    *  New ``directory``/``rcs`` file naming convention ``underscore``: replace ``.`` in the plugin identifier by ``_`` and add ``.jar``.
 
+   *  CLI improvements.
+
 *  **Changes**
 
    *  The ``--output-format`` option is now only available in the context of commands where it makes sense.
 
 -----
 0.3.1
 -----
```

### Comparing `lockss_turtles-0.4.0.dev1/LICENSE` & `lockss_turtles-0.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/README.rst` & `lockss_turtles-0.4.0.dev2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =======
 Turtles
 =======
 
+.. |RELEASE| replace:: 0.4.0-dev2
+.. |RELEASE_DATE| replace:: ?
+
 .. |HELP| replace:: ``--help/-h``
 .. |IDENTIFIER| replace:: ``--identifier/-i``
 .. |IDENTIFIERS| replace:: ``--identifiers/-I``
 .. |JAR| replace:: ``--jar/-j``
 .. |JARS| replace:: ``--jars/-J``
 .. |LAYER| replace:: ``--layer/-l``
 .. |LAYERS| replace:: ``--layers/-L``
@@ -13,15 +16,15 @@
 .. |PLUGIN_SET_CATALOG| replace:: ``--plugin-set-catalog/-s``
 .. |PLUGIN_SIGNING_CREDENTIALS| replace:: ``--plugin-signing-credentials/-c``
 .. |PRODUCTION| replace:: ``--production/-p``
 .. |TESTING| replace:: ``--testing/-t``
 
 Turtles is a tool to manage LOCKSS plugin sets and LOCKSS plugin registries.
 
-**Latest release:** 0.4.0-dev1 (?)
+**Latest release:** |RELEASE| (|RELEASE_DATE|)
 
 -----------------
 Table of Contents
 -----------------
 
 *  `Installation`_
 
@@ -258,15 +261,24 @@
 *  Java Development Kit 8 (JDK).
 
 *  `Apache Maven <https://maven.apache.org/>`_.
 
 Maven Plugin Set Builder Declaration
 ++++++++++++++++++++++++++++++++++++
 
-For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure:
+For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure::
+
+    ---
+    kind: PluginSet
+    id: ...
+    name: ...
+    builder:
+      type: mvn
+      main: ...
+      test: ...
 
 ``type``
    *Required.* Must be set to ``mvn``.
 
 ``main``
    *Optional.* The path (relative to the root of the project) to the plugins' source code. *Default:* ``src/main/java``.
 
@@ -286,15 +298,24 @@
 *  `Apache Ant <https://ant.apache.org/>`_.
 
 *  ``JAVA_HOME`` must be set appropriately.
 
 Ant Plugin Set Builder Declaration
 ++++++++++++++++++++++++++++++++++
 
-For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure:
+For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure::
+
+    ---
+    kind: PluginSet
+    id: ...
+    name: ...
+    builder:
+      type: ant
+      main: ...
+      test: ...
 
 ``type``
    *Required.* Must be set to ``ant``.
 
 ``main``
    *Optional.* The path (relative to the root of the project) to the plugins' source code. *Default:* ``plugins/src``.
 
@@ -336,20 +357,14 @@
     kind: PluginRegistry
     id: mypluginregistry
     name: My Plugin Registry
     layout:
       type: ...
       ...
     layers:
-      - id: testing
-        name: My Plugin Registry (Testing)
-        path: /path/to/testing
-      - id: production
-        name: My Plugin Registry (Production)
-        path: /path/to/production
       - ...
     plugin-identifiers:
       - edu.myuniversity.plugin.publisherx.PublisherXPlugin
       - edu.myuniversity.plugin.publishery.PublisherYPlugin
       - ...
     suppressed-plugin-identifiers:
       - edu.myuniversity.plugin.old.OldPlugin
@@ -377,15 +392,15 @@
 
 ``layers``
    *Required.* A list of objects describing the layers of the plugin registry. See `Plugin Registry Layers`_ below.
 
 ``plugin-identifiers``
    *Required.* Non-empty list of the plugin identifiers in this plugin registry.
 
-``plugin-identifiers``
+``suppressed-plugin-identifiers``
    *Optional.* Non-empty list of plugin identifiers that are excluded from this plugin registry.
 
    Turtles does not currently do anything with this information, but it can be used to record plugins that have been abandoned or retracted over the lifetime of the plugin registry.
 
 Plugin Registry Layouts
 =======================
 
@@ -404,60 +419,117 @@
 ++++++++++++++++++++++++++++++++++++++++++++++
 
 None.
 
 Directory Plugin Registry Layout Declaration
 ++++++++++++++++++++++++++++++++++++++++++++
 
-For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure:
+For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure::
+
+    ---
+    kind: PluginRegistry
+    id: ...
+    name: ...
+    layout:
+      type: directory
+      file-naming-convention: ...
+    layers:
+      - ...
+    plugin-identifiers:
+      - ...
+    suppressed-plugin-identifiers:
+      - ...
 
 ``type``
    *Required.* Must be set to ``directory``.
 
-Currently, this layout type does not support the ``file-naming-convention`` option of the `RCS Plugin Registry Layout`_, but this feature will be introduced in a future release.
+``file-naming-convention``
+   *Optional.* A rule for what to name each deployed JAR file. If unspecified, the behavior is that of ``identifier``. Can be one of:
+
+   *  ``identifier``: Use the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu.myuniversity.plugin.publisherx.PublisherXPlugin.jar``.
+
+   *  ``underscore``: Replace ``.`` in the plugin identifier with ``_``, and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu_myuniversity_plugin_publisherx_PublisherXPlugin.jar``.
+
+   *  ``abbreviated``: Use the last dotted component of the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``PublisherXPlugin.jar``.
 
 RCS Plugin Registry Layout
 --------------------------
 
 In this specialization of the `Directory Plugin Registry Layout`_, each successive version of a given JAR is kept locally in RCS.
 
 RCS Plugin Registry Layout Prerequisites
 ++++++++++++++++++++++++++++++++++++++++
 
 *  `GNU RCS <https://www.gnu.org/software/rcs/>`_.
 
 RCS Plugin Registry Layout Declaration
 ++++++++++++++++++++++++++++++++++++++
 
-For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure:
+For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure::
+
+    ---
+    kind: PluginRegistry
+    id: ...
+    name: ...
+    layout:
+      type: rcs
+      file-naming-convention: ...
+    layers:
+      - ...
+    plugin-identifiers:
+      - ...
+    suppressed-plugin-identifiers:
+      - ...
 
 ``type``
    *Required.* Must be set to ``rcs``.
 
 ``file-naming-convention``
    *Optional.* A rule for what to name each deployed JAR file. If unspecified, the behavior is that of ``identifier``. Can be one of:
 
    *  ``identifier``: Use the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu.myuniversity.plugin.publisherx.PublisherXPlugin.jar``.
 
-   *  ``abbreviated``: Use the last component of the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``PublisherXPlugin.jar``.
+   *  ``underscore``: Replace ``.`` in the plugin identifier with ``_``, and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu_myuniversity_plugin_publisherx_PublisherXPlugin.jar``.
+
+   *  ``abbreviated``: Use the last dotted component of the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``PublisherXPlugin.jar``.
 
 Plugin Registry Layers
 ======================
 
 A plugin registry consists of one or more layers.
 
 Some plugin registries only one layer, in which case the LOCKSS boxes in a network using the plugin registry will get what is released to it. Some plugin registries may have two or more layers, with the additional layers used for plugin development or content processing quality assurance.
 
 Layers are sequential in nature; a new version of a plugin is released to the lowest layer first, then to the next layer (after some process), and so on until the highest layer. This sequencing is reflected in the ordering of the ``layers`` list in the plugin registry definition.
 
 Although the identifiers (see ``id`` below) and display names (see ``name`` below) of plugin registry layers are arbitrary, the highest layer is commonly referred to as the *production* layer, and when there are exactly two layers, the lower layer is commonly referred to as the *testing* layer. Turtles reflects this common idiom with built-in |PRODUCTION| and |TESTING| options that are shorthand for ``--layer=production`` and ``--layer=testing`` respectively.
 
 It is possible for multiple plugin registries to have a layer ``path`` in common. An example would be a team working on several plugin registries for different purposes, having distinct (public) production layer paths, but sharing a single (internal) testing layer path, if they are the only audience for it.
 
-A plugin registry layer is defined as one of the objects in the plugin registry definition's ``layers`` list. Each layer object has the following structure:
+A plugin registry layer is defined as one of the objects in the plugin registry definition's ``layers`` list. Each layer object has the following structure::
+
+    ---
+    kind: PluginRegistry
+    id: ...
+    name: ...
+    layout:
+      type: ...
+      ...
+    layers:
+      - id: testing
+        name: My Plugin Registry (Testing)
+        path: /path/to/testing
+      - id: production
+        name: My Plugin Registry (Production)
+        path: /path/to/production
+      - ...
+    plugin-identifiers:
+      - ...
+    suppressed-plugin-identifiers:
+      - ...
 
 ``id``
    *Required.* A short identifier for the plugin registry layer, for example ``testing``.
 
 ``name``
    *Required.* A display name for the plugin registry layer, for example ``My Plugin Registry (Testing)``.
 
@@ -564,15 +636,15 @@
     options:
       -h, --help            show this help message and exit
       --debug-cli           print the result of parsing command line arguments
       --non-interactive, -n
                             disallow interactive prompts (default: allow)
 
     commands:
-      Add --help to see the command's own help message
+      Add --help to see the command's own help message.
 
       COMMAND               DESCRIPTION
         build-plugin (bp)   build (package and sign) plugins
         copyright           show copyright and exit
         deploy-plugin (dp)  deploy plugins
         license             show license and exit
         release-plugin (rp)
@@ -589,15 +661,15 @@
 
     usage: turtles build-plugin [-h] [--output-format FMT] [--password PASS]
                                 [--plugin-set-catalog FILE]
                                 [--plugin-signing-credentials FILE]
                                 [--identifier PLUGID] [--identifiers FILE]
                                 [PLUGID ...]
 
-    Build (package and sign) plugins
+    Build (package and sign) plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -634,14 +706,16 @@
 
 *  `Plugin Signing Credentials`_, either from the |PLUGIN_SIGNING_CREDENTIALS| option or from ``plugin-signing-credentials.yaml`` in the `Configuration Files`_.
 
 *  A `Plugin Set Catalog`_, either from the |PLUGIN_SET_CATALOG| option or from ``plugin-set-catalog.yaml`` in the `Configuration Files`_.
 
 *  One or more plugin identifiers, from the `Plugin Identifier Arguments and Options`_ (bare arguments, |IDENTIFIER| options, |IDENTIFIERS| options).
 
+It also accepts `Options`_ for `Output Format Control`_
+
 Examples::
 
     # Help message
     turtles build-plugin --help
     # Abbreviation
     turtles bp -h
 
@@ -677,15 +751,15 @@
 
     usage: turtles deploy-plugin [-h] [--output-format FMT]
                                  [--plugin-registry-catalog FILE] [--production]
                                  [--testing] [--jar PLUGJAR] [--jars FILE]
                                  [--layer LAYER] [--layers FILE]
                                  [PLUGJAR ...]
 
-    Deploy plugins
+    Deploy plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -731,14 +805,16 @@
 
    *  The JAR paths listed as bare arguments to the command.
 
    *  The JAR paths listed as |JAR| options.
 
    *  The JAR paths found in the files listed as |JARS| options.
 
+It also accepts `Options`_ for `Output Format Control`_.
+
 Examples::
 
     # Help message
     turtles deploy-plugin --help
     # Abbreviation
     turtles dp -h
 
@@ -780,15 +856,15 @@
                                   [--plugin-set-catalog FILE]
                                   [--plugin-signing-credentials FILE]
                                   [--production] [--testing] [--identifier PLUGID]
                                   [--identifiers FILE] [--layer LAYER]
                                   [--layers FILE]
                                   [PLUGID ...]
 
-    Release (build and deploy) plugins
+    Release (build and deploy) plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -848,14 +924,16 @@
 
 *  A `Plugin Registry Catalog`_, either from the |PLUGIN_REGISTRY_CATALOG| option or from ``plugin-signing-credentials.yaml`` in the `Configuration Files`_.
 
 *  One or more plugin registry layer IDs, from the `Plugin Registry Layer Options`_ (|IDENTIFIER| options, |IDENTIFIERS| options, and alternatively, |TESTING| options, |PRODUCTION| option).
 
 *  One or more plugin identifiers, from the `Plugin Identifier Arguments and Options`_ (bare arguments, |IDENTIFIER| options, |IDENTIFIERS| options).
 
+It also accepts `Options`_ for `Output Format Control`_.
+
 Examples::
 
     # Help message
     turtles release-plugin --help
     # Abbreviation
     turtles rp -h
```

### Comparing `lockss_turtles-0.4.0.dev1/pyproject.toml` & `lockss_turtles-0.4.0.dev2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lockss-turtles"
-version = "0.4.0-dev1"
+version = "0.4.0-dev2"
 description = "Tool to manage LOCKSS plugin sets and LOCKSS plugin registries"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
@@ -25,14 +25,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 java-manifest = "^1.1.0"
 jsonschema = "^4.17.3"
 pyyaml = "^6.0"
+rich-argparse = "^1.1.0"
 tabulate = "^0.9.0"
 xdg = "^6.0.0"
 
 [tool.poetry.scripts]
 turtles = 'lockss.turtles.cli:main'
 
 [build-system]
```

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/__init__.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.4.0-dev1'
+__version__ = '0.4.0-dev2'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
```

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/__main__.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/__main__.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/app.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/app.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/cli.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import argparse
 import getpass
 from pathlib import Path
-import tabulate
 import sys
 
+import rich_argparse
+import tabulate
+
 import lockss.turtles
 from lockss.turtles.app import TurtlesApp
 from lockss.turtles.plugin_registry import PluginRegistryLayer
 from lockss.turtles.util import _path
 
 
 def _file_lines(path):
@@ -293,17 +295,25 @@
         group.add_argument('--layers', '-L',
                            metavar='FILE',
                            action='append',
                            default=list(),
                            help='add the layers in %(metavar)s to the list of plugin registry layers to process')
 
     def _make_parser(self):
-        self._parser = argparse.ArgumentParser(prog=TurtlesCli.PROG)
+        for cls in [rich_argparse.RichHelpFormatter]:
+            cls.styles.update({
+                'argparse.args': f'bold {cls.styles["argparse.args"]}',
+                'argparse.groups': f'bold {cls.styles["argparse.groups"]}',
+                'argparse.metavar': f'bold {cls.styles["argparse.metavar"]}',
+                'argparse.prog': f'bold {cls.styles["argparse.prog"]}',
+            })
+        self._parser = argparse.ArgumentParser(prog=TurtlesCli.PROG,
+                                               formatter_class=rich_argparse.RichHelpFormatter)
         self._subparsers = self._parser.add_subparsers(title='commands',
-                                                       description="Add --help to see the command's own help message",
+                                                       description="Add --help to see the command's own help message.",
                                                        # With subparsers, metavar is also used as the heading of the column of subcommands
                                                        metavar='COMMAND',
                                                        # With subparsers, help is used as the heading of the column of subcommand descriptions
                                                        help='DESCRIPTION')
         self._make_option_debug_cli(self._parser)
         self._make_option_non_interactive(self._parser)
         #self._make_parser_analyze_registry(self._subparsers)
@@ -322,72 +332,79 @@
     #     parser.set_defaults(fun=self._analyze_registry)
     #     self._make_option_plugin_registry_catalog(parser)
     #     self._make_option_plugin_set_catalog(parser)
     #     self._make_option_plugin_signing(parser)
 
     def _make_parser_build_plugin(self, container):
         parser = container.add_parser('build-plugin', aliases=['bp'],
-                                      description='Build (package and sign) plugins',
-                                      help='build (package and sign) plugins')
+                                      description='Build (package and sign) plugins.',
+                                      help='build (package and sign) plugins',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._build_plugin)
         self._make_option_output_format(parser)
         self._make_option_password(parser)
         self._make_option_plugin_set_catalog(parser)
         self._make_option_plugin_signing_credentials(parser)
         self._make_options_identifiers(parser)
 
     def _make_parser_copyright(self, container):
         parser = container.add_parser('copyright',
-                                      description='Show copyright and exit',
-                                      help='show copyright and exit')
+                                      description='Show copyright and exit.',
+                                      help='show copyright and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._copyright)
 
     def _make_parser_deploy_plugin(self, container):
         parser = container.add_parser('deploy-plugin', aliases=['dp'],
-                                      description='Deploy plugins',
-                                      help='deploy plugins')
+                                      description='Deploy plugins.',
+                                      help='deploy plugins',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._deploy_plugin)
         self._make_option_output_format(parser)
         self._make_option_plugin_registry_catalog(parser)
         self._make_option_production(parser)
         self._make_option_testing(parser)
         self._make_options_jars(parser)
         self._make_options_layers(parser)
 
     def _make_parser_license(self, container):
         parser = container.add_parser('license',
-                                      description='Show license and exit',
-                                      help='show license and exit')
+                                      description='Show license and exit.',
+                                      help='show license and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._license)
 
     def _make_parser_release_plugin(self, container):
         parser = container.add_parser('release-plugin', aliases=['rp'],
-                                      description='Release (build and deploy) plugins',
-                                      help='release (build and deploy) plugins')
+                                      description='Release (build and deploy) plugins.',
+                                      help='release (build and deploy) plugins',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._release_plugin)
         self._make_option_output_format(parser)
         self._make_option_password(parser)
         self._make_option_plugin_registry_catalog(parser)
         self._make_option_plugin_set_catalog(parser)
         self._make_option_plugin_signing_credentials(parser)
         self._make_option_production(parser)
         self._make_option_testing(parser)
         self._make_options_identifiers(parser)
         self._make_options_layers(parser)
 
     def _make_parser_usage(self, container):
         parser = container.add_parser('usage',
-                                      description='Show detailed usage and exit',
-                                      help='show detailed usage and exit')
+                                      description='Show detailed usage and exit.',
+                                      help='show detailed usage and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._usage)
 
     def _make_parser_version(self, container):
         parser = container.add_parser('version',
-                                      description='Show version and exit',
-                                      help='show version and exit')
+                                      description='Show version and exit.',
+                                      help='show version and exit',
+                                      formatter_class=self._parser.formatter_class)
         parser.set_defaults(fun=self._version)
 
     def _obtain_password(self):
         if self._args.password is not None:
             _p = self._args.password
         elif self._args.interactive:
             _p = getpass.getpass('Plugin signing password: ')
```

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/plugin.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/plugin_registry.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/plugin_set.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_set.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/__init__.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-registry-catalog-schema.json` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-catalog-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-registry-schema.json` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-set-catalog-schema.json` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-catalog-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-set-schema.json` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/resources/plugin-signing-credentials-schema.json` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-signing-credentials-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/src/lockss/turtles/util.py` & `lockss_turtles-0.4.0.dev2/src/lockss/turtles/util.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev1/PKG-INFO` & `lockss_turtles-0.4.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-turtles
-Version: 0.4.0.dev1
+Version: 0.4.0.dev2
 Summary: Tool to manage LOCKSS plugin sets and LOCKSS plugin registries
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,23 +19,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: java-manifest (>=1.1.0,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: rich-argparse (>=1.1.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Project-URL: Repository, https://github.com/lockss/lockss-turtles
 Description-Content-Type: text/x-rst
 
 =======
 Turtles
 =======
 
+.. |RELEASE| replace:: 0.4.0-dev2
+.. |RELEASE_DATE| replace:: ?
+
 .. |HELP| replace:: ``--help/-h``
 .. |IDENTIFIER| replace:: ``--identifier/-i``
 .. |IDENTIFIERS| replace:: ``--identifiers/-I``
 .. |JAR| replace:: ``--jar/-j``
 .. |JARS| replace:: ``--jars/-J``
 .. |LAYER| replace:: ``--layer/-l``
 .. |LAYERS| replace:: ``--layers/-L``
@@ -43,15 +47,15 @@
 .. |PLUGIN_SET_CATALOG| replace:: ``--plugin-set-catalog/-s``
 .. |PLUGIN_SIGNING_CREDENTIALS| replace:: ``--plugin-signing-credentials/-c``
 .. |PRODUCTION| replace:: ``--production/-p``
 .. |TESTING| replace:: ``--testing/-t``
 
 Turtles is a tool to manage LOCKSS plugin sets and LOCKSS plugin registries.
 
-**Latest release:** 0.4.0-dev1 (?)
+**Latest release:** |RELEASE| (|RELEASE_DATE|)
 
 -----------------
 Table of Contents
 -----------------
 
 *  `Installation`_
 
@@ -288,15 +292,24 @@
 *  Java Development Kit 8 (JDK).
 
 *  `Apache Maven <https://maven.apache.org/>`_.
 
 Maven Plugin Set Builder Declaration
 ++++++++++++++++++++++++++++++++++++
 
-For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure:
+For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure::
+
+    ---
+    kind: PluginSet
+    id: ...
+    name: ...
+    builder:
+      type: mvn
+      main: ...
+      test: ...
 
 ``type``
    *Required.* Must be set to ``mvn``.
 
 ``main``
    *Optional.* The path (relative to the root of the project) to the plugins' source code. *Default:* ``src/main/java``.
 
@@ -316,15 +329,24 @@
 *  `Apache Ant <https://ant.apache.org/>`_.
 
 *  ``JAVA_HOME`` must be set appropriately.
 
 Ant Plugin Set Builder Declaration
 ++++++++++++++++++++++++++++++++++
 
-For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure:
+For this plugin set builder type, the ``builder`` object in the plugin set definition has the following structure::
+
+    ---
+    kind: PluginSet
+    id: ...
+    name: ...
+    builder:
+      type: ant
+      main: ...
+      test: ...
 
 ``type``
    *Required.* Must be set to ``ant``.
 
 ``main``
    *Optional.* The path (relative to the root of the project) to the plugins' source code. *Default:* ``plugins/src``.
 
@@ -366,20 +388,14 @@
     kind: PluginRegistry
     id: mypluginregistry
     name: My Plugin Registry
     layout:
       type: ...
       ...
     layers:
-      - id: testing
-        name: My Plugin Registry (Testing)
-        path: /path/to/testing
-      - id: production
-        name: My Plugin Registry (Production)
-        path: /path/to/production
       - ...
     plugin-identifiers:
       - edu.myuniversity.plugin.publisherx.PublisherXPlugin
       - edu.myuniversity.plugin.publishery.PublisherYPlugin
       - ...
     suppressed-plugin-identifiers:
       - edu.myuniversity.plugin.old.OldPlugin
@@ -407,15 +423,15 @@
 
 ``layers``
    *Required.* A list of objects describing the layers of the plugin registry. See `Plugin Registry Layers`_ below.
 
 ``plugin-identifiers``
    *Required.* Non-empty list of the plugin identifiers in this plugin registry.
 
-``plugin-identifiers``
+``suppressed-plugin-identifiers``
    *Optional.* Non-empty list of plugin identifiers that are excluded from this plugin registry.
 
    Turtles does not currently do anything with this information, but it can be used to record plugins that have been abandoned or retracted over the lifetime of the plugin registry.
 
 Plugin Registry Layouts
 =======================
 
@@ -434,60 +450,117 @@
 ++++++++++++++++++++++++++++++++++++++++++++++
 
 None.
 
 Directory Plugin Registry Layout Declaration
 ++++++++++++++++++++++++++++++++++++++++++++
 
-For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure:
+For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure::
+
+    ---
+    kind: PluginRegistry
+    id: ...
+    name: ...
+    layout:
+      type: directory
+      file-naming-convention: ...
+    layers:
+      - ...
+    plugin-identifiers:
+      - ...
+    suppressed-plugin-identifiers:
+      - ...
 
 ``type``
    *Required.* Must be set to ``directory``.
 
-Currently, this layout type does not support the ``file-naming-convention`` option of the `RCS Plugin Registry Layout`_, but this feature will be introduced in a future release.
+``file-naming-convention``
+   *Optional.* A rule for what to name each deployed JAR file. If unspecified, the behavior is that of ``identifier``. Can be one of:
+
+   *  ``identifier``: Use the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu.myuniversity.plugin.publisherx.PublisherXPlugin.jar``.
+
+   *  ``underscore``: Replace ``.`` in the plugin identifier with ``_``, and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu_myuniversity_plugin_publisherx_PublisherXPlugin.jar``.
+
+   *  ``abbreviated``: Use the last dotted component of the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``PublisherXPlugin.jar``.
 
 RCS Plugin Registry Layout
 --------------------------
 
 In this specialization of the `Directory Plugin Registry Layout`_, each successive version of a given JAR is kept locally in RCS.
 
 RCS Plugin Registry Layout Prerequisites
 ++++++++++++++++++++++++++++++++++++++++
 
 *  `GNU RCS <https://www.gnu.org/software/rcs/>`_.
 
 RCS Plugin Registry Layout Declaration
 ++++++++++++++++++++++++++++++++++++++
 
-For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure:
+For this plugin registry layout type, the ``layout`` object in the plugin registry definition has the following structure::
+
+    ---
+    kind: PluginRegistry
+    id: ...
+    name: ...
+    layout:
+      type: rcs
+      file-naming-convention: ...
+    layers:
+      - ...
+    plugin-identifiers:
+      - ...
+    suppressed-plugin-identifiers:
+      - ...
 
 ``type``
    *Required.* Must be set to ``rcs``.
 
 ``file-naming-convention``
    *Optional.* A rule for what to name each deployed JAR file. If unspecified, the behavior is that of ``identifier``. Can be one of:
 
    *  ``identifier``: Use the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu.myuniversity.plugin.publisherx.PublisherXPlugin.jar``.
 
-   *  ``abbreviated``: Use the last component of the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``PublisherXPlugin.jar``.
+   *  ``underscore``: Replace ``.`` in the plugin identifier with ``_``, and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``edu_myuniversity_plugin_publisherx_PublisherXPlugin.jar``.
+
+   *  ``abbreviated``: Use the last dotted component of the plugin identifier and add ``.jar``. For example ``edu.myuniversity.plugin.publisherx.PublisherXPlugin`` results in ``PublisherXPlugin.jar``.
 
 Plugin Registry Layers
 ======================
 
 A plugin registry consists of one or more layers.
 
 Some plugin registries only one layer, in which case the LOCKSS boxes in a network using the plugin registry will get what is released to it. Some plugin registries may have two or more layers, with the additional layers used for plugin development or content processing quality assurance.
 
 Layers are sequential in nature; a new version of a plugin is released to the lowest layer first, then to the next layer (after some process), and so on until the highest layer. This sequencing is reflected in the ordering of the ``layers`` list in the plugin registry definition.
 
 Although the identifiers (see ``id`` below) and display names (see ``name`` below) of plugin registry layers are arbitrary, the highest layer is commonly referred to as the *production* layer, and when there are exactly two layers, the lower layer is commonly referred to as the *testing* layer. Turtles reflects this common idiom with built-in |PRODUCTION| and |TESTING| options that are shorthand for ``--layer=production`` and ``--layer=testing`` respectively.
 
 It is possible for multiple plugin registries to have a layer ``path`` in common. An example would be a team working on several plugin registries for different purposes, having distinct (public) production layer paths, but sharing a single (internal) testing layer path, if they are the only audience for it.
 
-A plugin registry layer is defined as one of the objects in the plugin registry definition's ``layers`` list. Each layer object has the following structure:
+A plugin registry layer is defined as one of the objects in the plugin registry definition's ``layers`` list. Each layer object has the following structure::
+
+    ---
+    kind: PluginRegistry
+    id: ...
+    name: ...
+    layout:
+      type: ...
+      ...
+    layers:
+      - id: testing
+        name: My Plugin Registry (Testing)
+        path: /path/to/testing
+      - id: production
+        name: My Plugin Registry (Production)
+        path: /path/to/production
+      - ...
+    plugin-identifiers:
+      - ...
+    suppressed-plugin-identifiers:
+      - ...
 
 ``id``
    *Required.* A short identifier for the plugin registry layer, for example ``testing``.
 
 ``name``
    *Required.* A display name for the plugin registry layer, for example ``My Plugin Registry (Testing)``.
 
@@ -594,15 +667,15 @@
     options:
       -h, --help            show this help message and exit
       --debug-cli           print the result of parsing command line arguments
       --non-interactive, -n
                             disallow interactive prompts (default: allow)
 
     commands:
-      Add --help to see the command's own help message
+      Add --help to see the command's own help message.
 
       COMMAND               DESCRIPTION
         build-plugin (bp)   build (package and sign) plugins
         copyright           show copyright and exit
         deploy-plugin (dp)  deploy plugins
         license             show license and exit
         release-plugin (rp)
@@ -619,15 +692,15 @@
 
     usage: turtles build-plugin [-h] [--output-format FMT] [--password PASS]
                                 [--plugin-set-catalog FILE]
                                 [--plugin-signing-credentials FILE]
                                 [--identifier PLUGID] [--identifiers FILE]
                                 [PLUGID ...]
 
-    Build (package and sign) plugins
+    Build (package and sign) plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -664,14 +737,16 @@
 
 *  `Plugin Signing Credentials`_, either from the |PLUGIN_SIGNING_CREDENTIALS| option or from ``plugin-signing-credentials.yaml`` in the `Configuration Files`_.
 
 *  A `Plugin Set Catalog`_, either from the |PLUGIN_SET_CATALOG| option or from ``plugin-set-catalog.yaml`` in the `Configuration Files`_.
 
 *  One or more plugin identifiers, from the `Plugin Identifier Arguments and Options`_ (bare arguments, |IDENTIFIER| options, |IDENTIFIERS| options).
 
+It also accepts `Options`_ for `Output Format Control`_
+
 Examples::
 
     # Help message
     turtles build-plugin --help
     # Abbreviation
     turtles bp -h
 
@@ -707,15 +782,15 @@
 
     usage: turtles deploy-plugin [-h] [--output-format FMT]
                                  [--plugin-registry-catalog FILE] [--production]
                                  [--testing] [--jar PLUGJAR] [--jars FILE]
                                  [--layer LAYER] [--layers FILE]
                                  [PLUGJAR ...]
 
-    Deploy plugins
+    Deploy plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -761,14 +836,16 @@
 
    *  The JAR paths listed as bare arguments to the command.
 
    *  The JAR paths listed as |JAR| options.
 
    *  The JAR paths found in the files listed as |JARS| options.
 
+It also accepts `Options`_ for `Output Format Control`_.
+
 Examples::
 
     # Help message
     turtles deploy-plugin --help
     # Abbreviation
     turtles dp -h
 
@@ -810,15 +887,15 @@
                                   [--plugin-set-catalog FILE]
                                   [--plugin-signing-credentials FILE]
                                   [--production] [--testing] [--identifier PLUGID]
                                   [--identifiers FILE] [--layer LAYER]
                                   [--layers FILE]
                                   [PLUGID ...]
 
-    Release (build and deploy) plugins
+    Release (build and deploy) plugins.
 
     options:
       -h, --help            show this help message and exit
       --output-format FMT   set tabular output format to FMT (default: simple;
                             choices: asciidoc, double_grid, double_outline,
                             fancy_grid, fancy_outline, github, grid, heavy_grid,
                             heavy_outline, html, jira, latex, latex_booktabs,
@@ -878,14 +955,16 @@
 
 *  A `Plugin Registry Catalog`_, either from the |PLUGIN_REGISTRY_CATALOG| option or from ``plugin-signing-credentials.yaml`` in the `Configuration Files`_.
 
 *  One or more plugin registry layer IDs, from the `Plugin Registry Layer Options`_ (|IDENTIFIER| options, |IDENTIFIERS| options, and alternatively, |TESTING| options, |PRODUCTION| option).
 
 *  One or more plugin identifiers, from the `Plugin Identifier Arguments and Options`_ (bare arguments, |IDENTIFIER| options, |IDENTIFIERS| options).
 
+It also accepts `Options`_ for `Output Format Control`_.
+
 Examples::
 
     # Help message
     turtles release-plugin --help
     # Abbreviation
     turtles rp -h
```

