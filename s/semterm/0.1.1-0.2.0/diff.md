# Comparing `tmp/semterm-0.1.1.tar.gz` & `tmp/semterm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semterm-0.1.1.tar", last modified: Tue May  2 00:58:00 2023, max compression
+gzip compressed data, was "semterm-0.2.0.tar", last modified: Tue May  2 05:58:02 2023, max compression
```

## Comparing `semterm-0.1.1.tar` & `semterm-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 00:57:40.000000 semterm-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 00:57:40.000000 semterm-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 00:58:00.400282 semterm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-02 00:57:40.000000 semterm-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 00:57:40.000000 semterm-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/UI/UserInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/agent/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/MrklAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/TerminalAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/TerminalAgentExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/TerminalAgentPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/config/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/langchain_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/langchain_extensions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/langchain_extensions/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/SemanticTerminalManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/SemanticTerminalProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/TerminalOutputParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/TerminalTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:57:40.000000 semterm-0.1.1/semterm/terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:00.400282 semterm-0.1.1/semterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 00:58:00.000000 semterm-0.1.1/semterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:58:00.400282 semterm-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 00:57:40.000000 semterm-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 05:57:42.000000 semterm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 05:57:42.000000 semterm-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 05:58:02.837864 semterm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-02 05:57:42.000000 semterm-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 05:57:42.000000 semterm-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.833863 semterm-0.2.0/semterm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.833863 semterm-0.2.0/semterm/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/UI/UserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/MrklAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/TerminalAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/TerminalAgentExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/TerminalAgentPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/config/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/langchain_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/langchain_extensions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/langchain_extensions/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/SemanticTerminalManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/SemanticTerminalProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/TerminalOutputParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/TerminalTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.833863 semterm-0.2.0/semterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:58:02.837864 semterm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 05:57:42.000000 semterm-0.2.0/setup.py
```

### Comparing `semterm-0.1.1/LICENSE` & `semterm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/README.md` & `semterm-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,45 +34,36 @@
   * tiktoken
   * pexpect 
   * pydantic
 * Linux (Debian-based recommended) or MacOS
 
 ## Installation 📦
 
-By default, the libraries use your `OPENAI_API_KEY` environment variable. You can set this variable in your `.bashrc` or `.zshrc` file:
+* Requires Python 3.10
 
-```bash
-export OPENAI_API_KEY="your-key-here"
-```
-
-1. Clone the SemTerm repository:
+Install via `pip`
 
 ```bash
-git clone https://github.com/lambrou/SemTerm
+pip install semterm
 ```
 
-2. Change into the project directory:
-
-```bash
-cd SemTerm
-```
+By default, the libraries use your `OPENAI_API_KEY` environment variable. 
 
-3. Install the required dependencies:
+You can set this variable in your `.bashrc` or `.zshrc` file:
 
 ```bash
-pip install -r requirements.txt
+export OPENAI_API_KEY="your-key-here"
 ```
 
-## Usage 🖥️ (Debian Package Coming Soon!)
+## Usage 🖥️
 
-```bash
-python -m semterm.main
-```
+Just type `semterm` in the terminal to get started!
 
 ```bash
+$ semterm
 You > Hey, will you spin me up a django project called more_human_than_human and run it?
 semterm > django-admin startproject more_human_than_human && cd more_human_than_human && python manage.py runserver
 
 You have 17 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
 Run 'python manage.py migrate' to apply them.
 May 01, 2023 - 18:19:51
 Django version 2.2.28, using settings 'more_human_than_human.settings'
```

### Comparing `semterm-0.1.1/semterm/agent/MrklAgent.py` & `semterm-0.2.0/semterm/agent/MrklAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/agent/TerminalAgent.py` & `semterm-0.2.0/semterm/agent/TerminalAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/agent/TerminalAgentExecutor.py` & `semterm-0.2.0/semterm/agent/TerminalAgentExecutor.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/langchain_extensions/tools.py` & `semterm-0.2.0/semterm/langchain_extensions/tools.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/terminal/SemanticTerminalManager.py` & `semterm-0.2.0/semterm/terminal/SemanticTerminalManager.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/terminal/SemanticTerminalProcess.py` & `semterm-0.2.0/semterm/terminal/SemanticTerminalProcess.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/terminal/TerminalOutputParser.py` & `semterm-0.2.0/semterm/terminal/TerminalOutputParser.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm/terminal/TerminalTool.py` & `semterm-0.2.0/semterm/terminal/TerminalTool.py`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/semterm.egg-info/SOURCES.txt` & `semterm-0.2.0/semterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semterm-0.1.1/setup.py` & `semterm-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="semterm",
-    version="0.1.1",
+    version="0.2.0",
     description="The Semantic Terminal",
     long_description="The Semantic Terminal",
     author="Lambrou",
     author_email="alexanderlambrou0602@gmail.com",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

