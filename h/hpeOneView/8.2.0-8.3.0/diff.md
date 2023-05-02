# Comparing `tmp/hpeOneView-8.2.0.tar.gz` & `tmp/hpeOneView-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpeOneView-8.2.0.tar", last modified: Wed Mar 15 05:45:44 2023, max compression
+gzip compressed data, was "hpeOneView-8.3.0.tar", last modified: Tue May  2 05:30:55 2023, max compression
```

## Comparing `hpeOneView-8.2.0.tar` & `hpeOneView-8.3.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.597218 hpeOneView-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    17132 2023-03-15 05:45:44.597218 hpeOneView-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16713 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.577217 hpeOneView-8.2.0/hpeOneView/
--rw-r--r--   0 runner    (1001) docker     (122)     3227 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26978 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    36104 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/oneview_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.577217 hpeOneView-8.2.0/hpeOneView/resources/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.581217 hpeOneView-8.2.0/hpeOneView/resources/activity/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/activity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5399 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/activity/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/activity/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4518 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/activity/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.581217 hpeOneView-8.2.0/hpeOneView/resources/data_services/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/data_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/data_services/metric_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.581217 hpeOneView-8.2.0/hpeOneView/resources/facilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6431 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/facilities/datacenters.py
--rw-r--r--   0 runner    (1001) docker     (122)    15134 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/facilities/power_devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     6081 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/facilities/racks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.581217 hpeOneView-8.2.0/hpeOneView/resources/fc_sans/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/fc_sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/fc_sans/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/fc_sans/managed_sans.py
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/fc_sans/san_managers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/fc_sans/san_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.585217 hpeOneView-8.2.0/hpeOneView/resources/hypervisors/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/hypervisors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5173 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/hypervisors/hypervisor_cluster_profiles.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2834 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/hypervisors/hypervisor_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.589217 hpeOneView-8.2.0/hpeOneView/resources/networking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/connection_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6862 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/ethernet_networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/fabrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/fc_networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/fcoe_networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/interconnect_link_topologies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/interconnect_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/interconnects.py
--rw-r--r--   0 runner    (1001) docker     (122)     3152 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/internal_link_sets.py
--rw-r--r--   0 runner    (1001) docker     (122)     4829 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/logical_downlinks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/logical_interconnect_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    21567 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/logical_interconnects.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/logical_switch_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6868 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/logical_switches.py
--rw-r--r--   0 runner    (1001) docker     (122)     3525 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/network_sets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/sas_interconnect_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/sas_interconnects.py
--rw-r--r--   0 runner    (1001) docker     (122)     3358 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/sas_logical_interconnect_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     7140 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/sas_logical_interconnects.py
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/switch_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     5961 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/switches.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4566 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/networking/uplink_sets.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    71677 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.589217 hpeOneView-8.2.0/hpeOneView/resources/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7034 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/search/index_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     4806 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/search/labels.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.589217 hpeOneView-8.2.0/hpeOneView/resources/security/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3883 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/certificate_authority.py
--rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/certificate_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/certificates_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/login_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7597 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/security/users.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.593217 hpeOneView-8.2.0/hpeOneView/resources/servers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3267 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/enclosure_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     9623 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/enclosures.py
--rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools.py
--rw-r--r--   0 runner    (1001) docker     (122)     4850 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools_ipv4_ranges.py
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools_ipv4_subnets.py
--rw-r--r--   0 runner    (1001) docker     (122)     7171 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools_ranges.py
--rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/logical_enclosures.py
--rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/migratable_vc_domains.py
--rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/rack_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    15631 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/server_hardware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/server_hardware_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/server_profile_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    14299 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/servers/server_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.597218 hpeOneView-8.2.0/hpeOneView/resources/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_configuration_timeconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_read_community.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_snmp_v1_trap_destinations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_snmp_v3_trap_destinations.py
--rw-r--r--   0 runner    (1001) docker     (122)     3102 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_snmp_v3_users.py
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_health_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2218 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_node_information.py
--rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_ssh_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_time_and_locale_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4868 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/backups.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/firmware_bundles.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/firmware_drivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/ha_nodes.py
--rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/repositories.py
--rw-r--r--   0 runner    (1001) docker     (122)     2557 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/restores.py
--rw-r--r--   0 runner    (1001) docker     (122)     7717 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/scopes.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1727 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/settings/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.597218 hpeOneView-8.2.0/hpeOneView/resources/storage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/drive_enclosures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/sas_logical_jbod_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/sas_logical_jbods.py
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/storage_pools.py
--rw-r--r--   0 runner    (1001) docker     (122)     6416 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/storage_systems.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/storage_volume_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/storage_volume_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/storage/volumes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9045 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/task_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.597218 hpeOneView-8.2.0/hpeOneView/resources/uncategorized/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/uncategorized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7064 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/hpeOneView/resources/uncategorized/unmanaged_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 05:45:44.577217 hpeOneView-8.2.0/hpeOneView.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17132 2023-03-15 05:45:44.000000 hpeOneView-8.2.0/hpeOneView.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-03-15 05:45:44.000000 hpeOneView-8.2.0/hpeOneView.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 05:45:44.000000 hpeOneView-8.2.0/hpeOneView.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-15 05:45:44.000000 hpeOneView-8.2.0/hpeOneView.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-15 05:45:44.000000 hpeOneView-8.2.0/hpeOneView.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-15 05:45:44.597218 hpeOneView-8.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-03-15 05:45:34.000000 hpeOneView-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.662091 hpeOneView-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    17420 2023-05-02 05:30:55.662091 hpeOneView-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17001 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.646090 hpeOneView-8.3.0/hpeOneView/
+-rw-r--r--   0 runner    (1001) docker     (122)     3227 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26978 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    36104 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/oneview_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView/resources/activity/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/activity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5399 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/activity/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/activity/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4518 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/activity/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView/resources/data_services/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/data_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/data_services/metric_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView/resources/facilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6431 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/facilities/datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15134 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/facilities/power_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6081 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/facilities/racks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView/resources/fc_sans/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/fc_sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/fc_sans/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/fc_sans/managed_sans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/fc_sans/san_managers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/fc_sans/san_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView/resources/hypervisors/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/hypervisors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5173 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/hypervisors/hypervisor_cluster_profiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2834 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/hypervisors/hypervisor_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.654091 hpeOneView-8.3.0/hpeOneView/resources/networking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/connection_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6862 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/ethernet_networks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/fabrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/fc_networks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/fcoe_networks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/interconnect_link_topologies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/interconnect_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/interconnects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3152 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/internal_link_sets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4829 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/logical_downlinks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/logical_interconnect_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21567 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/logical_interconnects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/logical_switch_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6868 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/logical_switches.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3525 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/network_sets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/sas_interconnect_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/sas_interconnects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3358 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/sas_logical_interconnect_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7140 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/sas_logical_interconnects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/switch_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5961 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/switches.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4566 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/networking/uplink_sets.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    71677 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.654091 hpeOneView-8.3.0/hpeOneView/resources/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7034 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/search/index_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4806 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/search/labels.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.654091 hpeOneView-8.3.0/hpeOneView/resources/security/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3883 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/certificate_authority.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/certificate_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/certificates_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/login_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7597 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/security/users.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.658091 hpeOneView-8.3.0/hpeOneView/resources/servers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3267 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/enclosure_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9623 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4850 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools_ipv4_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools_ipv4_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7171 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/logical_enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/migratable_vc_domains.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/rack_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15631 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/server_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/server_hardware_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/server_profile_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14299 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/servers/server_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.662091 hpeOneView-8.3.0/hpeOneView/resources/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_configuration_timeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_read_community.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_snmp_v1_trap_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_snmp_v3_trap_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3102 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_snmp_v3_users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_health_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2218 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_node_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_ssh_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_time_and_locale_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4868 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/backups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/firmware_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/firmware_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/ha_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2557 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/restores.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7717 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/scopes.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1727 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/settings/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.662091 hpeOneView-8.3.0/hpeOneView/resources/storage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/drive_enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/sas_logical_jbod_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/sas_logical_jbods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/storage_pools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6416 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/storage_systems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/storage_volume_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/storage_volume_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/storage/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9045 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/task_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.662091 hpeOneView-8.3.0/hpeOneView/resources/uncategorized/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/uncategorized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7064 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/hpeOneView/resources/uncategorized/unmanaged_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 05:30:55.650090 hpeOneView-8.3.0/hpeOneView.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17420 2023-05-02 05:30:55.000000 hpeOneView-8.3.0/hpeOneView.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-05-02 05:30:55.000000 hpeOneView-8.3.0/hpeOneView.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 05:30:55.000000 hpeOneView-8.3.0/hpeOneView.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-02 05:30:55.000000 hpeOneView-8.3.0/hpeOneView.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-02 05:30:55.000000 hpeOneView-8.3.0/hpeOneView.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-02 05:30:55.662091 hpeOneView-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-02 05:30:42.000000 hpeOneView-8.3.0/setup.py
```

### Comparing `hpeOneView-8.2.0/LICENSE` & `hpeOneView-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/PKG-INFO` & `hpeOneView-8.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: hpeOneView
-Version: 8.2.0
+Version: 8.3.0
 Summary: HPE OneView Python Library
 Home-page: https://github.com/HewlettPackard/oneview-python
-Download-URL: https://github.com/HewlettPackard/oneview-python/tarball/v8.2.0
+Download-URL: https://github.com/HewlettPackard/oneview-python/tarball/v8.3.0
 Author: Hewlett Packard Enterprise Development LP
 Author-email: oneview-pythonsdk@hpe.com
 License: Apache
 Keywords: oneview,hpe
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HPE OneView SDK for Python
 
 ## Build Status 
 
-| OV Version | 8.20 | 8.10 | 8.00 | 7.20 | 7.10 | 7.00                                                                                                                                                                                    | 6.60                                                                                                                                                                                    | 6.50                                                                                                                                                                                    |                                                                                      6.40                                                                                       |                                                                                      6.30                                                                                       |                                                                                          6.20                                                                                          |                                                                                          6.10                                                                                          |                                                                                          6.00                                                                                          |                                                                                            5.60                                                                                            |
-| ------------- |  ------------- |  ------------- |  ------------- |   --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |----------------------------------------------------------------------------: |
-| SDK Version/Tag |[v8.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.2.0)|[v8.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.1.0)|[v8.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.0.0)|[v7.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.2.0)|[v7.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.1.0)| [v7.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v7.0.0)                                                                                                          | [v6.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.6.0)                                                                                                          | [v6.5.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.5.0)                                                                                                          |                                                 [v6.4.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.4.0)                                                  |                                                 [v6.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.3.0)                                                  |                                                     [v6.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.2.0)                                                     |                                                     [v6.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.1.0)                                                     |                                                     [v6.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.0.0)                                                     |                                                       [v5.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v5.6.0)                                                       |
-| Build Status    | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4371621558) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3626826357)| [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3006374044) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2675986741) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2376290875) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1967921808) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1658469670) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/4236699714) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/3524286157) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/986745563) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/726148134) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/623585124) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://travis-ci.com/github/HewlettPackard/oneview-python/builds/214352373) |
+| OV Version | 8.30 | 8.20 | 8.10 | 8.00 | 7.20 | 7.10 | 7.00                                                                                                                                                                                    | 6.60                                                                                                                                                                                    | 6.50                                                                                                                                                                                    |                                                                                      6.40                                                                                       |                                                                                      6.30                                                                                       |                                                                                          6.20                                                                                          |                                                                                          6.10                                                                                          |                                                                                          6.00                                                                                          |                                                                                            5.60                                                                                            |
+| ------------- |  ------------- |  ------------- |  ------------- |  ------------- |   --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |----------------------------------------------------------------------------: |
+| SDK Version/Tag |[v8.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.3.0)|[v8.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.2.0)|[v8.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.1.0)|[v8.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.0.0)|[v7.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.2.0)|[v7.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.1.0)| [v7.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v7.0.0)                                                                                                          | [v6.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.6.0)                                                                                                          | [v6.5.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.5.0)                                                                                                          |                                                 [v6.4.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.4.0)                                                  |                                                 [v6.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.3.0)                                                  |                                                     [v6.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.2.0)                                                     |                                                     [v6.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.1.0)                                                     |                                                     [v6.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.0.0)                                                     |                                                       [v5.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v5.6.0)                                                       |
+| Build Status    | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4800354967) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4371621558) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3626826357)| [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3006374044) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2675986741) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2376290875) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1967921808) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1658469670) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/4236699714) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/3524286157) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/986745563) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/726148134) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/623585124) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://travis-ci.com/github/HewlettPackard/oneview-python/builds/214352373) |
 
 ## Introduction
 
 HPE OneView makes it simple to deploy and manage today’s complex hybrid cloud infrastructure. HPE OneView can help you transform your data center to software-defined, and it supports HPE’s broad portfolio of servers, storage, and networking solutions, ensuring the simple and automated management of your hybrid infrastructure. Software-defined intelligence enables a template-driven approach for deploying, provisioning, updating, and integrating compute, storage, and networking infrastructure.
 
 The HPE OneView Python library provides a pure Python interface to the HPE OneView REST APIs. It depends on the [Python-Future](http://python-future.org/index.html) library to provide Python 2/3 compatibility.
 
@@ -31,15 +31,15 @@
 Refer to
 
 Supported HPE OneView Python [APIs Implementation](https://github.com/HewlettPackard/oneview-python/blob/master/endpoints-support.md) and
 Latest version of the OneView Python [SDK Documentation](https://hewlettpackard.github.io/oneview-python/index.html)
 
 ## What's New
 
-HPE OneView Python library extends support of the SDK to OneView REST API version 5000 (OneView v8.20)
+HPE OneView Python library extends support of the SDK to OneView REST API version 5200 (OneView v8.30)
 ### Migration script
 Perform migration from HPE OneView 6.x to HPE OneView 7.0 for non-Synergy appliance using below script.
 ```bash
    $ git clone https://github.com/HewlettPackard/oneview-python.git
    $ cd oneview-python/examples/migration/
    $ python migrate.py [<list of server hardwware names to be migrated>] 
 ```
@@ -106,21 +106,21 @@
    contains an installation of oneview-python installation you can use by just pulling down the Docker Image:
 
    The Docker Store image tag consist of two sections: <sdk_version-OV_version>
 
    Download and store a local copy of hpe-oneview-sdk-for-python and use it as a Docker image. <br />
    ```bash
 
-   $ docker pull hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.2.0-OV8.2
+   $ docker pull hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.3.0-OV8.3
    ```
 
    Run docker commands and this will in turn create sh session where you can create files, issue commands and execute the tests <br />
    ```bash
 
-   $ docker run -it hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.2.0-OV8.2 /bin/sh
+   $ docker run -it hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.3.0-OV8.3 /bin/sh
 
    ```
    
 ## Configuration
 
   ### JSON: 
   Connection properties for accessing the OneView appliance can be set in a JSON file.
```

### Comparing `hpeOneView-8.2.0/README.md` & `hpeOneView-8.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # HPE OneView SDK for Python
 
 ## Build Status 
 
-| OV Version | 8.20 | 8.10 | 8.00 | 7.20 | 7.10 | 7.00                                                                                                                                                                                    | 6.60                                                                                                                                                                                    | 6.50                                                                                                                                                                                    |                                                                                      6.40                                                                                       |                                                                                      6.30                                                                                       |                                                                                          6.20                                                                                          |                                                                                          6.10                                                                                          |                                                                                          6.00                                                                                          |                                                                                            5.60                                                                                            |
-| ------------- |  ------------- |  ------------- |  ------------- |   --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |----------------------------------------------------------------------------: |
-| SDK Version/Tag |[v8.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.2.0)|[v8.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.1.0)|[v8.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.0.0)|[v7.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.2.0)|[v7.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.1.0)| [v7.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v7.0.0)                                                                                                          | [v6.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.6.0)                                                                                                          | [v6.5.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.5.0)                                                                                                          |                                                 [v6.4.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.4.0)                                                  |                                                 [v6.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.3.0)                                                  |                                                     [v6.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.2.0)                                                     |                                                     [v6.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.1.0)                                                     |                                                     [v6.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.0.0)                                                     |                                                       [v5.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v5.6.0)                                                       |
-| Build Status    | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4371621558) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3626826357)| [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3006374044) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2675986741) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2376290875) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1967921808) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1658469670) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/4236699714) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/3524286157) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/986745563) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/726148134) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/623585124) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://travis-ci.com/github/HewlettPackard/oneview-python/builds/214352373) |
+| OV Version | 8.30 | 8.20 | 8.10 | 8.00 | 7.20 | 7.10 | 7.00                                                                                                                                                                                    | 6.60                                                                                                                                                                                    | 6.50                                                                                                                                                                                    |                                                                                      6.40                                                                                       |                                                                                      6.30                                                                                       |                                                                                          6.20                                                                                          |                                                                                          6.10                                                                                          |                                                                                          6.00                                                                                          |                                                                                            5.60                                                                                            |
+| ------------- |  ------------- |  ------------- |  ------------- |  ------------- |   --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |----------------------------------------------------------------------------: |
+| SDK Version/Tag |[v8.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.3.0)|[v8.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.2.0)|[v8.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.1.0)|[v8.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.0.0)|[v7.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.2.0)|[v7.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.1.0)| [v7.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v7.0.0)                                                                                                          | [v6.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.6.0)                                                                                                          | [v6.5.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.5.0)                                                                                                          |                                                 [v6.4.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.4.0)                                                  |                                                 [v6.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.3.0)                                                  |                                                     [v6.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.2.0)                                                     |                                                     [v6.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.1.0)                                                     |                                                     [v6.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.0.0)                                                     |                                                       [v5.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v5.6.0)                                                       |
+| Build Status    | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4800354967) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4371621558) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3626826357)| [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3006374044) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2675986741) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2376290875) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1967921808) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1658469670) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/4236699714) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/3524286157) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/986745563) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/726148134) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/623585124) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://travis-ci.com/github/HewlettPackard/oneview-python/builds/214352373) |
 
 ## Introduction
 
 HPE OneView makes it simple to deploy and manage today’s complex hybrid cloud infrastructure. HPE OneView can help you transform your data center to software-defined, and it supports HPE’s broad portfolio of servers, storage, and networking solutions, ensuring the simple and automated management of your hybrid infrastructure. Software-defined intelligence enables a template-driven approach for deploying, provisioning, updating, and integrating compute, storage, and networking infrastructure.
 
 The HPE OneView Python library provides a pure Python interface to the HPE OneView REST APIs. It depends on the [Python-Future](http://python-future.org/index.html) library to provide Python 2/3 compatibility.
 
@@ -18,15 +18,15 @@
 Refer to
 
 Supported HPE OneView Python [APIs Implementation](https://github.com/HewlettPackard/oneview-python/blob/master/endpoints-support.md) and
 Latest version of the OneView Python [SDK Documentation](https://hewlettpackard.github.io/oneview-python/index.html)
 
 ## What's New
 
-HPE OneView Python library extends support of the SDK to OneView REST API version 5000 (OneView v8.20)
+HPE OneView Python library extends support of the SDK to OneView REST API version 5200 (OneView v8.30)
 ### Migration script
 Perform migration from HPE OneView 6.x to HPE OneView 7.0 for non-Synergy appliance using below script.
 ```bash
    $ git clone https://github.com/HewlettPackard/oneview-python.git
    $ cd oneview-python/examples/migration/
    $ python migrate.py [<list of server hardwware names to be migrated>] 
 ```
@@ -93,21 +93,21 @@
    contains an installation of oneview-python installation you can use by just pulling down the Docker Image:
 
    The Docker Store image tag consist of two sections: <sdk_version-OV_version>
 
    Download and store a local copy of hpe-oneview-sdk-for-python and use it as a Docker image. <br />
    ```bash
 
-   $ docker pull hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.2.0-OV8.2
+   $ docker pull hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.3.0-OV8.3
    ```
 
    Run docker commands and this will in turn create sh session where you can create files, issue commands and execute the tests <br />
    ```bash
 
-   $ docker run -it hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.2.0-OV8.2 /bin/sh
+   $ docker run -it hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.3.0-OV8.3 /bin/sh
 
    ```
    
 ## Configuration
 
   ### JSON: 
   Connection properties for accessing the OneView appliance can be set in a JSON file.
```

### Comparing `hpeOneView-8.2.0/hpeOneView/__init__.py` & `hpeOneView-8.3.0/hpeOneView/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 
 standard_library.install_aliases()
 
 __title__ = 'hpeOneView'
-__version__ = '8.2.0'
+__version__ = '8.3.0'
 __copyright__ = '(C) Copyright (2012-2021) Hewlett Packard Enterprise Development LP'
 __license__ = 'Apache'
 
 ###
 # (C) Copyright [2021] Hewlett Packard Enterprise Development LP
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `hpeOneView-8.2.0/hpeOneView/connection.py` & `hpeOneView-8.3.0/hpeOneView/connection.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/exceptions.py` & `hpeOneView-8.3.0/hpeOneView/exceptions.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/oneview_client.py` & `hpeOneView-8.3.0/hpeOneView/oneview_client.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/activity/alerts.py` & `hpeOneView-8.3.0/hpeOneView/resources/activity/alerts.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/activity/events.py` & `hpeOneView-8.3.0/hpeOneView/resources/activity/events.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/activity/tasks.py` & `hpeOneView-8.3.0/hpeOneView/resources/activity/tasks.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/data_services/metric_streaming.py` & `hpeOneView-8.3.0/hpeOneView/resources/data_services/metric_streaming.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/facilities/datacenters.py` & `hpeOneView-8.3.0/hpeOneView/resources/facilities/datacenters.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/facilities/power_devices.py` & `hpeOneView-8.3.0/hpeOneView/resources/facilities/power_devices.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/facilities/racks.py` & `hpeOneView-8.3.0/hpeOneView/resources/facilities/racks.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/fc_sans/endpoints.py` & `hpeOneView-8.3.0/hpeOneView/resources/fc_sans/endpoints.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/fc_sans/managed_sans.py` & `hpeOneView-8.3.0/hpeOneView/resources/fc_sans/managed_sans.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/fc_sans/san_managers.py` & `hpeOneView-8.3.0/hpeOneView/resources/fc_sans/san_managers.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/fc_sans/san_providers.py` & `hpeOneView-8.3.0/hpeOneView/resources/fc_sans/san_providers.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/hypervisors/hypervisor_cluster_profiles.py` & `hpeOneView-8.3.0/hpeOneView/resources/hypervisors/hypervisor_cluster_profiles.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/hypervisors/hypervisor_managers.py` & `hpeOneView-8.3.0/hpeOneView/resources/hypervisors/hypervisor_managers.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/connection_templates.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/connection_templates.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/ethernet_networks.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/ethernet_networks.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/fabrics.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/fabrics.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/fc_networks.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/fc_networks.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/fcoe_networks.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/fcoe_networks.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/interconnect_link_topologies.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/interconnect_link_topologies.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/interconnect_types.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/interconnect_types.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/interconnects.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/interconnects.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/internal_link_sets.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/internal_link_sets.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/logical_downlinks.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/logical_downlinks.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/logical_interconnect_groups.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/logical_interconnect_groups.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/logical_interconnects.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/logical_interconnects.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/logical_switch_groups.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/logical_switch_groups.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/logical_switches.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/logical_switches.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/network_sets.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/network_sets.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/sas_interconnect_types.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/sas_interconnect_types.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/sas_interconnects.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/sas_interconnects.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/sas_logical_interconnect_groups.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/sas_logical_interconnect_groups.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/sas_logical_interconnects.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/sas_logical_interconnects.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/switch_types.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/switch_types.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/switches.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/switches.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/networking/uplink_sets.py` & `hpeOneView-8.3.0/hpeOneView/resources/networking/uplink_sets.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/resource.py` & `hpeOneView-8.3.0/hpeOneView/resources/resource.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/search/index_resources.py` & `hpeOneView-8.3.0/hpeOneView/resources/search/index_resources.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/search/labels.py` & `hpeOneView-8.3.0/hpeOneView/resources/search/labels.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/security/certificate_authority.py` & `hpeOneView-8.3.0/hpeOneView/resources/security/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/security/certificate_rabbitmq.py` & `hpeOneView-8.3.0/hpeOneView/resources/security/certificate_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/security/certificates_server.py` & `hpeOneView-8.3.0/hpeOneView/resources/security/certificates_server.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/security/login_details.py` & `hpeOneView-8.3.0/hpeOneView/resources/security/login_details.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/security/roles.py` & `hpeOneView-8.3.0/hpeOneView/resources/security/roles.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/security/users.py` & `hpeOneView-8.3.0/hpeOneView/resources/security/users.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/connections.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/connections.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/enclosure_groups.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/enclosure_groups.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/enclosures.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/enclosures.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools_ipv4_ranges.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools_ipv4_ranges.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools_ipv4_subnets.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools_ipv4_subnets.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/id_pools_ranges.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/id_pools_ranges.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/logical_enclosures.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/logical_enclosures.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/migratable_vc_domains.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/migratable_vc_domains.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/rack_manager.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/rack_manager.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/server_hardware.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/server_hardware.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/server_hardware_types.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/server_hardware_types.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/server_profile_templates.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/server_profile_templates.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/servers/server_profiles.py` & `hpeOneView-8.3.0/hpeOneView/resources/servers/server_profiles.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_configuration_timeconfig.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_configuration_timeconfig.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_read_community.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_read_community.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_snmp_v1_trap_destinations.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_snmp_v1_trap_destinations.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_snmp_v3_trap_destinations.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_snmp_v3_trap_destinations.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_device_snmp_v3_users.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_device_snmp_v3_users.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_health_status.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_health_status.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_network_interfaces.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_node_information.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_node_information.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_proxy_configuration.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_ssh_access.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_ssh_access.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/appliance_time_and_locale_configuration.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/appliance_time_and_locale_configuration.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/backups.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/backups.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/firmware_bundles.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/firmware_bundles.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/firmware_drivers.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/firmware_drivers.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/ha_nodes.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/ha_nodes.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/licenses.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/licenses.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/repositories.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/repositories.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/restores.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/restores.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/scopes.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/scopes.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/settings/versions.py` & `hpeOneView-8.3.0/hpeOneView/resources/settings/versions.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/drive_enclosures.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/drive_enclosures.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/sas_logical_jbod_attachments.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/sas_logical_jbod_attachments.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/sas_logical_jbods.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/sas_logical_jbods.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/storage_pools.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/storage_pools.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/storage_systems.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/storage_systems.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/storage_volume_attachments.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/storage_volume_attachments.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/storage_volume_templates.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/storage_volume_templates.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/storage/volumes.py` & `hpeOneView-8.3.0/hpeOneView/resources/storage/volumes.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/task_monitor.py` & `hpeOneView-8.3.0/hpeOneView/resources/task_monitor.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView/resources/uncategorized/unmanaged_devices.py` & `hpeOneView-8.3.0/hpeOneView/resources/uncategorized/unmanaged_devices.py`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/hpeOneView.egg-info/PKG-INFO` & `hpeOneView-8.3.0/hpeOneView.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: hpeOneView
-Version: 8.2.0
+Version: 8.3.0
 Summary: HPE OneView Python Library
 Home-page: https://github.com/HewlettPackard/oneview-python
-Download-URL: https://github.com/HewlettPackard/oneview-python/tarball/v8.2.0
+Download-URL: https://github.com/HewlettPackard/oneview-python/tarball/v8.3.0
 Author: Hewlett Packard Enterprise Development LP
 Author-email: oneview-pythonsdk@hpe.com
 License: Apache
 Keywords: oneview,hpe
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HPE OneView SDK for Python
 
 ## Build Status 
 
-| OV Version | 8.20 | 8.10 | 8.00 | 7.20 | 7.10 | 7.00                                                                                                                                                                                    | 6.60                                                                                                                                                                                    | 6.50                                                                                                                                                                                    |                                                                                      6.40                                                                                       |                                                                                      6.30                                                                                       |                                                                                          6.20                                                                                          |                                                                                          6.10                                                                                          |                                                                                          6.00                                                                                          |                                                                                            5.60                                                                                            |
-| ------------- |  ------------- |  ------------- |  ------------- |   --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |----------------------------------------------------------------------------: |
-| SDK Version/Tag |[v8.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.2.0)|[v8.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.1.0)|[v8.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.0.0)|[v7.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.2.0)|[v7.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.1.0)| [v7.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v7.0.0)                                                                                                          | [v6.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.6.0)                                                                                                          | [v6.5.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.5.0)                                                                                                          |                                                 [v6.4.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.4.0)                                                  |                                                 [v6.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.3.0)                                                  |                                                     [v6.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.2.0)                                                     |                                                     [v6.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.1.0)                                                     |                                                     [v6.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.0.0)                                                     |                                                       [v5.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v5.6.0)                                                       |
-| Build Status    | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4371621558) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3626826357)| [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3006374044) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2675986741) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2376290875) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1967921808) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1658469670) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/4236699714) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/3524286157) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/986745563) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/726148134) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/623585124) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://travis-ci.com/github/HewlettPackard/oneview-python/builds/214352373) |
+| OV Version | 8.30 | 8.20 | 8.10 | 8.00 | 7.20 | 7.10 | 7.00                                                                                                                                                                                    | 6.60                                                                                                                                                                                    | 6.50                                                                                                                                                                                    |                                                                                      6.40                                                                                       |                                                                                      6.30                                                                                       |                                                                                          6.20                                                                                          |                                                                                          6.10                                                                                          |                                                                                          6.00                                                                                          |                                                                                            5.60                                                                                            |
+| ------------- |  ------------- |  ------------- |  ------------- |  ------------- |   --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |----------------------------------------------------------------------------: |
+| SDK Version/Tag |[v8.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.3.0)|[v8.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.2.0)|[v8.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.1.0)|[v8.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/8.0.0)|[v7.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.2.0)|[v7.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/7.1.0)| [v7.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v7.0.0)                                                                                                          | [v6.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.6.0)                                                                                                          | [v6.5.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.5.0)                                                                                                          |                                                 [v6.4.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.4.0)                                                  |                                                 [v6.3.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.3.0)                                                  |                                                     [v6.2.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.2.0)                                                     |                                                     [v6.1.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.1.0)                                                     |                                                     [v6.0.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v6.0.0)                                                     |                                                       [v5.6.0](https://github.com/HewlettPackard/oneview-python/releases/tag/v5.6.0)                                                       |
+| Build Status    | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4800354967) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/4371621558) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3626826357)| [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/3006374044) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2675986741) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/2376290875) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1967921808) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/1658469670) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/4236699714) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/runs/3524286157) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/986745563) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/726148134) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://github.com/HewlettPackard/oneview-python/actions/runs/623585124) | [![Build status](https://github.com/HewlettPackard/oneview-python/actions/workflows/run_tests.yml/badge.svg)](https://travis-ci.com/github/HewlettPackard/oneview-python/builds/214352373) |
 
 ## Introduction
 
 HPE OneView makes it simple to deploy and manage today’s complex hybrid cloud infrastructure. HPE OneView can help you transform your data center to software-defined, and it supports HPE’s broad portfolio of servers, storage, and networking solutions, ensuring the simple and automated management of your hybrid infrastructure. Software-defined intelligence enables a template-driven approach for deploying, provisioning, updating, and integrating compute, storage, and networking infrastructure.
 
 The HPE OneView Python library provides a pure Python interface to the HPE OneView REST APIs. It depends on the [Python-Future](http://python-future.org/index.html) library to provide Python 2/3 compatibility.
 
@@ -31,15 +31,15 @@
 Refer to
 
 Supported HPE OneView Python [APIs Implementation](https://github.com/HewlettPackard/oneview-python/blob/master/endpoints-support.md) and
 Latest version of the OneView Python [SDK Documentation](https://hewlettpackard.github.io/oneview-python/index.html)
 
 ## What's New
 
-HPE OneView Python library extends support of the SDK to OneView REST API version 5000 (OneView v8.20)
+HPE OneView Python library extends support of the SDK to OneView REST API version 5200 (OneView v8.30)
 ### Migration script
 Perform migration from HPE OneView 6.x to HPE OneView 7.0 for non-Synergy appliance using below script.
 ```bash
    $ git clone https://github.com/HewlettPackard/oneview-python.git
    $ cd oneview-python/examples/migration/
    $ python migrate.py [<list of server hardwware names to be migrated>] 
 ```
@@ -106,21 +106,21 @@
    contains an installation of oneview-python installation you can use by just pulling down the Docker Image:
 
    The Docker Store image tag consist of two sections: <sdk_version-OV_version>
 
    Download and store a local copy of hpe-oneview-sdk-for-python and use it as a Docker image. <br />
    ```bash
 
-   $ docker pull hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.2.0-OV8.2
+   $ docker pull hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.3.0-OV8.3
    ```
 
    Run docker commands and this will in turn create sh session where you can create files, issue commands and execute the tests <br />
    ```bash
 
-   $ docker run -it hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.2.0-OV8.2 /bin/sh
+   $ docker run -it hewlettpackardenterprise/hpe-oneview-sdk-for-python:v8.3.0-OV8.3 /bin/sh
 
    ```
    
 ## Configuration
 
   ### JSON: 
   Connection properties for accessing the OneView appliance can be set in a JSON file.
```

### Comparing `hpeOneView-8.2.0/hpeOneView.egg-info/SOURCES.txt` & `hpeOneView-8.3.0/hpeOneView.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hpeOneView-8.2.0/setup.py` & `hpeOneView-8.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 ###
 
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(name='hpeOneView',
-      version='8.2.0',
+      version='8.3.0',
       description='HPE OneView Python Library',
       url='https://github.com/HewlettPackard/oneview-python',
-      download_url="https://github.com/HewlettPackard/oneview-python/tarball/v8.2.0",
+      download_url="https://github.com/HewlettPackard/oneview-python/tarball/v8.3.0",
       author='Hewlett Packard Enterprise Development LP',
       author_email='oneview-pythonsdk@hpe.com',
       license='Apache',
       packages=find_packages(exclude=['examples*', 'tests*']),
       keywords=['oneview', 'hpe'],
       long_description_content_type="text/markdown",
       install_requires=['future>=0.15.2', 'docutils<0.18'])
```

