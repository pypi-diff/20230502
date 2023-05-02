# Comparing `tmp/ou_container_builder-2.2.1.tar.gz` & `tmp/ou_container_builder-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_container_builder-2.2.1.tar", max compression
+gzip compressed data, was "ou_container_builder-2.3.0.tar", max compression
```

## Comparing `ou_container_builder-2.2.1.tar` & `ou_container_builder-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0       32 2022-11-30 14:12:19.917611 ou_container_builder-2.2.1/ou_container_builder/__init__.py
--rw-r--r--   0        0        0     1454 2022-11-30 14:12:19.917611 ou_container_builder-2.2.1/ou_container_builder/__main__.py
--rw-r--r--   0        0        0     6189 2022-11-30 14:12:19.917611 ou_container_builder-2.2.1/ou_container_builder/builder.py
--rw-r--r--   0        0        0      158 2022-11-30 14:12:19.918611 ou_container_builder-2.2.1/ou_container_builder/core/__init__.py
--rw-r--r--   0        0        0     1035 2022-11-30 14:12:19.918611 ou_container_builder-2.2.1/ou_container_builder/core/base.py
--rw-r--r--   0        0        0     2435 2022-11-30 14:12:19.918611 ou_container_builder-2.2.1/ou_container_builder/core/content.py
--rw-r--r--   0        0        0      815 2022-11-30 14:12:19.918611 ou_container_builder-2.2.1/ou_container_builder/core/env.py
--rw-r--r--   0        0        0     1137 2022-11-30 14:12:19.919611 ou_container_builder-2.2.1/ou_container_builder/core/hacks.py
--rw-r--r--   0        0        0     3096 2022-11-30 14:12:19.919611 ou_container_builder-2.2.1/ou_container_builder/core/jupyter_server.py
--rw-r--r--   0        0        0     1172 2022-11-30 14:12:19.919611 ou_container_builder-2.2.1/ou_container_builder/core/packages.py
--rw-r--r--   0        0        0     4219 2022-11-30 14:12:19.919611 ou_container_builder-2.2.1/ou_container_builder/core/scripts.py
--rw-r--r--   0        0        0     1522 2022-11-30 14:12:19.919611 ou_container_builder-2.2.1/ou_container_builder/core/services.py
--rw-r--r--   0        0        0     2216 2022-11-30 14:12:19.920611 ou_container_builder-2.2.1/ou_container_builder/core/startup.py
--rw-r--r--   0        0        0     2613 2022-11-30 14:12:19.920611 ou_container_builder-2.2.1/ou_container_builder/core/web_apps.py
--rw-r--r--   0        0        0      152 2022-11-30 14:12:19.920611 ou_container_builder-2.2.1/ou_container_builder/packs/__init__.py
--rw-r--r--   0        0        0     3952 2022-11-30 14:12:19.920611 ou_container_builder-2.2.1/ou_container_builder/packs/code_server.py
--rw-r--r--   0        0        0     1558 2022-11-30 14:12:19.921610 ou_container_builder-2.2.1/ou_container_builder/packs/jupyterlab.py
--rw-r--r--   0        0        0     2895 2022-11-30 14:12:19.921610 ou_container_builder-2.2.1/ou_container_builder/packs/mariadb.py
--rw-r--r--   0        0        0     1853 2022-11-30 14:12:19.921610 ou_container_builder-2.2.1/ou_container_builder/packs/nbclassic.py
--rw-r--r--   0        0        0     2733 2022-11-30 14:12:19.921610 ou_container_builder-2.2.1/ou_container_builder/packs/tutorial_server.py
--rw-r--r--   0        0        0     3599 2022-11-30 14:12:19.921610 ou_container_builder-2.2.1/ou_container_builder/templates/Dockerfile.jinja2
--rw-r--r--   0        0        0      990 2022-11-30 14:12:19.922611 ou_container_builder-2.2.1/ou_container_builder/templates/core/content/content_config.yaml
--rw-r--r--   0        0        0      190 2022-11-30 14:12:19.922611 ou_container_builder-2.2.1/ou_container_builder/templates/core/services/sudoers
--rw-r--r--   0        0        0      140 2022-11-30 14:12:19.922611 ou_container_builder-2.2.1/ou_container_builder/templates/core/startup/home-dir.sudoers
--rw-r--r--   0        0        0      486 2022-11-30 14:12:19.922611 ou_container_builder-2.2.1/ou_container_builder/templates/core/startup/start.sh
--rw-r--r--   0        0        0     4451 2022-11-30 14:12:19.923611 ou_container_builder-2.2.1/ou_container_builder/templates/packs/code_server/vscode.svg
--rw-r--r--   0        0        0      615 2022-11-30 14:12:19.923611 ou_container_builder-2.2.1/ou_container_builder/templates/packs/mariadb/setup.sh
--rw-r--r--   0        0        0      942 2022-11-30 14:12:19.923611 ou_container_builder-2.2.1/ou_container_builder/templates/packs/tutorial-server/production.ini
--rw-r--r--   0        0        0     2142 2022-11-30 14:12:19.924610 ou_container_builder-2.2.1/ou_container_builder/utils.py
--rw-r--r--   0        0        0    12432 2022-11-30 14:12:19.924610 ou_container_builder-2.2.1/ou_container_builder/validator.py
--rw-r--r--   0        0        0      629 2022-11-30 14:12:19.925611 ou_container_builder-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 ou_container_builder-2.2.1/setup.py
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 ou_container_builder-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/__init__.py
+-rw-r--r--   0        0        0     1454 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/__main__.py
+-rw-r--r--   0        0        0     6189 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/builder.py
+-rw-r--r--   0        0        0      158 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/__init__.py
+-rw-r--r--   0        0        0     1035 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/base.py
+-rw-r--r--   0        0        0     2435 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/content.py
+-rw-r--r--   0        0        0      815 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/env.py
+-rw-r--r--   0        0        0     1137 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/hacks.py
+-rw-r--r--   0        0        0     3096 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/jupyter_server.py
+-rw-r--r--   0        0        0     1172 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/packages.py
+-rw-r--r--   0        0        0     4219 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/scripts.py
+-rw-r--r--   0        0        0     1522 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/services.py
+-rw-r--r--   0        0        0     2216 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/startup.py
+-rw-r--r--   0        0        0     2613 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/web_apps.py
+-rw-r--r--   0        0        0      152 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/__init__.py
+-rw-r--r--   0        0        0     4579 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/code_server.py
+-rw-r--r--   0        0        0     1558 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/jupyterlab.py
+-rw-r--r--   0        0        0     2895 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/mariadb.py
+-rw-r--r--   0        0        0     1853 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/packs/nbclassic.py
+-rw-r--r--   0        0        0     2733 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/packs/tutorial_server.py
+-rw-r--r--   0        0        0     3599 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/Dockerfile.jinja2
+-rw-r--r--   0        0        0      990 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/content/content_config.yaml
+-rw-r--r--   0        0        0      190 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/services/sudoers
+-rw-r--r--   0        0        0      140 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/startup/home-dir.sudoers
+-rw-r--r--   0        0        0      486 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/startup/start.sh
+-rw-r--r--   0        0        0     4451 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/packs/code_server/vscode.svg
+-rw-r--r--   0        0        0      615 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/templates/packs/mariadb/setup.sh
+-rw-r--r--   0        0        0      942 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/templates/packs/tutorial-server/production.ini
+-rw-r--r--   0        0        0     2142 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/utils.py
+-rw-r--r--   0        0        0    12432 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/validator.py
+-rw-r--r--   0        0        0      629 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 ou_container_builder-2.3.0/PKG-INFO
```

### Comparing `ou_container_builder-2.2.1/ou_container_builder/__main__.py` & `ou_container_builder-2.3.0/ou_container_builder/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/builder.py` & `ou_container_builder-2.3.0/ou_container_builder/builder.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/base.py` & `ou_container_builder-2.3.0/ou_container_builder/core/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/content.py` & `ou_container_builder-2.3.0/ou_container_builder/core/content.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/env.py` & `ou_container_builder-2.3.0/ou_container_builder/core/env.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/hacks.py` & `ou_container_builder-2.3.0/ou_container_builder/core/hacks.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/jupyter_server.py` & `ou_container_builder-2.3.0/ou_container_builder/core/jupyter_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/packages.py` & `ou_container_builder-2.3.0/ou_container_builder/core/packages.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/scripts.py` & `ou_container_builder-2.3.0/ou_container_builder/core/scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/services.py` & `ou_container_builder-2.3.0/ou_container_builder/core/services.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/startup.py` & `ou_container_builder-2.3.0/ou_container_builder/core/startup.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/core/web_apps.py` & `ou_container_builder-2.3.0/ou_container_builder/core/web_apps.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/packs/code_server.py` & `ou_container_builder-2.3.0/ou_container_builder/packs/code_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :param pack_settings: The pack-specific settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
+    if 'version' in pack_settings:
+        version = pack_settings['version']
+    else:
+        version = '4.12.0'
     warn('Automatically setting the code_server as the default web-app is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.', FutureWarning)  # noqa: E501
     settings = merge_settings(settings, {
         'sources': {
             'apt': [
                 {
                     'name': 'nodesource',
                     'key_url': 'https://deb.nodesource.com/gpgkey/nodesource.gpg.key',
@@ -41,17 +45,17 @@
             ],
         },
         'scripts': {
             'build': [
                 {
                     'commands': [
                         'cd /opt',
-                        'wget https://github.com/coder/code-server/releases/download/v4.6.1/code-server-4.6.1-linux-amd64.tar.gz',  # noqa: E501
-                        'tar -zxvf code-server-4.6.1-linux-amd64.tar.gz',
-                        'ln -s /opt/code-server-4.6.1-linux-amd64/bin/code-server /usr/local/bin',
+                        f'curl -L --output code-server.tar.gz https://github.com/coder/code-server/releases/download/v{version}/code-server-{version}-linux-amd64.tar.gz',  # noqa: E501
+                        'tar -zxvf code-server.tar.gz',
+                        f'ln -s /opt/code-server-{version}-linux-amd64/bin/code-server /usr/local/bin',
                     ]
                 }
             ]
         },
         'content': [
             {
                 'source': 'ou-builder-build/packs/code_server/logo.svg',
@@ -78,14 +82,27 @@
                 'launcher_entry': {
                     'title': 'VS Code',
                     'icon_path': '/var/lib/code_server/logo.svg'
                 }
             }
         ],
     })
+    if 'extensions' in pack_settings and isinstance(pack_settings['extensions'], list):
+        settings = merge_settings(settings, {
+            'scripts': {
+                'build': [
+                    {
+                        'commands': [
+                            f'code-server --install-extension {extension}'
+                            for extension in pack_settings['extensions']
+                        ]
+                    }
+                ]
+            }
+        })
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> None:
     """Generate the build files for the code-server pack.
 
     This ensures that the the code-server is installed
```

### Comparing `ou_container_builder-2.2.1/ou_container_builder/packs/jupyterlab.py` & `ou_container_builder-2.3.0/ou_container_builder/packs/jupyterlab.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/packs/mariadb.py` & `ou_container_builder-2.3.0/ou_container_builder/packs/mariadb.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/packs/nbclassic.py` & `ou_container_builder-2.3.0/ou_container_builder/packs/nbclassic.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/packs/tutorial_server.py` & `ou_container_builder-2.3.0/ou_container_builder/packs/tutorial_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/templates/Dockerfile.jinja2` & `ou_container_builder-2.3.0/ou_container_builder/templates/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/templates/core/content/content_config.yaml` & `ou_container_builder-2.3.0/ou_container_builder/templates/core/content/content_config.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/templates/packs/code_server/vscode.svg` & `ou_container_builder-2.3.0/ou_container_builder/templates/packs/code_server/vscode.svg`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/templates/packs/mariadb/setup.sh` & `ou_container_builder-2.3.0/ou_container_builder/templates/packs/mariadb/setup.sh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/templates/packs/tutorial-server/production.ini` & `ou_container_builder-2.3.0/ou_container_builder/templates/packs/tutorial-server/production.ini`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/utils.py` & `ou_container_builder-2.3.0/ou_container_builder/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/ou_container_builder/validator.py` & `ou_container_builder-2.3.0/ou_container_builder/validator.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.2.1/pyproject.toml` & `ou_container_builder-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ou-container-builder"
-version = "2.2.1"
+version = "2.3.0"
 description = ""
 authors = ["Mark Hall <mark.hall@open.ac.uk>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyyaml = "^5.4.1"
 jinja2 = "^3.0.0"
```

### Comparing `ou_container_builder-2.2.1/PKG-INFO` & `ou_container_builder-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-container-builder
-Version: 2.2.1
+Version: 2.3.0
 Summary: 
 Author: Mark Hall
 Author-email: mark.hall@open.ac.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

