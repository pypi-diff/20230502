# Comparing `tmp/semterm-0.1.0.tar.gz` & `tmp/semterm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semterm-0.1.0.tar", last modified: Tue May  2 00:19:28 2023, max compression
+gzip compressed data, was "semterm-0.1.1.tar", last modified: Tue May  2 00:58:00 2023, max compression
```

## Comparing `semterm-0.1.0.tar` & `semterm-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.251297 semterm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 00:19:07.000000 semterm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 00:19:28.251297 semterm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-02 00:19:07.000000 semterm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 00:19:07.000000 semterm-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.247297 semterm-0.1.0/semterm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.247297 semterm-0.1.0/semterm/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/UI/UserInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.251297 semterm-0.1.0/semterm/agent/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/agent/MrklAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/agent/TerminalAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/agent/TerminalAgentExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/agent/TerminalAgentPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.251297 semterm-0.1.0/semterm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.251297 semterm-0.1.0/semterm/langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/langchain_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/langchain_extensions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/langchain_extensions/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.251297 semterm-0.1.0/semterm/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/terminal/SemanticTerminalManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/terminal/SemanticTerminalProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/terminal/TerminalOutputParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/terminal/TerminalTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:07.000000 semterm-0.1.0/semterm/terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:19:28.247297 semterm-0.1.0/semterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 00:19:28.000000 semterm-0.1.0/semterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-02 00:19:28.000000 semterm-0.1.0/semterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:19:28.000000 semterm-0.1.0/semterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 00:19:28.000000 semterm-0.1.0/semterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 00:19:28.000000 semterm-0.1.0/semterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 00:19:28.000000 semterm-0.1.0/semterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:19:28.251297 semterm-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 00:19:07.000000 semterm-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 00:57:40.000000 semterm-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 00:57:40.000000 semterm-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 00:58:00.400282 semterm-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-02 00:57:40.000000 semterm-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 00:57:40.000000 semterm-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/UI/UserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/MrklAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/TerminalAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/TerminalAgentExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/TerminalAgentPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/config/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/langchain_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/langchain_extensions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/langchain_extensions/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/SemanticTerminalManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/SemanticTerminalProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/TerminalOutputParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/TerminalTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:58:00.400282 semterm-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 00:57:40.000000 semterm-0.1.1/setup.py
```

### Comparing `semterm-0.1.0/LICENSE` & `semterm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/README.md` & `semterm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/agent/MrklAgent.py` & `semterm-0.1.1/semterm/agent/MrklAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/agent/TerminalAgent.py` & `semterm-0.1.1/semterm/agent/TerminalAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/agent/TerminalAgentExecutor.py` & `semterm-0.1.1/semterm/agent/TerminalAgentExecutor.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/agent/TerminalAgentPrompt.py` & `semterm-0.1.1/semterm/agent/TerminalAgentPrompt.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/langchain_extensions/tools.py` & `semterm-0.1.1/semterm/langchain_extensions/tools.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/terminal/SemanticTerminalManager.py` & `semterm-0.1.1/semterm/terminal/SemanticTerminalManager.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/terminal/SemanticTerminalProcess.py` & `semterm-0.1.1/semterm/terminal/SemanticTerminalProcess.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/terminal/TerminalOutputParser.py` & `semterm-0.1.1/semterm/terminal/TerminalOutputParser.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm/terminal/TerminalTool.py` & `semterm-0.1.1/semterm/terminal/TerminalTool.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.0/semterm.egg-info/SOURCES.txt` & `semterm-0.1.1/semterm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 semterm/__init__.py
 semterm/main.py
 semterm.egg-info/PKG-INFO
 semterm.egg-info/SOURCES.txt
@@ -15,14 +16,15 @@
 semterm/agent/MrklAgent.py
 semterm/agent/TerminalAgent.py
 semterm/agent/TerminalAgentExecutor.py
 semterm/agent/TerminalAgentPrompt.py
 semterm/agent/__init__.py
 semterm/config/Config.py
 semterm/config/__init__.py
+semterm/config/config.ini
 semterm/langchain_extensions/__init__.py
 semterm/langchain_extensions/schema.py
 semterm/langchain_extensions/tools.py
 semterm/terminal/SemanticTerminalManager.py
 semterm/terminal/SemanticTerminalProcess.py
 semterm/terminal/TerminalOutputParser.py
 semterm/terminal/TerminalTool.py
```

