# Comparing `tmp/odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2.tar.gz` & `tmp/odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2.tar", last modified: Tue Nov 16 11:29:15 2021, max compression
+gzip compressed data, was "odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2.tar", last modified: Tue May  2 10:46:20 2023, max compression
```

## Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2.tar` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)      537 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/
--rw-rw-rw-   0 root         (0) root         (0)       42 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/models/
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     3736 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/models/subscription_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/tests/
--rw-rw-rw-   0 root         (0) root         (0)       51 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/tests/test_member_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2883 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/tests/test_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/views/
--rw-rw-rw-   0 root         (0) root         (0)      239 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/views/menus.xml
--rw-rw-rw-   0 root         (0) root         (0)     1596 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/views/res_partner_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      873 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/views/subscription_request_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/wizard/
--rw-rw-rw-   0 root         (0) root         (0)       35 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/wizard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/
--rw-r--r--   0 root         (0) root         (0)      537 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1226 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-16 11:29:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      100 2021-11-16 11:29:05.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      523 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/PKG-INFO
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.928672 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.928672 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       42 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      560 2023-04-26 10:00:41.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/__manifest__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/models/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       61 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/models/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1405 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/models/res_partner.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4233 2023-04-24 13:05:15.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/models/subscription_request.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/tests/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2412 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/tests/test_member_wizard.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3070 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/tests/test_subscription.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/views/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      239 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/views/menus.xml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1596 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/views/res_partner_view.xml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      873 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/views/subscription_request_view.xml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/wizard/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       36 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/wizard/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2314 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1226 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.xml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      523 2023-05-02 10:46:20.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1226 2023-05-02 10:46:20.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-02 10:46:20.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-02 10:46:20.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/not-zip-safe
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       47 2023-05-02 10:46:20.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-05-02 10:46:20.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-02 10:46:20.932005 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      100 2023-04-24 10:26:53.000000 odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/PKG-INFO` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: odoo12-addon-easy_my_coop_sponsorship
-Version: 12.0.0.0.0rc2
+Version: 12.0.0.0.2
 Summary: Odoo Sponsorship module for Easy My Coop cooperative addons
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
+Description: 
+            Odoo Sponsorship module for Easy My Coop cooperative addons.
+            
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
-Classifier: Framework :: Odoo :: 12.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.5
-
-
-    Odoo Sponsorship module for Easy My Coop cooperative addons.
-    
-
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/__manifest__.py` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/__manifest__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 {
-    'name': "Odoo Sponsorship module for Easy My Coop cooperative addons",
-    'version': '12.0.0.0.0-rc2',
-    'depends': ['easy_my_coop'],
-    'author': "Coopdevs Treball SCCL",
-    'website': 'https://coopdevs.org',
-    'category': "Cooperative management",
-    'description': """
+    "name": "Odoo Sponsorship module for Easy My Coop cooperative addons",
+    "version": "12.0.0.0.2",
+    "depends": ["easy_my_coop"],
+    "author": "Coopdevs Treball SCCL",
+    "website": "https://coopdevs.org",
+    "category": "Cooperative management",
+    "description": """
     Odoo Sponsorship module for Easy My Coop cooperative addons.
     """,
     "license": "AGPL-3",
-    'data': [
-        'views/subscription_request_view.xml',
-        'views/res_partner_view.xml',
-        'wizard/sponsee_member_wizard.xml',
-        'views/menus.xml',
+    "data": [
+        "views/subscription_request_view.xml",
+        "views/res_partner_view.xml",
+        "wizard/sponsee_member_wizard.xml",
+        "views/menus.xml",
     ],
 }
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/models/res_partner.py` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/models/res_partner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 from odoo import models, fields, api
 
 
 class ResPartner(models.Model):
-    _inherit = 'res.partner'
+    _inherit = "res.partner"
 
     sponsee_ids = fields.One2many(
-        'res.partner',
-        'sponsor_id',
-        string='Sponsees',
-        readonly=True
+        "res.partner", "sponsor_id", string="Sponsees", readonly=True
     )
 
     sponsor_id = fields.Many2one(
-        'res.partner',
-        string='Sponsor',
+        "res.partner",
+        string="Sponsor",
         domain=lambda self: self._domain_sponsor_id(),
     )
-    coop_sponsee = fields.Boolean(string="Is Cooperator Sponsee?",
-                                  compute="_compute_coop_sponsee",
-                                  store=True,
-                                  readonly=True)
+    coop_sponsee = fields.Boolean(
+        string="Is Cooperator Sponsee?",
+        compute="_compute_coop_sponsee",
+        store=True,
+        readonly=True,
+    )
 
     def _domain_sponsor_id(self):
         return [
-            ('member', '=', True),
+            ("member", "=", True),
         ]
 
     @api.multi
     @api.depends("sponsor_id")
     @api.depends("subscription_request_ids.state")
     def _compute_coop_candidate(self):
         for partner in self:
             if partner.member:
                 is_candidate = False
             else:
                 sub_requests = partner.subscription_request_ids.filtered(
-                    lambda record: (
-                            record.state == 'done' and
-                            not record.sponsor_id
-                    )
+                    lambda record: (record.state == "done" and not record.sponsor_id)
                 )
                 is_candidate = bool(sub_requests)
             partner.coop_candidate = is_candidate
 
     @api.multi
     @api.depends("sponsor_id")
     def _compute_coop_sponsee(self):
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/models/subscription_request.py` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/models/subscription_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #
 from odoo import models, fields, api, _
 from odoo.exceptions import UserError
 
 
 class SubscriptionRequest(models.Model):
-    _inherit = 'subscription.request'
-    _rec_name = 'type'
+    _inherit = "subscription.request"
+    _rec_name = "type"
     share_product_id = fields.Many2one(required=False)
-    type = fields.Selection(selection_add=[('sponsorship', 'Sponsorship')])
+    type = fields.Selection(selection_add=[("sponsorship", "Sponsorship")])
 
     sponsor_id = fields.Many2one(
-        'res.partner',
-        string='Sponsor',
+        "res.partner",
+        string="Sponsor",
         domain=lambda self: self._domain_sponsor_id(),
     )
 
     def _domain_sponsor_id(self):
         return [
-            ('member', '=', True),
+            ("member", "=", True),
         ]
 
     @api.one
     def validate_subscription_request(self):
         try:
             invoice = super().validate_subscription_request()
         except UserError:
-            if self.ordered_parts == 0 and self.type == 'sponsorship':
+            if self.ordered_parts == 0 and self.type == "sponsorship":
                 pass
             else:
                 raise
         else:
             return invoice
 
-        self.partner_obj = self.env['res.partner']
+        self.partner_obj = self.env["res.partner"]
         self.partner = False
 
         self._check_already_cooperator()
 
         if not self.partner:
             self.partner = self.create_coop_partner()
             self.partner_id = self.partner
         else:
             self.partner = self.partner[0]
 
         self.partner.cooperator = True
 
         self._create_company_contact()
 
-        self.write({'state': 'done'})
+        self.write({"state": "done"})
         return True
 
     def _check_already_cooperator(self):
         domain = False
 
         if self.already_cooperator:
             raise UserError(
@@ -74,39 +74,58 @@
         if domain:
             self.partner = self.partner_obj.search(domain)
 
     def _create_company_contact(self):
         if self.is_company and not self.partner.has_representative():
             contact = False
             if self.email:
-                domain = [('email', '=', self.email)]
+                domain = [("email", "=", self.email)]
                 contact = self.partner_obj.search(domain)
                 if contact:
-                    contact.type = 'representative'
+                    contact.type = "representative"
             if not contact:
                 contact_vals = self.get_representative_vals()
                 self.partner_obj.create(contact_vals)
             else:
                 if len(contact) > 1:
-                    raise UserError(_('There is two different persons with the'
-                                      ' same national register number. Please'
-                                      ' proceed to a merge before to continue')
-                                    )
+                    raise UserError(
+                        _(
+                            "There is two different persons with the"
+                            " same national register number. Please"
+                            " proceed to a merge before to continue"
+                        )
+                    )
                 if contact.parent_id and contact.parent_id.id != self.partner.id:
-                    raise UserError(_('This contact person is already defined'
-                                      ' for another company. Please select'
-                                      ' another contact'))
+                    raise UserError(
+                        _(
+                            "This contact person is already defined"
+                            " for another company. Please select"
+                            " another contact"
+                        )
+                    )
                 else:
-                    contact.write({'parent_id': self.partner.id,
-                                   'representative': True})
+                    contact.write(
+                        {"parent_id": self.partner.id, "representative": True}
+                    )
 
     def get_partner_company_vals(self):
         values = super().get_partner_company_vals()
-        values['sponsor_id'] = self.sponsor_id.id
-        values['customer'] = True
+        values["sponsor_id"] = self.sponsor_id.id
+        values["customer"] = True
         return values
 
     def get_partner_vals(self):
         values = super().get_partner_vals()
-        values['sponsor_id'] = self.sponsor_id.id
-        values['customer'] = True
+        values["sponsor_id"] = self.sponsor_id.id
+        values["customer"] = True
         return values
+
+    def update_partner_info(self):
+        self.ensure_one()
+        if self.type == "sponsorship":
+            self.partner_id.sponsor_id = self.sponsor_id and self.sponsor_id.id
+
+    def get_required_field(self):
+        req_fields = super().get_required_field()
+        if "iban" in req_fields:
+            req_fields.remove("iban")
+        return req_fields
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/tests/test_member_wizard.py` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/tests/test_member_wizard.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 from odoo.tests.common import TransactionCase
 from datetime import datetime, timedelta
 
 
 class TestMemberWizard(TransactionCase):
-
     def setUp(self, *args, **kwargs):
         result = super().setUp(*args, **kwargs)
-        self.SubscriptionRequest = self.env['subscription.request']
-        self.SponseeMemberWizard = self.env['subscription.upgrade.sponsee']
+        self.SubscriptionRequest = self.env["subscription.request"]
+        self.SponseeMemberWizard = self.env["subscription.upgrade.sponsee"]
         sponsor_id = self.ref("easy_my_coop.res_partner_cooperator_1_demo")
         vals_subscription_sponsorship = {
-            'already_cooperator': False,
-            'name': 'Manuel Dublues Test',
-            'email': 'manuel@demo-test.net',
-            'ordered_parts': False,
-            'address': 'schaerbeekstraat',
-            'city': 'Brussels',
-            'zip_code': '1111',
-            'country_id': 20,
-            'date': datetime.now()-timedelta(days=12),
-            'company_id': 1,
-            'source': 'manual',
-            'share_product_id': False,
-            'lang': 'en_US',
-            'sponsor_id': sponsor_id,
-            'type': 'sponsorship'
+            "already_cooperator": False,
+            "name": "Manuel Dublues Test",
+            "email": "manuel@demo-test.net",
+            "ordered_parts": False,
+            "address": "schaerbeekstraat",
+            "city": "Brussels",
+            "zip_code": "1111",
+            "country_id": 20,
+            "date": datetime.now() - timedelta(days=12),
+            "company_id": 1,
+            "source": "manual",
+            "share_product_id": False,
+            "lang": "en_US",
+            "sponsor_id": sponsor_id,
+            "type": "sponsorship",
         }
-        subscription_sponsorship = self.SubscriptionRequest.create(vals_subscription_sponsorship)
+        subscription_sponsorship = self.SubscriptionRequest.create(
+            vals_subscription_sponsorship
+        )
         subscription_sponsorship.validate_subscription_request()
         self.sponsee = subscription_sponsorship.partner_id
 
     def testSponseeToMemberWizardCreation(self):
         WizardSponsee = self.SponseeMemberWizard
-        product_template = self.browse_ref('easy_my_coop.product_template_share_type_2_demo')
-        wizardSponsee = WizardSponsee.create({
-            'share_product_id': product_template.product_variant_id.id,
-            'partner_id': self.sponsee.id
-        })
+        product_template = self.browse_ref(
+            "easy_my_coop.product_template_share_type_2_demo"
+        )
+        wizardSponsee = WizardSponsee.create(
+            {
+                "share_product_id": product_template.product_variant_id.id,
+                "partner_id": self.sponsee.id,
+            }
+        )
         self.assertEqual(wizardSponsee.partner_id, self.sponsee)
         self.assertEqual(wizardSponsee.start_date, datetime.now().date())
 
     def testSponseeToMemberWizardUpgrade(self):
         WizardSponsee = self.SponseeMemberWizard
-        product_template = self.browse_ref('easy_my_coop.product_template_share_type_2_demo')
-        wizardSponsee = WizardSponsee.create({
-            'share_product_id': product_template.product_variant_id.id,
-            'partner_id': self.sponsee.id
-        })
+        product_template = self.browse_ref(
+            "easy_my_coop.product_template_share_type_2_demo"
+        )
+        wizardSponsee = WizardSponsee.create(
+            {
+                "share_product_id": product_template.product_variant_id.id,
+                "partner_id": self.sponsee.id,
+            }
+        )
         wizardSponsee.upgrade()
         self.assertTrue(self.sponsee.coop_candidate)
         self.assertFalse(self.sponsee.coop_sponsee)
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/tests/test_subscription.py` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/tests/test_subscription.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,79 @@
 from odoo.tests.common import TransactionCase
 from datetime import datetime, timedelta
 
 
 class TestSubscription(TransactionCase):
-
     def setUp(self, *args, **kwargs):
         result = super().setUp(*args, **kwargs)
-        self.SubscriptionRequest = self.env['subscription.request']
+        self.SubscriptionRequest = self.env["subscription.request"]
         self.vals_subscription = {
-            'already_cooperator': False,
-            'name': 'Manuel Dublues Test',
-            'email': 'manuel@demo-test.net',
-            'ordered_parts': 1,
-            'address': 'schaerbeekstraat',
-            'city': 'Brussels',
-            'zip_code': '1111',
-            'country_id': 20,
-            'date': datetime.now()-timedelta(days=12),
-            'company_id': 1,
-            'source': 'manual',
-            'share_product_id': None,
-            'lang': 'en_US'
+            "already_cooperator": False,
+            "name": "Manuel Dublues Test",
+            "email": "manuel@demo-test.net",
+            "ordered_parts": 1,
+            "address": "schaerbeekstraat",
+            "city": "Brussels",
+            "zip_code": "1111",
+            "country_id": 20,
+            "date": datetime.now() - timedelta(days=12),
+            "company_id": 1,
+            "source": "manual",
+            "share_product_id": None,
+            "lang": "en_US",
         }
         return result
 
     def test_create_subscription_regular(self):
         vals_subscription_regular = self.vals_subscription.copy()
         self.product_template_test = self.browse_ref(
             "easy_my_coop.product_template_share_type_1_demo"
         )
-        vals_subscription_regular.update({
-            'share_product_id': self.product_template_test.product_variant_id.id,
-            'ordered_parts': 1
-        })
-        subscription_regular = self.SubscriptionRequest.create(vals_subscription_regular)
+        vals_subscription_regular.update(
+            {
+                "share_product_id": self.product_template_test.product_variant_id.id,
+                "ordered_parts": 1,
+            }
+        )
+        subscription_regular = self.SubscriptionRequest.create(
+            vals_subscription_regular
+        )
         self.assertEqual(subscription_regular.subscription_amount, 50.0)
 
     def test_create_subscription_sponsorship(self):
         vals_subscription_sponsorship = self.vals_subscription.copy()
         sponsor_id = self.ref("easy_my_coop.res_partner_cooperator_1_demo")
-        vals_subscription_sponsorship.update({
-            'share_product_id': False,
-            'ordered_parts': False,
-            'type': 'sponsorship',
-            'sponsor_id': sponsor_id,
-        })
-        subscription_regular = self.SubscriptionRequest.create(vals_subscription_sponsorship)
+        vals_subscription_sponsorship.update(
+            {
+                "share_product_id": False,
+                "ordered_parts": False,
+                "type": "sponsorship",
+                "sponsor_id": sponsor_id,
+            }
+        )
+        subscription_regular = self.SubscriptionRequest.create(
+            vals_subscription_sponsorship
+        )
         self.assertEqual(subscription_regular.subscription_amount, 0.0)
 
     def test_validate_subscription_sponsorship(self):
         vals_subscription_sponsorship = self.vals_subscription.copy()
         sponsor_id = self.ref("easy_my_coop.res_partner_cooperator_1_demo")
-        vals_subscription_sponsorship.update({
-            'share_product_id': False,
-            'ordered_parts': False,
-            'sponsor_id': sponsor_id,
-            'type': 'sponsorship',
-        })
+        vals_subscription_sponsorship.update(
+            {
+                "share_product_id": False,
+                "ordered_parts": False,
+                "sponsor_id": sponsor_id,
+                "type": "sponsorship",
+            }
+        )
 
-        subscription_sponsorship = self.SubscriptionRequest.create(vals_subscription_sponsorship)
+        subscription_sponsorship = self.SubscriptionRequest.create(
+            vals_subscription_sponsorship
+        )
         subscription_sponsorship.validate_subscription_request()
 
         partner = subscription_sponsorship.partner_id
 
         self.assertTrue(partner.cooperator)
         self.assertTrue(partner.customer)
         self.assertFalse(partner.member)
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/views/res_partner_view.xml` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/views/subscription_request_view.xml` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/views/subscription_request_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.py` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 from odoo import api, fields, models
 from datetime import datetime
 
 
 class SubscriptionUpgradeSponsee(models.TransientModel):
-    _name = 'subscription.upgrade.sponsee'
-    _description = 'Change a partner from sponsee to member'
+    _name = "subscription.upgrade.sponsee"
+    _description = "Change a partner from sponsee to member"
 
-    partner_id = fields.Many2one('res.partner',
-                                 domain=[('coop_sponsee', '=', True)],
-                                 required=True)
-    share_product_id = fields.Many2one('product.product',
-                                       string='Share type',
-                                       domain=[('is_share', '=', True)],
-                                       required=True)
-    ordered_parts = fields.Integer(string='Number of Share',
-                                   required=True,
-                                   default=1)
-    start_date = fields.Date(string='Start date',
-                             required=True,
-                             default=lambda self: self._get_default_start_date())
+    partner_id = fields.Many2one(
+        "res.partner", domain=[("coop_sponsee", "=", True)], required=True
+    )
+    share_product_id = fields.Many2one(
+        "product.product",
+        string="Share type",
+        domain=[("is_share", "=", True)],
+        required=True,
+    )
+    ordered_parts = fields.Integer(string="Number of Share", required=True, default=1)
+    start_date = fields.Date(
+        string="Start date",
+        required=True,
+        default=lambda self: self._get_default_start_date(),
+    )
 
     @api.model
     def _get_default_start_date(self):
         return datetime.now().date()
 
     @api.multi
     def upgrade(self):
         self.ensure_one()
-        SubscriptionRequest = self.env['subscription.request']
+        SubscriptionRequest = self.env["subscription.request"]
         vals_subscription = {
-            'already_cooperator': True,
-            'partner_id': self.partner_id.id,
-            'ordered_parts': self.ordered_parts,
-            'date': self.start_date,
-            'source': 'manual',
-            'share_product_id': self.share_product_id.id,
-            'firstname': self.partner_id.firstname,
-            'name': self.partner_id.name,
-            'iban': self.partner_id.bank_ids[0].acc_number,
-            'lastname': self.partner_id.lastname,
-            'email': self.partner_id.email,
-            'birthdate': self.partner_id.birthdate_date,
-            'gender': self.partner_id.gender,
-            'address': self.partner_id.street,
-            'city': self.partner_id.city,
-            'zip_code': self.partner_id.zip,
-            'country_id': self.partner_id.country_id.id,
-            'phone': self.partner_id.phone,
-            'lang': self.partner_id.lang,
+            "already_cooperator": True,
+            "partner_id": self.partner_id.id,
+            "ordered_parts": self.ordered_parts,
+            "date": self.start_date,
+            "source": "manual",
+            "share_product_id": self.share_product_id.id,
+            "firstname": self.partner_id.firstname,
+            "name": self.partner_id.name,
+            "iban": self.partner_id.bank_ids[0].acc_number,
+            "lastname": self.partner_id.lastname,
+            "email": self.partner_id.email,
+            "birthdate": self.partner_id.birthdate_date,
+            "gender": self.partner_id.gender,
+            "address": self.partner_id.street,
+            "city": self.partner_id.city,
+            "zip_code": self.partner_id.zip,
+            "country_id": self.partner_id.country_id.id,
+            "phone": self.partner_id.phone,
+            "lang": self.partner_id.lang,
         }
         subscription = SubscriptionRequest.create(vals_subscription)
         subscription.validate_subscription_request()
         self.partner_id.sponsor_id = False
         return {
-            'view_mode': 'form',
-            'view_id': False,
-            'view_type': 'form',
-            'res_model': 'res.partner',
-            'res_id': self.partner_id.id,
-            'type': 'ir.actions.act_window',
+            "view_mode": "form",
+            "view_id": False,
+            "view_type": "form",
+            "res_model": "res.partner",
+            "res_id": self.partner_id.id,
+            "type": "ir.actions.act_window",
         }
```

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.xml` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo/addons/easy_my_coop_sponsorship/wizard/sponsee_member_wizard.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.0rc2/odoo12_addon_easy_my_coop_sponsorship.egg-info/SOURCES.txt` & `odoo12-addon-easy_my_coop_sponsorship-12.0.0.0.2/odoo12_addon_easy_my_coop_sponsorship.egg-info/SOURCES.txt`

 * *Files identical despite different names*

