# Comparing `tmp/xia_scw_vpc-0.0.9-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_vpc-0.1.0-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 110347 bytes, number of entries: 12
--rw-r--r--  2.0 unx       87 b- defN 23-May-01 09:10 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   259072 b- defN 23-May-01 09:20 xia_scw_vpc/vpc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/backend.tf
--rw-rw-rw-  2.0 unx      991 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/main.tf
--rw-rw-rw-  2.0 unx      651 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/provider.tf
--rw-rw-rw-  2.0 unx     1953 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 09:20 xia_scw_vpc-0.0.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      642 b- defN 23-May-01 09:20 xia_scw_vpc-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 09:20 xia_scw_vpc-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-01 09:20 xia_scw_vpc-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1053 b- defN 23-May-01 09:20 xia_scw_vpc-0.0.9.dist-info/RECORD
-12 files, 265124 bytes uncompressed, 108545 bytes compressed:  59.1%
+Zip file size: 88662 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       87 b- defN 23-May-02 18:49 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   235400 b- defN 23-May-02 18:49 xia_scw_vpc/vpc.cpython-310-darwin.so
+-rw-r--r--  2.0 unx     1210 b- defN 23-May-02 08:46 xia_scw_vpc/templates/ScwVpc/main.tf
+-rw-r--r--  2.0 unx     1028 b- defN 23-May-02 18:49 xia_scw_vpc/templates/ScwVpc/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/provider.tf
+-rw-r--r--  2.0 unx     2295 b- defN 23-May-02 08:46 xia_scw_vpc/templates/ScwVpc/variables.tf
+-rw-r--r--  2.0 unx      150 b- defN 23-May-02 18:49 xia_scw_vpc-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      635 b- defN 23-May-02 18:49 xia_scw_vpc-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-02 18:49 xia_scw_vpc-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-02 18:49 xia_scw_vpc-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      965 b- defN 23-May-02 18:49 xia_scw_vpc-0.1.0.dist-info/RECORD
+11 files, 242233 bytes uncompressed, 87008 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
 Filename: xia_scw_vpc/__init__.py
 Comment: 
 
-Filename: xia_scw_vpc/vpc.cp39-win_amd64.pyd
-Comment: 
-
-Filename: xia_scw_vpc/templates/ScwVpc/backend.tf
+Filename: xia_scw_vpc/vpc.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/main.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/output.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/provider.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/variables.tf
 Comment: 
 
-Filename: xia_scw_vpc-0.0.9.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.9.dist-info/METADATA
+Filename: xia_scw_vpc-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.0.9.dist-info/WHEEL
+Filename: xia_scw_vpc-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.0.9.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.9.dist-info/RECORD
+Filename: xia_scw_vpc-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_vpc/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_vpc.vpc import ScwVpc
 
 
 __all__ = [
     "ScwVpc"
 ]
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
```

## xia_scw_vpc/templates/ScwVpc/main.tf

```diff
@@ -1,31 +1,39 @@
+resource scaleway_vpc_public_gateway_ip main {
+    zone = var.zone
+}
+
 resource "scaleway_vpc_public_gateway_dhcp" "dhcp01" {
+  zone       = var.zone
   subnet             = var.lan_subnet
   push_default_route = true
   enable_dynamic     = false
   address            = var.lan_address
   pool_high          = var.lan_high
   pool_low           = var.lan_low
 }
 
 resource scaleway_vpc_private_network main {
-  name = var.lan_name
+  zone       = var.zone
+  name       = var.lan_name
   depends_on = [scaleway_vpc_public_gateway_dhcp.dhcp01]
 }
 
 resource scaleway_vpc_public_gateway main {
+  zone            = var.zone
   name            = var.name
   type            = var.type
-  ip_id           = var.ip_id
+  ip_id           = scaleway_vpc_public_gateway_ip.main.id
   bastion_enabled = true
   bastion_port    = var.bastion_port
-  depends_on = [scaleway_vpc_public_gateway_dhcp.dhcp01]
+  depends_on      = [scaleway_vpc_public_gateway_dhcp.dhcp01]
 }
 
 resource scaleway_vpc_gateway_network main {
+  zone               = var.zone
   gateway_id         = scaleway_vpc_public_gateway.main.id
   private_network_id = scaleway_vpc_private_network.main.id
   dhcp_id            = scaleway_vpc_public_gateway_dhcp.dhcp01.id
   cleanup_dhcp       = true
   enable_masquerade  = true
   depends_on         = [scaleway_vpc_private_network.main]
 }
```

## xia_scw_vpc/templates/ScwVpc/output.tf

```diff
@@ -2,20 +2,36 @@
   value = var.project_id
 }
 
 output "name" {
   value = scaleway_vpc_private_network.main.name
 }
 
+output "zone" {
+  value = scaleway_vpc_public_gateway.main.zone
+}
+
 output "type" {
   value = scaleway_vpc_public_gateway.main.type
 }
 
 output "ip_id" {
-  value = var.ip_id
+  value = scaleway_vpc_public_gateway_ip.main.id
+}
+
+output "wan_ip" {
+  value = scaleway_vpc_public_gateway_ip.main.address
+}
+
+output "private_network_id" {
+  value = scaleway_vpc_private_network.main.id
+}
+
+output "gateway_network_id" {
+  value = scaleway_vpc_gateway_network.main.id
 }
 
 output "lan_name" {
   value = var.lan_name
 }
 
 output "lan_subnet" {
@@ -33,7 +49,11 @@
 output "lan_high" {
   value = scaleway_vpc_public_gateway_dhcp.dhcp01.pool_high
 }
 
 output "bastion_port" {
   value = scaleway_vpc_public_gateway.main.bastion_port
 }
+
+output "tf_state" {
+  value = var.tf_state
+}
```

## xia_scw_vpc/templates/ScwVpc/variables.tf

```diff
@@ -8,21 +8,35 @@
 variable "name" {
   type = string
   default = null  #xia#
   #xia# default = {% if name is defined and name is not none %}"{{ name }}"{% else %}null{% endif %}
 
 }
 
+variable "zone" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if zone is defined and zone is not none %}"{{ zone }}"{% else %}null{% endif %}
+
+}
+
 variable "type" {
   type = string
   default = null  #xia#
   #xia# default = {% if type is defined and type is not none %}"{{ type }}"{% else %}null{% endif %}
 
 }
 
+variable "tf_state" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if tf_state is defined and tf_state is not none %}"{{ tf_state }}"{% else %}null{% endif %}
+
+}
+
 variable "ip_id" {
   type = string
   default = null  #xia#
   #xia# default = {% if ip_id is defined and ip_id is not none %}"{{ ip_id }}"{% else %}null{% endif %}
 
 }
```

## Comparing `xia_scw_vpc-0.0.9.dist-info/METADATA` & `xia_scw_vpc-0.1.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: xia-scw-vpc
-Version: 0.0.9
+Version: 0.1.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.9/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.1.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine
+Requires-Dist: xia-fields-scw
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-vpc.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-scw-vpc/
 
 ====================================
 X-I-A
@@ -26,9 +25,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

