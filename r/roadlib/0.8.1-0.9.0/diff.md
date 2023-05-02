# Comparing `tmp/roadlib-0.8.1.tar.gz` & `tmp/roadlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roadlib-0.8.1.tar", last modified: Fri May  8 13:02:17 2020, max compression
+gzip compressed data, was "dist/roadlib-0.9.0.tar", last modified: Tue Jul 21 15:38:53 2020, max compression
```

## Comparing `roadlib-0.8.1.tar` & `roadlib-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 dirkjan   (1000) dirkjan   (1000)        0 2020-05-08 13:02:17.337667 roadlib-0.8.1/
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)      562 2020-05-08 13:02:17.337667 roadlib-0.8.1/PKG-INFO
-drwxrwxr-x   0 dirkjan   (1000) dirkjan   (1000)        0 2020-05-08 13:02:17.337667 roadlib-0.8.1/roadlib.egg-info/
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)      562 2020-05-08 13:02:17.000000 roadlib-0.8.1/roadlib.egg-info/PKG-INFO
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)      502 2020-05-08 13:02:17.000000 roadlib-0.8.1/roadlib.egg-info/SOURCES.txt
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)        1 2020-05-08 13:02:17.000000 roadlib-0.8.1/roadlib.egg-info/dependency_links.txt
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)        1 2020-04-15 17:13:48.000000 roadlib-0.8.1/roadlib.egg-info/not-zip-safe
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)       16 2020-05-08 13:02:17.000000 roadlib-0.8.1/roadlib.egg-info/requires.txt
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)       10 2020-05-08 13:02:17.000000 roadlib-0.8.1/roadlib.egg-info/top_level.txt
-drwxrwxr-x   0 dirkjan   (1000) dirkjan   (1000)        0 2020-05-08 13:02:17.333667 roadlib-0.8.1/roadtools/
-drwxrwxr-x   0 dirkjan   (1000) dirkjan   (1000)        0 2020-05-08 13:02:17.337667 roadlib-0.8.1/roadtools/roadlib/
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)        0 2019-06-22 08:47:00.000000 roadlib-0.8.1/roadtools/roadlib/__init__.py
--rwxrwxr-x   0 dirkjan   (1000) dirkjan   (1000)     8366 2020-04-16 11:35:07.000000 roadlib-0.8.1/roadtools/roadlib/auth.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)     8618 2020-05-08 10:34:05.000000 roadlib-0.8.1/roadtools/roadlib/dbgen.py
-drwxrwxr-x   0 dirkjan   (1000) dirkjan   (1000)        0 2020-05-08 13:02:17.337667 roadlib-0.8.1/roadtools/roadlib/metadef/
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)        0 2019-06-21 19:40:32.000000 roadlib-0.8.1/roadtools/roadlib/metadef/__init__.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)      810 2019-06-28 13:16:31.000000 roadlib-0.8.1/roadtools/roadlib/metadef/basetypes.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)    13747 2020-03-29 11:06:36.000000 roadlib-0.8.1/roadtools/roadlib/metadef/complextypes.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)    25938 2020-05-08 10:34:14.000000 roadlib-0.8.1/roadtools/roadlib/metadef/database.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)    25545 2020-03-29 11:06:36.000000 roadlib-0.8.1/roadtools/roadlib/metadef/entitytypes.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)     2721 2020-03-29 11:06:33.000000 roadlib-0.8.1/roadtools/roadlib/metagen.py
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)       38 2020-05-08 13:02:17.337667 roadlib-0.8.1/setup.cfg
--rw-rw-r--   0 dirkjan   (1000) dirkjan   (1000)      785 2020-05-08 13:00:49.000000 roadlib-0.8.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-07-21 15:38:53.285435 roadlib-0.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (116)      562 2020-07-21 15:38:53.285435 roadlib-0.9.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-07-21 15:38:53.285435 roadlib-0.9.0/roadlib.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)      562 2020-07-21 15:38:53.000000 roadlib-0.9.0/roadlib.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)      502 2020-07-21 15:38:53.000000 roadlib-0.9.0/roadlib.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-07-21 15:38:53.000000 roadlib-0.9.0/roadlib.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-07-21 15:38:53.000000 roadlib-0.9.0/roadlib.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (116)       16 2020-07-21 15:38:53.000000 roadlib-0.9.0/roadlib.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       10 2020-07-21 15:38:53.000000 roadlib-0.9.0/roadlib.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-07-21 15:38:53.281435 roadlib-0.9.0/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-07-21 15:38:53.285435 roadlib-0.9.0/roadtools/roadlib/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)    10885 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/auth.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8791 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/dbgen.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-07-21 15:38:53.285435 roadlib-0.9.0/roadtools/roadlib/metadef/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/metadef/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      810 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/metadef/basetypes.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13747 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/metadef/complextypes.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    26465 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/metadef/database.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    25545 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/metadef/entitytypes.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2721 2020-07-21 15:34:44.000000 roadlib-0.9.0/roadtools/roadlib/metagen.py
+-rw-r--r--   0 vsts      (1001) docker     (116)       38 2020-07-21 15:38:53.285435 roadlib-0.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)      785 2020-07-21 15:34:44.000000 roadlib-0.9.0/setup.py
```

### Comparing `roadlib-0.8.1/PKG-INFO` & `roadlib-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: roadlib
-Version: 0.8.1
+Version: 0.9.0
 Summary: ROADtools common components library
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@dirkjanm.io
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `roadlib-0.8.1/roadlib.egg-info/PKG-INFO` & `roadlib-0.9.0/roadlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: roadlib
-Version: 0.8.1
+Version: 0.9.0
 Summary: ROADtools common components library
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@dirkjanm.io
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `roadlib-0.8.1/roadtools/roadlib/dbgen.py` & `roadlib-0.9.0/roadtools/roadlib/dbgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 # Relationships defined here
 relations = {
     # Relationship name: (LeftGroup, RightGroup, relation name, reverse relation name)
     'group_member_user': ('Group', 'User', 'memberUsers', 'memberOf'),
     'group_member_group': ('Group', 'Group', 'memberGroups', 'memberOf'),
     'group_member_contact': ('Group', 'Contact', 'memberContacts', 'memberOf'),
     'group_member_device': ('Group', 'Device', 'memberDevices', 'memberOf'),
+    'group_member_serviceprincipal': ('Group', 'ServicePrincipal', 'memberServicePrincipals', 'memberOf'),
     'device_owner': ('Device', 'User', 'owner', 'ownedDevices'),
     'application_owner_user': ('Application', 'User', 'ownerUsers', 'ownedApplications'),
     'application_owner_serviceprincipal': ('Application', 'ServicePrincipal', 'ownerServicePrincipals', 'ownedApplications'),
     'serviceprincipal_owner_user': ('ServicePrincipal', 'User', 'ownerUsers', 'ownedServicePrincipals'),
     'serviceprincipal_owner_serviceprincipal': ('ServicePrincipal', 'ServicePrincipal', 'ownerServicePrincipals', 'ownedServicePrincipals'),
     'role_member_user': ('DirectoryRole', 'User', 'memberUsers', 'memberOfRole'),
     'role_member_serviceprincipal': ('DirectoryRole', 'ServicePrincipal', 'memberServicePrincipals', 'memberOfRole'),
@@ -197,16 +198,16 @@
 def gen_link_fkey(link_name, ref_table, rel_name, rev_rel_name, ref_column, sec_ref_column):
     return link_tpl_fkey.format(rel_name, ref_table, link_name, ref_column, sec_ref_column, rev_rel_name)
 
 # Tables to generate and relationships with other tables are defined here
 tables = [
     # Table, relation, back_relation
     (User, [], ['group_member_user', 'application_owner_user', 'serviceprincipal_owner_user', 'role_member_user', 'device_owner']),
-    (ServicePrincipal, ['serviceprincipal_owner_user', 'serviceprincipal_owner_serviceprincipal'], ['role_member_serviceprincipal', 'serviceprincipal_owner_serviceprincipal', 'application_owner_serviceprincipal']),
-    (Group, ['group_member_group', 'group_member_user', 'group_member_contact', 'group_member_device'], ['group_member_group']),
+    (ServicePrincipal, ['serviceprincipal_owner_user', 'serviceprincipal_owner_serviceprincipal'], ['role_member_serviceprincipal', 'serviceprincipal_owner_serviceprincipal', 'application_owner_serviceprincipal', 'group_member_serviceprincipal']),
+    (Group, ['group_member_group', 'group_member_user', 'group_member_contact', 'group_member_device', 'group_member_serviceprincipal'], ['group_member_group']),
     (Application, ['application_owner_user', 'application_owner_serviceprincipal'], []),
     (Device, ['device_owner'], ['group_member_device']),
     # (Domain, [], []),
     (DirectoryRole, ['role_member_user', 'role_member_serviceprincipal'], []),
     (TenantDetail, [], []),
     (ApplicationRef, [], []),
     (ExtensionProperty, [], []),
```

### Comparing `roadlib-0.8.1/roadtools/roadlib/metadef/basetypes.py` & `roadlib-0.9.0/roadtools/roadlib/metadef/basetypes.py`

 * *Files identical despite different names*

### Comparing `roadlib-0.8.1/roadtools/roadlib/metadef/complextypes.py` & `roadlib-0.9.0/roadtools/roadlib/metadef/complextypes.py`

 * *Files identical despite different names*

### Comparing `roadlib-0.8.1/roadtools/roadlib/metadef/database.py` & `roadlib-0.9.0/roadtools/roadlib/metadef/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,19 @@
 )
 
 lnk_group_member_device = Table('lnk_group_member_device', Base.metadata,
     Column('Group', Text, ForeignKey('Groups.objectId')),
     Column('Device', Text, ForeignKey('Devices.objectId'))
 )
 
+lnk_group_member_serviceprincipal = Table('lnk_group_member_serviceprincipal', Base.metadata,
+    Column('Group', Text, ForeignKey('Groups.objectId')),
+    Column('ServicePrincipal', Text, ForeignKey('ServicePrincipals.objectId'))
+)
+
 lnk_device_owner = Table('lnk_device_owner', Base.metadata,
     Column('Device', Text, ForeignKey('Devices.objectId')),
     Column('User', Text, ForeignKey('Users.objectId'))
 )
 
 lnk_application_owner_user = Table('lnk_application_owner_user', Base.metadata,
     Column('Application', Text, ForeignKey('Applications.objectId')),
@@ -317,14 +322,18 @@
         secondaryjoin=objectId==lnk_serviceprincipal_owner_serviceprincipal.c.ServicePrincipal,
         back_populates="ownerServicePrincipals")
 
     ownedApplications = relationship("Application",
         secondary=lnk_application_owner_serviceprincipal,
         back_populates="ownerServicePrincipals")
 
+    memberOf = relationship("Group",
+        secondary=lnk_group_member_serviceprincipal,
+        back_populates="memberServicePrincipals")
+
 
 class Group(Base, SerializeMixin):
     __tablename__ = "Groups"
     objectType = Column(Text)
     objectId = Column(Text, primary_key=True)
     deletionTimestamp = Column(DateTime)
     appMetadata = Column(JSON)
@@ -380,14 +389,18 @@
         secondary=lnk_group_member_contact,
         back_populates="memberOf")
 
     memberDevices = relationship("Device",
         secondary=lnk_group_member_device,
         back_populates="memberOf")
 
+    memberServicePrincipals = relationship("ServicePrincipal",
+        secondary=lnk_group_member_serviceprincipal,
+        back_populates="memberOf")
+
     memberOf = relationship("Group",
         secondary=lnk_group_member_group,
         primaryjoin=objectId==lnk_group_member_group.c.childGroup,
         secondaryjoin=objectId==lnk_group_member_group.c.Group,
         back_populates="memberGroups")
```

### Comparing `roadlib-0.8.1/roadtools/roadlib/metadef/entitytypes.py` & `roadlib-0.9.0/roadtools/roadlib/metadef/entitytypes.py`

 * *Files identical despite different names*

### Comparing `roadlib-0.8.1/roadtools/roadlib/metagen.py` & `roadlib-0.9.0/roadtools/roadlib/metagen.py`

 * *Files identical despite different names*

### Comparing `roadlib-0.8.1/setup.py` & `roadlib-0.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 setup(name='roadlib',
-      version='0.8.1',
+      version='0.9.0',
       description='ROADtools common components library',
       author='Dirk-jan Mollema',
       author_email='dirkjan@dirkjanm.io',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
```

