# Comparing `tmp/nautobot-ssot-1.2.0.tar.gz` & `tmp/nautobot_ssot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot-ssot-1.2.0.tar", max compression
+gzip compressed data, was "nautobot_ssot-1.3.0.tar", max compression
```

## Comparing `nautobot-ssot-1.2.0.tar` & `nautobot_ssot-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      591 2022-10-05 13:56:01.868952 nautobot-ssot-1.2.0/LICENSE
--rw-r--r--   0        0        0     2527 2022-10-05 13:56:01.868952 nautobot-ssot-1.2.0/README.md
--rw-r--r--   0        0        0      872 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/__init__.py
--rw-r--r--   0        0        0       48 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/api/__init__.py
--rw-r--r--   0        0        0      828 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/choices.py
--rw-r--r--   0        0        0     1054 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/filters.py
--rw-r--r--   0        0        0     1527 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/forms.py
--rw-r--r--   0        0        0      916 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/jobs/__init__.py
--rw-r--r--   0        0        0    15491 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/jobs/base.py
--rw-r--r--   0        0        0    25274 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/jobs/examples.py
--rw-r--r--   0        0        0     3036 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/migrations/0001_initial.py
--rw-r--r--   0        0        0     2379 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/migrations/0002_performance_metrics.py
--rw-r--r--   0        0        0      587 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py
--rw-r--r--   0        0        0        0 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/migrations/__init__.py
--rw-r--r--   0        0        0     8710 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/models.py
--rw-r--r--   0        0        0      601 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/navigation.py
--rw-r--r--   0        0        0     6527 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tables.py
--rw-r--r--   0        0        0     1017 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/template_content.py
--rw-r--r--   0        0        0     3798 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/dashboard.html
--rw-r--r--   0        0        0     4655 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/data_source_target.html
--rw-r--r--   0        0        0      432 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/history.html
--rw-r--r--   0        0        0     8843 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_detail.html
--rw-r--r--   0        0        0     2513 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_header.html
--rw-r--r--   0        0        0      365 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_jobresult.html
--rw-r--r--   0        0        0      322 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_logentries.html
--rw-r--r--   0        0        0     1474 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_run.html
--rw-r--r--   0        0        0      397 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/synclogentry_list.html
--rw-r--r--   0        0        0      579 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html
--rw-r--r--   0        0        0        0 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templatetags/__init__.py
--rw-r--r--   0        0        0      694 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templatetags/dashboard_helpers.py
--rw-r--r--   0        0        0      787 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templatetags/humanize_bytes.py
--rw-r--r--   0        0        0     2214 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templatetags/render_diff.py
--rw-r--r--   0        0        0      570 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/templatetags/shorter_timedelta.py
--rw-r--r--   0        0        0      257 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/__init__.py
--rw-r--r--   0        0        0      662 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/jobs/__init__.py
--rw-r--r--   0        0        0      983 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/test_api.py
--rw-r--r--   0        0        0      608 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/test_basic.py
--rw-r--r--   0        0        0     5018 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/test_jobs.py
--rw-r--r--   0        0        0     3058 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/test_models.py
--rw-r--r--   0        0        0     2437 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/test_render_diff.py
--rw-r--r--   0        0        0     5424 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/tests/test_views.py
--rw-r--r--   0        0        0     1004 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/urls.py
--rw-r--r--   0        0        0     6125 2022-10-05 13:56:01.880952 nautobot-ssot-1.2.0/nautobot_ssot/views.py
--rw-r--r--   0        0        0     2809 2022-10-05 13:56:28.212969 nautobot-ssot-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3904 1970-01-01 00:00:00.000000 nautobot-ssot-1.2.0/setup.py
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 nautobot-ssot-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-02 16:07:14.051603 nautobot_ssot-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4936 2023-05-02 16:07:14.051603 nautobot_ssot-1.3.0/README.md
+-rw-r--r--   0        0        0     1089 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/api/__init__.py
+-rw-r--r--   0        0        0      828 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/choices.py
+-rw-r--r--   0        0        0     1054 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/filters.py
+-rw-r--r--   0        0        0     1541 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/forms.py
+-rw-r--r--   0        0        0      916 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/jobs/__init__.py
+-rw-r--r--   0        0        0    15543 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/jobs/base.py
+-rw-r--r--   0        0        0    25274 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/jobs/examples.py
+-rw-r--r--   0        0        0     4846 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/metrics.py
+-rw-r--r--   0        0        0     3036 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2379 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/migrations/0002_performance_metrics.py
+-rw-r--r--   0        0        0      587 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py
+-rw-r--r--   0        0        0      409 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/migrations/0004_sync_summary.py
+-rw-r--r--   0        0        0        0 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/migrations/__init__.py
+-rw-r--r--   0        0        0     8764 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/models.py
+-rw-r--r--   0        0        0      601 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/navigation.py
+-rw-r--r--   0        0        0     6527 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tables.py
+-rw-r--r--   0        0        0     1017 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/template_content.py
+-rw-r--r--   0        0        0     3847 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/dashboard.html
+-rw-r--r--   0        0        0     4682 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/data_source_target.html
+-rw-r--r--   0        0        0      432 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/history.html
+-rw-r--r--   0        0        0     8843 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/sync_detail.html
+-rw-r--r--   0        0        0     2513 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/sync_header.html
+-rw-r--r--   0        0        0      365 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/sync_jobresult.html
+-rw-r--r--   0        0        0      322 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/sync_logentries.html
+-rw-r--r--   0        0        0      397 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/synclogentry_list.html
+-rw-r--r--   0        0        0      579 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html
+-rw-r--r--   0        0        0        0 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templatetags/__init__.py
+-rw-r--r--   0        0        0      694 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templatetags/dashboard_helpers.py
+-rw-r--r--   0        0        0      787 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templatetags/humanize_bytes.py
+-rw-r--r--   0        0        0     2214 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templatetags/render_diff.py
+-rw-r--r--   0        0        0      570 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/templatetags/shorter_timedelta.py
+-rw-r--r--   0        0        0      257 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/__init__.py
+-rw-r--r--   0        0        0      662 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/jobs/__init__.py
+-rw-r--r--   0        0        0      983 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/test_api.py
+-rw-r--r--   0        0        0     1518 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/test_basic.py
+-rw-r--r--   0        0        0     5018 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/test_jobs.py
+-rw-r--r--   0        0        0     3058 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/test_models.py
+-rw-r--r--   0        0        0     2437 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/test_render_diff.py
+-rw-r--r--   0        0        0     5634 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/tests/test_views.py
+-rw-r--r--   0        0        0     1004 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/urls.py
+-rw-r--r--   0        0        0     6326 2023-05-02 16:07:14.059603 nautobot_ssot-1.3.0/nautobot_ssot/views.py
+-rw-r--r--   0        0        0     3798 2023-05-02 16:07:25.751642 nautobot_ssot-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6345 1970-01-01 00:00:00.000000 nautobot_ssot-1.3.0/PKG-INFO
```

### Comparing `nautobot-ssot-1.2.0/LICENSE` & `nautobot_ssot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/__init__.py` & `nautobot_ssot-1.3.0/nautobot_ssot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Plugin declaration for nautobot_ssot."""
-# flake8: noqa
+# Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
 try:
     from importlib import metadata
 except ImportError:
-    # Running on pre-3.8 Python; use importlib-metadata package
+    # Python version < 3.8
     import importlib_metadata as metadata
 
-__version__ = metadata.version(__name__)
-
 from nautobot.extras.plugins import PluginConfig
 
+__version__ = metadata.version(__name__)
+
 
 class NautobotSSOTPluginConfig(PluginConfig):
     """Plugin configuration for the nautobot_ssot plugin."""
 
     name = "nautobot_ssot"
     verbose_name = "Single Source of Truth"
     version = __version__
     author = "Network to Code, LLC"
-    description = "Nautobot Single Source of Truth"
+    description = "Nautobot App that enables Single Source of Truth.  Allows users to aggregate distributed data sources and/or distribute Nautobot data to other data sources such as databases and SDN controllers."
     base_url = "ssot"
     required_settings = []
-    min_version = "1.0.3"
+    min_version = "1.4.0"
     max_version = "1.9999"
     default_settings = {
         "hide_example_jobs": False,
     }
     caching_config = {}
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/choices.py` & `nautobot_ssot-1.3.0/nautobot_ssot/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/filters.py` & `nautobot_ssot-1.3.0/nautobot_ssot/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/forms.py` & `nautobot_ssot-1.3.0/nautobot_ssot/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         fields = ["dry_run"]
 
 
 class SyncLogEntryFilterForm(BootstrapMixin, forms.ModelForm):
     """Form for filtering SyncLogEntry records."""
 
     q = forms.CharField(required=False, label="Search")
-    sync = forms.ModelChoiceField(queryset=Sync.objects.all(), required=False)
+    sync = forms.ModelChoiceField(queryset=Sync.objects.defer("diff").all(), required=False)
     action = forms.ChoiceField(choices=add_blank_choice(SyncLogEntryActionChoices), required=False)
     status = forms.ChoiceField(choices=add_blank_choice(SyncLogEntryStatusChoices), required=False)
 
     class Meta:
         """Metaclass attributes of SyncLogEntryFilterForm."""
 
         model = SyncLogEntry
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/jobs/__init__.py` & `nautobot_ssot-1.3.0/nautobot_ssot/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/jobs/base.py` & `nautobot_ssot-1.3.0/nautobot_ssot/jobs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         """Method to calculate the difference from SOURCE to TARGET adapter and store in `self.diff`.
 
         This is a generic implementation that you could overwrite completely in your custom logic.
         """
         if self.source_adapter is not None and self.target_adapter is not None:
             self.diff = self.source_adapter.diff_to(self.target_adapter, flags=self.diffsync_flags)
             self.sync.diff = self.diff.dict()
+            self.sync.summary = self.diff.summary()
             self.sync.save()
             self.log_info(message=self.diff.summary())
         else:
             self.log_warning(message="Not both adapters were properly initialized prior to diff calculation.")
 
     def execute_sync(self):
         """Method to synchronize the difference from `self.diff`, from SOURCE to TARGET adapter.
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/jobs/examples.py` & `nautobot_ssot-1.3.0/nautobot_ssot/jobs/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
 
     # Model classes used by this adapter class
     region = RegionRemoteModel
     site = SiteRemoteModel
     prefix = PrefixRemoteModel
 
     # Top-level class labels, i.e. those classes that are handled directly rather than as children of other models
-    top_level = ("region", "site", "prefix")
+    top_level = ["region", "site", "prefix"]
 
     def __init__(self, *args, url=None, token=None, job=None, **kwargs):
         """Instantiate this class, but do not load data immediately from the remote system.
 
         Args:
             url (str): URL of the remote Nautobot system
             token (str): REST API authentication token
@@ -482,15 +482,15 @@
 
     # Model classes used by this adapter class
     region = RegionLocalModel
     site = SiteLocalModel
     prefix = PrefixLocalModel
 
     # Top-level class labels, i.e. those classes that are handled directly rather than as children of other models
-    top_level = ("region", "site", "prefix")
+    top_level = ["region", "site", "prefix"]
 
     def __init__(self, *args, job=None, **kwargs):
         """Instantiate this class, but do not load data immediately from the local system."""
         super().__init__(*args, **kwargs)
         self.job = job
 
     def load(self):
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/migrations/0001_initial.py` & `nautobot_ssot-1.3.0/nautobot_ssot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/migrations/0002_performance_metrics.py` & `nautobot_ssot-1.3.0/nautobot_ssot/migrations/0002_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py` & `nautobot_ssot-1.3.0/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/models.py` & `nautobot_ssot-1.3.0/nautobot_ssot/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     sync_memory_final = models.PositiveBigIntegerField(blank=True, null=True)
     sync_memory_peak = models.PositiveBigIntegerField(blank=True, null=True)
 
     dry_run = models.BooleanField(
         default=False, help_text="Report what data would be synced but do not make any changes"
     )
     diff = models.JSONField(blank=True)
+    summary = models.JSONField(blank=True, null=True)
 
     job_result = models.ForeignKey(to=JobResult, on_delete=models.PROTECT, blank=True, null=True)
 
     class Meta:
         """Metaclass attributes of Sync model."""
 
         ordering = ["start_time"]
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/navigation.py` & `nautobot_ssot-1.3.0/nautobot_ssot/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tables.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/template_content.py` & `nautobot_ssot-1.3.0/nautobot_ssot/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/dashboard.html` & `nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/dashboard.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-{% extends 'base.html' %}
+{% extends 'generic/object_list.html' %}
 {% load buttons %}
 {% load helpers %}
 {% load static %}
 {% load dashboard_helpers %}
 
+{% block header %}{% endblock %}
+
 {% block content %}
     <h1>{% block title %}Single Source of Truth{% endblock %}</h1>
 
     <div class="row">
         <div class="col-md-6">
             <div class="panel panel-default">
                 <div class="panel-heading">
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% extends 'base.html' %} {% load buttons %} {% load helpers %} {% load static
-%} {% load dashboard_helpers %} {% block content %}
+{% extends 'generic/object_list.html' %} {% load buttons %} {% load helpers %}
+{% load static %} {% load dashboard_helpers %} {% block header %}{% endblock %}
+{% block content %}
 ****** {% block title %}Single Source of Truth{% endblock %} ******
 Data Sources
 {% if data_sources %} {% for data_source in data_sources %}
  {% dashboard_data data_source queryset "source" %}
 *** {{_data_source.name_}} ***
 
  Sync
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/data_source_target.html` & `nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/data_source_target.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-{% extends 'base.html' %}
+{% extends 'generic/object_detail.html' %}
 {% load helpers %}
 {% load render_table from django_tables2 %}
 
 {% block header %}
     <div class="row">
         <div class="col-md-12">
             <ol class="breadcrumb">
                 <li><a href="{% url 'plugins:nautobot_ssot:dashboard' %}">Single Source of Truth</a></li>
                 <li>Data {{ source_or_target | title }}s</li>
-                <li>{{ job_class }}</li>
+                <li>{{ object }}</li>
             </ol>
         </div>
     </div>
     <div class="pull-right noprint">
-        <a class="btn btn-primary" href="{% url 'extras:job' class_path=job_class.class_path %}">
+        <a class="btn btn-primary" href="{% url 'extras:job' class_path=object.class_path %}">
             <i class="mdi mdi-play"></i> Sync Now
         </a>
     </div>
-    <h1>{% block title %}SSoT - {{ job_class }}{% endblock %}</h1>
+    <h1>{% block title %}SSoT - {{ object }}{% endblock %}</h1>
     <style>
         .mdi-database::before {
             font-size: 200px;
             line-height: 200px;
         }
     </style>
 {% endblock %}
@@ -108,11 +108,11 @@
             </div>
         </div>
     </div>
     <hr>
     <div class="row">
         <div class="col-md-12">
             <h2>Sync History</h2>
-            {% render_table table 'inc/table.html' %}
+            {% include table_template|default:'responsive_table.html' %}
         </div>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-{% extends 'base.html' %} {% load helpers %} {% load render_table from
-django_tables2 %} {% block header %}
+{% extends 'generic/object_detail.html' %} {% load helpers %} {% load
+render_table from django_tables2 %} {% block header %}
    1. Single_Source_of_Truth
    2. Data {{ source_or_target | title }}s
-   3. {{ job_class }}
+   3. {{ object }}
  Sync_Now
-****** {% block title %}SSoT - {{ job_class }}{% endblock %} ******
+****** {% block title %}SSoT - {{ object }}{% endblock %} ******
  {% endblock %} {% block content %}
 {% if                                            {% if
 job_class.data_source_icon %}  ****** â¹ ****job_class.data_target_icon %}
 [{{ job_class.data_source_icon                   [{{ job_class.data_target_icon
 }}] {% else %}  {% endif %}                      }}] {% else %}  {% endif %}
 ***** {{ job_class.data_source                   ***** {{ job_class.data_target
 }} *****                                         }} *****
@@ -21,9 +21,9 @@
 {{ job_class.data_source }}            {{ job_class.data_target }}
 {% if source_url %} {{_source_name_}}  {% if target_url %} {{_target_name_}} {%
 {% else %} {{ source_name }} {% endif  else %} {{ target_name }} {% endif %}
 %}
 â                                 â
 ===============================================================================
 ***** Sync History *****
-{% render_table table 'inc/table.html' %}
+{% include table_template|default:'responsive_table.html' %}
 {% endblock %}
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_detail.html` & `nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/sync_detail.html`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/sync_header.html` & `nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/sync_header.html`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html` & `nautobot_ssot-1.3.0/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templatetags/dashboard_helpers.py` & `nautobot_ssot-1.3.0/nautobot_ssot/templatetags/dashboard_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templatetags/humanize_bytes.py` & `nautobot_ssot-1.3.0/nautobot_ssot/templatetags/humanize_bytes.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templatetags/render_diff.py` & `nautobot_ssot-1.3.0/nautobot_ssot/templatetags/render_diff.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/templatetags/shorter_timedelta.py` & `nautobot_ssot-1.3.0/nautobot_ssot/templatetags/shorter_timedelta.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tests/jobs/__init__.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tests/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tests/test_api.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tests/test_jobs.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tests/test_models.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tests/test_render_diff.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tests/test_render_diff.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/tests/test_views.py` & `nautobot_ssot-1.3.0/nautobot_ssot/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """View test cases for nautobot_ssot."""
 
 from datetime import datetime
 import uuid
+from unittest import skip
 
 from django.contrib.contenttypes.models import ContentType
 from django.urls import reverse
 
 from nautobot.extras.models import Job, JobResult
 from nautobot.users.models import ObjectPermission
 from nautobot.utilities.testing import ViewTestCases
@@ -104,14 +105,18 @@
             ),
             200,
         )
 
     def test_has_advanced_tab(self):
         pass
 
+    @skip("Not implemented")
+    def test_list_objects_with_permission(self):
+        pass
+
 
 class SyncLogEntryViewsTestCase(ViewTestCases.ListObjectsViewTestCase):  # pylint: disable=too-many-ancestors
     """Test views related to the SyncLogEntry model."""
 
     model = SyncLogEntry
 
     @classmethod
@@ -141,7 +146,11 @@
                 synced_object=None,
                 object_repr="Placeholder",
                 message="Log message",
             )
 
     def test_has_advanced_tab(self):
         pass
+
+    @skip("Not implemented")
+    def test_list_objects_with_permission(self):
+        pass
```

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/urls.py` & `nautobot_ssot-1.3.0/nautobot_ssot/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot-ssot-1.2.0/nautobot_ssot/views.py` & `nautobot_ssot-1.3.0/nautobot_ssot/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Django views for Single Source of Truth (SSoT)."""
 
 import pprint
 
 from django.contrib.contenttypes.models import ContentType
 from django.http import Http404
-from django.shortcuts import get_object_or_404, render
-from django.views.generic import View
+from django.shortcuts import get_object_or_404
 
 from django_tables2 import RequestConfig
 
+from nautobot.extras.models import Job as JobModel
 from nautobot.extras.jobs import get_job
 from nautobot.core.views.generic import BulkDeleteView, ObjectDeleteView, ObjectListView, ObjectView
 from nautobot.utilities.paginator import EnhancedPaginator
-from nautobot.utilities.views import ContentTypePermissionRequiredMixin
 
 from .filters import SyncFilterSet, SyncLogEntryFilterSet
 from .forms import SyncFilterForm, SyncLogEntryFilterForm
 from .jobs import get_data_jobs, DataSource, DataTarget
 from .models import Sync, SyncLogEntry
 from .tables import DashboardTable, SyncTable, SyncTableSingleSourceOrTarget, SyncLogEntryTable
 
 
 class DashboardView(ObjectListView):
     """Dashboard / overview of SSoT."""
 
-    queryset = Sync.objects.all()
+    queryset = Sync.objects.defer("diff").all()
     table = DashboardTable
     action_buttons = []
     template_name = "nautobot_ssot/dashboard.html"
 
     def extra_context(self):
         """Extend the view context with additional details."""
         data_sources, data_targets = get_data_jobs()
@@ -60,41 +59,45 @@
                 job_result__obj_type=sync_ct,
                 job_result__name=target.class_path,
             )
 
         return context
 
 
-class DataSourceTargetView(ContentTypePermissionRequiredMixin, View):
+class DataSourceTargetView(ObjectView):
     """Detail view of a given Data Source or Data Target Job."""
 
     additional_permissions = ("nautobot_ssot.view_sync",)
+    queryset = JobModel.objects.all()
+    template_name = "nautobot_ssot/data_source_target.html"
 
     def get_required_permission(self):
         """Permissions required to access this view."""
         return "extras.view_job"
 
+    # pylint: disable-next=arguments-differ
     def get(self, request, class_path):
         """HTTP GET request handler."""
-        job_class = get_job(class_path)
+        job = JobModel.objects.get_for_class_path(class_path)
+        return super().get(request, id=job.id)
+
+    def get_extra_context(self, request, instance):
+        """Return template context extension with job_class, table and source_or_target."""
+        job_class = get_job(instance.class_path)
         if not job_class or not issubclass(job_class, (DataSource, DataTarget)):
             raise Http404
 
         syncs = Sync.annotated_queryset().filter(source=job_class.data_source, target=job_class.data_target)
         table = SyncTableSingleSourceOrTarget(syncs, user=request.user)
 
-        return render(
-            request,
-            "nautobot_ssot/data_source_target.html",
-            {
-                "job_class": job_class,
-                "table": table,
-                "source_or_target": "source" if issubclass(job_class, DataSource) else "target",
-            },
-        )
+        return {
+            "job_class": job_class,
+            "table": table,
+            "source_or_target": "source" if issubclass(job_class, DataSource) else "target",
+        }
 
 
 class SyncListView(ObjectListView):
     """View for listing Sync records."""
 
     queryset = Sync.annotated_queryset()
     filterset = SyncFilterSet
```

### Comparing `nautobot-ssot-1.2.0/pyproject.toml` & `nautobot_ssot-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "nautobot-ssot"
-version = "v1.2.0"
+version = "v1.3.0"
 description = "Nautobot Single Source of Truth"
-authors = ["Network to Code, LLC <opensource@networktocode.com>"]
+authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-ssot"
 repository = "https://github.com/nautobot/nautobot-plugin-ssot"
 documentation = "https://nautobot-plugin-ssot.readthedocs.io"
 keywords = ["nautobot", "nautobot-plugin"]
 classifiers = [
@@ -23,39 +23,56 @@
 ]
 packages = [
     { include = "nautobot_ssot" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-nautobot = "*"
+nautobot = "^1.4.0"
 diffsync = "^1.6.0"
 Markdown = "!=3.3.5"
-packaging = "^21.3"
+packaging = ">=21.3, <24"
+prometheus-client = "^0.16.0"
 
 [tool.poetry.dev-dependencies]
-invoke = "*"
+bandit = "*"
 black = "*"
+coverage = "*"
 django-debug-toolbar = "*"
-yamllint = "*"
-bandit = "*"
+# we need to pin flake8 because of package dependencies that cause it to downgrade and
+# therefore cause issues with linting since older versions do not take .flake8 as config
+flake8 = "^3.9.2"
+invoke = "*"
+ipython = "*"
+pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
-pydocstyle = "*"
-flake8 = "*"
-coverage = "*"
-mkdocs = "*"
-
+pytest = "*"
+yamllint = "*"
+Markdown = "*"
+toml = "*"
+# Rendering docs to HTML
+mkdocs = "1.4.2"
+# Material for MkDocs theme
+mkdocs-material = "9.0.11"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
+# Automatic documentation from sources, for MkDocs
+mkdocstrings = "0.20"
+mkdocstrings-python = "0.8.3"
 
 [tool.poetry.plugins."nautobot_ssot.data_sources"]
 "example" = "nautobot_ssot.sync.example:ExampleSyncWorker"
 
 [tool.poetry.plugins."nautobot_ssot.data_targets"]
 "example" = "nautobot_ssot.sync.example:ExampleSyncWorker"
 
+[tool.poetry.extras]
+nautobot = ["nautobot"]
+
 [tool.black]
 line-length = 120
 target-version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
@@ -74,36 +91,47 @@
                      # the root of the project
 )
 '''
 
 [tool.pylint.master]
 # Include the pylint_django plugin to avoid spurious warnings about Django patterns
 load-plugins="pylint_django"
+ignore=".venv"
 
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
-# "too-few-public-methods" is just plain noise.
 disable = """,
     line-too-long,
-    bad-continuation,
     too-few-public-methods,
     """
 
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
     """
 
+[tool.pydocstyle]
+convention = "google"
+inherit = false
+match = "(?!__init__).*\\.py"
+match-dir = "(?!tests|migrations|development)[^\\.].*"
+# D212 is enabled by default in google convention, and complains if we have a docstring like:
+# """
+# My docstring is on the line after the opening quotes instead of on the same line as them.
+# """
+# We've discussed and concluded that we consider this to be a valid style choice.
+add_ignore = "D212"
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests"
```

