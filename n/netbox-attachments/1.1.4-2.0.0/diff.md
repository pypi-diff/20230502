# Comparing `tmp/netbox-attachments-1.1.4.tar.gz` & `tmp/netbox-attachments-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-attachments-1.1.4.tar", last modified: Wed Mar  1 09:36:44 2023, max compression
+gzip compressed data, was "netbox-attachments-2.0.0.tar", last modified: Tue May  2 11:22:09 2023, max compression
```

## Comparing `netbox-attachments-1.1.4.tar` & `netbox-attachments-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/netbox_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/netbox_attachments/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/netbox_attachments/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/migrations/0003_alter_netboxattachment_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.743477 netbox-attachments-1.1.4/netbox_attachments/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/add_attachment_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/generic_tab_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/netboxattachment.html
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/netbox_attachments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/netbox_attachments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-03-01 09:36:44.000000 netbox-attachments-1.1.4/netbox_attachments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-01 09:36:44.000000 netbox-attachments-1.1.4/netbox_attachments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 09:36:44.000000 netbox-attachments-1.1.4/netbox_attachments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 09:36:44.000000 netbox-attachments-1.1.4/netbox_attachments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 09:36:44.000000 netbox-attachments-1.1.4/netbox_attachments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 09:36:44.747477 netbox-attachments-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-01 09:36:36.000000 netbox-attachments-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.572636 netbox-attachments-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-02 11:22:09.572636 netbox-attachments-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.568637 netbox-attachments-2.0.0/netbox_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.568637 netbox-attachments-2.0.0/netbox_attachments/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.568637 netbox-attachments-2.0.0/netbox_attachments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/migrations/0003_alter_netboxattachment_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.564637 netbox-attachments-2.0.0/netbox_attachments/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.568637 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/add_attachment_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/generic_tab_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/netboxattachment.html
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/netbox_attachments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:09.568637 netbox-attachments-2.0.0/netbox_attachments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-02 11:22:09.000000 netbox-attachments-2.0.0/netbox_attachments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-02 11:22:09.000000 netbox-attachments-2.0.0/netbox_attachments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:22:09.000000 netbox-attachments-2.0.0/netbox_attachments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:22:09.000000 netbox-attachments-2.0.0/netbox_attachments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 11:22:09.000000 netbox-attachments-2.0.0/netbox_attachments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:22:09.572636 netbox-attachments-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-02 11:22:00.000000 netbox-attachments-2.0.0/setup.py
```

### Comparing `netbox-attachments-1.1.4/PKG-INFO` & `netbox-attachments-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-attachments
-Version: 1.1.4
+Version: 2.0.0
 Summary: Netbox plugin to manage attachments for any model
 Home-page: https://github.com/Kani999/netbox-attachments
 Author: Jan Krupa
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -23,14 +23,15 @@
 ## Compatibility
 
 | Netbox   | Plugin          |
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
+| >= 3.5.0 | 2.0.0           |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
@@ -63,14 +64,17 @@
   - **Type**: Dict
   - **Default**: {}
   - **Options**: {<app_label.model>: <prefeered_display>}
   - **Example**: {'dcim.devicerole': 'full_width_page', 'dcim.device': 'left_page', 'ipam.vlan': 'additional_tab'}
   - **Description**: Set display setting for concrete model
   - **Tip**: Proper `app_label` and `model` names could be found at API `<your_netbox_url>/api/extras/content-types/`
 
+> **Warning**
+> `additional_tab` does not work for Plugin models
+
 ### Configuration Example:
 
 ```
 PLUGINS_CONFIG = {
     'netbox_attachments': {
         'apps': ['dcim', 'ipam', 'circuits', 'tenancy', 'virtualization', 'wireless', 'inventory_monitor'],
         'display_default': "right_page",
```

### Comparing `netbox-attachments-1.1.4/README.md` & `netbox-attachments-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ## Compatibility
 
 | Netbox   | Plugin          |
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
+| >= 3.5.0 | 2.0.0           |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
@@ -51,14 +52,17 @@
   - **Type**: Dict
   - **Default**: {}
   - **Options**: {<app_label.model>: <prefeered_display>}
   - **Example**: {'dcim.devicerole': 'full_width_page', 'dcim.device': 'left_page', 'ipam.vlan': 'additional_tab'}
   - **Description**: Set display setting for concrete model
   - **Tip**: Proper `app_label` and `model` names could be found at API `<your_netbox_url>/api/extras/content-types/`
 
+> **Warning**
+> `additional_tab` does not work for Plugin models
+
 ### Configuration Example:
 
 ```
 PLUGINS_CONFIG = {
     'netbox_attachments': {
         'apps': ['dcim', 'ipam', 'circuits', 'tenancy', 'virtualization', 'wireless', 'inventory_monitor'],
         'display_default': "right_page",
```

### Comparing `netbox-attachments-1.1.4/netbox_attachments/__init__.py` & `netbox-attachments-2.0.0/netbox_attachments/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     base_url = 'netbox-attachments'
     default_settings = {
         'apps': ['dcim', 'ipam', 'circuits', 'tenancy', 'virtualization', 'wireless'],
         'display_default': "additional_tab",
         'display_setting': {}
     }
     required_settings = []
-    min_version = '3.4.3'
-    max_version = '3.4.99'
+    min_version = '3.5.0'
+    max_version = '3.5.99'
 
 
 config = NetBoxAttachmentsConfig
```

### Comparing `netbox-attachments-1.1.4/netbox_attachments/api/serializers.py` & `netbox-attachments-2.0.0/netbox_attachments/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist
-from drf_yasg.utils import swagger_serializer_method
+#from drf_yasg.utils import swagger_serializer_method
 from netbox.api.fields import ContentTypeField
 from netbox.api.serializers import NetBoxModelSerializer
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from rest_framework import serializers
 from utilities.api import get_serializer_for_model
 
 from ..models import NetBoxAttachment
@@ -37,12 +37,12 @@
             )
 
         # Enforce model validation
         super().validate(data)
 
         return data
 
-    @swagger_serializer_method(serializer_or_field=serializers.JSONField)
+    #@swagger_serializer_method(serializer_or_field=serializers.JSONField)
     def get_parent(self, obj):
         serializer = get_serializer_for_model(
             obj.parent, prefix=NESTED_SERIALIZER_PREFIX)
         return serializer(obj.parent, context={'request': self.context['request']}).data
```

### Comparing `netbox-attachments-1.1.4/netbox_attachments/filtersets.py` & `netbox-attachments-2.0.0/netbox_attachments/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/forms.py` & `netbox-attachments-2.0.0/netbox_attachments/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django import forms
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext as _
 from netbox.forms import NetBoxModelFilterSetForm, NetBoxModelForm
-from utilities.forms import (APISelectMultiple,
-                             DynamicModelMultipleChoiceField, TagFilterField)
-from utilities.forms.fields import CommentField
+from utilities.forms.widgets.apiselect import APISelectMultiple
+from utilities.forms.fields import DynamicModelMultipleChoiceField, TagFilterField, CommentField
 
 from .models import NetBoxAttachment
 
 
 class NetBoxAttachmentForm(NetBoxModelForm):
     comments = CommentField(label="Comment")
```

### Comparing `netbox-attachments-1.1.4/netbox_attachments/migrations/0001_initial.py` & `netbox-attachments-2.0.0/netbox_attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py` & `netbox-attachments-2.0.0/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py` & `netbox-attachments-2.0.0/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/models.py` & `netbox-attachments-2.0.0/netbox_attachments/models.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/tables.py` & `netbox-attachments-2.0.0/netbox_attachments/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/template_content.py` & `netbox-attachments-2.0.0/netbox_attachments/template_content.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_attachments', {})
 template_extensions = []
 
 
 def create_attachments_panel(self):
     obj = self.context['object']
     app_label, model = self.model.split(".")
-    content_type_id = ContentType.objects.get(app_label=app_label,
-                                              model=model).id
-
-    return self.render(
-        'netbox_attachments/netbox_attachment_panel.html',
-        extra_context={
-            'netbox_attachments': NetBoxAttachment.objects.filter(content_type_id=content_type_id,
-                                                                  object_id=obj.id),
-        }
-    )
+    try:
+        content_type_id = ContentType.objects.get(app_label=app_label,
+                                                  model=model).id
+
+        return self.render(
+            'netbox_attachments/netbox_attachment_panel.html',
+            extra_context={
+                'netbox_attachments': NetBoxAttachment.objects.filter(content_type_id=content_type_id,
+                                                                      object_id=obj.id),
+            }
+        )
+    except ContentType.DoesNotExist as e:
+        logging.error(
+            f"ContentType for {app_label} {self.model} does not exist")
+        return ""
 
 
 def get_display_on(app_model_name):
     """Get prefered display setting (left_page, right_page, full_width_page, additional_tab) for attachment panel
 
     Args:
         app_model_name (str): <app_label>.<model> = (dcim.device, ipam.vlan, ...)
@@ -115,22 +120,28 @@
 try:
     # Iterate over all NetBox models
     for content_type in ContentType.objects.all():
         app_label = content_type.app_label
         model = content_type.model
         app_model_name = f"{app_label}.{model}"
 
+        try:
+            model = ContentType.objects.get(
+                app_label=app_label, model=model).model_class()
+        except ContentType.DoesNotExist as e:
+            logging.error(
+                f"ContentType for {app_label} {model} does not exist")
+            continue
+
         # Skip if app is not present in configuration
         if app_label not in plugin_settings.get("apps"):
             continue
 
         # Load prefeed display setting and model class
         display = get_display_on(app_model_name)
-        model = ContentType.objects.get(
-            app_label=app_label, model=model).model_class()
 
         # Special case - if display setting is set as additional_tab
         # https://docs.netbox.dev/en/stable/plugins/development/views/#additional-tabs
         if display == "additional_tab" and model:
             # create add attachment button at the top of the parent view
             template_extensions.append(create_add_button(app_model_name))
             # add attachment tab to the parent view
```

### Comparing `netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/generic_tab_list.html` & `netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/generic_tab_list.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html` & `netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html` & `netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/templates/netbox_attachments/netboxattachment.html` & `netbox-attachments-2.0.0/netbox_attachments/templates/netbox_attachments/netboxattachment.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/urls.py` & `netbox-attachments-2.0.0/netbox_attachments/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/utils.py` & `netbox-attachments-2.0.0/netbox_attachments/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments/views.py` & `netbox-attachments-2.0.0/netbox_attachments/views.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/netbox_attachments.egg-info/PKG-INFO` & `netbox-attachments-2.0.0/netbox_attachments.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-attachments
-Version: 1.1.4
+Version: 2.0.0
 Summary: Netbox plugin to manage attachments for any model
 Home-page: https://github.com/Kani999/netbox-attachments
 Author: Jan Krupa
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -23,14 +23,15 @@
 ## Compatibility
 
 | Netbox   | Plugin          |
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
+| >= 3.5.0 | 2.0.0           |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
@@ -63,14 +64,17 @@
   - **Type**: Dict
   - **Default**: {}
   - **Options**: {<app_label.model>: <prefeered_display>}
   - **Example**: {'dcim.devicerole': 'full_width_page', 'dcim.device': 'left_page', 'ipam.vlan': 'additional_tab'}
   - **Description**: Set display setting for concrete model
   - **Tip**: Proper `app_label` and `model` names could be found at API `<your_netbox_url>/api/extras/content-types/`
 
+> **Warning**
+> `additional_tab` does not work for Plugin models
+
 ### Configuration Example:
 
 ```
 PLUGINS_CONFIG = {
     'netbox_attachments': {
         'apps': ['dcim', 'ipam', 'circuits', 'tenancy', 'virtualization', 'wireless', 'inventory_monitor'],
         'display_default': "right_page",
```

### Comparing `netbox-attachments-1.1.4/netbox_attachments.egg-info/SOURCES.txt` & `netbox-attachments-2.0.0/netbox_attachments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-attachments-1.1.4/setup.py` & `netbox-attachments-2.0.0/setup.py`

 * *Files identical despite different names*

