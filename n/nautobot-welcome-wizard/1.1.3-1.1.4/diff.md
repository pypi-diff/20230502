# Comparing `tmp/nautobot_welcome_wizard-1.1.3.tar.gz` & `tmp/nautobot_welcome_wizard-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_welcome_wizard-1.1.3.tar", max compression
+gzip compressed data, was "nautobot_welcome_wizard-1.1.4.tar", max compression
```

## Comparing `nautobot_welcome_wizard-1.1.3.tar` & `nautobot_welcome_wizard-1.1.4.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      591 2022-12-21 15:30:23.238329 nautobot_welcome_wizard-1.1.3/LICENSE
--rw-r--r--   0        0        0     8328 2022-12-21 15:30:23.238329 nautobot_welcome_wizard-1.1.3/README.md
--rw-r--r--   0        0        0     2206 2022-12-21 15:30:33.526523 nautobot_welcome_wizard-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      928 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/__init__.py
--rw-r--r--   0        0        0      320 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/admin.py
--rw-r--r--   0        0        0       49 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/api/__init__.py
--rw-r--r--   0        0        0      742 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/api/serializers.py
--rw-r--r--   0        0        0      337 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/api/urls.py
--rw-r--r--   0        0        0      746 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/api/views.py
--rw-r--r--   0        0        0     1220 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/banner.py
--rw-r--r--   0        0        0     2878 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/datasources.py
--rw-r--r--   0        0        0     1613 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/filters.py
--rw-r--r--   0        0        0     1247 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/forms.py
--rw-r--r--   0        0        0     3579 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/jobs.py
--rw-r--r--   0        0        0     2676 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/middleware.py
--rw-r--r--   0        0        0     2801 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/migrations/0001_initial.py
--rw-r--r--   0        0        0      406 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/migrations/0002_merlin_nautobot_list_link.py
--rw-r--r--   0        0        0      431 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/migrations/0003_auto_20210705_1912.py
--rw-r--r--   0        0        0        0 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/migrations/__init__.py
--rw-r--r--   0        0        0        0 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/models/__init__.py
--rw-r--r--   0        0        0     1549 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/models/importer.py
--rw-r--r--   0        0        0     1029 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/models/merlin.py
--rw-r--r--   0        0        0      314 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/navigation.py
--rw-r--r--   0        0        0     3627 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tables.py
--rw-r--r--   0        0        0      612 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/dashboard.html
--rw-r--r--   0        0        0      666 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/devicetype.html
--rw-r--r--   0        0        0      985 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/import.html
--rw-r--r--   0        0        0      670 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/manufacturer.html
--rw-r--r--   0        0        0       44 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/__init__.py
--rw-r--r--   0        0        0     3212 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_api.py
--rw-r--r--   0        0        0      609 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_basic.py
--rw-r--r--   0        0        0     5193 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_datasources.py
--rw-r--r--   0        0        0     3233 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_filters.py
--rw-r--r--   0        0        0     1750 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_forms.py
--rw-r--r--   0        0        0     3176 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_models.py
--rw-r--r--   0        0        0    18782 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_views.py
--rw-r--r--   0        0        0      905 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/urls.py
--rw-r--r--   0        0        0    10419 2022-12-21 15:30:23.318330 nautobot_welcome_wizard-1.1.3/welcome_wizard/views.py
--rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 nautobot_welcome_wizard-1.1.3/setup.py
--rw-r--r--   0        0        0     9179 1970-01-01 00:00:00.000000 nautobot_welcome_wizard-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-01 22:08:46.105182 nautobot_welcome_wizard-1.1.4/LICENSE
+-rw-r--r--   0        0        0     5541 2023-05-01 22:08:46.105182 nautobot_welcome_wizard-1.1.4/README.md
+-rw-r--r--   0        0        0     3300 2023-05-01 22:08:58.929342 nautobot_welcome_wizard-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      928 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/admin.py
+-rw-r--r--   0        0        0       49 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/api/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/api/serializers.py
+-rw-r--r--   0        0        0      337 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/api/urls.py
+-rw-r--r--   0        0        0      746 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/api/views.py
+-rw-r--r--   0        0        0     1220 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/banner.py
+-rw-r--r--   0        0        0     2878 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/datasources.py
+-rw-r--r--   0        0        0     1613 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/filters.py
+-rw-r--r--   0        0        0     1247 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/forms.py
+-rw-r--r--   0        0        0     3817 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/jobs.py
+-rw-r--r--   0        0        0     2676 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/middleware.py
+-rw-r--r--   0        0        0     2801 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/migrations/0001_initial.py
+-rw-r--r--   0        0        0      406 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/migrations/0002_merlin_nautobot_list_link.py
+-rw-r--r--   0        0        0      431 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/migrations/0003_auto_20210705_1912.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/models/__init__.py
+-rw-r--r--   0        0        0     1549 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/models/importer.py
+-rw-r--r--   0        0        0     1029 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/models/merlin.py
+-rw-r--r--   0        0        0      314 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/navigation.py
+-rw-r--r--   0        0        0     3627 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tables.py
+-rw-r--r--   0        0        0      210 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/dashboard.html
+-rw-r--r--   0        0        0      666 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/devicetype.html
+-rw-r--r--   0        0        0      985 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/import.html
+-rw-r--r--   0        0        0      670 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/manufacturer.html
+-rw-r--r--   0        0        0       44 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_api.py
+-rw-r--r--   0        0        0     1519 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_basic.py
+-rw-r--r--   0        0        0     5193 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_datasources.py
+-rw-r--r--   0        0        0     3233 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_filters.py
+-rw-r--r--   0        0        0     1750 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_forms.py
+-rw-r--r--   0        0        0     3176 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_models.py
+-rw-r--r--   0        0        0    18882 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_views.py
+-rw-r--r--   0        0        0      905 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/urls.py
+-rw-r--r--   0        0        0    10596 2023-05-01 22:08:46.193183 nautobot_welcome_wizard-1.1.4/welcome_wizard/views.py
+-rw-r--r--   0        0        0     6484 1970-01-01 00:00:00.000000 nautobot_welcome_wizard-1.1.4/PKG-INFO
```

### Comparing `nautobot_welcome_wizard-1.1.3/LICENSE` & `nautobot_welcome_wizard-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/__init__.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Plugin declaration for Welcome Wizard."""
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 from nautobot.extras.plugins import PluginConfig
 
 
 class WelcomeWizardConfig(PluginConfig):
     """Plugin configuration for the welcome_wizard plugin."""
 
     name = "welcome_wizard"
     verbose_name = "Nautobot Welcome Wizard"
     version = __version__
     author = "Network to Code, LLC"
     description = "Nautobot's Getting Started Wizard."
     base_url = "welcome_wizard"
     required_settings = []
-    min_version = "1.2.0"
+    min_version = "1.5.0"
     default_settings = {
         # Add devicetype-library to Nautobot Git Repositories
         "enable_devicetype-library": True,
         "enable_welcome_banner": True,
     }
     caching_config = {}
     middleware = ["welcome_wizard.middleware.Prerequisites"]
```

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/api/serializers.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/api/views.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/banner.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/banner.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/datasources.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/filters.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/forms.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/jobs.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 COMPONENTS["power-ports"] = PowerPortTemplate
 COMPONENTS["power-outlets"] = PowerOutletTemplate
 COMPONENTS["interfaces"] = InterfaceTemplate
 COMPONENTS["rear-ports"] = RearPortTemplate
 COMPONENTS["front-ports"] = FrontPortTemplate
 COMPONENTS["device-bays"] = DeviceBayTemplate
 
+STRIP_KEYWORDS = {
+    "interfaces": ["poe_mode", "poe_type"],
+}
+
 
 def import_device_type(data):
     """Import DeviceType."""
     slug = data.get("slug")
 
     try:
         devtype = DeviceType.objects.get(slug=data.get("slug"))
@@ -42,15 +46,21 @@
 
     dtif = DeviceTypeImportForm(data)
     devtype = dtif.save()
 
     # Import All Components
     for key, component_class in COMPONENTS.items():
         if key in data:
-            component_list = [component_class(device_type=devtype, **item) for item in data[key]]
+            component_list = [
+                component_class(
+                    device_type=devtype,
+                    **{k: v for k, v in item.items() if k not in STRIP_KEYWORDS.get(key, [])},
+                )
+                for item in data[key]
+            ]
             component_class.objects.bulk_create(component_list)
 
     return devtype
 
 
 class WelcomeWizardImportManufacturer(Job):
     """Manufacturer Import."""
```

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/middleware.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/middleware.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/migrations/0001_initial.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/models/importer.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/models/importer.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/models/merlin.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/models/merlin.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tables.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/devicetype.html` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/devicetype.html`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/import.html` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/import.html`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/templates/welcome_wizard/manufacturer.html` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/templates/welcome_wizard/manufacturer.html`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_api.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_datasources.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_filters.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_forms.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_models.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/tests/test_views.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,29 +351,31 @@
     def test_dashboard_view_no_entries(self):
         self.add_permissions("welcome_wizard.view_merlin")
         url = reverse("plugins:welcome_wizard:dashboard")
         resp = self.client.get(url)
         self.assertHttpStatus(resp, 200)
         self.assertContains(resp, "Dashboard")
         self.assertContains(resp, "mdi-wizard-hat", 2)
-        self.assertContains(resp, "mdi-plus-thick", 8)
+        # 9th is from nautobot formset javascript
+        self.assertContains(resp, "mdi-plus-thick", 9)
         self.assertContains(resp, "mdi-checkbox-blank-outline", 8)
         self.assertContains(resp, "mdi-checkbox-marked-outline", 0)
 
     def test_dashboard_view_with_content(self):
         # Setup a site and manufacturer
         self.add_permissions("welcome_wizard.view_merlin")
         Manufacturer.objects.create(name="Manufacturer1", slug="manufacturer1")
         Site.objects.create(name="site01", slug="site01")
         url = reverse("plugins:welcome_wizard:dashboard")
         resp = self.client.get(url)
         self.assertHttpStatus(resp, 200)
         self.assertContains(resp, "Dashboard")
         self.assertContains(resp, "mdi-wizard-hat", 2)
-        self.assertContains(resp, "mdi-plus-thick", 8)
+        # 9th is from nautobot formset javascript
+        self.assertContains(resp, "mdi-plus-thick", 9)
         self.assertContains(resp, "mdi-checkbox-blank-outline", 6)
         self.assertContains(resp, "mdi-checkbox-marked-outline", 2)
 
     def test_dashboard_view_permission_denied(self):
         """Test failed connection."""
         url = reverse("plugins:welcome_wizard:dashboard")
         resp = self.client.get(url)
```

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/urls.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_welcome_wizard-1.1.3/welcome_wizard/views.py` & `nautobot_welcome_wizard-1.1.4/welcome_wizard/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,11 +268,18 @@
                 )
 
     def get(self, request, *args, **kwargs):
         """Get request."""
         self.check_data()
         return super().get(request, *args, **kwargs)
 
+    def extra_context(self):
+        """Override search and table config."""
+        return {
+            "table_config_form": None,
+            "search_form": None,
+        }
+
     permission_required = "welcome_wizard.view_merlin"
     queryset = Merlin.objects.all()
     template_name = "welcome_wizard/dashboard.html"
     table = DashboardTable
```

