# Comparing `tmp/djangocms-simple-admin-style-0.2.0.tar.gz` & `tmp/djangocms-simple-admin-style-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-simple-admin-style-0.2.0.tar", last modified: Mon May  1 11:03:25 2023, max compression
+gzip compressed data, was "djangocms-simple-admin-style-0.2.1.tar", last modified: Tue May  2 06:38:39 2023, max compression
```

## Comparing `djangocms-simple-admin-style-0.2.0.tar` & `djangocms-simple-admin-style-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.143558 djangocms-simple-admin-style-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-01 11:03:25.143558 djangocms-simple-admin-style-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.139558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.139558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.139558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.143558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.139558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.143558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:03:25.143558 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-01 11:03:25.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 11:03:25.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:03:25.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:03:24.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 11:03:25.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 11:03:25.000000 djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 11:03:25.143558 djangocms-simple-admin-style-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-01 11:03:13.000000 djangocms-simple-admin-style-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-02 06:38:39.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 06:38:39.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:38:39.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:38:39.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 06:38:39.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 06:38:39.000000 djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-02 06:38:39.221935 djangocms-simple-admin-style-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-02 06:38:26.000000 djangocms-simple-admin-style-0.2.1/setup.py
```

### Comparing `djangocms-simple-admin-style-0.2.0/LICENSE` & `djangocms-simple-admin-style-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.2.0/PKG-INFO` & `djangocms-simple-admin-style-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-simple-admin-style-0.2.0/README.rst` & `djangocms-simple-admin-style-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css` & `djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.css`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     --body-bg: var(--dca-white);
     --body-quiet-color: #666;
     --body-loud-color: #000;
 
     --header-color: var(--dca-black);
     --header-branding-color: var(--accent);
     --header-bg: var(--secondary);
-    --header-link-color: var(--dca-primary);
+    --header-link-color: var(--body-fg);
 
-    --breadcrumbs-fg: #var(--dca-gray);
+    --breadcrumbs-fg: var(--dca-gray);
     --breadcrumbs-link-fg: var(--dca-primary);
     --breadcrumbs-bg: var(--dca-gray-lightest);
 
     --link-fg: var(--dca-primary);
     --link-hover-color: #48abd9;
     --link-selected-fg: #5b80b2;
 
@@ -123,18 +123,29 @@
 
 li, dt, dd {
     font-size: 0.875rem;
     line-height: 1.4rem;
 }
 
 .module h2, .module caption, .inline-group h2 {
-    background: 0 0;
+    background: var(--body-bg);
+    color: var(--body-fg)
 }
 
-a.section:link, a.section:visited {
+#nav-sidebar .module caption {
+    background: var(--primary);
+}
+#nav-sidebar .section:link,
+#nav-sidebar .section:visited,
+#nav-sidebar .current-app .section:link,
+#nav-sidebar .current-app .section:visited {
+    color: var(--dca-white);
+}
+
+#nav-sidebar a {
     color: var(--body-fg);
 }
 
 .submit-row {
     background: var(--dca-white, #fff);
 }
 
@@ -145,56 +156,80 @@
 .submit-row a.deletelink, .submit-row a.deletelink,
 .submit-row a.deletelink {
     color: var(--dca-white, #fff);
 }
 
 .object-tools a {
     border-radius: 3px;
-    border: 1px solid var(--dca-gray-lighter, #ddd);
+    border: 1px solid var(--dca-gray-lighter);
 }
 
 .object-tools a.addlink {
     color: var(--default-button-fg);
+    border-color: var(--default-button-fg);
     background-color: var(--default-button-bg);
 }
 
 .object-tools a.addlink:focus, .object-tools a.addlink:hover{
     background-color: var(--default-button-hover-bg);
 }
 
+body.djangocms-simple-admin-style #page_form_lang_tabs input[type=button].language_button.selected {
+    color: var(--default-button-fg);
+    background-color: var(--default-button-bg);
+    border-color: var(--default-button-bg);
+}
+
 th {
     font-weight: 400;
 }
 
 .module h2, .module caption, .inline-group h2 {
     font-weight: 600;
 }
 
 .aligned label {
     float: unset;
     width: unset;
-    display: inline-block;
+    display: block;
     color: var(--body-fg);
     font-weight: 600;
 }
 
+.flex-container {
+    display: block;
+}
+
 .aligned .fieldBox > label:first-child, .form-row > div > label {
     display: block;
 }
 
 .required label:not(.vCheckboxLabel):after, label.required:not(.vCheckboxLabel):after {
     color: var(--delete-button-bg);
     content: "*";
 }
 
 form .aligned p.help, form .aligned div.help {
     margin-left: 0;
     padding-left: 0;
 }
 
+form button {
+    margin: 2px 0;
+    padding: 5px 6px;
+    vertical-align: middle;
+    font-family: var(--font-family-primary);
+    font-weight: normal;
+    font-size: 0.8125rem;
+    background-color: var(--default-button-bg);
+    color: var(--default-button-fg);
+    border: 1px solid var(--default-button-bg);
+    border-radius: 3px;
+}
+
 .aligned label + p, .aligned label + div.help, .aligned label + div.readonly,
 form .aligned input + p.help, form .aligned textarea + p.help, form .aligned select + p.help,
 form .aligned input + div.help, form .aligned textarea + div.help, form .aligned select + div.help {
     margin-left: 0;
 }
 
 .button, input[type=submit], input[type=button], .submit-row input, a.button {
@@ -203,52 +238,74 @@
 
 a.btn {
     color: var(--body-fg);
     border: 1px solid var(--dca-gray-lighter, #ddd);
 }
 
 input[type="text"], .vLargeTextField, .vXMLLargeTextField, .vTextField, .vUUIDField,
-.colM .aligned .vLargeTextField, .colM .aligned .vXMLLargeTextField, .vURLField {
+.colM .aligned .vLargeTextField, .colM .aligned .vXMLLargeTextField, .vURLField,
+.flex-container textarea {
     width: calc(100% - 10px);
 }
 
+#changelist-search input[type="text"] {
+    width: unset;
+}
+
 input, textarea, select, .form-row p, form .button {
     font-family: unset;
 }
 
 div.form-row {
     display: flex;
-    flex: 1 0 0%;
+    flex: 1 0 0;
 }
 
 .form-row > div {
     width: 100%;
     max-width: 100%;
 }
 
 fieldset.collapse.collapsed .form-row {
     display: none;
 }
+
 .select2 {
     width: calc(100% - 40px) !important;
 }
 
+.flex-container .related-widget-wrapper, .flex-container select, .flex-container .select2-container {
+    width: 100%;
+}
+
+.related-widget-wrapper select {
+    width: calc(100% - 92px);
+}
+
 .colMS .aligned .vLargeTextField, .colMS .aligned .vXMLLargeTextField {
     width: unset;
 }
 
 body.cms-admin-sideframe #header, body.cms-admin-modal #header {
     display: none;
 }
 
-body.cms-admin-sideframe .breadcrumbs {
-    margin-top: 46px;
+body.cms-admin-sideframe #container {
+    padding-top: 46px;
+}
+
+body.cms-admin-sideframe #content > h1 {
+    display: none;
 }
 
 body.cms-admin-modal .content {
     margin-top: 36px;
 }
 body.cms-admin-modal .breadcrumbs,
 body.cms-admin-modal #toggle-nav-sidebar,
 body.cms-admin-modal #nav-sidebar {
     display: none;
 }
+
+body.cms-admin-sideframe.djangocms-simple-admin-style {
+    margin-top: 0;
+}
```

### Comparing `djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style/templates/admin/base_site.html` & `djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/PKG-INFO` & `djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-simple-admin-style-0.2.0/djangocms_simple_admin_style.egg-info/SOURCES.txt` & `djangocms-simple-admin-style-0.2.1/djangocms_simple_admin_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.2.0/setup.cfg` & `djangocms-simple-admin-style-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.2.0/setup.py` & `djangocms-simple-admin-style-0.2.1/setup.py`

 * *Files identical despite different names*

