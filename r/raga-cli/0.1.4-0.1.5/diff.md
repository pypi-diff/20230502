# Comparing `tmp/raga-cli-0.1.4.tar.gz` & `tmp/raga-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.1.4.tar", last modified: Thu Apr 27 08:00:22 2023, max compression
+gzip compressed data, was "raga-cli-0.1.5.tar", last modified: Mon May  1 18:22:04 2023, max compression
```

## Comparing `raga-cli-0.1.4.tar` & `raga-cli-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.925590 raga-cli-0.1.4/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.4/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.4/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-27 08:00:22.925237 raga-cli-0.1.4/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.4/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-27 07:59:56.000000 raga-cli-0.1.4/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.920156 raga-cli-0.1.4/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.920757 raga-cli-0.1.4/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.921891 raga-cli-0.1.4/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.4/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.4/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.4/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)    10165 2023-04-27 07:55:00.000000 raga-cli-0.1.4/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.922870 raga-cli-0.1.4/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.4/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-27 06:41:59.000000 raga-cli-0.1.4/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9205 2023-04-27 07:51:17.000000 raga-cli-0.1.4/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.923662 raga-cli-0.1.4/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5457 2023-04-27 07:35:31.000000 raga-cli-0.1.4/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.4/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.923914 raga-cli-0.1.4/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.924866 raga-cli-0.1.4/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6463 2023-04-26 13:39:34.000000 raga-cli-0.1.4/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-27 08:00:22.925658 raga-cli-0.1.4/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.4/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.443190 raga-cli-0.1.5/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.5/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.5/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-01 18:22:04.442818 raga-cli-0.1.5/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.5/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-05-01 18:21:04.000000 raga-cli-0.1.5/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.436190 raga-cli-0.1.5/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-01 18:22:04.000000 raga-cli-0.1.5/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      631 2023-05-01 18:22:04.000000 raga-cli-0.1.5/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-05-01 18:22:04.000000 raga-cli-0.1.5/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-05-01 18:22:04.000000 raga-cli-0.1.5/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-05-01 18:22:04.000000 raga-cli-0.1.5/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-05-01 18:22:04.000000 raga-cli-0.1.5/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.436952 raga-cli-0.1.5/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.438144 raga-cli-0.1.5/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.5/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.5/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2073 2023-05-01 18:21:39.000000 raga-cli-0.1.5/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    11674 2023-05-01 18:16:51.000000 raga-cli-0.1.5/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.439427 raga-cli-0.1.5/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3393 2023-05-01 17:37:27.000000 raga-cli-0.1.5/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.5/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1839 2023-05-01 17:31:10.000000 raga-cli-0.1.5/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    10377 2023-05-01 17:27:49.000000 raga-cli-0.1.5/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.440332 raga-cli-0.1.5/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5562 2023-05-01 17:58:40.000000 raga-cli-0.1.5/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.5/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.440650 raga-cli-0.1.5/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-01 18:22:04.442315 raga-cli-0.1.5/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1996 2023-05-01 08:38:56.000000 raga-cli-0.1.5/rc/utils/config.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6721 2023-05-01 16:53:53.000000 raga-cli-0.1.5/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-05-01 07:24:17.000000 raga-cli-0.1.5/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.5/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-05-01 18:22:04.443264 raga-cli-0.1.5/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.5/setup.py
```

### Comparing `raga-cli-0.1.4/.gitignore` & `raga-cli-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/LICENSE` & `raga-cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/PKG-INFO` & `raga-cli-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.4/pyproject.toml` & `raga-cli-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.1.4/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.5/raga_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.4/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.5/raga_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,10 +22,11 @@
 rc/commands/repo.py
 rc/repo/get.py
 rc/repo/put.py
 rc/repo/repo.py
 rc/stage/exceptions.py
 rc/utils/__init__.py
 rc/utils/auditLog.py
+rc/utils/config.py
 rc/utils/fileLog.py
 rc/utils/request.py
 rc/utils/sshKeyGen.py
```

### Comparing `raga-cli-0.1.4/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.5/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/cli/__init__.py` & `raga-cli-0.1.5/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/cli/parser.py` & `raga-cli-0.1.5/rc/cli/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         add_help=False,
     )
 
     parser.add_argument(
         "-V",
         "--version",
         action="version",
-        version='0.0.13',
+        version='0.1.5',
         help="Show program's version.",
     )
 
     # Sub commands
     subparsers = parser.add_subparsers(
         title="Available Commands",
         metavar="COMMAND",
```

### Comparing `raga-cli-0.1.4/rc/cli/utils.py` & `raga-cli-0.1.5/rc/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import subprocess
 import time
 import sys
 from rc.utils import DEBUG
 from multiprocessing import cpu_count
 from pathlib import Path
 import pathlib
+import re
+from datetime import datetime
 
 from rc.utils.request import get_commit_repo, get_config_value_by_key, get_repo_version
 
 logger = logging.getLogger(__name__)
 
 class RctlValidSubprocessError(Exception):
     def __init__(self, msg, *args):
@@ -95,16 +97,45 @@
     return stdout.strip()
 
 def branch_commit_checkout(branch,commitId):
     result = subprocess.run('git checkout {0} -b {1}'.format(commitId,branch), capture_output=True, shell=True)    
     stdout = str(result.stdout, 'UTF-8')
     return stdout.strip()
 
+def is_repo_exist_in_gh(repo):
+    logger.debug("Check existence of repo in GIT HUB : {}".format(repo))
+    result = subprocess.run('gh repo view {}'.format(repo), capture_output=True, shell=True)    
+    stdout = str(result.stdout, 'UTF-8').strip()
+    stderr = str(result.stderr, 'UTF-8').strip()
+    logger.debug(f"STD OUT: {stdout}")
+    logger.debug(f"STD ERR: {stderr}")
+    match = re.search(r'Could not resolve to a Repository with the name', stderr)
+    if match:
+        logger.debug("Repo not found in GH")
+        return False  
+    logger.debug("Repo found in GH")
+    return True
 
 
+def check_push_left():
+    logger.debug("Check PUSH left")
+    result = subprocess.run('git status', capture_output=True, shell=True)    
+    stdout = str(result.stdout, 'UTF-8').strip()
+    stderr = str(result.stderr, 'UTF-8').strip()
+    logger.debug(f"STD OUT: {stdout}")
+    logger.debug(f"STD ERR: {stderr}")
+    if re.search(r'(use "git push" to publish your local commits)', stdout):
+        logger.debug("Push left")
+        return True  
+    elif re.search(r'(use "git push" to publish your local commits)', stderr):
+        logger.debug("Push left")
+        return True  
+    logger.debug("Clean PUSH")
+    return False
+
 def is_current_version_stable():
     from rc.utils.request import get_commit_version, get_repo_version
     repo = get_repo()
     commit_id = current_commit_hash()
     repo_version = get_repo_version(repo)
     commit_version = get_commit_version(commit_id)
     if not commit_version and not repo_version:
@@ -208,26 +239,32 @@
 def repo_name_valid(name):
     for c in name:        
         if c == '_':
             raise RctlValidSubprocessError("Error: Bucket name contains invalid characters")
     if len(name) <3 or len(name)>63:
         raise RctlValidSubprocessError("Error: Bucket names should be between 3 and 63 characters long")   
     
-def path_to_dict(path):                   
-        if path != "./.git":
-            d = {'name': os.path.basename(path)}
-            if os.path.isdir(path):
-                d['type'] = "directory"
-                d['children'] = [path_to_dict(os.path.join(path,x)) for x in os.listdir\
-        (path)]
-            else:
-                d['type'] = "file"
-            return d 
+def path_to_dict(path):
+    name = os.path.basename(path)
+    if name == ".rc" or name == ".git":
+        return None
+    d = {'name': name}
+    if os.path.isdir(path):
+        d['type'] = "directory"
+        children = [path_to_dict(os.path.join(path, x)) for x in os.listdir(path)]
+        d['children'] = [c for c in children if c is not None]
+    else:
+        d['type'] = "file"
+        d['last_updated'] = datetime.fromtimestamp(os.path.getmtime(path)).strftime('%Y-%m-%d %H:%M:%S')
+    return d
 
-def upload_model_file_list_json(version):
+def upload_model_file_list_json(version, cwd = None):
+    if cwd:
+        owd = os.getcwd()
+        os.chdir(f"{owd}/{cwd}") 
     logger.debug("MODEL FILE UPLOADING")
     import botocore.session   
     model_file_list = json.loads(json.dumps(path_to_dict('.')))
     CLOUD_STORAGE_BUCKET = get_config_value_by_key('bucket_name')
     CLOUD_STORAGE_DIR = get_config_value_by_key('cloud_storage_dir')
     AWS_SECRET = get_config_value_by_key('remote_storage_secret_key')
     AWS_ACCESS = get_config_value_by_key('remote_storage_access_key')
@@ -243,14 +280,17 @@
     with open(f'{version}.json', 'w', encoding='utf-8') as cred:    
         json.dump(model_file_list, cred, ensure_ascii=False, indent=4)  
 
     # Upload the file to S3
     with open(f'{version}.json', 'rb') as file:
         s3.put_object(Bucket=CLOUD_STORAGE_BUCKET, Key=dest, Body=file)          
     pathlib.Path(f'{version}.json').unlink(missing_ok=True)
+
+    if cwd:
+        os.chdir(owd)
     
 def retry(ExceptionToCheck, tries=4, delay=3, backoff=2):
     """
     Retry calling the decorated function using an exponential backoff.
 
     Args:
         ExceptionToCheck (Exception): the exception to check. When an exception of this type is raised, the function will be retried.
```

### Comparing `raga-cli-0.1.4/rc/commands/get.py` & `raga-cli-0.1.5/rc/commands/get.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from timeit import default_timer as timer
 import json
 from rc.cli import log_setup
 
 from rc.cli.command import CmdBase
 from rc.cli.utils import run_command_on_subprocess,branch_commit_checkout
 from rc.cli.utils import *
-from rc.utils.request import get_repo_commit_id, get_repository
+from rc.utils.request import get_repo_commit_id, get_repository, get_repo_commit
 
 logger = logging.getLogger(__name__)
 
 class CmdGet(CmdBase):
     def __init__(self, args):
         super().__init__(args)
     def run(self):
@@ -21,15 +21,17 @@
         repo = get_repo()
         
         tag = get_repository(repo)
        
         version = self.args.version
         if not version:
             print("Files downloading...") 
-            run_command_on_subprocess('git pull') 
+            repo_commit = get_repo_commit(repo)
+            run_command_on_subprocess('git reset --hard')
+            run_command_on_subprocess('git reset --hard {0}'.format(repo_commit['commit_id']))
             if tag == "dataset":
                 run_command_on_subprocess('dvc pull -f') 
             print("Files downloaded successfully") 
             logger.debug('DOWNLOAD TIME {0}'.format(timedelta(seconds=timer()-start))) 
         else:  
             if tag == "model":
                 user_input = input("Are you sure you want to get it? [y/n]").lower()
```

### Comparing `raga-cli-0.1.4/rc/commands/list.py` & `raga-cli-0.1.5/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/commands/put.py` & `raga-cli-0.1.5/rc/commands/put.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 
 
 from rc.cli.command import CmdBase
 from rc.cli.utils import *
 from rc.cli import RctlValidReqError, log_setup
 from rc.repo.put import *
+from rc.utils.config import get_config_value
 
 logger = logging.getLogger(__name__)
 
 class CmdPut(CmdBase):
     def __init__(self, args):
         super().__init__(args)
         self.dirs = None
@@ -18,14 +19,16 @@
         if getattr(self.args, "path", None):
             self.dirs = [self.args.path]
         else:
             self.dirs = get_all_data_folder()         
 
     def run(self):        
         log_setup(self.args)
+        # print(get_config_value("repo"))
+        # return
         self.args.path = self.dirs
         put(self.args) 
         return 0
 
 
 def add_parser(subparsers, parent_parser):
     REPO_HELP = "Put File or folder. Use: `rc put <file or folder path> -m <commit message>`"
```

### Comparing `raga-cli-0.1.4/rc/commands/repo.py` & `raga-cli-0.1.5/rc/commands/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import os
 from datetime import timedelta
 import sys 
 from timeit import default_timer as timer
 import os, pwd
 
 from rc.cli.command import CmdBase
-from rc.cli.utils import current_commit_hash, folder_exists, run_command_on_subprocess, repo_name_valid, get_git_url
+from rc.cli.utils import current_commit_hash, folder_exists, is_repo_exist_in_gh, run_command_on_subprocess, repo_name_valid, get_git_url, upload_model_file_list_json
+from rc.utils.config import create_rc_folder, set_config_value
 from rc.utils.request import get_config_value_by_key, create_repository, create_repo_lock, get_repository, insert_repo_commit
 from rc.cli import RctlValidReqError, log_setup
 
 logger = logging.getLogger(__name__)
    
  
 
@@ -35,87 +36,124 @@
         self.CLOUD_STORAGE_LOCATION = f"s3://{self.CLOUD_STORAGE_BUCKET}/{self.CLOUD_STORAGE_DIR}"
         self.INITIAL_COMMIT = get_config_value_by_key('git_initial_commit')
         self.GIT_BRANCH = get_config_value_by_key('git_initial_branch')
         self.GIT_ORG = get_config_value_by_key('git_org')
         self.TAGS = {"dataset", "model"}
         self.created_by = pwd.getpwuid(os.getuid()).pw_name 
 
+    def run_git_commands(self,repo_name, repo_tag):
+        run_command_on_subprocess("git add .rc", repo_name)       
+        run_command_on_subprocess("git commit -m '{0}' -a".format(self.INITIAL_COMMIT), repo_name)    
+        run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
+        run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)
+
     def run_repo_create_subprocesses(self,repo_name, repo_tag):     
         logger.debug(f"Repository Name: {repo_name}")
-
+        secret_key = get_config_value_by_key('remote_storage_secret_key')
+        access_key = get_config_value_by_key('remote_storage_access_key')
         if repo_tag =="dataset":
             run_command_on_subprocess("gh config set git_protocol ssh")  
             run_command_on_subprocess("gh repo create {0}/{1} --private --clone".format(self.GIT_ORG, repo_name))    
             run_command_on_subprocess("dvc init", repo_name)    
             run_command_on_subprocess("dvc remote add -d {0} {1}/{2} -f".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repo_name), repo_name)           
-            run_command_on_subprocess("dvc remote modify {0} secret_access_key {1}".format(self.CLOUD_STORAGE_BUCKET, get_config_value_by_key('remote_storage_secret_key')), repo_name)         
-            run_command_on_subprocess("dvc remote modify {0} access_key_id {1}".format(self.CLOUD_STORAGE_BUCKET, get_config_value_by_key('remote_storage_access_key')), repo_name)        
-            run_command_on_subprocess("dvc config core.autostage true", repo_name)           
-            run_command_on_subprocess("git commit -m '{0}' -a".format(self.INITIAL_COMMIT), repo_name)    
-            run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
-            run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)   
+            run_command_on_subprocess("dvc remote modify {0} secret_access_key {1}".format(self.CLOUD_STORAGE_BUCKET,secret_key ), repo_name)         
+            run_command_on_subprocess("dvc remote modify {0} access_key_id {1}".format(self.CLOUD_STORAGE_BUCKET, access_key), repo_name)        
+            run_command_on_subprocess("dvc config core.autostage true", repo_name)            
         if repo_tag == "model":
             run_command_on_subprocess("gh config set git_protocol ssh")  
             run_command_on_subprocess("gh repo create {0}/{1} --private --clone".format(self.GIT_ORG, repo_name)) 
             run_command_on_subprocess("touch README.md", repo_name)      
-            run_command_on_subprocess("git add README.md", repo_name)      
-            run_command_on_subprocess("git commit -m '{0}' -a".format("Model repo init"), repo_name)  
-            run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
-            run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)    
+            run_command_on_subprocess("git add README.md", repo_name)       
+
+        configs = {
+            "repo":repo_name,
+            "git_org":self.GIT_ORG,
+            "remote_bucket":self.CLOUD_STORAGE_BUCKET,
+            "remote_bucket_dir":self.CLOUD_STORAGE_DIR,
+            "remote_bucket_location":self.CLOUD_STORAGE_LOCATION,
+            "secret_key":secret_key,
+            "access_key":access_key,
+            "version":0,
+            "repo_id":"", 
+            "tag":repo_tag
+        }  
+        create_rc_folder(repo_name, configs)
 
     
     def create_repo(self, args):
         if self.check_git_init():
             print("The repo creating process inside the repository is not possible.")
             sys.exit(50) 
         logger.debug(f"START CREATE REPO COMMAND")
         repository_name = args.name    
+        repository_tag = args.tag 
+        if is_repo_exist_in_gh("{0}/{1}".format(self.GIT_ORG, repository_name)):
+            print("The repo creating process could not be completed because the repo already exists. Please rename repo and try again.")
+            sys.exit(50)
 
         if folder_exists(repository_name):
             print("The repo creating process could not be completed because the directory already exists. Please rename repo and try again.")
             sys.exit(50)
+
         print("Repo creating...")  
-        repository_tag = args.tag  
+
         if repository_tag not in self.TAGS:
             logger.error("'{0}' tag is not available. Please select from {1}".format(repository_tag, self.TAGS))
-            sys.exit(50)                      
-        self.run_repo_create_subprocesses(repository_name, repository_tag)
+            sys.exit(50)   
 
+        
+        self.run_repo_create_subprocesses(repository_name, repository_tag)
         git_repo = get_git_url(repository_name)
+        
         if repository_tag == "dataset":
-            s3_repo = "{1}/{2}".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repository_name)    
+
+            s3_repo = "{1}/{2}".format(self.CLOUD_STORAGE_BUCKET, self.CLOUD_STORAGE_LOCATION, repository_name)  
+
             req_body = json.dumps({
                 "repo_name":repository_name,
                 "tag":repository_tag,
                 "created_by":self.created_by,
                 "git_repo":git_repo.replace('\n', ''),
                 "remote_storage_url":s3_repo,
             })
+
             logger.debug(req_body)
+
         if repository_tag == "model":
             req_body = json.dumps({
                 "repo_name":repository_name,
                 "tag":repository_tag,
                 "created_by":self.created_by,
                 "git_repo":git_repo.replace('\n', ''),
             })
             logger.debug(req_body)
-        commit_hash = current_commit_hash(repository_name)
-        request_payload = {
-                "commit_message" : "Initial commit",
-                "repo" : repository_name,
-                "commit_id":commit_hash,
-                "version":1,
-                "branch":"master"
-            }  
-        create_repository(req_body)
-        insert_repo_commit(json.dumps(request_payload))
+
+        created_repo_data = create_repository(req_body)
+        set_config_value("repo_id", created_repo_data['id'], repository_name)
+        
+        if repository_tag == "dataset":
+            self.run_git_commands(repository_name, repository_tag)
+
+        if repository_tag == "model":
+            set_config_value("version", 1, repository_name)
+            self.run_git_commands(repository_name, repository_tag)
+            commit_hash = current_commit_hash(repository_name)
+            request_payload = {
+                    "commit_message" : "Initial commit",
+                    "repo" : repository_name,
+                    "commit_id":commit_hash,
+                    "version":1,
+                    "branch":"master"
+                }  
+            insert_repo_commit(json.dumps(request_payload))
+            upload_model_file_list_json(commit_hash, repository_name)
+
         create_repo_lock(json.dumps({"repo_name":repository_name, "user_name":self.created_by, "locked":False}))
+        print("Repository has been created. `cd {}`".format(repository_name))  
 
-        print("Repository has been created. `cd {}`".format(repository_name))    
         logger.debug(f"END CREATE REPO COMMAND")
     
     def check_git_init(self):
         current_dir = os.getcwd()
         while current_dir != '/':  # Stop when we reach the root directory
             if os.path.exists(os.path.join(current_dir, '.git')):
                 return True  # .git folder exists, so project has been initialized
```

### Comparing `raga-cli-0.1.4/rc/exceptions.py` & `raga-cli-0.1.5/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/prompt.py` & `raga-cli-0.1.5/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/repo/get.py` & `raga-cli-0.1.5/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/repo/put.py` & `raga-cli-0.1.5/rc/repo/put.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from timeit import default_timer as timer
 from rc.cli.utils import *
 from rc.utils.request import get_commit_version, is_repo_lock, update_repo_commit_id, update_repo_lock, insert_repo_commit, get_repository
 
 logger = logging.getLogger(__name__)
 repo_commit_ids = []
 pool_time = 10
+#Create an Event object
+stop_event = threading.Event()
 
 def dir_add(path):
     start = timer()
     if compare_dot_dvc_file(path):
         run_command_on_subprocess("dvc commit {0} -f".format(path))
     else:
         run_command_on_subprocess("dvc add {0}".format(path))
@@ -113,16 +115,14 @@
     # return
 
     tag = get_repository(repo)
     is_repo_lock(repo)
     
     if tag == "dataset":
         current_version = dataset_current_version(paths, repo)
-        # Create an Event object
-        stop_event = threading.Event()
         # Create a thread for making an HTTP request
         http_thread = threading.Thread(target=make_repo_lock, args=(stop_event,))
         http_thread.start() 
         try:
             if dataset_upload(paths,message,repo, current_version):
                 # Set the stop event
                 stop_event.set()
@@ -141,12 +141,15 @@
         # Start both threads
         
         # Wait for both threads to finish
         http_thread.join()
         make_repo_commit(message)
         
     elif tag == "model":
+        if check_push_left():
+            print('Please use "git push" to publish your local commits')
+            sys.exit()
         model_version = model_current_version(repo)
         model_upload(message, repo, model_version)
-        
+    
     update_repo_lock(repo, json.dumps({"locked":False}))
     logger.debug('TOTAL UPLOAD TIME {0}'.format(timedelta(seconds=timer()-start)))
```

### Comparing `raga-cli-0.1.4/rc/utils/__init__.py` & `raga-cli-0.1.5/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.4/rc/utils/request.py` & `raga-cli-0.1.5/rc/utils/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,21 @@
 def get_repo_commit_id(obj):
     url = f"{BASE_URL}/repocommit/data"
     response = valid_response(make_request(url, "POST", obj))
     data = response['data']
     logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
     return data
 
+def get_repo_commit(repo):
+    url = f"{BASE_URL}/repocommit/repo/{repo}"
+    response = valid_response(make_request(url, "GET"))
+    data = response['data']
+    logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
+    return data
+
 def get_repo_version(repo):
     url = f"{BASE_URL}/repocommit/repo/{repo}"
     response = make_request(url, "GET")
     if not isinstance(response, dict):
         raise RctlValidRequestError("HTTP response is not a dict type.")
 
     if 'success' not in response.keys():
```

### Comparing `raga-cli-0.1.4/rc/utils/sshKeyGen.py` & `raga-cli-0.1.5/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

