# Comparing `tmp/edwh_restic_plugin-0.1.1.tar.gz` & `tmp/edwh_restic_plugin-0.1.2.tar.gz`

## Comparing `edwh_restic_plugin-0.1.1.tar` & `edwh_restic_plugin-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,15 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/.env
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/README.md
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/docker-compose.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/init_setup.sh
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/b2/edwh-backup-test/backup-testapplication/config
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/b2/edwh-backup-test/backup-testapplication/keys/c478566461172905eccfdbcae6dc998ca254ecfe9df93e83ff34ad56541376e7
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup-testapplication/config
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup-testapplication/keys/c23d582a6200d01d036c9306375dd8b4d29af639e5652845ffd1425a26eb2d18
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/config
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/17/179c7738522485b9492ee2497fd2fbdd8e70bd355f2b9414189f9b2f0bbd78fe
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/2a/2a9a28749c08e8e50b7fa16e60e828dd28e7c8a33faeaf07107a2b04573e3ade
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/2c/2c558eaaab62dc034164cb3fc9c32cf108141aa287b1aa09089979a8597720fc
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/5b/5bd380c6acf0811fd7f88d703a601200958b5958b207eea99276889184ff56b2
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/6c/6cb2fe6bda65a60fa99dea7f8d1963f7aab7441c20f05e724c051122e913b4a5
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/94/948414318785a325373e30c2b395245ac66859ffa924e1a197eec5d6b6ce19c1
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/b1/b1e6c0ec5d9c7fa036614ac6ba4a7ce563b3aeadac7cd3c618a744b529a7ccac
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/c4/c471141549f29b81b2d633657258bf78974eddf4405fc63b804b404e81def891
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/cd/cd57dae9e1f907c8620c7a4ef796aa6f4345133f36f9e6baf3e851923df19bcf
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/de/dede3d5b53f1fc272b2c43ac3bb944dbb44c600abaeb9907d53aef216088c18d
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/data/f1/f16a53bbc6937701666485ad5c1b27944550439bc6bfe013ee0c17c81d0cc79d
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/2e9f9bd3dbac4b6fcf559be5e79a17b80870f12d70833d25ab234f3ce5bde2b5
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/345bb728ded155b0024e1e43e630b69e2b24f1b5cc5b94d381a125392a8ca333
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/60d6718f6b0826a7d4e32336a0df8ca363a069db760583ab9bd2991d93c3a26e
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/b0c7314b6cccbff38a9de3c76ecdadd41b31a2dd7341d02367dd97c971d71b8e
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/b63a3413e88d25d9d7a7f621c7ae19c4fbee01387227c1a5609f8587adce2e0c
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/cdadd5d27853a715eefe24ff021757f057ba9427695fdb5966a716a7414fe5ca
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/dc3d219839d964c77d338aa2c57c47cba99fdf228c0d6fae2712261690bbc63d
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/index/e620ce7d15942886c9e6bc2b6c1fe1fa94abf459511939970902d63d043dabcf
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/keys/7aa0b0f309774b9f50b1815876d7d209883a3871af3cd6dacd0e01a59cd366d0
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/0732d073c4d1472182138abed6678e816ae26dfa23a3f0cdb6846e6e75f810eb
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/2fd78da7ecad3601ffd6d65d3a80a15677a4cd3b7a707a48b606e5958efcf852
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/71cde9e83949215467674538aa7f2db6855a0226a6e7e7a69bb2b76814c0911d
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/bce9095d5e93309c557d51e1936ff43cb32a13e48fa91d94d177a933e5222402
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/d4605772b65f85628fa57a794c31750770dc0b4d6c1beff42aaf5ce8863dcd4e
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/d845dc99d7fdfd3c2b6aad7c61b127ee0aa7cd75a22515774358855554c02f52
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/e21355a8d91ec8450d646758deb64f5dfbcdc95278ffcb894f39be4effb1e213
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/backup_test/snapshots/e2766b0a431988be73c17ff21d7612501a6df58c047532790ad4e46547a02c02
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/captain-hooks/backup_files_pg.sh
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/captain-hooks/backup_files_sql.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/captain-hooks/restore_stream_pg.sh
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/captain-hooks/restore_stream_sql.sh
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/init_setup.sh
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/backup_files.sh
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/backup_files_pg.sh
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/backup_files_sql.sh
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/backup_stream_pg.sh
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/restore_stream_pg.sh
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/examples/recover_data/captain-hooks/restore_stream_sql.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    23435 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/README.md
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/examples/captain-hooks/backup_files_pg.sh
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      438 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/examples/captain-hooks/restore_stream_pg.sh
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/examples/captain-hooks/restore_stream_sql.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    28448 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.2/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.1.1/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.1.2/src/edwh_restic_plugin/tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 from collections import defaultdict, OrderedDict
 
 import invoke
-from invoke import task, run, Result, Context
+from invoke import task
 
 import datetime
 import io
 import os
 from pathlib import Path
 import re
 import sys
 import typing
 import json
 
+from tqdm import tqdm
+
 # the path where the restic command is going to be executed
 DEFAULT_BACKUP_FOLDER = Path("captain-hooks")
 # the path where the environment variables are going
 DOTENV = Path(".env")
 _dotenv_settings = {}
 
 
-class Repository:
+def fix_tags(tags):
+    """
+    removes all None type elements from list
+    :param tags: list of string
+    :return:
+    """
+    i = 0
+    while i < len(tags):
+        if tags[i] is not None:
+            i += 1
+        else:
+            del tags[i]
 
-    # _targets: a list of file and directory paths that should be included in the backup.
-    # _excluded: a list of file and directory paths that should be excluded from the backup.
-    # _stream_backup_cmd: a command line string that will be used to create a backup of a stream.
-    # _stream_restore_cmd: a command line string that will be used to restore a backup from a stream.
-    # _stream_filename: the name of the file where the stream is saved.
-    # _should_exist: the path of a file that should exist.
+    return tags
 
 
+class Repository:
     # _targets: a list of file and directory paths that should be included in the backup.
     _targets = [".env", "./backup"]
     # _excluded: a list of file and directory paths that should be excluded from the backup.
     _excluded = [
         ".git",
         ".idea",
         "backups",
@@ -40,359 +49,454 @@
         "*.bak",
         "../",
         "./..",
         "errors",
         "sessions",
         "__pycache__",
     ]
-    # _stream_backup_cmd: a command line string that will be used to create a backup of a stream.
-    _stream_backup_cmd = "docker-compose run -T  --rm pg-0 pg_dump --format=p --dbname=backend --clean --create -h pgpool -U postgres"
-    # _stream_restore_cmd: a command line string that will be used to restore a backup from a stream.
-    _stream_restore_cmd = "cat - > ./migrate/data/database_to_restore.sql"
-    # naam van de stream, dus waar die in zit
-    _stream_filename = "/postgres-backend-database.sql"
-    _should_exist = "/.env"
 
     def __init__(self) -> None:
         super().__init__()
         self._restichostname = read_dotenv(DOTENV).get(
             "RESTICHOSTNAME"
-        )  # or None als niet voorkomt
+        )  # or None if it is not there
 
     @property
     def uri(self):
-        """Return de prefix nodig voor restic om het protocol aan te geven, bijvoorbeeld sftp:hostname:"""
-        raise NotImplementedError("Prefix onbekend op base class")
+        """Return the prefix required for restic to indicate the protocol, for example sftp:hostname:"""
+        raise NotImplementedError("Prefix unknown in base class")
 
     def setup(self):
-        """Zorg ervoor dat de settings in de .env file staan"""
+        """Ensure that the settings are in the .env file"""
         raise NotImplementedError("Setup undefined")
 
     def prepare_for_restic(self, c):
-        """No environment variables need be defined for local"""
+        """No environment variables need to be defined for local"""
         raise NotImplementedError("Prepare for restic undefined")
 
     def configure(self, c):
+        """Configure the backup environment variables."""
         self.prepare_for_restic(c)
         print("configure")
-        # eerst ervoor zorgen dat restic up-to-date is
+        # First, make sure restic is up-to-date
         c.run("sudo restic self-update", hide=True, warn=True)
-        # Dit is de command die gebruik wordt om de omgevingsvariabelen goed te configureren.
+        # This is the command used to configure the environment variables properly.
         c.run(f"restic init --repository-version 2 -r {self.uri}")
 
     @property
     def hostarg(self):
+        """Return the host argument for restic command."""
         return f" --host {self._restichostname} " if self._restichostname else ""
 
     @property
     def targets(self):
-        # Hierin staat de target
+        """Return the target files and directories for the backup."""
         return " ".join(self._targets)
 
     @property
     def excluded(self):
-        # wat moet er uitgesloten worden?
+        """Return the excluded files and directories for the backup.
+        Here comes the files that are going to be excluded"""
         return " --exclude ".join(self._excluded)
 
-    def get_snapshot_from(self, stdout: str):
+    @staticmethod
+    def get_snapshot_from(stdout: str):
+        """
+        Parses the stdout from a Restic command to extract the snapshot ID.
+
+        Args:
+        - stdout (str): The stdout output from a Restic command.
+
+        Returns:
+        - The snapshot ID as a string.
+                """
         snapshots_ids = re.findall(r"snapshot (.*?) saved", stdout)
         return snapshots_ids[-1] if snapshots_ids else None
 
-    def get_scripts(self, target, verb):
-        print("target =", target, "verb =", verb)
-        files = []
-        print(verb + "_" + target + "*")
-        for file in DEFAULT_BACKUP_FOLDER.glob(verb + "_" + target + "*"):
-            files.append(str(file))
-
-        if len(files) == 0:
+    @staticmethod
+    def get_scripts(target, verb):
+        """Retrieves the scripts that contain a restic command and returns them to 'execute_files' to execute them.
+
+        Args:
+        - target (str): target is a string that specifies the target of the backup, can be a file, stream, directory,
+        or any other object that needs to be backed up.
+        - verb (str): is also a string that specifies the action to be performed on the target.
+        For example, the verb could be "backup" or "restore". The verb is used in combination with the target to
+        search for the backup script files that contain the restic command.
+        """
+        # get files by verb and target. EXAMPLE backup_files_*.sh
+        files = [str(file) for file in DEFAULT_BACKUP_FOLDER.glob(f"{verb}_{target}*")]
+        # check if no files are found
+        if not files:
             print("no files found with target:", target)
             sys.exit(255)
 
         return files
 
-    def execute_files(self, c, verbose: bool, target: str, verb: str, message: str = None, snapshot: str = "latest"):
+    def execute_files(self, c, target: str, verb: str, verbose: bool, message: str = None, snapshot: str = "latest"):
+        """
+        Executes the backup scripts retrieved by 'get_scripts' function.
+
+        Args:
+        - verbose (bool): A flag indicating whether to display verbose output.
+        - target (str): The target of the backup.
+        - verb (str): The verb associated with the backup.
+        - message (str, optional): The message to be associated with the backup.
+        If not provided, the current local time is used. Defaults to None.
+        - snapshot (str, optional): The snapshot to be used for the backup. Defaults to "latest".
+        """
         self.prepare_for_restic(c)
+
+        # set snapshot available in environment for sh files
         os.environ["SNAPSHOT"] = snapshot
 
+        # Here you can make a message that you will see in the snapshots list
         if message is None:
-            message = str(datetime.datetime.now()) + " localtime"
+            # If no message is provided, use the current local time as the backup message
+            message = f"{str(datetime.datetime.now())} localtime"
 
+        # set MSG in environment for sh files
         os.environ["MSG"] = message
 
+        # get files by target and verb. see self.get_scripts for more info
         files = self.get_scripts(target, verb)
 
         snapshots_created = []
-        for file in files:
+        # run all backup/restore files
+        for file in tqdm(files):
             if verbose:
                 print("running", file)
 
-            script_stdout = c.run(file).stdout
+            script_stdout = c.run(file, warn=True).stdout
+
             snapshot = self.get_snapshot_from(script_stdout)
             snapshots_created.append(snapshot)
 
-        tags = ["message"] + snapshots_created
+        # send message with backup. see message for more info
+        # also if a tag in tags is None it will be removed by fix_tags
+        tags = fix_tags(["message"] + snapshots_created)
         c.run(
             f"restic {self.hostarg} -r {self.uri} backup --tag {','.join(tags)} --stdin --stdin-filename message",
             in_stream=io.StringIO(message),
         )
 
-    def backup(self, c, verbose: bool, target: str, verb: str, message: str):
-        self.execute_files(c, verbose, target, verb, message)
-
-    def restore(self, c, verbose: bool, target: str, verb: str, snapshot: str = "latest"):
-        self.execute_files(c, verbose, target, verb, None, snapshot)
+    def backup(self, c, verbose: bool, target: str, message: str):
+        """
+        Backs up the specified target.
+
+        Args:
+        - verbose (bool): A flag indicating whether to display verbose output.
+        - target (str): The target of the backup.
+        - verb (str): The verb associated with the backup.
+        - message (str): The message to be associated with the backup.
+        """
+        self.execute_files(c, target, "backup", verbose, message)
+
+    def restore(self, c, verbose: bool, target: str, snapshot: str = "latest"):
+        """
+            Restores the specified target using the specified snapshot or the latest if None is given.
+
+            Args:
+            - verbose (bool): A flag indicating whether to display verbose output.
+            - target (str): The target of the restore.
+            - verb (str): The verb associated with the restore.
+            - snapshot (str, optional): The snapshot to be used for the restore. Defaults to "latest".
+            """
+        self.execute_files(c, target, "restore", verbose, snapshot=snapshot)
 
     def check(self, c):
+        """
+        Checks the integrity of the backup repository.
+        """
         self.prepare_for_restic(c)
-        # Dit is de command die gebruik wordt om een check uit te voeren.
-        print("check")
         c.run(f"restic {self.hostarg} -r {self.uri} check --read-data")
 
     def snapshot(self, c, tags: list = None, n=2):
+        """
+        a list of all the backups with a message
+
+        Args:
+        - tags (list, optional): A list of tags to use for the snapshot. Defaults to None.
+        - n (int, optional): The number of latest snapshots to show. Defaults to 2.
+
+        Returns:
+        None. This function only prints the output to the console.
+        """
+        # choose to see only the files or the stream snapshots
         if tags is None:
             tags = ["files", "stream"]
 
         self.prepare_for_restic(c)
-        # Dit is de command die gebruik wordt om een snapshot uit te voeren.
         tags = "--tag " + " --tag ".join(tags) if tags else ""
         stdout = c.run(
             f"restic {self.hostarg} -r {self.uri} snapshots --latest {n} {tags} -c",
             hide=True,
         ).stdout
 
-        snapshots = re.findall(r"^([0-9a-z]{8})\s", stdout, re.MULTILINE)
+        snapshot_lines = re.findall(r"^([0-9a-z]{8})\s", stdout, re.MULTILINE)
         main_tag_per_snapshot = {
             snapshot: re.findall(rf"^{snapshot}.*?(\w*)$", stdout, re.MULTILINE)
-            for snapshot in snapshots
+            for snapshot in snapshot_lines
             # snapshot: re.findall(rf"^{snapshot}", stdout) for snapshot in snapshots
         }
 
         message_snapshot_per_snapshot = defaultdict(
             list
         )  # key is source, value is snapshot containing the message
         for snapshot, possible_tag_names in main_tag_per_snapshot.items():
             tag_name = possible_tag_names[0]
             if tag_name not in ["message"]:
                 continue
-            # print(snapshot, tag_name)
             for _, is_message_for_snapshot_id in re.findall(
                     rf"\n{snapshot}.*(\n\s+(.*)\n)+", stdout
             ):
                 message_snapshot_per_snapshot[is_message_for_snapshot_id].append(
                     snapshot
                 )
 
         for snapshot, message_snapshots in message_snapshot_per_snapshot.items():
-            # print de inhoud van de message  die hoort bij deze snapshot
+            # print all Restic messages
             restore_output = c.run(
                 f"restic {self.hostarg} -r {self.uri} dump {message_snapshots[0]} --tag message message",
                 hide=True,
                 warn=True,
             ).stdout
             message = restore_output.strip()
             stdout = re.sub(
                 rf"\n{snapshot}(.*)\n", rf"\n{snapshot}\1 : [{message}]\n", stdout
             )
         print(stdout)
 
-    def new_snapshots(self, c, tags: list = None, n=2, messages=True):
-        tags = "--tag " + " --tag ".join(tags) if tags else ""
-
 
 class LocalRepository(Repository):
+    def __init__(self):
+        super().__init__()
+        self.password = None
+        self.name = None
+
     def setup(self):
-        """Zorg ervoor dat de settings in de .env file staan"""
+        """Ensure the required settings are defined in the .env file."""
         self.name = check_env(
             DOTENV,
             "LOCAL_NAME",
             default=None,
-            comment="reponaam is verplicht",
+            comment="Repository name  is mandatory (directory)",
         )
         self.password = check_env(
             DOTENV,
             "LOCAL_PASSWORD",
             default=None,
-            comment="maak een wachtwoord, bewaar deze goed.",
+            comment="Create a password, keep it safe.",
         )
 
     def prepare_for_restic(self, c):
         """No environment variables need be defined for local"""
         env = read_dotenv(DOTENV)
         self.name = env["LOCAL_NAME"]
         os.environ["HOST"] = self.hostarg
         os.environ["URI"] = self.uri
         os.environ["RESTIC_PASSWORD"] = self.password = env["LOCAL_PASSWORD"]
 
     @property
     def uri(self):
+        """
+        Get the URI of the class instance.
+
+        The function returns the value of the 'name' attribute, which represents the URI of the class instance.
+        """
         return self.name
 
 
 class SFTPRepository(Repository):
+    def __init__(self):
+        super().__init__()
+        self.hostname = None
+        self.password = None
+        self.name = None
+
     def setup(self):
-        """Zorg ervoor dat de settings in de .env file staan"""
+        """Ensure the required settings are defined in the .env file."""
         check_env(
             DOTENV,
             "SFTP_NAME",
             default=None,
-            comment="reponaam is verplicht",
+            comment="Repository name  is mandatory (directory)",
         )
         check_env(
             DOTENV,
             "SFTP_PASSWORD",
             default=None,
-            comment="maak een wachtwoord, bewaar deze goed.",
+            comment="Create a password, keep it safe.",
         )
         check_env(
             DOTENV,
             "SFTP_HOSTNAME",
             default=None,
-            comment="voer hier de juiste hostname in.",
+            comment="Use the correnct hostname (directory above the repo name)",
         )  #
 
     def prepare_for_restic(self, c):
-        """lees variableen uit de .env file"""
+        """read out of .env file"""
         env = read_dotenv(DOTENV)
         self.name = env["SFTP_NAME"]
         self.password = env["SFTP_PASSWORD"]
         self.hostname = env["SFTP_HOSTNAME"]
         os.environ["HOST"] = self.hostarg
         os.environ["URI"] = self.uri
         os.environ["RESTIC_PASSWORD"] = self.password
-        try:
-            c.run(f'ssh {self.hostname} "exit"')
-        except:
+        ran = c.run(f'ssh {self.hostname} "exit"', warn=True, hide=True)
+        if not ran.ok:
             print(
                 """
-            SSH config bestand niet (goed) geconfigureerd, configureer volgens volgend format:
-            Host romy
+                SSH config file not (properly) configured, configure according to the following format:
+                Host romy
                 HostName romy.edwh.nl
                 User ubuntu
-                IdentityFile /home/romy/romy.key
-            Om een nieuwe host op te slaan in de ssh config file ga naar ~/.ssh en ga daar de config file in.
-            Voor meer informatie lees de ssh_config manual (man ssh_config)
-            """
+                IdentityFile ~/romy.key
+                To save a new host in the ssh config file, go to ~/.ssh and edit the config file there.
+                For more information, read the ssh_config manual (man ssh_config)
+                """
             )
             exit(1)
 
     @property
     def uri(self):
-        return "sftp:" + self.hostname + ":" + self.name
+        """
+        :return: sftp uri with self.hostname and self.name
+        """
+        return f"sftp:{self.hostname}:{self.name}"
 
 
 class B2Repository(Repository):
+    def __init__(self):
+        super().__init__()
+        self.key = None
+        self.keyid = None
+        self.bucket_name = None
+        self.password = None
+        self.name = None
+
     def setup(self):
-        """Zorg ervoor dat de settings in de .env file staan"""
+        """Ensure the required settings are defined in the .env file."""
         check_env(
             DOTENV,
             "B2_NAME",
             default=None,
-            comment="reponaam is verplicht",
+            comment="Repository name  is mandatory (directory)",
         )
         check_env(
             DOTENV,
             "B2_PASSWORD",
             default=None,
-            comment="maak een wachtwoord, bewaar deze goed.",
+            comment="Create a password, keep it safe.",
         )
         check_env(
             DOTENV,
             "B2_BUCKETNAME",
             default=None,
-            comment="voer hier de juiste bucketname in.",
+            comment="Use the correct bucketname (directory above repo name",
         )
         check_env(
             DOTENV,
             "B2_ACCOUNT_ID",
             default=None,
-            comment="voer hier de juiste KEY ID in.",
+            comment="enter the correct KEY ID here.",
         )
         check_env(
             DOTENV,
             "B2_ACCOUNT_KEY",
             default=None,
-            comment="gvoer hier de juiste KEY in.",
+            comment="enter the correct KEY here.",
         )
 
     def prepare_for_restic(self, c):
-        """lees variableen uit de .env file"""
+        """read variables out of .env file"""
         env = read_dotenv(DOTENV)
         self.name = env["B2_NAME"]
         self.password = env["B2_PASSWORD"]
-        self.bucketname = env["B2_BUCKETNAME"]
+        self.bucket_name = env["B2_BUCKETNAME"]
         self.keyid = env["B2_ACCOUNT_ID"]
         self.key = env["B2_ACCOUNT_KEY"]
         os.environ["B2_ACCOUNT_ID"] = self.keyid
         os.environ["B2_ACCOUNT_KEY"] = self.key
         os.environ["RESTIC_PASSWORD"] = self.password
         os.environ["HOST"] = self.hostarg
         os.environ["URI"] = self.uri
 
     @property
     def uri(self):
-        return "b2:" + self.bucketname + ":" + self.name
+        """
+        :return: uri of b2 with self.bucketname and self.name
+        """
+        return f"b2:{self.bucket_name}:{self.name}"
 
 
 class SwiftRepository(Repository):
+    def __init__(self):
+        super().__init__()
+        self.restic_password = None
+        self.password = None
+        self.container_name = None
+        self.name = None
+
     def setup(self):
-        """Zorg ervoor dat de settings in de .env file staan"""
+        """Ensure the required settings are defined in the .env file."""
         check_env(
             DOTENV,
             "OS_AUTH_URL",
             default="https://identity.stack.cloudvps.com/v2.0",
-            comment="Auth URL voor deze openstack omgeving",
+            comment="Auth URL for this openstack environment",
         )
         check_env(
             DOTENV,
             "OS_TENANT_ID",
             default=None,
-            comment='Tenant naam, komt uit de openrc file, of uit de auth info, lijkt op "f8d15....269"',
+            comment='Tenant name, comes from the openrc file, or from the auth info, looks like "f8d15....269"',
         )
         check_env(
             DOTENV,
             "OS_TENANT_NAME",
             default="BST000425 productie-backups",
-            comment="Projectnaam binnen openstack, bijvoorbeeld 'BST000425 productie-backups'",
+            comment="Project name within openstack, for example 'BST000425 production backups'",
         )
         check_env(
             DOTENV,
             "OS_REGION_NAME",
             default="NL",
-            comment="NL wordt ondersteund, andere zijn onbekend.",
+            comment="NL is supported, others are unknown.",
         )
         check_env(
             DOTENV,
             "OS_USERNAME",
             default="backup@edwh.nl",
-            comment="Username is het openstack username",
+            comment="Username is the openstack username",
         )
         check_env(
             DOTENV,
             "OS_PASSWORD",
             default=None,
-            comment="Password behorend bij de openstack gebruiker",
+            comment="Password belonging to the openstack user",
         )
         check_env(
             DOTENV,
             "OS_CONTAINERNAME",
             default="backups",
-            comment="Objectstore container naam, zou automatisch aangemaakt moeten worden als het niet bestaat.",
+            comment="Objectstore container name, should be created automatically if it doesn't exist.",
         )
         check_env(
             DOTENV,
             "OS_NAME",
             default=None,
-            comment="Repository naam binnen de bucket",
+            comment="Repository name within the bucket",
         )
         check_env(
             DOTENV,
             "OS_RESTIC_PASSWORD",
             default=None,
-            comment="Wachtwoord van de repository binnen de container",
+            comment="Password of the repository within the container",
         )
 
         # check_env(
         #     DOTENV,
         #     "OS_STORAGE_URL",
         #     default=None,
         #     comment="voer hier de juiste URL in.",
@@ -401,33 +505,36 @@
         #     DOTENV,
         #     "OS_AUTH_TOKEN",
         #     default=None,
         #     comment="gvoer hier de juiste TOKEN in.",
         # )
 
     def prepare_for_restic(self, c):
-        """lees variableen uit de .env file"""
+        """read variables out of .env file"""
         env = read_dotenv(DOTENV)
         self.name = env["OS_NAME"]
-        self.containername = env["OS_CONTAINERNAME"]
+        self.container_name = env["OS_CONTAINERNAME"]
         os.environ["OS_USERNAME"] = env["OS_USERNAME"]
         os.environ["OS_AUTH_URL"] = env["OS_AUTH_URL"]
         os.environ["OS_TENANT_ID"] = env["OS_TENANT_ID"]
         os.environ["OS_TENANT_NAME"] = env["OS_TENANT_NAME"]
         os.environ["OS_REGION_NAME"] = env["OS_REGION_NAME"]
         # os.environ["OS_STORAGE_URL"] = self.keyid = env["OS_STORAGE_URL"]
         # os.environ["OS_AUTH_TOKEN"] = self.key = env["OS_AUTH_TOKEN"]
         os.environ["OS_PASSWORD"] = self.password = env["OS_PASSWORD"]
         os.environ["RESTIC_PASSWORD"] = self.restic_password = env["OS_RESTIC_PASSWORD"]
         os.environ["HOST"] = self.hostarg
         os.environ["URI"] = self.uri
 
     @property
     def uri(self):
-        return "swift:" + self.containername + ":/" + self.name
+        """
+        :return: the swift uri with self.containername and self.name
+        """
+        return f"swift:{self.container_name}:/{self.name}"
 
 
 def set_env_value(path: Path, target: str, value: str) -> None:
     """update/set environment variables in the .env file, keeping comments intact
 
     set_env_value(Path('.env'), 'SCHEMA_VERSION', schemaversion)
 
@@ -460,21 +567,34 @@
             # add the new tuple to the lines
             outlines.append(f"{key}={value}")
             geschreven = True
         else:
             # or leave it as it is
             outlines.append(line)
     if not geschreven:
-        outlines.append(f"{target.strip().upper()}={str(value).strip()}")
+        # if target in .env file
+        outlines.append(f"{target.strip().upper()}={value.strip()}")
     with path.open(mode="w") as env_file:
+        # write outlines to .env file
         env_file.write("\n".join(outlines))
         env_file.write("\n")
 
 
 def read_dotenv(path: Path) -> dict:
+    """Reads a .env file at the specified path and returns a dictionary of key - value pairs.
+
+    If the specified key is not found in the.env file, the function prompts the user to enter a value for the key,
+    with a default value provided.The key-value pair is then appended to the.env file.
+
+    Args:
+        path(Path): The path to the .env file.
+
+    Returns:
+        dict: A dictionary containing the key - value pairs in the .env file."""
+
     if existing := _dotenv_settings.get(path):
         # 'cache'
         return existing
 
     items = {}
     with path.open(mode="r") as env_file:
         for line in env_file:
@@ -503,154 +623,178 @@
         prefix: str | None = None,
         postfix: str | None = None,
 ):
     """
     Test if key is in .env file path, appends prompted or default value if missing.
     """
     env = read_dotenv(path)
-    if key not in env:
-        with path.open(mode="r+") as env_file:
-            response = input(
-                f"Enter value for {key} ({comment})\n default=`{default}`: "
-            )
-            value = response.strip() or default
-            if prefix:
-                value = prefix + value
-            if postfix:
-                value += postfix
-            env_file.seek(0, 2)
-            env_file.write(f"\n{key.upper()}={value}\n")
-
-            # update in memory too:
-            env[key] = value
-            return value
-    else:
+    if key in env:
         return env[key]
-
-
+    with path.open(mode="r+") as env_file:
+        # get response value from prompt/input
+        response = input(
+            f"Enter value for {key} ({comment})\n default=`{default}`: "
+        )
+        # if response_value is none make value default else value is response_value
+        value = response.strip() or default
+        if prefix:
+            value = prefix + value
+        if postfix:
+            value += postfix
+        env_file.seek(0, 2)
+        # write key and value to .env file
+        env_file.write(f"\n{key.upper()}={value}\n")
+
+        # update in memory too:
+        env[key] = value
+        return value
+
+
+# the order in which the backup will be saved
+# Swift is the most secure for us, because of the keys
+# B2 is also very secure, only less
+# SFTP is the least secure, if were talking about remote saving
+# Local can be a good option, but if your pc got broken, you have lost your backup
 CONNECTION_CLASS_MAP = OrderedDict(
     os=SwiftRepository,
     b2=B2Repository,
     sftp=SFTPRepository,
     local=LocalRepository,
 )
 
 
-def cli_repo(c, connection_choice=None, restichostname=None):
+def cli_repo(connection_choice=None, restichostname=None):
+    """
+    Create a repository object and set up the connection to the backend.
+    :param connection_choice: choose where you want to store the repo (local, SFTP, B2, swift)
+    :param restichostname: which hostname to force for restic, or blank for default.
+    :return: repository object
+    """
     env = read_dotenv(DOTENV)
     if restichostname:
         set_env_value(DOTENV, "RESTICHOSTNAME", restichostname)
     if connection_choice is None:
-        #  zoek de meest belangrijke backup mogelijk op als default.
+        # search for the most important backup and use it as default
         for connection_choice in CONNECTION_CLASS_MAP.keys():
             connection_lowercase = connection_choice.lower()
-            if connection_choice.upper() + "_NAME" in env:
+            if f"{connection_choice.upper()}_NAME" in env:
                 break
     else:
         connection_lowercase = connection_choice.lower()
     repoclass = CONNECTION_CLASS_MAP[connection_lowercase]
-    print("Gebruikt connectie: ", connection_lowercase)
+    print("Use connection: ", connection_lowercase)
     repo = repoclass()
     repo.setup()
     return repo
 
 
 @task
 def configure(c, connection_choice=None, restichostname=None):
     """Setup or update the backup command for your environment.
     connection_choice: choose where you want to store the repo (local, SFTP, B2, swift)
     restichostname: which hostname to force for restic, or blank for default.
     """
 
-    # Er is gekozen om voor elke repository een hoofdpad aan te maken genaamd 'backups'.
-    # Deze kan eventueel veranderd en weggehaald worden indien gewenst.
-    # Een password wordt slechts bij een aantal fucnties meegegeven.
-    cli_repo(c, connection_choice, restichostname).configure(c)
+    # It has been decided to create a main path called 'backups' for each repository.
+    # This can be changed or removed if desired.
+    # A password is only passed with a few functions.
+    cli_repo(connection_choice, restichostname).configure(c)
 
 
 @task
 def backup(c, target="", connection_choice=None, message=None, verbose=False):
-    # Na 'backup' kan een bestandspad worden opgegeven, in dit script is gekozen voor een testbestand.
-    # './test/testbestand' kan vervangen worden door het gewenste pad waarover restic een backup moet uitvoeren.
-    # De optie --verbose geeft meet informatie mee over de backup die gemaakt is. Deze kan ev. weggehaald worden.
+    """Performs a backup operation using restic on a local or remote/cloud file system.
+
+    Args:
+        target (str): The path of the file or directory to backup. Defaults to an empty string.
+        connection_choice (str): The name of the connection to use for the backup.
+            Defaults to None, which means the default connection will be used.
+        message (str): A message to attach to the backup snapshot.
+            Defaults to None, which means no message will be attached.
+        verbose (bool): If True, outputs more information about the backup process. Defaults to False.
+
+    Raises:
+        Exception: If an error occurs during the backup process.
+
+    """
+    # After 'backup', a file path can be specified.In this script, a test file is chosen at './test/testbestand'.
+    # It can be replaced with the desired path over which restic should perform a backup.
+    # The option --verbose provides more information about the backup that is made.It can be removed if desired.
 
-    # Door gebruik te maken van toevoegingen kan specifiek weergegeven worden wat meegenomen moet worden:
+    # By using additions, it is possible to specify what should be included:
     # --exclude ,Specified one or more times to exclude one or more items.
     # --iexclude, Same as --exclude but ignores the case of paths.
     # --exclude-caches, Specified once to exclude folders containing this special file.
     # --exclude-file, Specified one or more times to exclude items listed in a given file.
     # --iexclude-file, Same as exclude-file but ignores cases like in --iexclude.
     # --exclude-if-present 'foo', Specified one or more times to exclude a folder’s content if it contains.
     # a file called 'foo' (optionally having a given header, no wildcards for the file name supported).
     # --exclude-larger-than 'size', Specified once to excludes files larger than the given size.
     # Please see 'restic help backup' for more specific information about each exclude option.
-    # cli_repo(c, connection_choice).backup(c, files, message)
 
-    try:
-        cli_repo(c, connection_choice).backup(c, verbose, target, "backup", message)
-    except:
-        print(f"[ERROR] while backing up to {connection_choice or 'default connection'}")
-        raise
+    cli_repo(connection_choice).backup(c, verbose, target, message)
 
 
 @task
 def restore(
-    c,
-    connection_choice=None,
-    snapshot="latest",
-    target="",
-    verbose=False
+        c,
+        connection_choice=None,
+        snapshot="latest",
+        target="",
+        verbose=False
 ):
     """
-    IMPORTANT: please fill in -t for a path where the restore can go. Also remember to put in a -c for at what service
-    you stored the backup.
+    The restore function restores the latest backed-up files by default and puts them in a restore folder.
+
+    IMPORTANT: please provide -t for the path where the restore should go. Also remember to include -c for the service
+    where the backup is stored.
 
-    the restore function restores the latest backup-ed files by default and puts it into a restore folder.
-    :param c: invoke
-    :param connection_choice: service where the files are backed op, think about local or openstack
-    :param snapshot: by default snapshot is latest, snapshot is the id where the files are backed-up
-    :param target: location where the backup gets dumped
-    :param verbose: logs(inv restore -v)
+    :param connection_choice: the service where the files are backed up, e.g., 'local' or 'openstack'.
+    :param snapshot: the ID where the files are backed up, default value is 'latest'.
+    :param target: the location where the backup should be restored.
+    :param verbose: display verbose logs (inv restore -v).
     :return: None
     """
-    # Bij restore is --target de locatie waarin de restore geplaatst mag worden, --path is het bestand/pad die uit de
-    # repository gehaald mag worden. 'which_restore' is hierbij een input van de gebruiker, om zo een eerdere restore
-    # mogelijk te maken (default = latest).
-    # stoppen van de postgres services
+    # For restore, --target is the location where the restore should be placed, --path is the file/path that should be
+    # retrieved from the repository.
+    # 'which_restore' is a user input to enable restoring an earlier backup (default = latest).
+    # Stop the postgres services.
     c.run("docker-compose stop -t 1 pg-0 pg-1 pgpool", warn=True, hide=True)
 
-    # opvragen welke volumes gebruikt worden
+    # Get the volumes that are being used.
     docker_inspect: invoke.Result = c.run(
         "docker inspect pg-0 pg-1", hide=True, warn=True
     )
     if docker_inspect.ok:
-        # alleen als ok, want als pg-0 en pg-1 niet bestaan, is dit er niet, en hoeft er ook niets verwijderd te worden.
+        # Only if ok, because if pg-0 and pg-1 do not exist, this does not exist either, and nothing needs to be removed
         inspected = json.loads(docker_inspect.stdout)
-        te_verwijderen_volumes = []
+        volumes_to_remove = []
         for service in inspected:
-            for mount in service["Mounts"]:
-                if mount["Type"] == "volume":
-                    te_verwijderen_volumes.append(mount["Name"])
-        # containers verwijderen, voordat een volume verwijderd kan worden
+            volumes_to_remove.extend(
+                mount["Name"]
+                for mount in service["Mounts"]
+                if mount["Type"] == "volume"
+            )
+        # Remove the containers before a volume can be removed.
         c.run("docker-compose rm -f pg-0 pg-1")
-        # volumes verwijderen
-        for volume_name in te_verwijderen_volumes:
-            c.run("docker volume rm " + volume_name)
+        # Remove the volumes.
+        for volume_name in volumes_to_remove:
+            c.run(f"docker volume rm {volume_name}")
 
-    cli_repo(c, connection_choice).restore(c, verbose, target, "restore", snapshot)
-    # print("`inv up` om de services te herstarten ")
+    cli_repo(connection_choice).restore(c, verbose, target, snapshot)
+    # print("`inv up` to restart the services.")
 
 
 @task(iterable=['tag'])
 def snapshots(c, connection_choice=None, tag=None, n=1):
     """
     With this je can see per repo which repo is made when and where, the repo-id can be used at inv restore as an option
-    :param c: invoke
     :param connection_choice: service
     :param tag: files, stream ect
     :param n: amount of snapshot to view, default=1(latest)
     :return: None
     """
+    # if tags is None set tag to default tags
     if tag is None:
         tag = ["files", "stream"]
 
-    cli_repo(c, connection_choice).snapshot(c, tags=tag, n=n)
+    cli_repo(connection_choice).snapshot(c, tags=tag, n=n)
```

### Comparing `edwh_restic_plugin-0.1.1/LICENSE.txt` & `edwh_restic_plugin-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.1.1/pyproject.toml` & `edwh_restic_plugin-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
- 'invoke'
+  'invoke',
+  'tqdm'
 ]
 
 [project.entry-points."edwh.tasks"]
 restic = "edwh_restic_plugin.tasks"
 
 [project.urls]
 Documentation = "https://github.com/unknown/edwh-restic-plugin#readme"
@@ -156,7 +157,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.semantic_release]
+branch = "main"
+version_variable = "src/edwh_restic_plugin/__about__.py:__version__"
+change_log = "CHANGELOG.md"
+upload_to_repository = false
+upload_to_release = false
+build_command = "hatch build"
```

