# Comparing `tmp/jncep-42.tar.gz` & `tmp/jncep-43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jncep-42.tar", last modified: Sat Feb 25 14:27:21 2023, max compression
+gzip compressed data, was "dist/jncep-43.tar", last modified: Tue May  2 21:44:38 2023, max compression
```

## Comparing `jncep-42.tar` & `jncep-43.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-25 14:27:21.000000 jncep-42/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-25 14:27:21.000000 jncep-42/jncep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-02-25 14:27:20.000000 jncep-42/jncep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-02-25 14:27:20.000000 jncep-42/jncep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-25 14:27:20.000000 jncep-42/jncep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-25 14:27:20.000000 jncep-42/jncep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-02-25 14:27:20.000000 jncep-42/jncep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    36313 2023-02-25 14:27:20.000000 jncep-42/jncep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    30324 2023-02-25 14:26:51.000000 jncep-42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-25 14:27:21.000000 jncep-42/jncep/
--rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-02-25 14:26:51.000000 jncep-42/jncep/spec.py
--rw-r--r--   0 runner    (1001) docker     (122)    10251 2023-02-25 14:26:51.000000 jncep-42/jncep/jnclabs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-02-25 14:26:51.000000 jncep-42/jncep/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-25 14:27:21.000000 jncep-42/jncep/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/track.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-02-25 14:26:51.000000 jncep-42/jncep/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-02-25 14:26:51.000000 jncep-42/jncep/jncweb.py
--rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-02-25 14:26:51.000000 jncep-42/jncep/trio_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-02-25 14:26:51.000000 jncep-42/jncep/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-02-25 14:26:51.000000 jncep-42/jncep/jncep.py
--rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-02-25 14:26:51.000000 jncep-42/jncep/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     7629 2023-02-25 14:26:51.000000 jncep-42/jncep/track.py
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-02-25 14:26:51.000000 jncep-42/jncep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29142 2023-02-25 14:26:51.000000 jncep-42/jncep/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-02-25 14:26:51.000000 jncep-42/jncep/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    17914 2023-02-25 14:26:51.000000 jncep-42/jncep/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-02-25 14:26:51.000000 jncep-42/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-02-25 14:27:21.000000 jncep-42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    36313 2023-02-25 14:27:21.000000 jncep-42/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/
+-rw-r--r--   0 runner    (1001) docker     (122)    36394 2023-05-02 21:44:38.000000 jncep-43/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    36394 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/jncep/
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-02 21:44:16.000000 jncep-43/jncep/jncep.py
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-02 21:44:16.000000 jncep-43/jncep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17914 2023-05-02 21:44:16.000000 jncep-43/jncep/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29459 2023-05-02 21:44:16.000000 jncep-43/jncep/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7695 2023-05-02 21:44:16.000000 jncep-43/jncep/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-05-02 21:44:16.000000 jncep-43/jncep/trio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-02 21:44:16.000000 jncep-43/jncep/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-05-02 21:44:16.000000 jncep-43/jncep/spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-05-02 21:44:16.000000 jncep-43/jncep/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-05-02 21:44:16.000000 jncep-43/jncep/jnclabs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-05-02 21:44:16.000000 jncep-43/jncep/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-05-02 21:44:16.000000 jncep-43/jncep/jncweb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-05-02 21:44:16.000000 jncep-43/jncep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/jncep/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6804 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-02 21:44:16.000000 jncep-43/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30389 2023-05-02 21:44:16.000000 jncep-43/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-02 21:44:38.000000 jncep-43/setup.cfg
```

### Comparing `jncep-42/jncep.egg-info/SOURCES.txt` & `jncep-43/jncep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep.egg-info/PKG-INFO` & `jncep-43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 42
+Version: 43
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
@@ -130,15 +130,15 @@
                                   current directory]
           -s, --parts TEXT        Specification of a range of parts to download in the
                                   form of <vol>[.part]:<vol>[.part] [default: All the
                                   content linked by the JNOVEL_CLUB_URL argument,
                                   either a single part, a whole volume or the whole
                                   series]
           -v, --byvolume          Flag to indicate that the parts of different volumes
-                                  shoud be output in separate EPUBs
+                                  should be output in separate EPUBs
           -i, --images            Flag to indicate that the images of the novel should
                                   be extracted into the output folder
           -c, --content           Flag to indicate that the raw content of the parts
                                   should be extracted into the output folder
           -n, --no-replace        Flag to indicate that some unicode characters
                                   unlikely to be in an EPUB reader font should NOT be
                                   replaced and instead kept as is
@@ -155,15 +155,15 @@
         
         ```console
         jncep epub -o /Users/guilhem/Documents/jncbooks https://j-novel.club/read/tearmoon-empire-volume-1-part-1
         ```
         
         Account credentials must be passed (in this case, by using the env vars, as explained above), as well as a URL link to a part or volume or series on the J-Novel Club website. Whatever the URL links to is downloaded (single part or whole volume or whole series).
         
-        The tool will then communicate with the J-Novel Club API using the specified credentials and download the necessary parts (texts and images), as well as a book cover. The EPUB file will be created inside the specified (optional) output directory, `/Users/guilhem/Documents/jncbooks`, which must exist (not created by the tool).
+        The tool will then communicate with the J-Novel Club API using the specified credentials and download the necessary parts (texts and images), as well as a book cover. The EPUB file will be created inside the specified (optional) output directory, `/Users/guilhem/Documents/jncbooks`. The directory will be created if it doesn't exist.
         
         If the `--output` or `-o` switch is not present, the EPUB is output in the current directory. The `JNCEP_OUTPUT` env var can also be used instead of the switch to indicate a download directory.
         
         ##### URL
         
         To get the URL to pass as argument, you should first go to the series page on the the J-Novel Club website. Then copy the URL found in the browser URL bar:
         - For series: Simply use the URL of the series page on J-Novel Club. It will have a shape like `https://j-novel.club/series/redefining-the-meta-at-vrmmo-academy`.
@@ -172,14 +172,16 @@
         
         It is also possible to pass the index of the series shown using the [`track list`](#list-tracked-series) command:
         
         ```console
         jncep epub 5
         ```
         
+        It is equivalent to passing the URL of the corresponding series.
+        
         #### Range of parts
         
         The following command will create a single EPUB file with Parts 5 to 10 of Volume 1 of the 'Tearmoon Empire' novel (as long as the pre-pubs have not expired) in the current directory:
         
         ```console
         jncep epub --parts 1.5:1.10 https://j-novel.club/read/tearmoon-empire-volume-1-part-1
         ```
@@ -255,15 +257,15 @@
         
         The options that set flags (BYVOLUME and below in the list above) should have one of the following values: `1`, `true`, `t`, `yes`, `y` or `on`. The value can be in upper case. 
         
         For unsetting, the simplest is to use `config unset` to remove the configuration option (the default value for all those flags is `False`). If a value is set, it should be one of the following: `0`, `false`, `f`, `no`, `n` or `off`.
         
         ### Environment variables
         
-        The options can also be set using an environment variable. They are the same as the configuration options, but with a `JNCEP_` prefix:
+        The options can also be set using environment variables. They are the same as the configuration options, but with a `JNCEP_` prefix:
         
         For example:
         - JNCEP_PASSWORD
         - JNCEP_OUTPUT
         - JNCEP_CSS
         - and so on ...
         
@@ -275,15 +277,15 @@
         
         ### Priority order for option values
         
         The priority order for option values is as follows:
         1. If a value is passed on the command-line, it has the highest priority
         2. If no value is passed, the value is taken from an environment variable if present
         3. After that, the value is taken from the configuration file
-        4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, this will raise an error.
+        4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, an error will be raised.
         
         ## track
         
         This command is used to manage series to track. It has 4 subcommands:
         - `add`: Add a new series for tracking. After a series has been added, it can be updated using the `update` command.
         - `rm`: Remove a series from tracking
         - `list`: List tracked serie
@@ -293,15 +295,15 @@
         
         ### Tracking configuration
         
         The tracking is performed by updating a local config file called `tracked.json` and located inside the configuration folder. The location of the folder will vary depending on the OS. See the [section dedicated to the configuration](#configuration-folder) for more details.
         
         The configuration folder, as well the `tracked.json` file will be created by the tool if they don't exist.
         
-        The `tracked.json` file can be updated manually with a text editor if really needed but should generally be left alone (or the `jncep` could malfunction).
+        The `tracked.json` file can be updated manually with a text editor if really needed but should generally be left alone (or `jncep` could malfunction).
         
         ### Options
         
         To get some help about the arguments to the `track` command, just launch with the `--help` option:
         
         ```console
         ~$ jncep track --help
@@ -403,15 +405,15 @@
         
         Options:
           -l, --email TEXT        Login email for J-Novel Club account  [required]
           -p, --password TEXT     Login password for J-Novel Club account  [required]
           -o, --output DIRECTORY  Existing folder to write the output [default: The
                                   current directory]
           -v, --byvolume          Flag to indicate that the parts of different volumes
-                                  shoud be output in separate EPUBs
+                                  should be output in separate EPUBs
           -i, --images            Flag to indicate that the images of the novel should
                                   be extracted into the output folder
           -c, --content           Flag to indicate that the raw content of the parts
                                   should be extracted into the output folder
           -n, --no-replace        Flag to indicate that some unicode characters
                                   unlikely to be in an EPUB reader font should NOT be
                                   replaced and instead kept as is
@@ -553,15 +555,15 @@
         jncep config list
         ```
         
         This will display something like:
         
         ```console
         BYVOLUME       Flag to indicate that the parts of      
-                       different volumes shoud be output in    
+                       different volumes should be output in
                        separate EPUBs
         CONTENT        Flag to indicate that the raw content of
                        the parts should be extracted into the  
                        output folder
         CSS            Path to custom CSS file for the EPUBs   
         EMAIL          Login email for J-Novel Club account
         ...
```

### Comparing `jncep-42/README.md` & `jncep-43/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                           current directory]
   -s, --parts TEXT        Specification of a range of parts to download in the
                           form of <vol>[.part]:<vol>[.part] [default: All the
                           content linked by the JNOVEL_CLUB_URL argument,
                           either a single part, a whole volume or the whole
                           series]
   -v, --byvolume          Flag to indicate that the parts of different volumes
-                          shoud be output in separate EPUBs
+                          should be output in separate EPUBs
   -i, --images            Flag to indicate that the images of the novel should
                           be extracted into the output folder
   -c, --content           Flag to indicate that the raw content of the parts
                           should be extracted into the output folder
   -n, --no-replace        Flag to indicate that some unicode characters
                           unlikely to be in an EPUB reader font should NOT be
                           replaced and instead kept as is
@@ -145,15 +145,15 @@
 
 ```console
 jncep epub -o /Users/guilhem/Documents/jncbooks https://j-novel.club/read/tearmoon-empire-volume-1-part-1
 ```
 
 Account credentials must be passed (in this case, by using the env vars, as explained above), as well as a URL link to a part or volume or series on the J-Novel Club website. Whatever the URL links to is downloaded (single part or whole volume or whole series).
 
-The tool will then communicate with the J-Novel Club API using the specified credentials and download the necessary parts (texts and images), as well as a book cover. The EPUB file will be created inside the specified (optional) output directory, `/Users/guilhem/Documents/jncbooks`, which must exist (not created by the tool).
+The tool will then communicate with the J-Novel Club API using the specified credentials and download the necessary parts (texts and images), as well as a book cover. The EPUB file will be created inside the specified (optional) output directory, `/Users/guilhem/Documents/jncbooks`. The directory will be created if it doesn't exist.
 
 If the `--output` or `-o` switch is not present, the EPUB is output in the current directory. The `JNCEP_OUTPUT` env var can also be used instead of the switch to indicate a download directory.
 
 ##### URL
 
 To get the URL to pass as argument, you should first go to the series page on the the J-Novel Club website. Then copy the URL found in the browser URL bar:
 - For series: Simply use the URL of the series page on J-Novel Club. It will have a shape like `https://j-novel.club/series/redefining-the-meta-at-vrmmo-academy`.
@@ -162,14 +162,16 @@
 
 It is also possible to pass the index of the series shown using the [`track list`](#list-tracked-series) command:
 
 ```console
 jncep epub 5
 ```
 
+It is equivalent to passing the URL of the corresponding series.
+
 #### Range of parts
 
 The following command will create a single EPUB file with Parts 5 to 10 of Volume 1 of the 'Tearmoon Empire' novel (as long as the pre-pubs have not expired) in the current directory:
 
 ```console
 jncep epub --parts 1.5:1.10 https://j-novel.club/read/tearmoon-empire-volume-1-part-1
 ```
@@ -245,15 +247,15 @@
 
 The options that set flags (BYVOLUME and below in the list above) should have one of the following values: `1`, `true`, `t`, `yes`, `y` or `on`. The value can be in upper case. 
 
 For unsetting, the simplest is to use `config unset` to remove the configuration option (the default value for all those flags is `False`). If a value is set, it should be one of the following: `0`, `false`, `f`, `no`, `n` or `off`.
 
 ### Environment variables
 
-The options can also be set using an environment variable. They are the same as the configuration options, but with a `JNCEP_` prefix:
+The options can also be set using environment variables. They are the same as the configuration options, but with a `JNCEP_` prefix:
 
 For example:
 - JNCEP_PASSWORD
 - JNCEP_OUTPUT
 - JNCEP_CSS
 - and so on ...
 
@@ -265,15 +267,15 @@
 
 ### Priority order for option values
 
 The priority order for option values is as follows:
 1. If a value is passed on the command-line, it has the highest priority
 2. If no value is passed, the value is taken from an environment variable if present
 3. After that, the value is taken from the configuration file
-4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, this will raise an error.
+4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, an error will be raised.
 
 ## track
 
 This command is used to manage series to track. It has 4 subcommands:
 - `add`: Add a new series for tracking. After a series has been added, it can be updated using the `update` command.
 - `rm`: Remove a series from tracking
 - `list`: List tracked serie
@@ -283,15 +285,15 @@
 
 ### Tracking configuration
 
 The tracking is performed by updating a local config file called `tracked.json` and located inside the configuration folder. The location of the folder will vary depending on the OS. See the [section dedicated to the configuration](#configuration-folder) for more details.
 
 The configuration folder, as well the `tracked.json` file will be created by the tool if they don't exist.
 
-The `tracked.json` file can be updated manually with a text editor if really needed but should generally be left alone (or the `jncep` could malfunction).
+The `tracked.json` file can be updated manually with a text editor if really needed but should generally be left alone (or `jncep` could malfunction).
 
 ### Options
 
 To get some help about the arguments to the `track` command, just launch with the `--help` option:
 
 ```console
 ~$ jncep track --help
@@ -393,15 +395,15 @@
 
 Options:
   -l, --email TEXT        Login email for J-Novel Club account  [required]
   -p, --password TEXT     Login password for J-Novel Club account  [required]
   -o, --output DIRECTORY  Existing folder to write the output [default: The
                           current directory]
   -v, --byvolume          Flag to indicate that the parts of different volumes
-                          shoud be output in separate EPUBs
+                          should be output in separate EPUBs
   -i, --images            Flag to indicate that the images of the novel should
                           be extracted into the output folder
   -c, --content           Flag to indicate that the raw content of the parts
                           should be extracted into the output folder
   -n, --no-replace        Flag to indicate that some unicode characters
                           unlikely to be in an EPUB reader font should NOT be
                           replaced and instead kept as is
@@ -543,15 +545,15 @@
 jncep config list
 ```
 
 This will display something like:
 
 ```console
 BYVOLUME       Flag to indicate that the parts of      
-               different volumes shoud be output in    
+               different volumes should be output in
                separate EPUBs
 CONTENT        Flag to indicate that the raw content of
                the parts should be extracted into the  
                output folder
 CSS            Path to custom CSS file for the EPUBs   
 EMAIL          Login email for J-Novel Club account
 ...
```

### Comparing `jncep-42/jncep/spec.py` & `jncep-43/jncep/spec.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/jnclabs.py` & `jncep-43/jncep/jnclabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,15 @@
         )
         r.raise_for_status()
 
         return r
 
     async def fetch_follows(self):
         path = "/users/me"
+        # filter for only novels, exclude manga
         qfilter = {"include": [{"serieFollows": "serie"}]}
         payload = {"filter": json.dumps(qfilter)}
 
         r = await self._call_legacy_api_authenticated("GET", path, params=payload)
         r.raise_for_status()
 
         me_data = Addict(r.json())
```

### Comparing `jncep-42/jncep/config.py` & `jncep-43/jncep/config.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/cli/config.py` & `jncep-43/jncep/cli/config.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/cli/epub.py` & `jncep-43/jncep/cli/epub.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     else:
         jnc_url = jnc_url_or_index
 
     async with core.JNCEPSession(email, password) as session:
         jnc_resource = jncweb.resource_from_url(jnc_url)
         series_id = await core.resolve_series(session, jnc_resource)
         series = await core.fetch_meta(session, series_id)
+        core.check_series_is_novel(series)
 
         if part_spec:
             console.info(f"Use part specification '[highlight]{part_spec}[/]'")
             part_spec_analyzed = spec.analyze_part_specs(part_spec)
             part_spec_analyzed.normalize_and_verify(series)
         else:
             part_spec_analyzed = await core.to_part_spec(series, jnc_resource)
```

### Comparing `jncep-42/jncep/cli/options.py` & `jncep-43/jncep/cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 byvolume_option = click.option(
     "-v",
     "--byvolume",
     "is_by_volume",
     is_flag=True,
     envvar=f"{ENVVAR_PREFIX}BYVOLUME",
     help=(
-        "Flag to indicate that the parts of different volumes shoud be output in "
+        "Flag to indicate that the parts of different volumes should be output in "
         "separate EPUBs"
     ),
 )
 
 images_option = click.option(
     "-i",
     "--images",
```

### Comparing `jncep-42/jncep/cli/base.py` & `jncep-43/jncep/cli/base.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/cli/track.py` & `jncep-43/jncep/cli/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         tracked_series = track_manager.read_tracked_series()
 
         console.status("Check tracking status...")
 
         jnc_resource = jncweb.resource_from_url(jnc_url)
         series_id = await core.resolve_series(session, jnc_resource)
         series = await core.fetch_meta(session, series_id)
+        core.check_series_is_novel(series)
 
         series_url = jncweb.url_from_series_slug(series.raw_data.slug)
         if series_url in tracked_series:
             console.warning(
                 f"The series '[highlight]{series.raw_data.title}[/]' is "
                 "already tracked!"
             )
```

### Comparing `jncep-42/jncep/cli/update.py` & `jncep-43/jncep/cli/update.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/jncweb.py` & `jncep-43/jncep/jncweb.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/trio_utils.py` & `jncep-43/jncep/trio_utils.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/model.py` & `jncep-43/jncep/model.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/jncep.py` & `jncep-43/jncep/jncep.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,22 @@
     "is_debug",
     is_flag=True,
     help=("Flag to activate debug mode"),
     required=False,
 )
 def main(is_debug):
     setup_logging(is_debug)
+    try:
+        apply_options_from_config()
+    except Exception:
+        console.warning(
+            "There was an error reading the configuration at: "
+            f"{DEFAULT_CONFIG_FILEPATH}. Continuing..." )
 
 
 main.add_command(generate_epub)
 main.add_command(track_series)
 main.add_command(update_tracked)
 main.add_command(config_manage)
 
 if __name__ == "__main__":
-    try:
-        apply_options_from_config()
-    except Exception:
-        console.warning(
-            "There was an error reading the configuration at: "
-            f"{DEFAULT_CONFIG_FILEPATH}. Continuing..."
-        )
     main()
```

### Comparing `jncep-42/jncep/epub.py` & `jncep-43/jncep/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/track.py` & `jncep-43/jncep/track.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     new_synced = []
     del_synced = []
 
     async def do_track(jnc_resource):
         series_id = await core.resolve_series(session, jnc_resource)
         series = await core.fetch_meta(session, series_id)
         await track_series(session, tracked_series, series)
+        # manga already excluded from follows so no need to check
 
         series_url = jncweb.url_from_series_slug(series.raw_data.slug)
         new_synced.append(series_url)
 
     tasks = []
     for jnc_resource in follows:
         if jnc_resource.url in tracked_series:
```

### Comparing `jncep-42/jncep/core.py` & `jncep-43/jncep/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 )
 
 
 class FilePathTooLongError(Exception):
     pass
 
 
+class SeriesNotANovelError(Exception):
+    pass
+
+
 class JNCEPSession:
     def __init__(self, email, password):
         self.api = jnclabs.JNCLabsAPI()
         self.email = email
         self.password = password
         self.now = datetime.now(tz=timezone.utc)
 
@@ -880,7 +884,15 @@
 
     events_with_pagination = await session.api.fetch_events(**params)
 
     events = events_with_pagination.events
     pagination = events_with_pagination.pagination
     has_reached_limit = not pagination.lastPage
     return EventFeed(events, has_reached_limit)
+
+
+def check_series_is_novel(series: Series):
+    if series.raw_data.type.upper() != "NOVEL":
+        raise SeriesNotANovelError(
+            f"Series '[highlight]{series.raw_data.title}[/]' is not a novel "
+            f"(type is '{series.raw_data.type}')"
+        )
```

### Comparing `jncep-42/jncep/utils.py` & `jncep-43/jncep/utils.py`

 * *Files identical despite different names*

### Comparing `jncep-42/jncep/update.py` & `jncep-43/jncep/update.py`

 * *Files identical despite different names*

### Comparing `jncep-42/setup.py` & `jncep-43/setup.py`

 * *Files identical despite different names*

### Comparing `jncep-42/PKG-INFO` & `jncep-43/jncep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 42
+Version: 43
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
@@ -130,15 +130,15 @@
                                   current directory]
           -s, --parts TEXT        Specification of a range of parts to download in the
                                   form of <vol>[.part]:<vol>[.part] [default: All the
                                   content linked by the JNOVEL_CLUB_URL argument,
                                   either a single part, a whole volume or the whole
                                   series]
           -v, --byvolume          Flag to indicate that the parts of different volumes
-                                  shoud be output in separate EPUBs
+                                  should be output in separate EPUBs
           -i, --images            Flag to indicate that the images of the novel should
                                   be extracted into the output folder
           -c, --content           Flag to indicate that the raw content of the parts
                                   should be extracted into the output folder
           -n, --no-replace        Flag to indicate that some unicode characters
                                   unlikely to be in an EPUB reader font should NOT be
                                   replaced and instead kept as is
@@ -155,15 +155,15 @@
         
         ```console
         jncep epub -o /Users/guilhem/Documents/jncbooks https://j-novel.club/read/tearmoon-empire-volume-1-part-1
         ```
         
         Account credentials must be passed (in this case, by using the env vars, as explained above), as well as a URL link to a part or volume or series on the J-Novel Club website. Whatever the URL links to is downloaded (single part or whole volume or whole series).
         
-        The tool will then communicate with the J-Novel Club API using the specified credentials and download the necessary parts (texts and images), as well as a book cover. The EPUB file will be created inside the specified (optional) output directory, `/Users/guilhem/Documents/jncbooks`, which must exist (not created by the tool).
+        The tool will then communicate with the J-Novel Club API using the specified credentials and download the necessary parts (texts and images), as well as a book cover. The EPUB file will be created inside the specified (optional) output directory, `/Users/guilhem/Documents/jncbooks`. The directory will be created if it doesn't exist.
         
         If the `--output` or `-o` switch is not present, the EPUB is output in the current directory. The `JNCEP_OUTPUT` env var can also be used instead of the switch to indicate a download directory.
         
         ##### URL
         
         To get the URL to pass as argument, you should first go to the series page on the the J-Novel Club website. Then copy the URL found in the browser URL bar:
         - For series: Simply use the URL of the series page on J-Novel Club. It will have a shape like `https://j-novel.club/series/redefining-the-meta-at-vrmmo-academy`.
@@ -172,14 +172,16 @@
         
         It is also possible to pass the index of the series shown using the [`track list`](#list-tracked-series) command:
         
         ```console
         jncep epub 5
         ```
         
+        It is equivalent to passing the URL of the corresponding series.
+        
         #### Range of parts
         
         The following command will create a single EPUB file with Parts 5 to 10 of Volume 1 of the 'Tearmoon Empire' novel (as long as the pre-pubs have not expired) in the current directory:
         
         ```console
         jncep epub --parts 1.5:1.10 https://j-novel.club/read/tearmoon-empire-volume-1-part-1
         ```
@@ -255,15 +257,15 @@
         
         The options that set flags (BYVOLUME and below in the list above) should have one of the following values: `1`, `true`, `t`, `yes`, `y` or `on`. The value can be in upper case. 
         
         For unsetting, the simplest is to use `config unset` to remove the configuration option (the default value for all those flags is `False`). If a value is set, it should be one of the following: `0`, `false`, `f`, `no`, `n` or `off`.
         
         ### Environment variables
         
-        The options can also be set using an environment variable. They are the same as the configuration options, but with a `JNCEP_` prefix:
+        The options can also be set using environment variables. They are the same as the configuration options, but with a `JNCEP_` prefix:
         
         For example:
         - JNCEP_PASSWORD
         - JNCEP_OUTPUT
         - JNCEP_CSS
         - and so on ...
         
@@ -275,15 +277,15 @@
         
         ### Priority order for option values
         
         The priority order for option values is as follows:
         1. If a value is passed on the command-line, it has the highest priority
         2. If no value is passed, the value is taken from an environment variable if present
         3. After that, the value is taken from the configuration file
-        4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, this will raise an error.
+        4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, an error will be raised.
         
         ## track
         
         This command is used to manage series to track. It has 4 subcommands:
         - `add`: Add a new series for tracking. After a series has been added, it can be updated using the `update` command.
         - `rm`: Remove a series from tracking
         - `list`: List tracked serie
@@ -293,15 +295,15 @@
         
         ### Tracking configuration
         
         The tracking is performed by updating a local config file called `tracked.json` and located inside the configuration folder. The location of the folder will vary depending on the OS. See the [section dedicated to the configuration](#configuration-folder) for more details.
         
         The configuration folder, as well the `tracked.json` file will be created by the tool if they don't exist.
         
-        The `tracked.json` file can be updated manually with a text editor if really needed but should generally be left alone (or the `jncep` could malfunction).
+        The `tracked.json` file can be updated manually with a text editor if really needed but should generally be left alone (or `jncep` could malfunction).
         
         ### Options
         
         To get some help about the arguments to the `track` command, just launch with the `--help` option:
         
         ```console
         ~$ jncep track --help
@@ -403,15 +405,15 @@
         
         Options:
           -l, --email TEXT        Login email for J-Novel Club account  [required]
           -p, --password TEXT     Login password for J-Novel Club account  [required]
           -o, --output DIRECTORY  Existing folder to write the output [default: The
                                   current directory]
           -v, --byvolume          Flag to indicate that the parts of different volumes
-                                  shoud be output in separate EPUBs
+                                  should be output in separate EPUBs
           -i, --images            Flag to indicate that the images of the novel should
                                   be extracted into the output folder
           -c, --content           Flag to indicate that the raw content of the parts
                                   should be extracted into the output folder
           -n, --no-replace        Flag to indicate that some unicode characters
                                   unlikely to be in an EPUB reader font should NOT be
                                   replaced and instead kept as is
@@ -553,15 +555,15 @@
         jncep config list
         ```
         
         This will display something like:
         
         ```console
         BYVOLUME       Flag to indicate that the parts of      
-                       different volumes shoud be output in    
+                       different volumes should be output in
                        separate EPUBs
         CONTENT        Flag to indicate that the raw content of
                        the parts should be extracted into the  
                        output folder
         CSS            Path to custom CSS file for the EPUBs   
         EMAIL          Login email for J-Novel Club account
         ...
```

