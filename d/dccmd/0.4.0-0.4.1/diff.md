# Comparing `tmp/dccmd-0.4.0.tar.gz` & `tmp/dccmd-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccmd-0.4.0.tar", max compression
+gzip compressed data, was "dccmd-0.4.1.tar", max compression
```

## Comparing `dccmd-0.4.0.tar` & `dccmd-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11343 2022-07-17 08:39:13.687368 dccmd-0.4.0/LICENSE
--rw-r--r--   0        0        0    15516 2023-01-22 15:39:41.700807 dccmd-0.4.0/README.md
--rw-r--r--   0        0        0    37614 2023-01-22 15:41:29.211301 dccmd-0.4.0/dccmd/__init__.py
--rw-r--r--   0        0        0        0 2022-07-17 08:39:13.688213 dccmd-0.4.0/dccmd/main/__init__.py
--rw-r--r--   0        0        0     2693 2022-07-22 20:15:29.962402 dccmd-0.4.0/dccmd/main/auth/__init__.py
--rw-r--r--   0        0        0     1971 2022-07-17 08:39:13.688616 dccmd-0.4.0/dccmd/main/auth/client.py
--rw-r--r--   0        0        0     2434 2022-07-17 08:39:13.688752 dccmd-0.4.0/dccmd/main/auth/credentials.py
--rw-r--r--   0        0        0    10257 2023-01-22 11:07:05.095863 dccmd-0.4.0/dccmd/main/auth/util.py
--rw-r--r--   0        0        0     3645 2022-07-17 08:39:13.689118 dccmd-0.4.0/dccmd/main/crypto/__init__.py
--rw-r--r--   0        0        0     1846 2022-07-17 08:39:13.689243 dccmd-0.4.0/dccmd/main/crypto/keys.py
--rw-r--r--   0        0        0     1769 2023-01-21 23:21:31.335275 dccmd-0.4.0/dccmd/main/crypto/util.py
--rw-r--r--   0        0        0     8669 2023-01-21 10:56:30.365757 dccmd-0.4.0/dccmd/main/download/__init__.py
--rw-r--r--   0        0        0     1516 2023-01-21 11:28:21.229986 dccmd-0.4.0/dccmd/main/models/__init__.py
--rw-r--r--   0        0        0     1158 2022-07-18 05:43:46.467561 dccmd-0.4.0/dccmd/main/models/errors.py
--rw-r--r--   0        0        0    11784 2023-01-22 01:34:41.689501 dccmd-0.4.0/dccmd/main/rooms/__init__.py
--rw-r--r--   0        0        0      118 2023-01-22 01:30:18.503409 dccmd-0.4.0/dccmd/main/rooms/models.py
--rw-r--r--   0        0        0    10485 2023-01-22 10:36:30.835650 dccmd-0.4.0/dccmd/main/rooms/permissions.py
--rw-r--r--   0        0        0     3128 2023-01-21 09:59:38.704681 dccmd-0.4.0/dccmd/main/rooms/print.py
--rw-r--r--   0        0        0    10483 2023-01-22 15:23:20.095446 dccmd-0.4.0/dccmd/main/upload/__init__.py
--rw-r--r--   0        0        0     4423 2022-07-19 16:30:43.809515 dccmd-0.4.0/dccmd/main/users/__init__.py
--rw-r--r--   0        0        0     9731 2023-01-21 11:06:14.389047 dccmd-0.4.0/dccmd/main/users/manage.py
--rw-r--r--   0        0        0     1902 2023-01-22 10:37:48.703546 dccmd-0.4.0/dccmd/main/users/print.py
--rw-r--r--   0        0        0     4747 2022-10-02 14:23:57.076852 dccmd-0.4.0/dccmd/main/util/__init__.py
--rw-r--r--   0        0        0      651 2023-01-21 10:55:55.856028 dccmd-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    17045 2023-01-22 15:41:35.590135 dccmd-0.4.0/setup.py
--rw-r--r--   0        0        0    16185 2023-01-22 15:41:35.590720 dccmd-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-07-17 08:39:13.687368 dccmd-0.4.1/LICENSE
+-rw-r--r--   0        0        0    15516 2023-01-24 17:08:53.088409 dccmd-0.4.1/README.md
+-rw-r--r--   0        0        0    37619 2023-05-02 17:15:58.749056 dccmd-0.4.1/dccmd/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-17 08:39:13.688213 dccmd-0.4.1/dccmd/main/__init__.py
+-rw-r--r--   0        0        0     2693 2022-07-22 20:15:29.962402 dccmd-0.4.1/dccmd/main/auth/__init__.py
+-rw-r--r--   0        0        0     1971 2022-07-17 08:39:13.688616 dccmd-0.4.1/dccmd/main/auth/client.py
+-rw-r--r--   0        0        0     2434 2022-07-17 08:39:13.688752 dccmd-0.4.1/dccmd/main/auth/credentials.py
+-rw-r--r--   0        0        0    10257 2023-01-24 17:08:53.089168 dccmd-0.4.1/dccmd/main/auth/util.py
+-rw-r--r--   0        0        0     3645 2022-07-17 08:39:13.689118 dccmd-0.4.1/dccmd/main/crypto/__init__.py
+-rw-r--r--   0        0        0     1846 2022-07-17 08:39:13.689243 dccmd-0.4.1/dccmd/main/crypto/keys.py
+-rw-r--r--   0        0        0     1769 2023-01-24 17:08:53.089465 dccmd-0.4.1/dccmd/main/crypto/util.py
+-rw-r--r--   0        0        0     8669 2023-05-02 16:44:40.001311 dccmd-0.4.1/dccmd/main/download/__init__.py
+-rw-r--r--   0        0        0     1516 2023-01-24 17:08:53.090050 dccmd-0.4.1/dccmd/main/models/__init__.py
+-rw-r--r--   0        0        0     1158 2022-07-18 05:43:46.467561 dccmd-0.4.1/dccmd/main/models/errors.py
+-rw-r--r--   0        0        0    11768 2023-05-02 17:14:14.445184 dccmd-0.4.1/dccmd/main/rooms/__init__.py
+-rw-r--r--   0        0        0      118 2023-01-24 17:08:53.090505 dccmd-0.4.1/dccmd/main/rooms/models.py
+-rw-r--r--   0        0        0    10440 2023-05-02 17:14:08.232455 dccmd-0.4.1/dccmd/main/rooms/permissions.py
+-rw-r--r--   0        0        0     3128 2023-01-24 17:08:53.090892 dccmd-0.4.1/dccmd/main/rooms/print.py
+-rw-r--r--   0        0        0    11196 2023-05-02 17:37:42.191534 dccmd-0.4.1/dccmd/main/upload/__init__.py
+-rw-r--r--   0        0        0     4423 2022-07-19 16:30:43.809515 dccmd-0.4.1/dccmd/main/users/__init__.py
+-rw-r--r--   0        0        0     9731 2023-05-02 16:44:45.195480 dccmd-0.4.1/dccmd/main/users/manage.py
+-rw-r--r--   0        0        0     1902 2023-01-24 17:08:53.097355 dccmd-0.4.1/dccmd/main/users/print.py
+-rw-r--r--   0        0        0     4747 2023-01-24 17:08:53.097677 dccmd-0.4.1/dccmd/main/util/__init__.py
+-rw-r--r--   0        0        0      652 2023-05-02 17:39:22.245290 dccmd-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17046 2023-05-02 17:39:55.363215 dccmd-0.4.1/setup.py
+-rw-r--r--   0        0        0    16186 2023-05-02 17:39:55.363829 dccmd-0.4.1/PKG-INFO
```

### Comparing `dccmd-0.4.0/LICENSE` & `dccmd-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/README.md` & `dccmd-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/__init__.py` & `dccmd-0.4.1/dccmd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 DRACOON Commander
 A CLI DRACOON client
 
 """
 
-__version__ = "0.4.0"
+__version__ = "0.4.2-SNAPSHOT"
 
 # std imports
 import sys
 import os
 import asyncio
 
 # external imports
@@ -932,15 +932,15 @@
 @app.command()
 def version():
     """
     Dsiplay current version of DRACOON Commander
     """
 
     typer.echo(
-               "@@@@@@@@@@@@@@@@@@      @@@@@@@@@@@@@@@@@@      @@@@@@@@@@@@@@@@@@      @@@@@@@@@        @@@@@@@@@   @@@@@@@@@@@@@@@@@@\n"                                               
+               "@@@@@@@@@@@@@@@@@@      @@@@@@@@@@@@@@@@@@      @@@@@@@@@@@@@@@@@@      @@@@@@@@@        @@@@@@@@@   @@@@@@@@@@@@@@@@@@\n"                                           
                "@@@@@@@@@@@@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@@  @@@@@@@@@@      @@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@\n"                                           
                "@@@@@@@@@@@@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@@  @@@@@@@@@@@    @@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@\n"                                           
                "@@@@@@@@@@@@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@@  @@@@@@@@@@@@   @@@@@@@@@@@   @@@@@@@@@@@@@@@@@@@@@\n"                                           
                "@@@@@@@@     @@@@@@@@   @@@@@@@@                @@@@@@@@                @@@@@@@@@@@@@ @@@@@@@@@@@@   @@@@@@@@     @@@@@@@@\n"                                           
                "@@@@@@@@     @@@@@@@@   @@@@@@@@                @@@@@@@@                @@@@@@@@@@@@@@@@@@@@@@@@@@   @@@@@@@@     @@@@@@@@\n"                                           
                "@@@@@@@@     @@@@@@@@   @@@@@@@@                @@@@@@@@                @@@@@@@@@@@@@@@@@@@@@@@@@@   @@@@@@@@     @@@@@@@@\n"                                           
                "@@@@@@@@     @@@@@@@@   @@@@@@@@                @@@@@@@@                @@@@@@@@@@@@@@@@@@@@@@@@@@   @@@@@@@@     @@@@@@@@\n"
```

### Comparing `dccmd-0.4.0/dccmd/main/auth/__init__.py` & `dccmd-0.4.1/dccmd/main/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/auth/client.py` & `dccmd-0.4.1/dccmd/main/auth/client.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/auth/credentials.py` & `dccmd-0.4.1/dccmd/main/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/auth/util.py` & `dccmd-0.4.1/dccmd/main/auth/util.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/crypto/__init__.py` & `dccmd-0.4.1/dccmd/main/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/crypto/keys.py` & `dccmd-0.4.1/dccmd/main/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/crypto/util.py` & `dccmd-0.4.1/dccmd/main/crypto/util.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/download/__init__.py` & `dccmd-0.4.1/dccmd/main/download/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/models/__init__.py` & `dccmd-0.4.1/dccmd/main/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/models/errors.py` & `dccmd-0.4.1/dccmd/main/models/errors.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/rooms/__init__.py` & `dccmd-0.4.1/dccmd/main/rooms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
         user_permissions = await get_room_user_permissions(room_id=node_info.id, dracoon=dracoon)
 
         if csv:
             csv_print_user_perms(user_permissions=user_permissions)
         else:
             pretty_print_user_perms(user_permissions=user_permissions)
-        
+
         await dracoon.logout()
 
     asyncio.run(_list_users())
 
 @rooms_app.command()
 def list_groups(
     source_path: str = typer.Argument(
@@ -339,12 +339,12 @@
 
         group_permissions = await get_room_group_permissions(room_id=node_info.id, dracoon=dracoon)
 
         if csv:
             csv_print_group_perms(group_permissions=group_permissions)
         else:
             pretty_print_group_perms(group_permissions=group_permissions)
-        
+
         await dracoon.logout()
 
     asyncio.run(_list_groups())
```

### Comparing `dccmd-0.4.0/dccmd/main/rooms/permissions.py` & `dccmd-0.4.1/dccmd/main/rooms/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 async def add_room_group(room_id: int, name: str, permission_template: PermissionTemplate, dracoon: DRACOON):
     """ assign a group to a room """
     group = await get_group_by_name(room_id=room_id, name=name, dracoon=dracoon)
     permissions = create_permissions(permissions=permission_template, dracoon=dracoon)
     #group_update = dracoon.nodes.make_permission_update(id=group.id, permission=permissions)
     groups_update = UpdateRoomGroups(items=[UpdateRoomGroupItem(id=group.id, permissions=permissions)])
-    dracoon.logger.debug(groups_update)
+
     try:
         await dracoon.nodes.update_room_groups(room_id=room_id, groups_update=groups_update)
     except HTTPForbiddenError:
         await dracoon.logout()
         typer.echo(
             format_error_message(
             msg="Insufficient permissions (room admin required)."
@@ -272,16 +272,16 @@
     """ set room admin specific permissions """
     permissions.manage = True
     permissions.deleteRecycleBin = True
 
 def create_permissions(permissions: PermissionTemplate, dracoon: DRACOON) -> Permissions:
     """ create permission payload from template """
 
-    perms = dracoon.nodes.make_permissions(manage=False, read=False, create=False, change=False, delete=False, manage_shares=False, 
-                                           manage_file_requests=False, delete_recycle_bin=False, restore_recycle_bin=False, 
+    perms = dracoon.nodes.make_permissions(manage=False, read=False, create=False, change=False, delete=False, manage_shares=False,
+                                           manage_file_requests=False, delete_recycle_bin=False, restore_recycle_bin=False,
                                            read_recycle_bin=False)
 
     if not isinstance(permissions, PermissionTemplate):
         raise DCInvalidArgumentError
 
     if permissions == PermissionTemplate.READ:
         set_read_perms(permissions=perms)
@@ -291,15 +291,15 @@
         set_edit_perms(permissions=perms)
 
 
     if permissions == PermissionTemplate.ROOM_ADMIN:
         set_read_perms(permissions=perms)
         set_read_perms(permissions=perms)
         set_room_admin_perms(permissions=perms)
-    
+
     return perms
 
 def parse_permissions_template(perms: str) -> PermissionTemplate:
     """ parse str into template """
     perms = perms.lower()
 
     if perms == 'read':
```

### Comparing `dccmd-0.4.0/dccmd/main/rooms/print.py` & `dccmd-0.4.1/dccmd/main/rooms/print.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/upload/__init__.py` & `dccmd-0.4.1/dccmd/main/upload/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,29 +81,33 @@
         self.abs_path = self.dir_path.replace(base_path, "")
         self.name = self.abs_path.split("/")[-1]
         self.parent_path = ("/").join(self.abs_path.split("/")[:-1])
         self.level = len(self.abs_path.split("/")) - 1
         self.size = os.path.getsize(self.dir_path)
         self.x_size = self.x_path.stat().st_size
 
-
 class FileItemList:
     """object representing all files in a path (recursively)"""
 
     def __init__(self, source_path: str):
 
         # reject invalid source paths
         if not is_directory(folder_path=source_path):
             raise InvalidPathError()
 
         # get list of all files
         self.file_list = [
             FileItem(dir_path, source_path)
             for dir_path in fast_scanfile(dirname=source_path)
         ]
+
+        self.ignored_files = [file_item for file_item in self.file_list if not validate_file_name(file_item.name)]
+        # reject invalid file names
+        self.file_list = [file_item for file_item in self.file_list if validate_file_name(file_item.name)]
+
         # get unique levels
         self.levels = set([file_item.level for file_item in self.file_list])
 
     def get_level(self, level: int) -> list[FileItem]:
         """get depth level by number"""
         return [item for item in self.file_list if item.level == level]
 
@@ -116,15 +120,15 @@
         """ returns file count """
         return len(self.file_list)
 
     @property
     def total_size(self):
         """ return total size in bytes """
         return sum([item.size for item in self.file_list])
-    
+
 def convert_to_dir_items(dir_list: list[str], base_dir: str) -> list[DirectoryItem]:
     """convert a list of paths to a list of directory items (helper class)"""
 
     #pylint: disable=W0108
     dir_list.sort(key=lambda x: len(x))
     parsed_list = [DirectoryItem(dir_path=x, base_path=base_dir) for x in dir_list]
     parsed_list.sort(key=lambda dir: dir.level)
@@ -176,15 +180,15 @@
         velocity = 10
     elif velocity < 1:
         velocity = 1
 
     async def process_batch(batch):
         """process a batch of folders to create"""
 
-        path = target + '/' + batch[0].parent_path
+        path = target.rstrip('/') + '/' + batch[0].parent_path.lstrip('/')
         parent_node = await dracoon.nodes.get_node_from_path(path)
 
         if parent_node is None:
             dracoon.logger.debug(path)
 
         parent_id = parent_node.id
 
@@ -254,33 +258,40 @@
     dracoon: DRACOON,
     resolution_strategy: str = "fail",
     velocity: int = 2,
 ):
     """upload a list of files in a given source path"""
 
     file_list = FileItemList(source_path=source)
+
+    dracoon.logger.info(f"Ignored files: {len(file_list.ignored_files)}")
+
+    for file in file_list.ignored_files:
+        dracoon.logger.info(f"Ignoring file: {file.dir_path}")
+
     file_list.sort_by_size()
     transfer_list = DCTransferList(total=file_list.total_size, file_count=file_list.file_count)
 
     if velocity > 10:
         velocity = 10
     elif velocity < 1:
         velocity = 1
 
     concurrent_reqs = velocity * 5
 
     upload_reqs = []
 
     for item in file_list.file_list:
         upload_job = DCTransfer(transfer=transfer_list)
-        dracoon.logger.info(target + '/' + item.parent_path)
-        dracoon.logger.info(item.dir_path)
+        dracoon.logger.debug(target + '/' + item.parent_path)
+        dracoon.logger.debug(item.dir_path)
+        target_path = target.rstrip('/') + '/' + item.parent_path.lstrip('/')
         req = dracoon.upload(
             file_path=item.dir_path,
-            target_path=(target + '/' + item.parent_path),
+            target_path=(target_path),
             resolution_strategy=resolution_strategy,
             callback_fn=upload_job.update
         )
         upload_reqs.append(asyncio.ensure_future(req))
 
     for batch in dracoon.batch_process(
             coro_list=upload_reqs, batch_size=concurrent_reqs
@@ -313,7 +324,15 @@
 
 
 def create_folder(name: str, parent_id: int, dracoon: DRACOON):
     """helper to create folder creation requests"""
 
     folder = dracoon.nodes.make_folder(name=name, parent_id=parent_id)
     return dracoon.nodes.create_folder(folder=folder, raise_on_err=True)
+
+def validate_file_name(name: str) -> str:
+    """ validate file name """
+    # return false if name length is more than 150 chars
+    if len(name) > 150:
+        return False
+
+    return True
```

### Comparing `dccmd-0.4.0/dccmd/main/users/__init__.py` & `dccmd-0.4.1/dccmd/main/users/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/users/manage.py` & `dccmd-0.4.1/dccmd/main/users/manage.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/users/print.py` & `dccmd-0.4.1/dccmd/main/users/print.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/dccmd/main/util/__init__.py` & `dccmd-0.4.1/dccmd/main/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.0/pyproject.toml` & `dccmd-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "dccmd"
-version = "0.4.0"
+version = "0.4.1"
 description = "DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)"
 authors = ["Octavio Simone <70800577+unbekanntes-pferd@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "^0.4.0"
-dracoon = "^1.9.0"
+dracoon = "^1.10.0"
 keyring = "^23.6.0"
 SecretStorage = "^3.3.1"
-tqdm = "^4.64.1"
+tqdm = "^4.65.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dccmd-0.4.0/setup.py` & `dccmd-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,25 +14,25 @@
  'dccmd.main.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['SecretStorage>=3.3.1,<4.0.0',
- 'dracoon>=1.9.0,<2.0.0',
+ 'dracoon>=1.10.0,<2.0.0',
  'keyring>=23.6.0,<24.0.0',
- 'tqdm>=4.64.1,<5.0.0',
+ 'tqdm>=4.65.0,<5.0.0',
  'typer>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['dccmd = dccmd:app']}
 
 setup_kwargs = {
     'name': 'dccmd',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)',
     'long_description': '<h1 align="center">DRACOON Commander</h1>\n\n\n## Table of Contents\n\n* [About the Project](#about-the-project)\n  * [Built With](#built-with)\n* [Getting Started](#getting-started)\n  * [Prerequisites](#prerequisites)\n  * [Installation](#installation)\n* [Usage](#usage)\n* [Configuration](#configuration)\n* [License](#license)\n\n\n## About the project\n_Disclaimer: This is an unofficial client and is not supported by DRACOON._<br>\nThis client is a CLI tool to perform basic commands in DRACOON and comes with the following functionalities:\n\n* Full support for S3 direct up- / download\n    * Chunked up- and downloads\n* Full support for DRACOON end-to-end encryption\n* Optimized for concurrent requests\n* Store credentials in OS-specific secure location\n    * Linux: Freedesktop Secret Service (secretstorage)\n    * macOS: Keychain\n    * Windows: Windows Credential Locker\n\n### Built With\n* [typer](https://typer.tiangolo.com)\n* [keyring](https://pypi.org/project/keyring)\n* [dracoon](https://github.com/unbekanntes-pferd/dracoon-python-api)\n    * [httpx](https://www.python-httpx.org/)\n* [poetry](https://python-poetry.org/)\n\nA full dependency list can be viewed in\n* [pyproject.toml](/pyproject.toml) - list of dependencies and project info\n* [poetry.lock](/poetry.lock)\n\nDRACOON Commander is built with typer as the CLI framework and uses keyring to store all credentials (OAuth2 tokens, client credentials and encryption password). \nThe tool is built on top of dracoon, an async API wrapper for DRACOON based on httpx.\nThe project is managed with poetry (dependencies, release build and publishing).\n\n## Getting Started\nIn order to get started, download the latest tarball from Github or install dccmd from pip:\n[Releases]()\n\n### Prerequisites\nYou need a working Python 3.10 installation – dccmd makes use of type annotations and uses 3.10 features.\nGet the latest Python version from: [python.org](https://python.org).\n\n```bash\npython3 --version\n```\n\nIn order to get going, you can install dccmd either in a virtual environment or globally.\n\n### Installation\n\nTo install a version, use `pip` and install the `dccmd` package.\n\n#### In a virtual environment\n```bash\nvirtualenv <DIR>\nsource <DIR>/bin/activate \npython3 -m pip install dccmd\n```\n#### Globally\n```bash\npython3 -m pip install dccmd\n```\n\n#### Set PATH\nIn order for the script to work, you might need to add the relevant script path to your PATH.\nWhen installing with pip, the output will already indicate if the path is present or not.\nIf you do not add the correct directory to PATH, you will *not* be able to use the `dccmd` command in your preferred shell.\n\n##### Windows\nIn Windows, just add the script path by editing the environment variables for your account:\nLook for an entry called \'Path\' and install the script directory from the `pip install` output.\n\n##### Unix\nOn Linux or macOS you can add a path to PATH by using the following command:<br>\n`export PATH="/your/directory/see/install/output:$PATH"`<br>\n\n\n## Usage\n\n### Display commands\n\nIn order to see all available commands, arguments and options, use the --help flag:\n```bash\ndccmd --help\n```\n\n```\nUsage: dccmd [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n\nCommands:\n  auth\n  client\n  crypto\n  download  Download a file from DRACOON by providing a source path and a...\n  ls        List all nodes in a DRACOON path\n  mkdir     Create a folder in a DRACOON parent path\n  mkroom    Create a room (inherit permissions) in a DRACOON parent path\n  rm        Delete a file / folder / room in DRACOON\n  upload    Upload a file into DRACOON by providing a source path and a...\n```\nAll commands display their own help message, e.g. \n`dccmd upload --help`.\n\n### Client registration and authentication\n\nBefore you can perform any command, you must authenticate and set up the client.\nIf you enter any command which requires authentication (e.g. `dccmd ls your.dracoon.domain.com/`), you will be prompted first for a client configuration:\n* client id\n* client secret\n\n#### Client \nBefore you can use `dccmd` you need to generate a client in your DRACOON instance (config manager role required).\n1. Create a client with a client id and client secret.\nPlease make sure you have the following settings active:\n* Authorization code \n* Redirect URI is set to `https://your.dracoon.domain.com/oauth/callback`\n* Optional: If you wish to use the CLI mode (enter password and username via CLI), you can activate password flow \n\n2. Copy client id and client secret and use any command (e.g. `dccmd ls your.dracoon.domain.com/`).\n\n3. Enter client id and client secret – the information will be securely stored in your OS-specific secret container.\n\n#### Authentication\nOnce the client is set up, you will receive a link to authenticate via OAuth2 authorization code flow – you will then receive a code which you need to enter into the terminal.\nWhen completed, you will be prompted to store credentials securely (OS-specific).\n\nAdditionally, you can skip the authorization code flow and provide credentials directly, e.g. for the `dccmd ls` command:\n\n```bash\ndccmd ls your-dracoon.domain.com/ --cli-mode username@mail.com topsecret123!\n```\n\n### Upload\n\n**Important: if you use Windows, you need to provide the path with \'/\' instead of \'\\\\\'!**\n\nYou can upload single files using the upload command:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/\n```\nIn order to upload a directory, use the `--recursive` (`-r`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/\n```\n\n#### Conflict resolution\nIf you upload a file which already exists (based on file name), the upload will be rejected.<br> \nIn order to force an overwrite, use the `--overwrite` flag:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/ --overwrite\n```\n\nIf you wish to auto-rename the file if it already exists, use the `auto-rename`flag:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/ --auto-rename\n```\n\n#### Advanced usage\nIf you upload folders recursively, you might encounter performance issues, specifically when uploading many small files. \nYou can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3\n```\nThe default value is 2 - it does not coincide with real request value.<br>\nMaximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>\nMinimum value is 1 - this will not upload a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.\n\nIf you need to understand why uploads fail, you can also run the command using the `--debug` flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ --debug\n```\n*Note: This will have impact on performance as the log will be streamed to terminal and the log level will be increased to DEBUG.*\n\n### Create folder\n\nIf you wish to create a folder, use the `mkdir` command:\n\n```bash\ndccmd mkdir your-dracoon.domain.com/parent/newfolder\n```\nJust enter the full new path to create a folder. \nYou will need *create* permission to do so.\n\n\n### Create room\n\nIf you wish to create a room, use the `mkroom` command:\n\n```bash\ndccmd mkroom your-dracoon.domain.com/parent/newroom\n```\nJust enter the full new path to create a room. \nThe room will be created as a room with inherited permissions from the parent.\nYou will need *manage* permission to do so.\n\nTo create a room on the root level (\'/\'), you need to provide an admin user using \nthe corresponding option (`-au` or `--admin-user`):\n\n```bash\ndccmd mkroom -au "admin.username" your-dracoon.domain.com/newroom\n```\n*Note: In order to use the username of an OIDC user, you need to escape the `\\`, meaning you need to enter multiple slashes like so: `OIDC\\\\\\user.name`*\n\nTo create a room on any level that does *not* inherit permissions, use the `-au` (`--admin-user`) flag and provide the room admin when creating the room as with root level rooms:\n\n```bash\ndccmd mkroom -au "admin.username" your-dracoon.domain.com/parent-room/newroom\n```\n\n### Delete node\n\nIf you wish to delete a node, use the `rm` command:\n\n```bash\ndccmd rm your-dracoon.domain.com/parent/somefile.pdf\n```\nIn order to delete a container (room, folder) you need to use the `--recursive` (`r`) flag:\n\n```bash\ndccmd rm your-dracoon.domain.com/parent/folder/to/delete\n```\n**Warning: Deleting rooms cannot be undone!**\n\n### List nodes\n\nIn order to list all nodes, use the `ls` command:\n\n```bash\ndccmd ls your-dracoon.domain.com/\n```\n*Note: In order to list the root node, you need to provide a trailing `/`*\nFor a specific container (room or folder), use the path:\n```bash\ndccmd ls your-dracoon.domain.com/your/room\n```\n\n#### Displaying additional information\nUsing the `ls` command by default only provides node names.\nIn order to display more information, use relevant flags:\n\n* Display all information (size, last updated, last update user): `--long` (`-l`)\n    * Display sizes in human readable format (B, KB..): `--human-readable` (`-h`)\n* Display node id: `--inode` (`-i`)\n\nExample displaying full information:\n\n```bash\ndccmd ls -h -i -l your-dracoon.domain.com/your/room\n```\n### Download\n\nTo download a file, use the `download` command:\n\n```bash\ndccmd download your-dracoon.domain.com/your/cool-file.mp4 /target/directory\n```\n\nTo download a room or a folder, use the `download` command with `--recursive` (`-r`) flag:\n\n```bash\ndccmd download -r your-dracoon.domain.com/your/cool-folder /target/directory\n```\n\n#### Advanced usage\nIf you download folders recursively, you might encounter performance issues, specifically when downloading many small files. \nYou can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3\n```\nThe default value is 2 - it does not coincide with real request value.<br>\nMaximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>\nMinimum value is 1 - this will not download a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.\n\n### User operations\n\nYou can list, edit and import users with relevant `dccmd users` command:\n\n* csv-import  Add a list of users to DRACOON from a CSV file\n* ls          Get a list of users in DRACOON\n* rm          Delete a user\n\n#### Importing users\n\nYou can import users by using the `csv-import` command and providing a path to the csv file:\n\n```bash\ndccmd users csv-import /path/to/users.csv your-dracoon.domain.com/\n```\n\nThe csv file must contain a header and should include the following attributes:\n\n* first name\n* last name\n* email \n* login (optional)\n\nBy default, local users are created - if you want to import oidc users, you need pass the oidc config id:\n\n```bash\n#example with OIDC config 5\ndccmd users csv-import /path/to/users.csv your-dracoon.domain.com/ 5\n```\n\n#### Listing users\n\nYou can list all users using the `ls` command:\n\n```bash\ndccmd users ls your-dracoon.domain.com/\n```\n\nYou can get all users also as csv format by using the `--csv` flag:\n\n```bash\ndccmd users ls your-dracoon.domain.com/ --csv > users.csv\n```\n\nTo find a user, you can pass a search string to search for either first name, last name or user name (search string applies to all):\n\n```bash\n# will return all users with either first name, last name or user name containing \'yourname\'\ndccmd users ls your-dracoon.domain.com/ yourname\n```\n\n#### Deleting users\n\nYou can delete a user by providing the username:\n```bash\ndccmd users rm your-dracoon.domain.com/ user123\n```\n\n### Room permissions management\n\nFor an overview of the available commands use \n\n```bash\ndccmd rooms --help\n```\n\n#### List user / group permissions in a room\n\nTo list user permissions in a room, use the `list-users` command:\n\n```bash\ndccmd rooms list-users your-dracoon.domain.com/your-room\n```\nYou need minimum `read` permissions to list users.\n\nTo list group permissions in a room, use the `list-groups` command:\n\n```bash\ndccmd rooms list-groups your-dracoon.domain.com/your-room\n```\nYou need minimum `read` permissions to list groups.\n\nAs with other commands, you can use the `--csv` flag to get a csv export for the room\npermissions (users and groups).\n\n#### Add user / group to a room\n\nCurrently, the following templates are available:\n- read: read-only perrmissions for a room \n- edit: edit permissions for a room\n- admin: room admin permissions\n\nThe permissions coincide with the templates in use of the official DRACOON Web App.\n\nYou need `manage` permissions (room admin) to add users / groups.\n\nTo add a user, use the `add-user` command and provide the user and permission template (`-u` and `-p`):\n\n```bash\ndccmd rooms add-user -u "user.name" -p admin your-dracoon.domain.com/your-room\n```\n\nTo add a group, use the `add-group` command and provide the group and permission template (`-g` and `-p`):\n\n```bash\ndccmd rooms add-group -g "group.name" -p admin your-dracoon.domain.com/your-room\n```\n\n#### Remove user / group from a room\n\nYou need `manage` permissions (room admin) to remove users / groups.\n\nTo add a user, use the `remove-user` command and provide the user (`-u`):\n\n```bash\ndccmd rooms remove-user -u "user.name" your-dracoon.domain.com/your-room\n```\n\nTo add a group, use the `remove-group` command and provide the group (`-g`):\n\n```bash\ndccmd rooms remove-group -g "group.name" your-dracoon.domain.com/your-room\n```\n\n## Configuration / administration\n\nYou can view / manage the configuration for `dccmd` using the relevant commands:\n\n* `dccmd auth` - manage credentials\n    * `dccmd auth ls your.dracoon.domain.com` will display if a refresh token has been stored for the provided domain\n    * `dccmd auth rm your-dracoon.domain.com` will remove stored credentials for the provided domain\n* `dccmd client` - manage client\n    * `dccmd client register your.dracoon.domain.com` will start the registration process for a client and given domain\n    * `dccmd client ls your.dracoon.domain.com` will display client information for the provided domain\n    * `dccmd client rm your-dracoon.domain.com` will remove the stored client config for the provided domain\n* `dccmd crypto` - manage encryption\n    * `dccmd crypto ls your.dracoon.domain.com` will display if encryption password is stored for the provided domain\n    * `dccmd crypto rm your-dracoon.domain.com` will remove the encryption password for the provided domain\n    * `dccmd crypto distribute your-dracoon.domain.com/` will generate file keys available to distribute - if providing a specific path (`dccmd crypto distribute your-dracoon.domain.com/some/path`), only keys for provided parent room will be generated.\n\n### Logging \nWhen using a command, a log will be created in the current working directory.\nCurrently it is not possible to configure a default path for a log.\n\nYou can stream the log to stdout by using the `--debug` flag with any DRACOON-specific command (`upload`, `download`, `ls`, `rm`, `mkdir`, `mkroom`).\n\n\n## License\nDistributed under the Apache License. See [LICENSE](/LICENSE) for more information.\n',
     'author': 'Octavio Simone',
     'author_email': '70800577+unbekanntes-pferd@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dccmd-0.4.0/PKG-INFO` & `dccmd-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dccmd
-Version: 0.4.0
+Version: 0.4.1
 Summary: DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)
 License: Apache-2.0
 Author: Octavio Simone
 Author-email: 70800577+unbekanntes-pferd@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SecretStorage (>=3.3.1,<4.0.0)
-Requires-Dist: dracoon (>=1.9.0,<2.0.0)
+Requires-Dist: dracoon (>=1.10.0,<2.0.0)
 Requires-Dist: keyring (>=23.6.0,<24.0.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">DRACOON Commander</h1>
 
 
 ## Table of Contents
```

