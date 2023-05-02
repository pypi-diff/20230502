# Comparing `tmp/mell-2.0.5.tar.gz` & `tmp/mell-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mell-2.0.5.tar", last modified: Tue May  2 13:38:50 2023, max compression
+gzip compressed data, was "mell-2.0.6.tar", last modified: Tue May  2 13:40:44 2023, max compression
```

## Comparing `mell-2.0.5.tar` & `mell-2.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:38:50.439722 mell-2.0.5/
--rw-rw-r--   0 diego     (1000) diego     (1000)     9348 2023-05-02 13:38:50.439722 mell-2.0.5/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     8919 2023-04-29 19:11:57.000000 mell-2.0.5/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:38:50.439722 mell-2.0.5/mell/
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.5/mell/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-05-02 13:38:49.000000 mell-2.0.5/mell/consts.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)    25557 2023-04-27 15:32:46.000000 mell-2.0.5/mell/main.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:38:50.439722 mell-2.0.5/mell.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     9348 2023-05-02 13:38:50.000000 mell-2.0.5/mell.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      316 2023-05-02 13:38:50.000000 mell-2.0.5/mell.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-02 13:38:50.000000 mell-2.0.5/mell.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-05-02 13:38:50.000000 mell-2.0.5/mell.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-05-02 13:38:50.000000 mell-2.0.5/mell.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-05-02 13:38:50.000000 mell-2.0.5/mell.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-02 13:38:50.439722 mell-2.0.5/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.5/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:38:50.439722 mell-2.0.5/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     1156 2023-04-29 14:53:17.000000 mell-2.0.5/tests/test_logic.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     2103 2023-04-29 14:55:06.000000 mell-2.0.5/tests/test_metadata.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1785 2023-04-29 14:55:27.000000 mell-2.0.5/tests/test_news.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1959 2023-04-29 14:28:44.000000 mell-2.0.5/tests/test_plugin.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.027508 mell-2.0.6/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     9172 2023-05-02 13:40:44.027508 mell-2.0.6/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     8743 2023-05-02 13:39:44.000000 mell-2.0.6/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.023508 mell-2.0.6/mell/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.6/mell/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-05-02 13:40:41.000000 mell-2.0.6/mell/consts.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    25557 2023-04-27 15:32:46.000000 mell-2.0.6/mell/main.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.023508 mell-2.0.6/mell.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     9172 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      316 2023-05-02 13:40:44.000000 mell-2.0.6/mell.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-02 13:40:44.027508 mell-2.0.6/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.6/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.027508 mell-2.0.6/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1156 2023-04-29 14:53:17.000000 mell-2.0.6/tests/test_logic.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2103 2023-04-29 14:55:06.000000 mell-2.0.6/tests/test_metadata.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1785 2023-04-29 14:55:27.000000 mell-2.0.6/tests/test_news.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1959 2023-04-29 14:28:44.000000 mell-2.0.6/tests/test_plugin.py
```

### Comparing `mell-2.0.5/PKG-INFO` & `mell-2.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.5
+Version: 2.0.6
 Summary: Generate anything from template files and metadata files!
 Home-page: https://github.com/diegofps/mell
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,34 +13,34 @@
 
 # Mell
 
 Mell is a tool designed to generate anything from template files and metadata files. You can use it to generate a single file or an entire projects composed of thousands of files. It works like a preprocessor, generating code before the compilation-time. Its name is an acronym for MEtaprogramming Logic Layer, meaning its a logical layer infering pieces of code to be generated.
 
 [![Tests](https://github.com/diegofps/mell/actions/workflows/python-app.yml/badge.svg)](https://github.com/diegofps/mell/actions/workflows/python-app.yml)
 
-# When should I use Mell? <font size="5">⭐</font>
+# When should I use Mell? ⭐
 
 Sometimes it is useful to render an entire project, not only an e-mail or a single webpage, like in a webserver response. This is when mell comes to help. So far, I have used it in the following situations:
 
 * Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
 * Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
 * Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
 Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
 As an example, consider the situation that we have metadata describing a mobile app and a style that can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on different platforms, like an IOS app.
 
 
-# When should I not use Mell? <font size="5">🚫</font>
+# When should I not use Mell? 🚫
 
 I don't recommend using this if you are not confortable programming in the stack you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just the same with a few different parameters. These few parameters will likely become your metadata when you use mell.
 
 You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
-# Concepts <font size="5">📕</font>
+# Concepts 📕
 
 To use this library, you must understand at least the following concepts:
 
 * `metadata:` The data describing what we want to generate. It is written using the json format.
 * `style:` Set of scripts, templates, and assets that will transform the metadata into something else.
 * `generated folder:` This is where the rendered files will be saved. You must never change these files as they will be overwritten the next time you execute mell. 
 
@@ -48,30 +48,30 @@
 
 * `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
 * `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
 * `asset:` files used by your style that are not automatically used by mell.
 * `plugin:` Scripts that will be automatically executed by mell. These scripts will usually interact with the `inflater` variable to generate multiple output files. It may load template files from the asset folder.
 * `logic:` Scripts that will be automatically executed, in order, by mell. These are used to validate and extend the metadata.
 
-# How to install / uninstall it? <font size="5">🚀</font>
+# How to install / uninstall it? 🚀
 
 ```shell
 # To install
 pip install mell
 
 # To upgrade
 pip install --upgrade mell
 
 # To uninstall
 pip uninstall mell
 ```
 
 After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your `$PATH` variable includes the local bin folder, tipicaly `~/.local/bin`; (2) install it in a virtual environment, like `virtualenv`; or (3) try to install it at the system level, running pip as root (should not be necessary);
 
-# Basic Usage <font size="5">🐣</font>
+# Basic Usage 🐣
 
 Create a project to hold your generator.
 
 ```shell
 mell --new test_project
 cd test_project
 ```
@@ -101,15 +101,15 @@
 The following is the content of `generate/example.txt`, created by mell using the metadata we specified and the style folder in this project.
 
 ```python
 for _ in range(33):
     print("I am hungry!")
 ```
 
-# Documentation <font size="5">📚</font>
+# Documentation 📚
 
 ## Hands on
 
 * [Generating Programs](https://github.com/diegofps/mell/blob/main/docs/hands_on/metadata.md) - Example showing the concept and how to generate 4 programs using 2 styles and 2 metadata files.
 * [Metadata](https://github.com/diegofps/mell/blob/main/docs/hands_on/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
 * [Template](https://github.com/diegofps/mell/blob/main/docs/hands_on/template.md) - Explains the template syntax and how to customize it;
 * [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/hands_on/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
@@ -117,15 +117,15 @@
 
 ## Extra concepts
 
 * [Basic Folder Structure](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/folder_structure.md) - describes the role of each folder.
 * [The variables args, meta, and inflater](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/variables.md) - describes the role of the special variables.
 * [Understanding the Pipeline](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/pipeline.md) - describes the order that mell processes everything.
 
-# TL;DR <font size="5">💻</font>
+# TL;DR 💻
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
 mell --new project_name
 
 # This will create a folder named style2 with the recommended style folder structure (use it inside the root directory to keep things organized)
 mell --new-style project_name
@@ -168,11 +168,11 @@
 # An example with custom style names, distinct output folders and two metadata files. We are assuming the style folders are on local directory and named python and cpp.
 mell --style styles/python --generate generates/python/en en
 mell --style styles/python --generate generates/python/pt pt
 mell --style styles/cpp --generate generates/cpp/en en
 mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
-# Source Code <font size="5">🎼</font>
+# Source Code 🎼
 
 The source code is available in the project's [repository](https://github.com/diegofps/mell).
```

### Comparing `mell-2.0.5/README.md` & `mell-2.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Mell
 
 Mell is a tool designed to generate anything from template files and metadata files. You can use it to generate a single file or an entire projects composed of thousands of files. It works like a preprocessor, generating code before the compilation-time. Its name is an acronym for MEtaprogramming Logic Layer, meaning its a logical layer infering pieces of code to be generated.
 
 [![Tests](https://github.com/diegofps/mell/actions/workflows/python-app.yml/badge.svg)](https://github.com/diegofps/mell/actions/workflows/python-app.yml)
 
-# When should I use Mell? <font size="5">⭐</font>
+# When should I use Mell? ⭐
 
 Sometimes it is useful to render an entire project, not only an e-mail or a single webpage, like in a webserver response. This is when mell comes to help. So far, I have used it in the following situations:
 
 * Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
 * Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
 * Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
 Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
 As an example, consider the situation that we have metadata describing a mobile app and a style that can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on different platforms, like an IOS app.
 
 
-# When should I not use Mell? <font size="5">🚫</font>
+# When should I not use Mell? 🚫
 
 I don't recommend using this if you are not confortable programming in the stack you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just the same with a few different parameters. These few parameters will likely become your metadata when you use mell.
 
 You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
-# Concepts <font size="5">📕</font>
+# Concepts 📕
 
 To use this library, you must understand at least the following concepts:
 
 * `metadata:` The data describing what we want to generate. It is written using the json format.
 * `style:` Set of scripts, templates, and assets that will transform the metadata into something else.
 * `generated folder:` This is where the rendered files will be saved. You must never change these files as they will be overwritten the next time you execute mell. 
 
@@ -35,30 +35,30 @@
 
 * `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
 * `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
 * `asset:` files used by your style that are not automatically used by mell.
 * `plugin:` Scripts that will be automatically executed by mell. These scripts will usually interact with the `inflater` variable to generate multiple output files. It may load template files from the asset folder.
 * `logic:` Scripts that will be automatically executed, in order, by mell. These are used to validate and extend the metadata.
 
-# How to install / uninstall it? <font size="5">🚀</font>
+# How to install / uninstall it? 🚀
 
 ```shell
 # To install
 pip install mell
 
 # To upgrade
 pip install --upgrade mell
 
 # To uninstall
 pip uninstall mell
 ```
 
 After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your `$PATH` variable includes the local bin folder, tipicaly `~/.local/bin`; (2) install it in a virtual environment, like `virtualenv`; or (3) try to install it at the system level, running pip as root (should not be necessary);
 
-# Basic Usage <font size="5">🐣</font>
+# Basic Usage 🐣
 
 Create a project to hold your generator.
 
 ```shell
 mell --new test_project
 cd test_project
 ```
@@ -88,15 +88,15 @@
 The following is the content of `generate/example.txt`, created by mell using the metadata we specified and the style folder in this project.
 
 ```python
 for _ in range(33):
     print("I am hungry!")
 ```
 
-# Documentation <font size="5">📚</font>
+# Documentation 📚
 
 ## Hands on
 
 * [Generating Programs](https://github.com/diegofps/mell/blob/main/docs/hands_on/metadata.md) - Example showing the concept and how to generate 4 programs using 2 styles and 2 metadata files.
 * [Metadata](https://github.com/diegofps/mell/blob/main/docs/hands_on/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
 * [Template](https://github.com/diegofps/mell/blob/main/docs/hands_on/template.md) - Explains the template syntax and how to customize it;
 * [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/hands_on/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
@@ -104,15 +104,15 @@
 
 ## Extra concepts
 
 * [Basic Folder Structure](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/folder_structure.md) - describes the role of each folder.
 * [The variables args, meta, and inflater](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/variables.md) - describes the role of the special variables.
 * [Understanding the Pipeline](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/pipeline.md) - describes the order that mell processes everything.
 
-# TL;DR <font size="5">💻</font>
+# TL;DR 💻
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
 mell --new project_name
 
 # This will create a folder named style2 with the recommended style folder structure (use it inside the root directory to keep things organized)
 mell --new-style project_name
@@ -155,11 +155,11 @@
 # An example with custom style names, distinct output folders and two metadata files. We are assuming the style folders are on local directory and named python and cpp.
 mell --style styles/python --generate generates/python/en en
 mell --style styles/python --generate generates/python/pt pt
 mell --style styles/cpp --generate generates/cpp/en en
 mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
-# Source Code <font size="5">🎼</font>
+# Source Code 🎼
 
 The source code is available in the project's [repository](https://github.com/diegofps/mell).
```

### Comparing `mell-2.0.5/mell/main.py` & `mell-2.0.6/mell/main.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.5/mell.egg-info/PKG-INFO` & `mell-2.0.6/mell.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.5
+Version: 2.0.6
 Summary: Generate anything from template files and metadata files!
 Home-page: https://github.com/diegofps/mell
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,34 +13,34 @@
 
 # Mell
 
 Mell is a tool designed to generate anything from template files and metadata files. You can use it to generate a single file or an entire projects composed of thousands of files. It works like a preprocessor, generating code before the compilation-time. Its name is an acronym for MEtaprogramming Logic Layer, meaning its a logical layer infering pieces of code to be generated.
 
 [![Tests](https://github.com/diegofps/mell/actions/workflows/python-app.yml/badge.svg)](https://github.com/diegofps/mell/actions/workflows/python-app.yml)
 
-# When should I use Mell? <font size="5">⭐</font>
+# When should I use Mell? ⭐
 
 Sometimes it is useful to render an entire project, not only an e-mail or a single webpage, like in a webserver response. This is when mell comes to help. So far, I have used it in the following situations:
 
 * Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
 * Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
 * Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
 Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
 As an example, consider the situation that we have metadata describing a mobile app and a style that can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on different platforms, like an IOS app.
 
 
-# When should I not use Mell? <font size="5">🚫</font>
+# When should I not use Mell? 🚫
 
 I don't recommend using this if you are not confortable programming in the stack you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just the same with a few different parameters. These few parameters will likely become your metadata when you use mell.
 
 You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
-# Concepts <font size="5">📕</font>
+# Concepts 📕
 
 To use this library, you must understand at least the following concepts:
 
 * `metadata:` The data describing what we want to generate. It is written using the json format.
 * `style:` Set of scripts, templates, and assets that will transform the metadata into something else.
 * `generated folder:` This is where the rendered files will be saved. You must never change these files as they will be overwritten the next time you execute mell. 
 
@@ -48,30 +48,30 @@
 
 * `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
 * `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
 * `asset:` files used by your style that are not automatically used by mell.
 * `plugin:` Scripts that will be automatically executed by mell. These scripts will usually interact with the `inflater` variable to generate multiple output files. It may load template files from the asset folder.
 * `logic:` Scripts that will be automatically executed, in order, by mell. These are used to validate and extend the metadata.
 
-# How to install / uninstall it? <font size="5">🚀</font>
+# How to install / uninstall it? 🚀
 
 ```shell
 # To install
 pip install mell
 
 # To upgrade
 pip install --upgrade mell
 
 # To uninstall
 pip uninstall mell
 ```
 
 After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your `$PATH` variable includes the local bin folder, tipicaly `~/.local/bin`; (2) install it in a virtual environment, like `virtualenv`; or (3) try to install it at the system level, running pip as root (should not be necessary);
 
-# Basic Usage <font size="5">🐣</font>
+# Basic Usage 🐣
 
 Create a project to hold your generator.
 
 ```shell
 mell --new test_project
 cd test_project
 ```
@@ -101,15 +101,15 @@
 The following is the content of `generate/example.txt`, created by mell using the metadata we specified and the style folder in this project.
 
 ```python
 for _ in range(33):
     print("I am hungry!")
 ```
 
-# Documentation <font size="5">📚</font>
+# Documentation 📚
 
 ## Hands on
 
 * [Generating Programs](https://github.com/diegofps/mell/blob/main/docs/hands_on/metadata.md) - Example showing the concept and how to generate 4 programs using 2 styles and 2 metadata files.
 * [Metadata](https://github.com/diegofps/mell/blob/main/docs/hands_on/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
 * [Template](https://github.com/diegofps/mell/blob/main/docs/hands_on/template.md) - Explains the template syntax and how to customize it;
 * [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/hands_on/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
@@ -117,15 +117,15 @@
 
 ## Extra concepts
 
 * [Basic Folder Structure](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/folder_structure.md) - describes the role of each folder.
 * [The variables args, meta, and inflater](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/variables.md) - describes the role of the special variables.
 * [Understanding the Pipeline](https://github.com/diegofps/mell/blob/main/docs/extra_concepts/pipeline.md) - describes the order that mell processes everything.
 
-# TL;DR <font size="5">💻</font>
+# TL;DR 💻
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
 mell --new project_name
 
 # This will create a folder named style2 with the recommended style folder structure (use it inside the root directory to keep things organized)
 mell --new-style project_name
@@ -168,11 +168,11 @@
 # An example with custom style names, distinct output folders and two metadata files. We are assuming the style folders are on local directory and named python and cpp.
 mell --style styles/python --generate generates/python/en en
 mell --style styles/python --generate generates/python/pt pt
 mell --style styles/cpp --generate generates/cpp/en en
 mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
-# Source Code <font size="5">🎼</font>
+# Source Code 🎼
 
 The source code is available in the project's [repository](https://github.com/diegofps/mell).
```

### Comparing `mell-2.0.5/setup.py` & `mell-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.5/tests/test_logic.py` & `mell-2.0.6/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.5/tests/test_metadata.py` & `mell-2.0.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.5/tests/test_news.py` & `mell-2.0.6/tests/test_news.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.5/tests/test_plugin.py` & `mell-2.0.6/tests/test_plugin.py`

 * *Files identical despite different names*

