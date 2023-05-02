# Comparing `tmp/ironic-9.1.6.tar.gz` & `tmp/ironic-9.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ironic-9.1.6.tar", last modified: Thu Dec 20 16:25:57 2018, max compression
+gzip compressed data, was "dist/ironic-9.1.7.tar", last modified: Fri Apr 26 15:41:44 2019, max compression
```

## Comparing `ironic-9.1.6.tar` & `ironic-9.1.7.tar`

### file list

```diff
@@ -1,1263 +1,1266 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/objects/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7703 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/notification.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6820 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/conductor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13116 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/objects/volume_connector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2078 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/objects/indirection.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17362 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/port.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18662 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1477 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10359 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/objects/chassis.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30236 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/node.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14316 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/objects/volume_target.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14982 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/portgroup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4120 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/objects/fields.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/db/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33459 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1560 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/db/sqlalchemy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1222 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/1e1d5ace7dc6_add_inspection_started_at_and_.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1020 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3ae36a5f5131_add_logical_name.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1177 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/f6fdb920c182_set_pxe_enabled_true.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1040 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/1d6951876d68_add_storage_interface_db_field_and_.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1096 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/31baaf680d2b_add_node_instance_info.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1208 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/487deb87cc9d_add_conductor_affinity_and_online.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1208 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/dbefd6bdaa2c_add_default_column_to_.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1022 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3d86a077a3f2_add_port_physical_network.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1022 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/242cc6a923b3_add_node_maintenance_reason.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      929 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3cb628139ea4_nodes_add_console_enabled.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      969 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/21b331f883ef_add_provision_updated_at.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2044 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/868cb606a74a_add_version_field_in_base_class.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2060 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/2353895ecfae_add_conductor_hardware_interfaces_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4331 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1314 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/493d8f27f235_add_portgroup_configuration_fields.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2057 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/daa1ba02d98_add_volume_connectors_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1084 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/789acc877671_add_raid_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      988 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/e294876e8028_add_node_network_interface.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2225 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/1a59178ebdf6_add_volume_targets_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1005 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/60cf717201bc_add_standalone_ports_supported.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1089 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/2fb93ffd2af1_increase_node_name_length.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1523 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/5674c57409b9_replace_nostate_with_available.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1074 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3bea56f25597_add_unique_constraint_to_instance_uuid.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      950 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/4f399b21ae71_add_node_clean_step.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1024 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/bb59b63f55a_add_node_driver_internal_info.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1385 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/c14cef6dfedf_populate_node_network_interface.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2485 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/5ea1b0d310e_added_port_group_table_and_altered_ports.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1440 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/48d6c242bb9b_add_node_tags.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1192 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/10b163d4481e_add_port_portgroup_internal_info.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1007 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/516faf1bb9b1_resizing_column_nodes_driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1009 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/dd34e1f1303b_add_resource_class_to_node.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1929 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/bcdd431ba0bf_add_fields_for_all_interfaces.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      434 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/README
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      349 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/script.py.mako
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1971 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic/env.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    49980 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10401 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3680 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/db/sqlalchemy/migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      975 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/db/sqlalchemy/alembic.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1121 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/snmp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6860 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/pxe.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3991 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/hardware_type.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1199 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/redfish.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12597 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/ilo/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8659 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    31611 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1882 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/ilo/console.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/ilo/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11840 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4406 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/vendor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25800 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/boot.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17982 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17634 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ilo/firmware_processor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18019 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/image_cache.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/network/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26268 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/network/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5260 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/network/flat.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/network/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3748 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/network/noop.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7831 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/network/neutron.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13399 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/console_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26243 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/snmp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      736 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/pxe_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      480 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/agent_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26174 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/pxe.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      776 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/elilo_efi_pxe_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      697 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/pxe_grub_config.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/irmc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12032 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/irmc/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8924 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/irmc/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/irmc/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6663 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/irmc/inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    44568 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/irmc/boot.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14532 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/irmc/management.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/storage/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/storage/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      938 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/storage/noop.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20168 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/storage/cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    29186 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/agent_base_vendor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/cimc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6610 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/cimc/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2709 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/cimc/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/cimc/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6101 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/cimc/management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    55794 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ipmitool.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/ucs/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8253 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ucs/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4381 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/ucs/helper.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/ucs/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5632 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/ucs/management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25065 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/iscsi_deploy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/redfish/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6498 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/redfish/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9133 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/redfish/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/redfish/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6782 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/redfish/management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30566 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/drac/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6766 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/drac/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2830 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/drac/job.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5437 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/drac/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    35257 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/drac/raid.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/drac/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5745 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/drac/inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14607 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/drac/management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6879 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/drac/bios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7523 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/drac/vendor_passthru.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      777 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/modules/boot.ipxe
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2308 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/noop.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    53171 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/deploy_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7583 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/fake.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6964 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8408 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/agent_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      131 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/master_grub_cfg.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/drivers/modules/oneview/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6780 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10263 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4309 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12537 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/deploy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9784 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14841 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/oneview/deploy_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1817 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/modules/ipxe_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    46482 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5029 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/ipmi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4292 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/oneview.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/drivers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4139 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/ilo.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3351 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/drac.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1972 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/cisco_ucs.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2474 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/fake_hardware.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3084 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/agent.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4258 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/irmc.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8708 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/fake.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4128 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/raid_config_schema.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3539 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/drivers/generic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/conf/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8279 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/glance.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1804 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/snmp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1533 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/audit.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6403 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/pxe.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1178 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/redfish.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8312 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/conductor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3160 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2354 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/console.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2651 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/ipmi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2255 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/oneview.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2325 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1312 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/swift.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4123 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/ilo.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1032 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/drac.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4610 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/deploy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1102 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/service_catalog.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14838 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/default.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4491 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/agent.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1250 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/metrics_statsd.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      985 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/dhcp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/iscsi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3641 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/opts.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2383 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/metrics.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2018 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/auth.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3160 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/irmc.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2090 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      874 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/keystone.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1451 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1771 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/cisco.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4108 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conf/neutron.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      928 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conf/database.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/api/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1352 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6459 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/hooks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/api/middleware/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      861 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/middleware/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2281 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/middleware/auth_token.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3876 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/middleware/parsable_error.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1045 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/app.wsgi
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/api/controllers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3802 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3790 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/api/controllers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2030 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/api/controllers/link.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/api/controllers/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1083 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/api/controllers/v1/state.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3524 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/api/controllers/v1/volume.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21274 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/volume_connector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1718 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/collection.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20567 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10776 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30830 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/port.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9293 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7093 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/notification_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14089 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/chassis.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77643 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/node.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21189 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/volume_target.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6940 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/ramdisk.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24724 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/portgroup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4486 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/versions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18125 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/controllers/v1/driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      897 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/api/expose.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3964 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/api/app.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/cmd/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12834 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/cmd/dbsync.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3146 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/cmd/conductor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1711 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/cmd/api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1076 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/conductor/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   147125 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conductor/manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25452 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conductor/base_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27329 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conductor/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conductor/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    45367 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conductor/rpcapi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7492 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/conductor/notification_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22392 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/conductor/task_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      705 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/common/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2455 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/profiler.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23059 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/exception.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1272 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5782 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/release_mappings.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1222 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5240 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/raid.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18304 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/isolinux_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3240 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/rpc_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7349 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/swift.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2578 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/context.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3565 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/dhcp_factory.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11275 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/image_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1284 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/boot_devices.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12495 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/states.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5220 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/rpc.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18722 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/grub_conf.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4019 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/keystone.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15304 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/policy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2316 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/wsgi_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      900 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/i18n.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6041 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/fsm.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3949 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/network.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/common/glance_service/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1431 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/glance_service/service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7961 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/glance_service/service_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/glance_service/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/common/glance_service/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/common/glance_service/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10410 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/glance_service/v2/image_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/common/glance_service/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/glance_service/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1072 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/glance_service/v1/image_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6568 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/glance_service/base_image_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22713 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/images.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21573 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/neutron.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23783 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/driver_factory.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2290 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/hash_ring.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15581 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/common/pxe_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/dhcp/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3028 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/dhcp/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/dhcp/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/dhcp/none.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9575 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/dhcp/neutron.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/objects/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    40621 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_objects.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5020 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/objects/test_fields.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6011 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/objects/test_chassis.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8869 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9931 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_volume_target.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7074 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_conductor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/objects/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9581 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_volume_connector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9282 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_port.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7658 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_portgroup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12651 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_node.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11955 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/objects/test_notification.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2193 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/stubs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/db/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5442 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/test_ports.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9199 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/test_portgroups.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3335 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/test_chassis.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15369 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/db/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18882 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/db/test_conductor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6721 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/test_volume_connectors.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2239 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7546 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/test_volume_targets.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4539 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/db/test_node_tags.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5667 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/db/test_api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27797 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/db/test_nodes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3385 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/test_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30775 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/test_migrations.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1448 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/test_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3360 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/third_party_driver_mock_specs.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      763 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/pxe_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6400 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_ipmi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      643 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/elilo_efi_pxe_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      673 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/pxe_grub_config.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6461 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_pxe.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18619 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2045 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_redfish.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1914 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_snmp.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10684 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2923 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_console.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    28070 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52035 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_boot.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22968 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52062 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26714 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_firmware_processor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5017 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_vendor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    61131 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_agent_base_vendor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2666 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_noop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/network/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3793 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_noop.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20222 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_neutron.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/network/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8872 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_flat.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    71186 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10308 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_agent_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33377 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_image_cache.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26542 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_console_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    59467 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_pxe.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20008 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22864 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    76588 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_boot.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11495 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10969 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4241 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ok.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4271 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ng.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/storage/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    31687 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/storage/test_cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/storage/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    66318 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_snmp.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13746 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5675 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5130 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/test_common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15211 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6124 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7283 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/test_helper.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    59054 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10741 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8645 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8421 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6845 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_bios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5109 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14860 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_periodic_task.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    59077 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_raid.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      822 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25499 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11638 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6704 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6492 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_job.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   108163 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_deploy_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    51573 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_iscsi_deploy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15681 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_power.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16274 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_management.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4768 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_inspect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23866 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_deploy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18349 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_deploy_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10872 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   122471 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_ipmitool.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9167 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/modules/test_inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7636 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_irmc.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1001 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7620 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_ilo.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4063 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_generic.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      909 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config_boot_from_volume_no_volumes.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      759 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/drivers/boot.ipxe
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16880 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6591 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_cisco.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10925 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/third_party_driver_mocks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      988 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config_boot_from_volume.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5086 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_fake.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7886 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_oneview.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6729 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/test_drac.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      631 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config_timeout.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      575 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/conf/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/conf/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2394 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conf/test_auth.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/api/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5290 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/test_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1464 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/test_ospmiddleware.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4195 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/api/test_acl.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6430 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10456 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/api/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/api/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1985 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/api/test_audit.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11219 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/api/test_hooks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4418 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/api/test_middleware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/api/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2502 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_versions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8162 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_ramdisk.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23848 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_drivers.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    99129 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_ports.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    64105 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_portgroups.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27294 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_chassis.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    46793 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_volume_connectors.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    44835 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_volume_targets.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2184 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_volume.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13835 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2863 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_expose.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    28744 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   193806 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_nodes.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2440 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10401 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/v1/test_notification_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3515 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/api/test_root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1573 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/cmd/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2687 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/cmd/test_conductor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/cmd/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9066 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/cmd/test_dbsync.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/conductor/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24218 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/test_base_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   321803 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/test_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    49551 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/test_task_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/conductor/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8111 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/mgr_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    74243 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2098 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/test__mgr_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20153 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/conductor/test_rpcapi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9639 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/conductor/test_notification_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/common/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4001 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_keystone.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1461 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/common/test_states.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    36176 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_driver_factory.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3255 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_hash_ring.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    39763 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_neutron.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7824 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_release_mappings.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18000 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_image_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8223 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/common/test_rpc.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2255 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/common/test_rpc_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2913 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/common/test_exception.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3719 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/common/test_fsm.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    42088 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_images.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11359 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_raid.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    39058 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_pxe_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2927 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_wsgi_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    36754 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/common/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    37409 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_glance_service.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14895 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_network.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6655 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_policy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26342 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3060 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_context.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9080 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/common/test_swift.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/unit/dhcp/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4085 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/dhcp/test_factory.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18642 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/dhcp/test_neutron.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/dhcp/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1666 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/unit/policy_fixture.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5877 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/unit/raid_constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/tests/functional/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/functional/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9038 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/tests/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/ironic/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      670 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/locale/ko_KR/LC_MESSAGES/ironic-log-critical.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      658 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/locale/pt_BR/LC_MESSAGES/ironic-log-critical.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    79900 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/locale/ja/LC_MESSAGES/ironic.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      789 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/locale/ja/LC_MESSAGES/ironic-log-critical.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17284 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/locale/fr/LC_MESSAGES/ironic-log-info.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      738 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic/locale/fr/LC_MESSAGES/ironic-log-critical.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      591 2018-12-20 16:24:00.000000 ironic-9.1.6/driver-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6041 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8116 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6540 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-bfv/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6585 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-bfv/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-bfv/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-inspector/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7615 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-inspector/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-inspector/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6925 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/ironic-dsvm-standalone/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3797 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/ironic-dsvm-standalone/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/ironic-dsvm-standalone/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6076 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5944 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9071 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6059 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:24:00.000000 ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/post.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1353 2018-12-20 16:24:00.000000 ironic-9.1.6/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   183132 2018-12-20 16:25:56.000000 ironic-9.1.6/ChangeLog
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      988 2018-12-20 16:24:00.000000 ironic-9.1.6/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      986 2018-12-20 16:24:00.000000 ironic-9.1.6/Vagrantfile
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      330 2018-12-20 16:24:00.000000 ironic-9.1.6/CONTRIBUTING.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       17 2018-12-20 16:23:54.000000 ironic-9.1.6/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16714 2018-12-20 16:25:56.000000 ironic-9.1.6/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6693 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56028 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic.egg-info/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      704 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/settings
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3169 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/plugin.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2694 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/common_settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/files/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      891 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/files/apache-ironic-api-redirect.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/files/hooks/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     2845 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/files/hooks/qemu.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1731 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/files/apache-ironic-api.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      283 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/files/apache-ipxe-ironic.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/files/debs/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1137 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/files/debs/ironic
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/files/rpms/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      260 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/files/rpms/ironic
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/upgrade/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1466 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/upgrade/settings
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      454 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/upgrade/shutdown.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4485 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/upgrade/upgrade.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     6625 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/upgrade/resources.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/tools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/tools/ironic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/tools/ironic/templates/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/tools/ironic/templates/brbm.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2278 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/tools/ironic/templates/vm.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      424 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/tools/ironic/templates/tftpd-xinetd.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/tools/ironic/scripts/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1091 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/tools/ironic/scripts/setup-network.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4802 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/tools/ironic/scripts/configure-vm.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4451 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/tools/ironic/scripts/create-node.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1053 2018-12-20 16:23:54.000000 ironic-9.1.6/devstack/tools/ironic/scripts/cleanup-node.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/devstack/lib/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    91921 2018-12-20 16:24:00.000000 ironic-9.1.6/devstack/lib/ironic
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/cli/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6220 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/cli/ironic-dbsync.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/cli/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/configuration/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      288 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/configuration/config.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      590 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/configuration/sample-config.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      236 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/configuration/policy.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      406 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/configuration/sample-policy.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      440 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/install/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11598 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/enabling-drivers.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      743 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/install-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      197 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/setup-drivers.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10111 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3090 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/enabling-https.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/next-steps.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7557 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/troubleshooting.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6549 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-tenant-networks.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      384 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/advanced.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3182 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-ipmi.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1174 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/install-obs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4838 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/configure-glance-images.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/install/include/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2856 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/configure-ironic-api.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2077 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/configure-ironic-api-mod_wsgi.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      657 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/common-configure.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2543 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/disk-label.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3585 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/root-device-hints.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1154 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/common-prerequisites.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6153 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/configure-ironic-conductor.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2103 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/local-boot-partition-images.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/console.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1798 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/boot-mode.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3846 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/kernel-boot-parameters.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      802 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/notifications.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2899 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/include/trusted-boot.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3992 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-identity.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7632 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/standalone.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2929 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/deploy-ramdisk.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    31467 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/enrollment.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1141 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/install-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3591 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/get_started.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3116 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-glance-swift.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3707 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-nova-flavors.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/configure-iscsi.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13414 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-pxe.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3695 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-networking.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      376 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/configure-integration.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6722 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-compute.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6129 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configdrive.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1098 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/configure-cleaning.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      662 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/install/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      355 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/install/install.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4390 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/images/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38252 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/images/deployment_architecture_2.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38085 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/images/logical_architecture.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25598 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/images/states.svg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    49070 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/images/conceptual_architecture.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77412 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/images/deployment_steps.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    84269 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/images/sample_trace_details.svg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    58011 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/images/sample_trace.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/user/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14634 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/images_src/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   158538 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/images_src/deployment_steps.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/contributor/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12232 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/code-contribution-guide.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1452 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/contributor/governance.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5606 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/vendor-passthru.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    29776 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/dev-quickstart.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2906 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/contributor/webapi.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4153 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/ironic-multitenant-networking.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8892 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/webapi-version-history.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4255 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/drivers.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3920 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/contributor/osprofiler-support.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4779 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/architecture.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3745 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/ironic-boot-from-volume.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4962 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/releasing.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6672 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/contributor/notifications.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4825 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/faq.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1759 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/contributor/third-party-ci.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3087 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1038 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/contributor/states.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2385 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/admin/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2575 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/radosgw.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6483 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/multitenancy.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13274 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/troubleshooting.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7195 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/console.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/doc/source/admin/drivers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3345 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/cimc.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15538 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/oneview.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6531 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/ipmitool.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5718 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/ipa.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77574 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/ilo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6011 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/snmp.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3307 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/ucs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3455 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/redfish.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      962 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/pxe.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18464 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers/irmc.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12481 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/cleaning.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1730 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/drivers.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4394 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/inspection.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5412 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/security.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13401 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/raid.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19350 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/report.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18553 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/upgrade-guide.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25167 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/notifications.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8149 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/adoption.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2845 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/boot-from-volume.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1968 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/admin/gmr.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1175 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5458 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/portgroups.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3746 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/admin/api-audit-support.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4273 2018-12-20 16:23:54.000000 ironic-9.1.6/doc/source/admin/metrics.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11184 2018-12-20 16:24:00.000000 ironic-9.1.6/doc/source/admin/upgrade-to-hardware-types.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2018-12-20 16:23:54.000000 ironic-9.1.6/LICENSE
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1745 2018-12-20 16:24:00.000000 ironic-9.1.6/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5565 2018-12-20 16:24:00.000000 ironic-9.1.6/vagrant.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      287 2018-12-20 16:24:00.000000 ironic-9.1.6/.testr.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2018-12-20 16:23:54.000000 ironic-9.1.6/setup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      148 2018-12-20 16:23:54.000000 ironic-9.1.6/.mailmap
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/zuul.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6006 2018-12-20 16:24:00.000000 ironic-9.1.6/zuul.d/legacy-ironic-jobs.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1514 2018-12-20 16:24:00.000000 ironic-9.1.6/zuul.d/project.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/etc/ironic/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      113 2018-12-20 16:24:00.000000 ironic-9.1.6/etc/ironic/policy.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/etc/ironic/rootwrap.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      992 2018-12-20 16:23:54.000000 ironic-9.1.6/etc/ironic/rootwrap.d/ironic-lib.filters
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      212 2018-12-20 16:23:54.000000 ironic-9.1.6/etc/ironic/rootwrap.d/ironic-images.filters
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      312 2018-12-20 16:23:54.000000 ironic-9.1.6/etc/ironic/rootwrap.d/ironic-utils.filters
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      739 2018-12-20 16:23:54.000000 ironic-9.1.6/etc/ironic/api_audit_map.conf.sample
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4286 2018-12-20 16:24:00.000000 ironic-9.1.6/etc/ironic/policy.json.sample
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2018-12-20 16:23:54.000000 ironic-9.1.6/etc/ironic/rootwrap.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   120564 2018-12-20 16:24:00.000000 ironic-9.1.6/etc/ironic/ironic.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/etc/apache2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1318 2018-12-20 16:24:00.000000 ironic-9.1.6/etc/apache2/ironic
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/releasenotes/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      181 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/source/ocata.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/source/mitaka.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      107 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/source/unreleased.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9480 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8375 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/releasenotes/source/_static/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/source/_static/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/source/newton.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/releasenotes/source/_templates/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/source/_templates/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      387 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/releasenotes/notes/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      284 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/inject-nmi-dacd692b1f259a30.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-api-access-logs-68b9ca4f411f339c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      434 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/lookup-ignore-malformed-macs-09e7e909f3a134a3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      255 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/snmp-reboot-delay-d18ee3f6c6fc0998.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      184 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/automated_clean_config-0170c95ae210f953.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      459 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-verbose-option-261f1b9e24212ee2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac_host-deprecated-b181149246eecb47.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      159 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/clear-target-stable-states-4545602d7aed9898.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/scciclient-0.4.0-6f01c0f0a5c39062.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      659 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipa-streams-raw-images-1010327b0dad763c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      137 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipmitool-vendor-3f0f52240ebbe489.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      230 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/disable-clean-step-reset-ilo-1869a6e08f39901c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      174 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/manual-abort-d3d8985a5de7376a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       76 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/snmp-outlet-validate-ffbe8e6687172efc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1032 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/mask-configdrive-contents-77fc557d6bc63b2b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      201 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/logging-keystoneauth-9db7e56c54c2473d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      758 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/shred-final-overwrite-with-zeros-50b5ba5b19c0da27.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      375 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-clean-steps-not-running-0d065cb022bc0419.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      162 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-clean-nodes-38cfa633ca518f99.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/inspector-for-cisco-bffe1d1af7aec677.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1518374-decd73fd82c2eb94.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/conductor_early_import-fd29fa8b89089977.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      639 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/erase-devices-metadata-config-f39b6ca415a87757.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       99 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1579635-cffd990b51bcb5ab.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add_infiniband_support-f497767f77277a1a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      532 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/no-root-device-as-kernel-param-5e5326acae7b77a4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      130 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/idrac-no-vendor-911904dd69457826.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      129 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/agent-wol-driver-4116f64907d0db9c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/context-domain-id-name-deprecation-ae6e40718273be8d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      679 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/newton-driver-deprecations-e40369be37203057.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      465 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-boot-from-volume-for-iscsi-deploy-71c1f2905498c50d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/restart-console-on-conductor-startup-5cff6128c325b18e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      262 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-messaging-aliases-0a6ba1ed392b1fed.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      245 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-oneview-deallocate-server-8256e279af837e5d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      327 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/glance-v2-83b04fec247cd22f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      198 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/periodic-tasks-drivers-ae9cddab88b546c6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1214 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/rely-on-standalone-ports-supported-8153e1135787828b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/validate-port-info-before-using-it-e26135982d37c698.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      747 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/enable-osprofiler-support-e3839b0fa90d3831.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      402 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-notifications-97b6c79c18b48073.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      378 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/soft-reboot-poweroff-9fdb0a4306dd668d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       68 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/irmc-boot-interface-8c2e26affd1ebfc4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      538 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1694645-57289200e35bd883.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1236 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/port-physical-network-a7009dc514353796.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      514 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/added-redfish-driver-00ff5e3f7e9d6ee8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/server_profile_template_uri-c79e4f15cc20a1cf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      686 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-agent-erase-fallback-b07613a7042fe236.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      323 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/story-2002637-4825d60b096e475b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      171 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-driver-periodic-task-f5e513b06b601ce4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      187 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-id-and-uuid-filtering-to-sqalchemy-api.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       54 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1611556-92cbfde5ee7f44d6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1570283-6cdc62e4ef43cb02.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/agent-takeover-60f27cef21ebfb48.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      100 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/root-device-hints-rotational-c21f02130394e1d4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-driver-object-periodic-tasks-1357a1cd3589becf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      570 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-snmp-inspection-support-e68fd6d57cb33846.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/lookup-heartbeat-f9772521d12a0549.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      414 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-gmr-3c9278d5d785895f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      622 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-deprecated-dhcp-provider-methods-582742f3000be3c7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      217 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/no-downward-sql-migration-52279e875cd8b7a3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      104 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/validate-image-url-wnen-deploying-8820f4398ea9de9f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      948 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/deprecate-dhcp-update-mac-address-f12a4959432c8e20.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      174 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/node-credentials-cleaning-b1903f49ffeba029.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      188 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/make-terminal-session-timeout-configurable-b2365b7699b0f98b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/support-root-device-hints-with-operators-96cf34fa37b5b2e8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      265 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/deprecate-agent-passthru-67d1e2cf25b30a30.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      284 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/conf-debug-ipa-1d75e2283ca83395.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      183 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/boot-ipxe-inc-workaround-548e10d1d6616752.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      100 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipmi-cmd-for-ipmi-consoles-2e1104f22df3efcd.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      191 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-socat-console-ipmitool-ab4402ec976c5c96.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1058 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/configdrive-support-using-ceph-radosgw-8c6f7b8bede2077c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/change-updated-at-object-field-a74466f7c4541072.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/root-api-version-info-9dd6cadd3d3d4bbe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/improve-conductor-shutdown-42687d8b9dac4054.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      435 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/bug-1696296-a972c8d879b98940.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/disk-label-fix-7580de913835ff44.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      468 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-mitaka-ipa-iscsi.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      530 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/security_groups-b57a5d6c30c2fae4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      119 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipxe_timeout_parameter-03fc3c76c520fac2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      228 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/debug-no-api-tracebacks-a8a0caddc9676b06.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/neutron-port-timeout-cbd82e1d09c6a46c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      223 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/5.0-release-afb1fbbe595b6bc8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      300 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/inspector-enabled-f8a643f03e1e0360.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/nodes-classic-drivers-cannot-set-interfaces-620b37c4e5c88b80.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      370 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/snmp-driver-udp-transport-settings-67419be988fcff40.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      304 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/build_instance_info-c7e3f12426b48965.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      306 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/cleaning-retry-fix-89a5d0e65920a064.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      216 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/iscsi-whole-disk-cd464d589d029b01.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      869 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/multi-arch-deploy-bcf840107fc94bef.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      195 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ipa-ephemeral-partition-1f1e020727a49078.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2522 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/volume-connector-and-target-api-dd172f121ab3af8e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      734 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-agent-passthru-432b18e6c430cee6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      152 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-net-ifaces-rebuild-1cc03df5d37f38dd.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-agent-clean-up-9a25deb85bc53d9b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-ipv6-pxe-support-8fb51c355cc977c4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      662 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipxe-use-swift-5ccf490daab809cc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1124 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/resources-crud-notifications-70cba9f761da3afe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/radosgw-temp-url-b04aac50698b4461.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/messaging-log-level-5f870ea69db53d26.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      784 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-vif-attach-detach-support-99eca43eea6e5a30.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      408 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-fix-double-manage-provide-cycle-6ac8a427068f87fe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      330 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-fix-get_bios_config-vendor-passthru-causes-exception-1e1dbeeb3e924f29.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      205 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/apache-multiple-workers-11d4ba52c89a13e3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      392 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/flag_always_reboot-62468a7058b58823.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      763 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/new_capabilities-5241619c4b46a460.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-DEPRECATED-options-from-[agent]-7b6cce21b5f52022.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      457 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/adding-audit-middleware-b95f2a00baed9750.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       58 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oneview-timing-metrics-0b6c1b54e80eb683.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/emit-metrics-for-api-calls-69f18fd1b9d54b05.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipxe_retry_on_failure-e71fc6b3e9a5be3b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oob-power-off-7bbdf5947ed24bf8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      240 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/error-resilient-enabled_drivers-4e9c864ed6eaddd1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      241 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/snmp-hardware-type-ee3d471cf5c596f4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      876 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-choice-to-some-options-9fb327c48e6bfda1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      736 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/net-names-b8a36aa30659ce2f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ipxe-template-for-whole-disk-image-943da0311ca7aeb5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       96 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/clear-hung-iscsi-sessions-d3b55c4c65fa4c8b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-api-node-name-updates-f3813295472795be.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      781 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/resource-classes-1bf903547236a473.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-cleaning-spawn-error-60b60281f3be51c2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      393 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/deprecate-clustered-compute-manager-3dd68557446bcc5c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      475 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/multiple-workers-for-send-sensor-data-89d29c12da30ec54.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1086 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/implement-policy-in-code-cbb0216ef5f8224f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      380 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/no-ssh-drivers-6ee5ff4c3ecdd3fb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/validate-node-properties-73509ee40f409ca2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      597 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-db-deadlock-handling-6bc10076537f3727.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-iscsi-portal-port-option-bde3b386f44f2a90.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      401 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-boot-from-volume-for-iscsi-deploy-60bc0790ada62b26.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      149 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oneview-onetime-boot-64a68e135a45f5e2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      134 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ipmi-numeric-password-75e080aa8bdfb9a2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/inspection-logging-e1172f549ef80b04.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       75 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-periodic-interval-45f57ebad9aaa14e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       78 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/xenserver-ssh-driver-398084fe91ac56f1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      161 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1592335-7c5835868fe364ea.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      512 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1506657-3bcb4ef46623124d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/backfill_version_column_db_race_condition-713fa05832b93ca5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      263 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/removal-pre-allocation-for-oneview-09310a215b3aaf3c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oneview-node-free-for-ironic-61b05fee827664cb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      197 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/correct-api-version-check-conditional-for-nodename-439bebc02fb5493d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1008 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-bug-1675529-479357c217819420.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      324 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/inspector-session-179f83cbb0dc169b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      221 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1626453-e8df46aa5db6dd5a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-deprecated-ilo-clean-priority-erase-devices-bb3073da562ed41d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      312 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/dont-validate-local_link_connection-when-port-has-client-id-8e584586dc4fca50.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      270 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/update-live-port-ee3fa9b77f5d0cf7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       96 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/inspection-agent-drivers-cad619ec8a4874b1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      172 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipxe-uefi-f5be11c7b0606a84.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      224 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/pass_portgroup_settings_to_neutron-a6aec830a82c38a3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bmc_reset-warm-9396ac444cafd734.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/pxe-snmp-driver-supported-9c559c6182c6ec4b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      201 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/update-proliantutils-version-20ebcc22dc2df527.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-disk-identifier-overwrite-42b33a5a0f7742d8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-get-deploy-info-port.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/hctl-root-device-hints-0cab86673bc4a924.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      215 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-erase-device-priority-config-509661955a11c28e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/raise-bad-request-exception-on-validating-inspection-failure-57d7fd2999cf4ecf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-noop-net-vif-list-a3d8ecee29097662.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       65 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipv6-provision-67bd9c1dbcc48c97.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      811 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/active-node-creation-a41c9869c966c82b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      229 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-storage-interface-d4e64224804207fc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      169 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-agent_last_heartbeat-65a9fe02f20465c5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      604 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/idrac-hardware-type-54383960af3459d0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      517 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-raid-interface-f4c02b1c4fb37e2d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      898 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add_portgroup_support-7d5c6663bb00684a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      186 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-vif-detach-fca221f1a1c0e9fa.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-license-activate-manual-clean-step-84d335998d708b49.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4098 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/multitenant-networking-0a13c4aba252573e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      237 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-pxe-support-for-petitboot-50d1fe4e7da4bfba.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      184 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/node-deletion-update-resources-53862e48ab658f77.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      105 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/node-name-remove-720aa8007f2f8b75.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      220 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/agent-api-bf9f18d8d38075e4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      273 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/notimplementederror-misspell-276a181afd652cf6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      125 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/deny-too-long-chassis-description-0690d6f67ed002d5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      187 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/update-irmc-set-boot-device-fd50d9dce42aaa89.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      131 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-sync-power-state-last-error-65fa42bad8e38c3b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      807 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/collect-deployment-logs-2ec1634847c3f6a5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1125 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-most-unsupported-049f3401c2554a3c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      412 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/adopt-oslo-config-generator-15afd2e7c2f008b4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      230 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ilo-drivers-log-message-c3c64c1ca0a0bca8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/duplicated-driver-entry-775370ad84736206.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/check-for-whole-disk-image-uefi-3bf2146588de2423.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       99 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/allow-set-interface-to-node-in-available-bd6f695620c2d77f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      350 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/uefi-grub2-by-default-6b797a9e690d2dd5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      177 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-chassis_uuid-removal-possibility-8b06341a91f7c676.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ilo-firmware-update-swift-path-with-pseudo-folder-0660345510ec0bb4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      439 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/reboot-do-not-power-off-if-already-1452256167d40009.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       81 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/agent_partition_image-48a03700f41a3980.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/dynamic-allocation-spt-has-physical-mac-8967a1d926ed9301.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       73 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/name-root-device-hints-a1484ea01e399065.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      268 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/proliantutils_version_update-b6e5ff0e496215a5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      454 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-support-for-no-poweroff-on-failure-86e43b3e39043990.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       94 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/catch-third-party-driver-validate-exceptions-94ed2a91c50d2d8e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      134 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-oneview-driver-96088bf470b16c34.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      394 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/dbsync-online_data_migration-edcf0b1cc3667582.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      215 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/clean-nodes-stuck-in-cleaning-on-startup-443823ea4f937965.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-clustered-compute-manager-6b45ed3803be53d1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3429 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/dynamic-driver-list-show-apis-235e9fca26fc580d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      113 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-fix-prepare-cleaning-d74ba45135d84531.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      523 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-node-resource-class-c31e26df4196293e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      266 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/pxe-takeover-d8f14bcb60e5b121.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/raid-to-support-jbod-568f88207b9216e2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/mask-ssh-creds-54ab7b2656578d2e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       98 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/wwn-extension-root-device-hints-de40ca1444ba4888.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      517 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-inconsistent-default-boot-mode-ef5a7c56372f89f1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/clear-node-target-power-state-de1f25be46d3e6d7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      126 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-policy-checkers-1a08203e3c2cf859.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      723 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/futurist-e9c55699f479f97a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      409 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-dir-permissions-bc56e83a651bbdb0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      277 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/validate-ilo-certificates-3ab98bb8cfad7d60.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/allow-to-attach-vif-to-active-node-55963be2ec269043.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      587 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-hardware-type-48fd1c8bccd70659.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      110 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1607527-75885e145db62d69.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1146 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-agent-proxy-support-790e629634ca2eb7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      351 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/irmc-boot-from-volume-4bc5d20a0a780669.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      119 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-secure-boot-suport-irmc-2c1f09271f96424d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/irmc-add-clean-step-reset-bios-config-a8bed625670b7fdf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1648387-92db52cbe007fabd.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      703 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/refactor-ironic-lib-22939896d8d46a77.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-mac-address-48060f9e2847a38c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      237 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-ipminative-driver-3367d25bbcc41fdc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1426 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1702158-79bf57bd4d8087b6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      223 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/pass-metrics-config-to-agent-on-lookup-6db9ae187c4e8151.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      348 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/configure-notifications-72824356e7d8832a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      467 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/adoption-feature-update-d2160954a2c36b0a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      490 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/glance-keystone-dd30b884f07f83fb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      677 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-cve-2016-4985-b62abae577025365.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      250 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/config-drive-support-for-whole-disk-images-in-iscsi-deploy-0193c5222a7cd129.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      447 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/swift-endpoint-override-4151d2fbb159950d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      339 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/non-persistent-boot-5e3a0cd78e9dc91b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      298 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-inspection-interface-b0abbad98fec1c2e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       80 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1672457-563d5354b41b060e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      228 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/pass-region-to-swiftclient-c8c8bf1020f62ebc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      243 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-deprecated-deploy-erase-devices-iterations-55680ab95cbce3e9.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      138 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-oneview-periodics-0f535fe7a0ad83cd.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/release-4.3.0-cc531ab7190f8a00.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      359 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/bug-1745630-d28c8de54cebd329.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      448 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1548086-ed88646061b88faf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      177 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-pxe-http-5a05c54f57747bfe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      200 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oneview-agent-mixin-removal-b7277e8f20df5ef2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1150 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-dynamic-allocation-feature-2fd6b4df7943f178.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-updating-node-driver-to-classic-16b0d5ba47e74d10.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      382 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-port-advanced-net-fields-55465091f019d962.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      138 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-url-collisions-43abfc8364ca34e7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      269 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-list-unfinished-jobs-10400419b6bc3c6e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      406 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-do-not-power-off-non-deploying-nodes-0a3aed7c8ea3940a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-keystone-parameters-cdb93576d7e7885b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      336 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-deprecated-build-instance-info-for-deploy-2fe165fc018010e4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      301 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/check-dynamic-allocation-enabled-e94f3b8963b114d0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2441 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/keystone-auth-3155762c524e44df.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      360 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/pike-901-release-c570884b8b2d8baf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      207 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/manual-clean-4cc2437be1aea69a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      508 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oneview-hardware-type-69bbb79da434871f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      354 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/create-port-on-conductor-b921738b4b2a5def.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      681 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oslopolicy-scripts-bdcaeaf7dd9ce2ac.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/oneview-inspection-interface-c2d6902bbeca0501.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      279 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/use-dhcp-option-numbers-8b0b0efae912ff5f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      293 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipminative-bootdev-uefi-954a0dd825bcef97.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      300 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-fix-oob-cleaning-b4b717895e243c9b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       99 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ipmitool-console-empty-password-a8edc5e2a1a7daf6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      694 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-migrate-to-dracclient-2bd8a6d1dd3fdc69.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipxe-dhcp-b799bc326cd2529a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      604 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/notify-node-storage-interface-7fd07ee7ee71cd22.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2056 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/pike-prelude-815f73ba4ad59f97.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      502 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/wipe-disk-before-deployment-0a8b9cede4a659e9.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      803 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-deprecated-dhcp-provider-method-89926a8f0f4793a4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipmitool-bootdev-persistent-uefi-b1181a3c82343c8f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      640 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/create-on-conductor-c1c52a1f022c4048.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-error-check-ipmitool-reboot-ca7823202c5ab71d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       89 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/opentack-baremetal-request-id-daa72b785eaaaa8d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      137 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/drac-missing-lookup-3ad98e918e1a852a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      227 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/always-return-chassis-uuid-4eecbc8da2170cb1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       85 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/list-nodes-by-driver-a1ab9f2b73f652f8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      262 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/kill-old-ramdisk-6fa7a16269ff11b0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       60 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ipxe-and-uefi-7722bd5db71df02c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      388 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/no-more-legacy-auth-eeb32f907d0ab5de.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      280 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-port-internal-info-b7e02889416570f7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/get-supported-boot-devices-manadatory-task-0462fc072d6ea517.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      516 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/resource-class-change-563797d5a3c35683.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      164 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-discoverd-group-03eaf75e9f94d7be.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      200 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/cleanup-provision-ports-before-retry-ec3c89c193766d70.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      384 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/default_boot_option-f22c01f976bc2de7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      165 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/no-instance-uuid-workaround-fc458deb168c7a8b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-ssl-support-4547801eedba5942.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      229 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add_standalone_ports_supported_field-4c59702a052acf38.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      138 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/iscsi-inband-cleaning-bff87aac16e5d488.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       56 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/bug-1611555-de1ec64ba46982ec.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      119 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-ipxe-macro-4ae8bc4fe82e8f19.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/add-tooz-dep-85c56c74733a222d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      772 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-agent-passthru-complete-a6b2df65b95889d5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      298 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/deprecate-elilo-2beca4800f475426.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      247 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/sort_key_allowed_field-091f8eeedd0a2ace.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      238 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-automated-cleaning-fails-14ee438de3dd8690.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      149 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-manage-tftp-0c2f4f417b92b1ee.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      173 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/Add-port-option-support-to-ipmitool-e125d07fe13c53e7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      181 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-baremetal-admin-user-not-neutron-admin-f163df90ab520dad.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      183 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/rolling-upgrades-ccad5159ca3cedbe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      199 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/vendor-passthru-shared-lock-6a9e32952ee6c2fe.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      206 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/deprecate-support-for-glance-v1-8b194e6b20cbfebb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      243 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/socat-address-conf-5cf043fabb10bd76.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      434 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/change-ramdisk-log-filename-142b10d0b02a5ca6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      975 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-cisco-ucs-hardware-types-ee597ff0416f158f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      228 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-exception-message-92100debeb40d4c7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-neutron-client-workarounds-996c59623684929b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/hexraw-support-removed-8e8fa07595a629f4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      346 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/agent-can-request-reboot-6238e13e2e898f68.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       67 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-boot-interface-92831b78c5614733.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/stop-console-during-unprovision-a29d8facb3f03be5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      814 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/pike-upgrade-fix-85091d0320ed273a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      576 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/idrac-uefi-boot-mode-86f4694b4247a1ca.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-firmware-update-manual-clean-step-e6763dc6dc0d441b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      117 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-boot-from-volume-support-9f64208f083d0691.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/add-agent-iboot-0a4b5471c6ace461.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      431 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/check_protocol_for_ironic_api-32f35c93a140d3ae.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/update-proliantutils-version-54c0cd5c5d3c01dc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fail-when-vif-port-id-is-missing-7640669f9d9e705d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/reusing-oneview-client-6a3936fb8f113c10.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      385 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-socat-command-afc840284446870a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      577 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/amt-driver-wake-up-0880ed85476968be.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/adopt-ironic-context-5e75540dc2b2f009.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      222 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-iscsi-deploy-ipa-mitaka-c0efa0d5c31933b6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      214 2018-12-20 16:24:00.000000 ironic-9.1.6/releasenotes/notes/bfv-pxe-boot-3375d331ee2f04f2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-fix-inspection-b169ad0a22aea2ff.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      280 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/update-python-scciclient-required-version-71398d5d5e1c0bf8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1263 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ocata-summary-a70f995cb3b18e18.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      281 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/reserved-node-names-67a08012ed1131ae.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/irmc-oob-inspection-6d072c60f6c88ecb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      205 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/node-save-internal-info-c5cc8f56f1d0dab0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      335 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-ssh-power-port-delay-7ae6e5eb893439cd.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      267 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/remove-deprecated-option-names-6d5d53cc70dd2d49.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-agent-ilo-temp-image-cleanup-711429d0e67807ae.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      161 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/dhcp-provider-clean-dhcp-9352717903d6047e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      525 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-rpc-exceptions-12c70eb6ba177e39.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      306 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/portgroup-crud-notifications-91204635528972b2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      804 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/node-storage-interface-api-1d6e217303bd53ff.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      179 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/disk-label-capability-d36d126e0ad36dca.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      175 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-oneview-deploy-return-values-ab2ec6ae568d95a5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ssh-console-58721af6830f8892.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      476 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/ilo-update-proliantutils-version-fd41a7c2a27be735.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      389 2018-12-20 16:23:54.000000 ironic-9.1.6/releasenotes/notes/fix-virtualbox-localboot-not-working-558a3dec72b5116b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3375 2018-12-20 16:24:00.000000 ironic-9.1.6/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/api-ref/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4063 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-chassis.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7752 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-drivers.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1602 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-vifs.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2341 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-portgroups.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7611 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3273 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-volume.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6037 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-portgroups.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2064 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-versions.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11009 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-node-management.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2603 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-portgroups-ports.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    32644 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/parameters.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13939 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9823 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-volume.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7385 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-ports.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2572 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-ports.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2485 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-node-passthru.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      805 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2788 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-driver-passthru.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3145 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/baremetal-api-v1-misc.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/api-ref/source/samples/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      696 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-target-list-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      191 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-create-request-dynamic.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      465 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-portgroup-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      425 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/chassis-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      348 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/node-validate-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2474 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/node-create-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      122 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-target-update-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5843 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/nodes-list-details-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      589 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-target-create-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        3 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-inject-nmi.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      765 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/lookup-node-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-raid-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      418 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/port-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/port-update-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      126 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-create-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       27 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-manage-state.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      836 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/chassis-list-details-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       44 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-maintenance-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1887 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/api-v1-root-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1881 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/drivers-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      326 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-vendor-passthru-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-update-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      292 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-get-state-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      596 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      571 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-target-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       54 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-boot-device.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      356 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-update-driver-info-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       29 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-power-off.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       55 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-soft-power-off.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4656 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/drivers-list-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-target-create-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      601 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/api-root-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       48 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-get-supported-boot-devices-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      465 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       40 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/chassis-create-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       87 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-update-driver.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1058 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/nodes-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      736 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/chassis-update-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      885 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/port-list-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2697 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/node-update-driver-info-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-update-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2561 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/node-show-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      554 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-connector-create-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      129 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-connector-update-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      705 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/chassis-show-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      418 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-port-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      619 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-target-update-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       83 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-vif-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      108 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/chassis-update-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      555 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-volume-connector-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-connector-create-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      584 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-connector-update-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      726 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-volume-target-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      166 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-create-request-classic.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      786 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/port-update-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1065 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-list-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      102 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-active-state.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      656 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-connector-list-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      907 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-create-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      915 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-port-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      756 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/port-create-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      854 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-volume-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      686 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-volume-connector-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      341 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/port-create-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1095 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-portgroup-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2431 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/driver-property-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      418 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-port-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      571 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-volume-target-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      555 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/volume-connector-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      217 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-clean-state.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       50 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-get-boot-device-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      915 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/portgroup-port-detail-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       53 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-vif-attach-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1593 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/driver-logical-disk-properties-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1465 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/source/samples/driver-get-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       28 2018-12-20 16:23:54.000000 ironic-9.1.6/api-ref/source/samples/node-set-available-state.json
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    10696 2018-12-20 16:24:00.000000 ironic-9.1.6/api-ref/regenerate-samples.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24349 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      607 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5315 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/common/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1421 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/common/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/common/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4739 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/common/waiters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/services/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9344 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/v1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/v1/json/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/v1/json/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23377 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/services/baremetal/v1/json/baremetal_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1599 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8863 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_nodestates.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2123 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_drivers.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14778 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_ports.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18808 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_ports_negative.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3278 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_portgroups.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3431 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_chassis.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9093 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_volume_target.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13094 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      993 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/api_microversion_fixture.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9593 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_volume_connector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17215 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_nodes.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1731 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_api_discovery.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8134 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/baremetal_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/ironic_standalone/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/ironic_standalone/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5228 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/ironic_standalone/test_basic_ops.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6027 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/test_baremetal_basic_ops.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5786 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/test_baremetal_multitenancy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6125 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/test_baremetal_boot_from_volume.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13089 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/tests/scenario/baremetal_standalone_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1909 2018-12-20 16:24:00.000000 ironic-9.1.6/ironic_tempest_plugin/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2018-12-20 16:25:57.000000 ironic-9.1.6/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/tools/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4634 2018-12-20 16:23:54.000000 ironic-9.1.6/tools/states_to_dot.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      477 2018-12-20 16:23:54.000000 ironic-9.1.6/tools/flake8wrap.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:23:54.000000 ironic-9.1.6/tools/__init__.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1068 2018-12-20 16:24:00.000000 ironic-9.1.6/tools/run_bashate.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1506 2018-12-20 16:24:00.000000 ironic-9.1.6/tools/check-releasenotes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/tools/config/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      586 2018-12-20 16:24:00.000000 ironic-9.1.6/tools/config/ironic-config-generator.conf
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      865 2018-12-20 16:24:00.000000 ironic-9.1.6/tools/config/check_uptodate.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1991 2018-12-20 16:23:54.000000 ironic-9.1.6/tools/test-setup.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-12-20 16:25:57.000000 ironic-9.1.6/tools/policy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       77 2018-12-20 16:23:54.000000 ironic-9.1.6/tools/policy/ironic-policy-generator.conf
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      218 2018-12-20 16:23:54.000000 ironic-9.1.6/tools/with_venv.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8085 2018-12-20 16:25:57.000000 ironic-9.1.6/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      986 2019-04-26 15:39:36.000000 ironic-9.1.7/Vagrantfile
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      330 2019-04-26 15:39:36.000000 ironic-9.1.7/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   183528 2019-04-26 15:41:43.000000 ironic-9.1.7/ChangeLog
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       17 2019-04-26 15:39:32.000000 ironic-9.1.7/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/etc/apache2/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1318 2019-04-26 15:39:36.000000 ironic-9.1.7/etc/apache2/ironic
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/etc/ironic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/etc/ironic/rootwrap.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      992 2019-04-26 15:39:32.000000 ironic-9.1.7/etc/ironic/rootwrap.d/ironic-lib.filters
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      312 2019-04-26 15:39:32.000000 ironic-9.1.7/etc/ironic/rootwrap.d/ironic-utils.filters
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      212 2019-04-26 15:39:32.000000 ironic-9.1.7/etc/ironic/rootwrap.d/ironic-images.filters
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   120564 2019-04-26 15:39:36.000000 ironic-9.1.7/etc/ironic/ironic.conf.sample
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2019-04-26 15:39:32.000000 ironic-9.1.7/etc/ironic/rootwrap.conf
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      739 2019-04-26 15:39:32.000000 ironic-9.1.7/etc/ironic/api_audit_map.conf.sample
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      113 2019-04-26 15:39:36.000000 ironic-9.1.7/etc/ironic/policy.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4286 2019-04-26 15:39:36.000000 ironic-9.1.7/etc/ironic/policy.json.sample
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5565 2019-04-26 15:39:36.000000 ironic-9.1.7/vagrant.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1353 2019-04-26 15:39:36.000000 ironic-9.1.7/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      148 2019-04-26 15:39:32.000000 ironic-9.1.7/.mailmap
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      591 2019-04-26 15:39:36.000000 ironic-9.1.7/driver-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/contributor/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2906 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/contributor/webapi.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3747 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/ironic-boot-from-volume.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4255 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/drivers.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6672 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/contributor/notifications.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3087 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    29780 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/dev-quickstart.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12232 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/code-contribution-guide.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4962 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/releasing.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4825 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/faq.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4779 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/architecture.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1038 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/states.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1452 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/contributor/governance.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3920 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/osprofiler-support.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1759 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/contributor/third-party-ci.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5606 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/vendor-passthru.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8892 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/webapi-version-history.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4153 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/contributor/ironic-multitenant-networking.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/cli/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/cli/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6220 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/cli/ironic-dbsync.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2385 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/images/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77412 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/images/deployment_steps.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38085 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/images/logical_architecture.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    58011 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/images/sample_trace.svg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    84269 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/images/sample_trace_details.svg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25598 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/images/states.svg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    49070 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/images/conceptual_architecture.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38252 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/images/deployment_architecture_2.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/admin/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1730 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2575 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/radosgw.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25167 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/notifications.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12481 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/cleaning.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11184 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/upgrade-to-hardware-types.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6483 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/multitenancy.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1175 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2845 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/boot-from-volume.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8149 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/adoption.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18553 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/upgrade-guide.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/admin/drivers/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3455 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/redfish.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3345 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/cimc.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18464 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/irmc.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      962 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/pxe.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15538 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/oneview.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6011 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/snmp.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5718 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/ipa.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77574 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/ilo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3307 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/ucs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6531 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/drivers/ipmitool.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19350 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/report.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13274 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/troubleshooting.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1968 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/admin/gmr.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4273 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/admin/metrics.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5458 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/portgroups.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3746 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/admin/api-audit-support.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5412 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/security.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13401 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/raid.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7195 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/console.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4394 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/admin/inspection.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4390 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/configuration/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      236 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/configuration/policy.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      440 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/configuration/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      590 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/configuration/sample-config.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      288 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/configuration/config.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      406 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/configuration/sample-policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/install/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3992 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-identity.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13414 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-pxe.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3695 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-networking.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2929 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/deploy-ramdisk.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3090 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/enabling-https.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      662 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1141 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/install-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7632 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/standalone.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1098 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-cleaning.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4838 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/install/configure-glance-images.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3591 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/get_started.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7557 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/troubleshooting.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6549 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-tenant-networks.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      384 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/advanced.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6129 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configdrive.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/install/configure-iscsi.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/install/next-steps.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      376 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/install/configure-integration.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6722 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-compute.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    31467 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/enrollment.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/install/include/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      802 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/notifications.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      657 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/common-configure.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2543 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/disk-label.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1154 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/common-prerequisites.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2899 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/trusted-boot.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2856 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/configure-ironic-api.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6153 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/configure-ironic-conductor.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1798 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/boot-mode.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/console.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2103 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/local-boot-partition-images.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3846 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/kernel-boot-parameters.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3585 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/root-device-hints.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2077 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/include/configure-ironic-api-mod_wsgi.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1174 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/install-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10111 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/conf.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3116 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-glance-swift.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      197 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/install/setup-drivers.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      743 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/install-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3707 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-nova-flavors.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3182 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/configure-ipmi.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11598 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/install/enabling-drivers.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      355 2019-04-26 15:39:32.000000 ironic-9.1.7/doc/source/install/install.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/user/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14634 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/doc/source/images_src/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   158538 2019-04-26 15:39:36.000000 ironic-9.1.7/doc/source/images_src/deployment_steps.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2019-04-26 15:41:44.000000 ironic-9.1.7/PKG-INFO
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      988 2019-04-26 15:39:36.000000 ironic-9.1.7/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/tools/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/tools/__init__.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1068 2019-04-26 15:39:36.000000 ironic-9.1.7/tools/run_bashate.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/tools/config/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      586 2019-04-26 15:39:36.000000 ironic-9.1.7/tools/config/ironic-config-generator.conf
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      865 2019-04-26 15:39:36.000000 ironic-9.1.7/tools/config/check_uptodate.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1506 2019-04-26 15:39:36.000000 ironic-9.1.7/tools/check-releasenotes.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      477 2019-04-26 15:39:32.000000 ironic-9.1.7/tools/flake8wrap.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4634 2019-04-26 15:39:32.000000 ironic-9.1.7/tools/states_to_dot.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      218 2019-04-26 15:39:32.000000 ironic-9.1.7/tools/with_venv.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/tools/policy/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       77 2019-04-26 15:39:32.000000 ironic-9.1.7/tools/policy/ironic-policy-generator.conf
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1991 2019-04-26 15:39:32.000000 ironic-9.1.7/tools/test-setup.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56220 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6693 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic.egg-info/entry_points.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-inspector/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7621 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-inspector/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-inspector/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5948 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6045 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9077 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6080 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6063 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/ironic-dsvm-standalone/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3801 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/ironic-dsvm-standalone/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/ironic-dsvm-standalone/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-bfv/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6589 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-bfv/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-bfv/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8122 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6544 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6929 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:36.000000 ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic/post.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      287 2019-04-26 15:39:36.000000 ironic-9.1.7/.testr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/api-ref/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)    10696 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/regenerate-samples.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/api-ref/source/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4063 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-chassis.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      805 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2485 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-node-passthru.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9823 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-volume.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2788 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-driver-passthru.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2572 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-ports.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2064 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-versions.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7385 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-ports.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3145 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-misc.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/api-ref/source/samples/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      425 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/chassis-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      129 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-connector-update-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      326 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-vendor-passthru-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       40 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/chassis-create-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      555 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-connector-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       28 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-available-state.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      696 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-target-list-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      589 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-target-create-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1065 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-list-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      418 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-port-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      786 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/port-update-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      596 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      756 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/port-create-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      418 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-port-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      356 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-update-driver-info-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-connector-create-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/port-update-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      292 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-get-state-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       87 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-update-driver.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4656 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/drivers-list-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      571 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-volume-target-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       27 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-manage-state.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       29 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-power-off.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      348 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-validate-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      765 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/lookup-node-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      915 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/portgroup-port-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      465 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      686 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-volume-connector-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1465 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/driver-get-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1058 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/nodes-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      726 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-volume-target-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-update-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      854 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-volume-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      555 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-volume-connector-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      122 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-target-update-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      166 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-create-request-classic.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-update-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      907 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-create-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2697 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-update-driver-info-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      619 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-target-update-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      554 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-connector-create-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2431 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/driver-property-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       55 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-soft-power-off.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       54 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-boot-device.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2561 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-show-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      418 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/port-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       50 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-get-boot-device-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1095 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-portgroup-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      915 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-port-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      584 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-connector-update-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      885 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/port-list-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-target-create-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       83 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-vif-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5843 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/nodes-list-details-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      571 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-target-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1881 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/drivers-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      836 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/chassis-list-details-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      736 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/chassis-update-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      191 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-create-request-dynamic.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       44 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-maintenance-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      102 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-active-state.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-raid-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      656 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/volume-connector-list-detail-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1593 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/driver-logical-disk-properties-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      705 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/chassis-show-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        3 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-inject-nmi.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      601 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/api-root-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       48 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-get-supported-boot-devices-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      465 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-portgroup-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      341 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/port-create-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2474 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/samples/node-create-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      108 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/chassis-update-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1887 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/api-v1-root-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      126 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/portgroup-create-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       53 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-vif-attach-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      217 2019-04-26 15:39:32.000000 ironic-9.1.7/api-ref/source/samples/node-set-clean-state.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    32644 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/parameters.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11009 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-node-management.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13939 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7611 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/conf.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6037 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-portgroups.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7752 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-drivers.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1602 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-vifs.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3273 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-volume.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2603 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-portgroups-ports.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2341 2019-04-26 15:39:36.000000 ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-portgroups.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16850 2019-04-26 15:41:43.000000 ironic-9.1.7/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/releasenotes/source/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      387 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/source/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8375 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/source/liberty.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      107 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/source/unreleased.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      181 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/source/ocata.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/source/newton.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/releasenotes/source/_templates/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/source/_templates/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/source/mitaka.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/releasenotes/source/_static/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/source/_static/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9480 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/releasenotes/notes/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      183 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/boot-ipxe-inc-workaround-548e10d1d6616752.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      686 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-agent-erase-fallback-b07613a7042fe236.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      217 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/no-downward-sql-migration-52279e875cd8b7a3.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      117 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-boot-from-volume-support-9f64208f083d0691.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1032 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/mask-configdrive-contents-77fc557d6bc63b2b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      360 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/pike-901-release-c570884b8b2d8baf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2522 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/volume-connector-and-target-api-dd172f121ab3af8e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipxe-dhcp-b799bc326cd2529a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-firmware-update-manual-clean-step-e6763dc6dc0d441b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      378 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/soft-reboot-poweroff-9fdb0a4306dd668d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      277 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/validate-ilo-certificates-3ab98bb8cfad7d60.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ssh-console-58721af6830f8892.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      216 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/iscsi-whole-disk-cd464d589d029b01.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-fix-inspection-b169ad0a22aea2ff.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      183 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/rolling-upgrades-ccad5159ca3cedbe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/scciclient-0.4.0-6f01c0f0a5c39062.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      137 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-missing-lookup-3ad98e918e1a852a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      255 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/snmp-reboot-delay-d18ee3f6c6fc0998.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/dynamic-allocation-spt-has-physical-mac-8967a1d926ed9301.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      250 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/config-drive-support-for-whole-disk-images-in-iscsi-deploy-0193c5222a7cd129.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      162 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-clean-nodes-38cfa633ca518f99.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      218 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-instance-master-path-config-fa524c907a7888e5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      119 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-secure-boot-suport-irmc-2c1f09271f96424d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      457 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/adding-audit-middleware-b95f2a00baed9750.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      300 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/inspector-enabled-f8a643f03e1e0360.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      336 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-deprecated-build-instance-info-for-deploy-2fe165fc018010e4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      394 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/dbsync-online_data_migration-edcf0b1cc3667582.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-noop-net-vif-list-a3d8ecee29097662.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/change-updated-at-object-field-a74466f7c4541072.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-mac-address-48060f9e2847a38c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      200 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oneview-agent-mixin-removal-b7277e8f20df5ef2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      228 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/debug-no-api-tracebacks-a8a0caddc9676b06.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipmitool-bootdev-persistent-uefi-b1181a3c82343c8f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       98 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/wwn-extension-root-device-hints-de40ca1444ba4888.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      280 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-port-internal-info-b7e02889416570f7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/inspection-logging-e1172f549ef80b04.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      105 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/node-name-remove-720aa8007f2f8b75.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/pxe-snmp-driver-supported-9c559c6182c6ec4b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      229 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-storage-interface-d4e64224804207fc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      200 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/cleanup-provision-ports-before-retry-ec3c89c193766d70.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oneview-inspection-interface-c2d6902bbeca0501.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1008 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-bug-1675529-479357c217819420.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      165 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/no-instance-uuid-workaround-fc458deb168c7a8b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bmc_reset-warm-9396ac444cafd734.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac_host-deprecated-b181149246eecb47.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      149 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-manage-tftp-0c2f4f417b92b1ee.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       96 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/clear-hung-iscsi-sessions-d3b55c4c65fa4c8b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      186 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-vif-detach-fca221f1a1c0e9fa.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      149 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oneview-onetime-boot-64a68e135a45f5e2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      359 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/bug-1745630-d28c8de54cebd329.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      265 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/deprecate-agent-passthru-67d1e2cf25b30a30.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1214 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/rely-on-standalone-ports-supported-8153e1135787828b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oneview-node-free-for-ironic-61b05fee827664cb.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      125 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/deny-too-long-chassis-description-0690d6f67ed002d5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      354 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/create-port-on-conductor-b921738b4b2a5def.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-disk-identifier-overwrite-42b33a5a0f7742d8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      284 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/inject-nmi-dacd692b1f259a30.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      502 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/wipe-disk-before-deployment-0a8b9cede4a659e9.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-cleaning-spawn-error-60b60281f3be51c2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      221 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1626453-e8df46aa5db6dd5a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      723 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/futurist-e9c55699f479f97a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      348 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/configure-notifications-72824356e7d8832a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      206 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/deprecate-support-for-glance-v1-8b194e6b20cbfebb.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       67 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-boot-interface-92831b78c5614733.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-agent-iboot-0a4b5471c6ace461.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      408 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-fix-double-manage-provide-cycle-6ac8a427068f87fe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      119 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipxe_timeout_parameter-03fc3c76c520fac2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      267 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-deprecated-option-names-6d5d53cc70dd2d49.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      223 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/pass-metrics-config-to-agent-on-lookup-6db9ae187c4e8151.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      869 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/multi-arch-deploy-bcf840107fc94bef.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      293 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipminative-bootdev-uefi-954a0dd825bcef97.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      351 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/irmc-boot-from-volume-4bc5d20a0a780669.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/support-root-device-hints-with-operators-96cf34fa37b5b2e8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1570283-6cdc62e4ef43cb02.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ilo-firmware-update-swift-path-with-pseudo-folder-0660345510ec0bb4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      184 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/node-deletion-update-resources-53862e48ab658f77.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      639 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/erase-devices-metadata-config-f39b6ca415a87757.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-api-access-logs-68b9ca4f411f339c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      177 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-chassis_uuid-removal-possibility-8b06341a91f7c676.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oob-power-off-7bbdf5947ed24bf8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      161 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1592335-7c5835868fe364ea.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       80 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1672457-563d5354b41b060e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      587 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-hardware-type-48fd1c8bccd70659.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      113 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-fix-prepare-cleaning-d74ba45135d84531.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      177 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-pxe-http-5a05c54f57747bfe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-DEPRECATED-options-from-[agent]-7b6cce21b5f52022.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       81 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/agent_partition_image-48a03700f41a3980.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      392 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/flag_always_reboot-62468a7058b58823.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      694 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-migrate-to-dracclient-2bd8a6d1dd3fdc69.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       85 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/list-nodes-by-driver-a1ab9f2b73f652f8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      576 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/idrac-uefi-boot-mode-86f4694b4247a1ca.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      134 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-oneview-driver-96088bf470b16c34.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      384 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/default_boot_option-f22c01f976bc2de7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      272 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-cpu-count-8904a4e1a24456f4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      284 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/conf-debug-ipa-1d75e2283ca83395.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      279 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/use-dhcp-option-numbers-8b0b0efae912ff5f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/raise-bad-request-exception-on-validating-inspection-failure-57d7fd2999cf4ecf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      134 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ipmi-numeric-password-75e080aa8bdfb9a2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      205 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/apache-multiple-workers-11d4ba52c89a13e3.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      412 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/adopt-oslo-config-generator-15afd2e7c2f008b4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      476 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-update-proliantutils-version-fd41a7c2a27be735.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      570 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-snmp-inspection-support-e68fd6d57cb33846.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      681 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oslopolicy-scripts-bdcaeaf7dd9ce2ac.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipxe_retry_on_failure-e71fc6b3e9a5be3b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      205 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/node-save-internal-info-c5cc8f56f1d0dab0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       99 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1579635-cffd990b51bcb5ab.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-iscsi-portal-port-option-bde3b386f44f2a90.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/emit-metrics-for-api-calls-69f18fd1b9d54b05.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      604 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/idrac-hardware-type-54383960af3459d0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       79 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/allow-to-attach-vif-to-active-node-55963be2ec269043.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-clustered-compute-manager-6b45ed3803be53d1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      523 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-node-resource-class-c31e26df4196293e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      138 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-oneview-periodics-0f535fe7a0ad83cd.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/clear-node-target-power-state-de1f25be46d3e6d7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      388 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/no-more-legacy-auth-eeb32f907d0ab5de.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/release-4.3.0-cc531ab7190f8a00.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       65 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipv6-provision-67bd9c1dbcc48c97.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      512 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1506657-3bcb4ef46623124d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      172 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipxe-uefi-f5be11c7b0606a84.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      811 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/active-node-creation-a41c9869c966c82b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add_infiniband_support-f497767f77277a1a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      159 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/clear-target-stable-states-4545602d7aed9898.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       76 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/snmp-outlet-validate-ffbe8e6687172efc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       96 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/inspection-agent-drivers-cad619ec8a4874b1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      238 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-automated-cleaning-fails-14ee438de3dd8690.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      330 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-fix-get_bios_config-vendor-passthru-causes-exception-1e1dbeeb3e924f29.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      298 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/deprecate-elilo-2beca4800f475426.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/hctl-root-device-hints-0cab86673bc4a924.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      454 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-support-for-no-poweroff-on-failure-86e43b3e39043990.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      301 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/check-dynamic-allocation-enabled-e94f3b8963b114d0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      191 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-socat-console-ipmitool-ab4402ec976c5c96.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      187 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/update-irmc-set-boot-device-fd50d9dce42aaa89.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/agent-takeover-60f27cef21ebfb48.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       89 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/opentack-baremetal-request-id-daa72b785eaaaa8d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      323 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/story-2002637-4825d60b096e475b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      201 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/logging-keystoneauth-9db7e56c54c2473d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       94 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/catch-third-party-driver-validate-exceptions-94ed2a91c50d2d8e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      772 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-agent-passthru-complete-a6b2df65b95889d5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-agent-ilo-temp-image-cleanup-711429d0e67807ae.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       99 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ipmitool-console-empty-password-a8edc5e2a1a7daf6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      459 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-verbose-option-261f1b9e24212ee2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/backfill_version_column_db_race_condition-713fa05832b93ca5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/check-for-whole-disk-image-uefi-3bf2146588de2423.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      747 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/enable-osprofiler-support-e3839b0fa90d3831.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      525 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-rpc-exceptions-12c70eb6ba177e39.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      129 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/agent-wol-driver-4116f64907d0db9c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      679 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/newton-driver-deprecations-e40369be37203057.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       68 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/irmc-boot-interface-8c2e26affd1ebfc4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      312 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/dont-validate-local_link_connection-when-port-has-client-id-8e584586dc4fca50.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      100 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/root-device-hints-rotational-c21f02130394e1d4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-error-check-ipmitool-reboot-ca7823202c5ab71d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      195 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ipa-ephemeral-partition-1f1e020727a49078.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       58 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oneview-timing-metrics-0b6c1b54e80eb683.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      465 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-boot-from-volume-for-iscsi-deploy-71c1f2905498c50d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      241 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/snmp-hardware-type-ee3d471cf5c596f4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      781 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/resource-classes-1bf903547236a473.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      803 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-deprecated-dhcp-provider-method-89926a8f0f4793a4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      266 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/pxe-takeover-d8f14bcb60e5b121.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       78 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/xenserver-ssh-driver-398084fe91ac56f1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      382 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-port-advanced-net-fields-55465091f019d962.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/radosgw-temp-url-b04aac50698b4461.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      339 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/non-persistent-boot-5e3a0cd78e9dc91b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      508 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/oneview-hardware-type-69bbb79da434871f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-get-deploy-info-port.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-deprecated-ilo-clean-priority-erase-devices-bb3073da562ed41d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      243 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-deprecated-deploy-erase-devices-iterations-55680ab95cbce3e9.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       60 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipxe-and-uefi-7722bd5db71df02c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      300 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-fix-oob-cleaning-b4b717895e243c9b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      327 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/glance-v2-83b04fec247cd22f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1150 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-dynamic-allocation-feature-2fd6b4df7943f178.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      514 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/added-redfish-driver-00ff5e3f7e9d6ee8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fail-when-vif-port-id-is-missing-7640669f9d9e705d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      271 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/stop-console-during-unprovision-a29d8facb3f03be5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      389 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-virtualbox-localboot-not-working-558a3dec72b5116b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      119 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ipxe-macro-4ae8bc4fe82e8f19.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/mask-ssh-creds-54ab7b2656578d2e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      414 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-gmr-3c9278d5d785895f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      237 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-ipminative-driver-3367d25bbcc41fdc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      375 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-clean-steps-not-running-0d065cb022bc0419.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1236 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/port-physical-network-a7009dc514353796.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2441 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/keystone-auth-3155762c524e44df.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/inspector-for-cisco-bffe1d1af7aec677.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/raid-to-support-jbod-568f88207b9216e2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3429 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/dynamic-driver-list-show-apis-235e9fca26fc580d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-ipv6-pxe-support-8fb51c355cc977c4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-driver-object-periodic-tasks-1357a1cd3589becf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      409 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-dir-permissions-bc56e83a651bbdb0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      138 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/iscsi-inband-cleaning-bff87aac16e5d488.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      597 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-db-deadlock-handling-6bc10076537f3727.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      181 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-baremetal-admin-user-not-neutron-admin-f163df90ab520dad.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/context-domain-id-name-deprecation-ae6e40718273be8d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/improve-conductor-shutdown-42687d8b9dac4054.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      110 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1607527-75885e145db62d69.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/reusing-oneview-client-6a3936fb8f113c10.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      380 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/no-ssh-drivers-6ee5ff4c3ecdd3fb.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      306 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/portgroup-crud-notifications-91204635528972b2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/hexraw-support-removed-8e8fa07595a629f4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      240 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/error-resilient-enabled_drivers-4e9c864ed6eaddd1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      138 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-url-collisions-43abfc8364ca34e7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/restart-console-on-conductor-startup-5cff6128c325b18e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      214 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/bfv-pxe-boot-3375d331ee2f04f2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      604 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/notify-node-storage-interface-7fd07ee7ee71cd22.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      538 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1694645-57289200e35bd883.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      975 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-cisco-ucs-hardware-types-ee597ff0416f158f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      876 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-choice-to-some-options-9fb327c48e6bfda1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      677 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-cve-2016-4985-b62abae577025365.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1125 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-most-unsupported-049f3401c2554a3c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      245 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-oneview-deallocate-server-8256e279af837e5d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      262 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-messaging-aliases-0a6ba1ed392b1fed.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      201 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/update-proliantutils-version-20ebcc22dc2df527.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      447 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/swift-endpoint-override-4151d2fbb159950d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/validate-port-info-before-using-it-e26135982d37c698.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      804 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/node-storage-interface-api-1d6e217303bd53ff.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/root-api-version-info-9dd6cadd3d3d4bbe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      237 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-pxe-support-for-petitboot-50d1fe4e7da4bfba.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1086 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/implement-policy-in-code-cbb0216ef5f8224f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      130 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/idrac-no-vendor-911904dd69457826.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      161 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/dhcp-provider-clean-dhcp-9352717903d6047e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-updating-node-driver-to-classic-16b0d5ba47e74d10.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      215 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/clean-nodes-stuck-in-cleaning-on-startup-443823ea4f937965.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      280 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/update-python-scciclient-required-version-71398d5d5e1c0bf8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      152 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-net-ifaces-rebuild-1cc03df5d37f38dd.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      734 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-agent-passthru-432b18e6c430cee6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      273 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/notimplementederror-misspell-276a181afd652cf6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      262 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/kill-old-ramdisk-6fa7a16269ff11b0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/server_profile_template_uri-c79e4f15cc20a1cf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      306 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/cleaning-retry-fix-89a5d0e65920a064.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      269 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-list-unfinished-jobs-10400419b6bc3c6e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      185 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/add-tooz-dep-85c56c74733a222d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1426 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1702158-79bf57bd4d8087b6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      475 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/multiple-workers-for-send-sensor-data-89d29c12da30ec54.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      174 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/node-credentials-cleaning-b1903f49ffeba029.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/disk-label-fix-7580de913835ff44.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1058 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/configdrive-support-using-ceph-radosgw-8c6f7b8bede2077c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      435 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/bug-1696296-a972c8d879b98940.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       97 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/adopt-ironic-context-5e75540dc2b2f009.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      490 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/glance-keystone-dd30b884f07f83fb.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      228 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/pass-region-to-swiftclient-c8c8bf1020f62ebc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      439 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/reboot-do-not-power-off-if-already-1452256167d40009.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      281 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/reserved-node-names-67a08012ed1131ae.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/get-supported-boot-devices-manadatory-task-0462fc072d6ea517.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      386 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/cleanwait_timeout_fail-4323ba7d4d4da3e6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      173 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/Add-port-option-support-to-ipmitool-e125d07fe13c53e7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      298 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-inspection-interface-b0abbad98fec1c2e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      222 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-iscsi-deploy-ipa-mitaka-c0efa0d5c31933b6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      346 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/agent-can-request-reboot-6238e13e2e898f68.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      401 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-boot-from-volume-for-iscsi-deploy-60bc0790ada62b26.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      662 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipxe-use-swift-5ccf490daab809cc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      703 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/refactor-ironic-lib-22939896d8d46a77.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-keystone-parameters-cdb93576d7e7885b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      153 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-agent-clean-up-9a25deb85bc53d9b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      268 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/proliantutils_version_update-b6e5ff0e496215a5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      577 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/amt-driver-wake-up-0880ed85476968be.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      207 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/manual-clean-4cc2437be1aea69a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      431 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/check_protocol_for_ironic_api-32f35c93a140d3ae.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      758 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/shred-final-overwrite-with-zeros-50b5ba5b19c0da27.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      434 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/lookup-ignore-malformed-macs-09e7e909f3a134a3.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      516 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/resource-class-change-563797d5a3c35683.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      763 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/new_capabilities-5241619c4b46a460.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      131 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-sync-power-state-last-error-65fa42bad8e38c3b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      948 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/deprecate-dhcp-update-mac-address-f12a4959432c8e20.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      304 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/build_instance_info-c7e3f12426b48965.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      126 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-policy-checkers-1a08203e3c2cf859.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1518374-decd73fd82c2eb94.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-ssl-support-4547801eedba5942.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      517 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/drac-raid-interface-f4c02b1c4fb37e2d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      230 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/disable-clean-step-reset-ilo-1869a6e08f39901c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       56 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1611555-de1ec64ba46982ec.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1146 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-agent-proxy-support-790e629634ca2eb7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       75 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-periodic-interval-45f57ebad9aaa14e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      640 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/create-on-conductor-c1c52a1f022c4048.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ipxe-template-for-whole-disk-image-943da0311ca7aeb5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      434 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/change-ramdisk-log-filename-142b10d0b02a5ca6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      100 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipmi-cmd-for-ipmi-consoles-2e1104f22df3efcd.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2056 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/pike-prelude-815f73ba4ad59f97.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      197 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/correct-api-version-check-conditional-for-nodename-439bebc02fb5493d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      229 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add_standalone_ports_supported_field-4c59702a052acf38.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      187 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-id-and-uuid-filtering-to-sqalchemy-api.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      270 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/update-live-port-ee3fa9b77f5d0cf7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      468 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-mitaka-ipa-iscsi.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      736 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/net-names-b8a36aa30659ce2f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      169 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-agent_last_heartbeat-65a9fe02f20465c5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      223 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/5.0-release-afb1fbbe595b6bc8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1648387-92db52cbe007fabd.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      228 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-exception-message-92100debeb40d4c7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-neutron-client-workarounds-996c59623684929b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       54 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1611556-92cbfde5ee7f44d6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      184 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/automated_clean_config-0170c95ae210f953.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      227 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/always-return-chassis-uuid-4eecbc8da2170cb1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4098 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/multitenant-networking-0a13c4aba252573e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      385 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-socat-command-afc840284446870a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1263 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ocata-summary-a70f995cb3b18e18.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       73 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/name-root-device-hints-a1484ea01e399065.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      370 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/snmp-driver-udp-transport-settings-67419be988fcff40.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      179 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/disk-label-capability-d36d126e0ad36dca.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      335 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-ssh-power-port-delay-7ae6e5eb893439cd.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      199 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/vendor-passthru-shared-lock-6a9e32952ee6c2fe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      230 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-ilo-drivers-log-message-c3c64c1ca0a0bca8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      402 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-notifications-97b6c79c18b48073.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/lookup-heartbeat-f9772521d12a0549.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      530 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/security_groups-b57a5d6c30c2fae4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      467 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/adoption-feature-update-d2160954a2c36b0a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       72 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/irmc-oob-inspection-6d072c60f6c88ecb.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      243 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/socat-address-conf-5cf043fabb10bd76.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1124 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/resources-crud-notifications-70cba9f761da3afe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/nodes-classic-drivers-cannot-set-interfaces-620b37c4e5c88b80.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      215 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-erase-device-priority-config-509661955a11c28e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/validate-node-properties-73509ee40f409ca2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      198 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/periodic-tasks-drivers-ae9cddab88b546c6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/conductor_early_import-fd29fa8b89089977.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      406 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-do-not-power-off-non-deploying-nodes-0a3aed7c8ea3940a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      263 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/removal-pre-allocation-for-oneview-09310a215b3aaf3c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      174 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/manual-abort-d3d8985a5de7376a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      324 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/inspector-session-179f83cbb0dc169b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/update-proliantutils-version-54c0cd5c5d3c01dc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/duplicated-driver-entry-775370ad84736206.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      137 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipmitool-vendor-3f0f52240ebbe489.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      814 2019-04-26 15:39:36.000000 ironic-9.1.7/releasenotes/notes/pike-upgrade-fix-85091d0320ed273a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      393 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/deprecate-clustered-compute-manager-3dd68557446bcc5c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      659 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ipa-streams-raw-images-1010327b0dad763c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/messaging-log-level-5f870ea69db53d26.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      164 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-discoverd-group-03eaf75e9f94d7be.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      247 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/sort_key_allowed_field-091f8eeedd0a2ace.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      350 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/uefi-grub2-by-default-6b797a9e690d2dd5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       99 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/allow-set-interface-to-node-in-available-bd6f695620c2d77f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      807 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/collect-deployment-logs-2ec1634847c3f6a5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/irmc-add-clean-step-reset-bios-config-a8bed625670b7fdf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      188 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/make-terminal-session-timeout-configurable-b2365b7699b0f98b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      220 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/agent-api-bf9f18d8d38075e4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      296 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-api-node-name-updates-f3813295472795be.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      104 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/validate-image-url-wnen-deploying-8820f4398ea9de9f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      175 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/fix-oneview-deploy-return-values-ab2ec6ae568d95a5.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      622 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-deprecated-dhcp-provider-methods-582742f3000be3c7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-license-activate-manual-clean-step-84d335998d708b49.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      448 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/bug-1548086-ed88646061b88faf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      171 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/remove-driver-periodic-task-f5e513b06b601ce4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      224 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/pass_portgroup_settings_to_neutron-a6aec830a82c38a3.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      784 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add-vif-attach-detach-support-99eca43eea6e5a30.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      532 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/no-root-device-as-kernel-param-5e5326acae7b77a4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/neutron-port-timeout-cbd82e1d09c6a46c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      898 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/add_portgroup_support-7d5c6663bb00684a.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      517 2019-04-26 15:39:32.000000 ironic-9.1.7/releasenotes/notes/ilo-inconsistent-default-boot-mode-ef5a7c56372f89f1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1745 2019-04-26 15:39:36.000000 ironic-9.1.7/requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-04-26 15:39:32.000000 ironic-9.1.7/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/cmd/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1076 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/cmd/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12834 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/cmd/dbsync.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1711 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/cmd/api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3146 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/cmd/conductor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/common/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3240 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/rpc_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2290 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/hash_ring.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      101 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/isolinux_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22713 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/images.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23783 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/driver_factory.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2455 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/profiler.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1284 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/boot_devices.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5782 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/release_mappings.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15304 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/policy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18304 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2578 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/context.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5220 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/rpc.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6041 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/fsm.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      900 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/i18n.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3949 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/network.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7349 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/swift.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11275 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/image_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1272 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1222 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12495 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/states.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18722 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/cinder.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3565 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/dhcp_factory.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2316 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/wsgi_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/common/glance_service/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/glance_service/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/common/glance_service/v2/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/glance_service/v2/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10410 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/glance_service/v2/image_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7961 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/glance_service/service_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1431 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/glance_service/service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6568 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/glance_service/base_image_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/common/glance_service/v1/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/glance_service/v1/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1072 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/glance_service/v1/image_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4019 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/keystone.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/common/grub_conf.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21573 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/neutron.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23059 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/exception.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15581 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/pxe_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5240 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/common/raid.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/objects/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1477 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13116 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/objects/volume_connector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17362 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/port.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10359 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/objects/chassis.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14316 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/objects/volume_target.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6820 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/conductor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2078 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/objects/indirection.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14982 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/portgroup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30236 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/node.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18662 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7703 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/notification.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4120 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/objects/fields.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      789 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/locale/ja/LC_MESSAGES/ironic-log-critical.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    79900 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/locale/ja/LC_MESSAGES/ironic.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      658 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/locale/pt_BR/LC_MESSAGES/ironic-log-critical.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      670 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/locale/ko_KR/LC_MESSAGES/ironic-log-critical.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      738 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/locale/fr/LC_MESSAGES/ironic-log-critical.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17284 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/locale/fr/LC_MESSAGES/ironic-log-info.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/dhcp/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/dhcp/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/dhcp/none.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3028 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/dhcp/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9575 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/dhcp/neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4258 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/irmc.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1199 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/redfish.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3084 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/agent.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5029 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/ipmi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12597 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6860 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/pxe.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2474 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/fake_hardware.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4128 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/raid_config_schema.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3991 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/hardware_type.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1972 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/cisco_ucs.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1121 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4292 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/oneview.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/drac/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/drac/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2830 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/drac/job.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14607 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6766 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7523 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/vendor_passthru.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6879 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/bios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6066 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5437 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    35257 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/drac/raid.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1817 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ipxe_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    29186 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/agent_base_vendor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8408 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/agent_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      131 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/master_grub_cfg.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30566 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/agent.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    53171 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/deploy_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/network/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/network/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5260 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/network/flat.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3748 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/network/noop.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26268 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/network/common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7831 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/network/neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/ucs/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/ucs/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5632 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ucs/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8253 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ucs/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4381 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/ucs/helper.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6964 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26174 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/pxe.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13399 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/console_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/oneview/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9784 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14841 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/deploy_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6780 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12537 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/deploy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4309 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10263 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/oneview/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/storage/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/storage/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      938 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/storage/noop.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20168 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/storage/cinder.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/ilo/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/ilo/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17982 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1882 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/ilo/console.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8659 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17634 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/firmware_processor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4406 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/vendor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25800 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/boot.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11840 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    31611 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ilo/common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      777 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/boot.ipxe
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2308 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/noop.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25107 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/iscsi_deploy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/irmc/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/irmc/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14532 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/irmc/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12032 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/irmc/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    44568 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/irmc/boot.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6663 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/irmc/inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8924 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/irmc/common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18019 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/image_cache.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      697 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/pxe_grub_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      776 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/elilo_efi_pxe_config.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/cimc/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/cimc/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6101 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/cimc/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6610 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/cimc/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2709 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/cimc/common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      480 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/agent_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26243 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7583 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/fake.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    55794 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/ipmitool.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      736 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/pxe_config.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/drivers/modules/redfish/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/redfish/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6782 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/redfish/management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9133 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/modules/redfish/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6498 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/drivers/modules/redfish/power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3539 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/generic.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4139 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/ilo.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    46482 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3351 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/drac.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8708 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/drivers/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/api/controllers/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/api/controllers/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3802 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/root.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2030 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/api/controllers/link.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3790 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/api/controllers/v1/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9293 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21274 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/volume_connector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4486 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/versions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1718 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/collection.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30830 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/port.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1083 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/api/controllers/v1/state.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20567 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14089 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/chassis.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21189 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/volume_target.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3524 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/api/controllers/v1/volume.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7093 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/notification_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18125 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6940 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/ramdisk.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10776 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24724 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/portgroup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77643 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/controllers/v1/node.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3964 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/app.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6459 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/api/middleware/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      861 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/middleware/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3876 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/middleware/parsable_error.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2281 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/middleware/auth_token.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      897 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/api/expose.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1352 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1045 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/api/app.wsgi
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/functional/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/cmd/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/cmd/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2687 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/cmd/test_conductor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9066 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/cmd/test_dbsync.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1573 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/common/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/common/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8223 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_rpc.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    37409 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_glance_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14895 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_network.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6655 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_policy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2913 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_exception.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3719 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/common/test_fsm.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    36176 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_driver_factory.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26342 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7824 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_release_mappings.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1461 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/common/test_states.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    39058 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_pxe_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4001 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_keystone.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3255 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_hash_ring.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2927 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_wsgi_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    39763 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_neutron.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11359 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_raid.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    36754 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_cinder.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    42088 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_images.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9080 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_swift.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3060 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_context.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2255 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/common/test_rpc_service.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18000 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/common/test_image_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/objects/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9581 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_volume_connector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5020 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/objects/test_fields.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/objects/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7074 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_conductor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9282 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_port.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11955 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_notification.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8869 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6011 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/objects/test_chassis.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    40621 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_objects.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7658 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_portgroup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12651 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_node.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9931 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/objects/test_volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/dhcp/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/dhcp/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4085 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/dhcp/test_factory.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18642 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/dhcp/test_neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1001 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10925 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/third_party_driver_mocks.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2045 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_redfish.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1914 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6591 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_cisco.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      575 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      909 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config_boot_from_volume_no_volumes.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16880 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4063 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_generic.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6400 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_ipmi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6461 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_pxe.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      759 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/boot.ipxe
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6729 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_drac.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      631 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config_timeout.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7636 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_irmc.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      673 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/pxe_grub_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      643 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/elilo_efi_pxe_config.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18619 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7620 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_ilo.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6492 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_job.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14860 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_periodic_task.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12222 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5109 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      822 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6845 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_bios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6704 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    59077 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_raid.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25499 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    66318 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   122471 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_ipmitool.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   108163 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_deploy_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/network/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/network/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8872 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_flat.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    71186 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20222 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_neutron.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3793 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_noop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15211 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7283 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/test_helper.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6124 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10308 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_agent_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52625 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_iscsi_deploy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4768 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18349 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_deploy_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15681 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23866 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_deploy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10872 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16274 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    59467 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_pxe.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/storage/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/storage/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    31687 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/storage/test_cinder.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22968 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26714 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_firmware_processor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10684 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2923 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_console.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52035 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_boot.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5017 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_vendor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52062 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    28070 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    61131 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_agent_base_vendor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11495 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_inspect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20008 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    76588 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_boot.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4241 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ok.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4271 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ng.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10969 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22864 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9167 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    59054 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13746 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5130 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/test_common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5675 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2666 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_noop.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    26542 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_console_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33377 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/test_image_cache.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10741 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/test_power.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8421 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/test_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8645 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/test_management.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3360 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/third_party_driver_mock_specs.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7886 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_oneview.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      988 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config_boot_from_volume.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5086 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/test_fake.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      763 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/drivers/pxe_config.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/api/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11219 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/api/test_hooks.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6430 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4195 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/api/test_acl.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1464 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/test_ospmiddleware.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4418 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/api/test_middleware.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5290 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/test_base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3515 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/test_root.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10456 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/api/v1/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2502 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_versions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23848 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_drivers.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    28744 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    46793 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_volume_connectors.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    99129 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_ports.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2863 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_expose.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27294 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_chassis.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10401 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_notification_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   193806 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_nodes.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    64105 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_portgroups.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2184 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_volume.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8162 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_ramdisk.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2440 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_root.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    44835 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_volume_targets.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13835 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/api/v1/test_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1985 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/api/test_audit.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5877 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/raid_constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/db/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5667 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/db/test_api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18882 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/db/test_conductor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15369 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/db/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6721 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/test_volume_connectors.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5442 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/test_ports.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1448 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/test_api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30775 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/test_migrations.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3385 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/test_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3335 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/test_chassis.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27797 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/db/test_nodes.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9199 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/test_portgroups.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2239 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4539 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/db/test_node_tags.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7546 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/db/test_volume_targets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/conf/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/conf/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2394 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conf/test_auth.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/tests/unit/conductor/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20153 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/test_rpcapi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    49551 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/test_task_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/conductor/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   321803 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/test_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    74767 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/test_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2098 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/test__mgr_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9639 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/conductor/test_notification_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8111 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/mgr_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24218 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/conductor/test_base_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2193 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/unit/stubs.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1666 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/tests/unit/policy_fixture.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9038 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/db/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1560 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/migration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33459 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/db/sqlalchemy/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10401 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/models.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1971 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1177 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/f6fdb920c182_set_pxe_enabled_true.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2060 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/2353895ecfae_add_conductor_hardware_interfaces_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1096 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/31baaf680d2b_add_node_instance_info.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      988 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/e294876e8028_add_node_network_interface.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1208 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/dbefd6bdaa2c_add_default_column_to_.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1314 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/493d8f27f235_add_portgroup_configuration_fields.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      950 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/4f399b21ae71_add_node_clean_step.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1208 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/487deb87cc9d_add_conductor_affinity_and_online.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1929 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/bcdd431ba0bf_add_fields_for_all_interfaces.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      969 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/21b331f883ef_add_provision_updated_at.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1084 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/789acc877671_add_raid_config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1007 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/516faf1bb9b1_resizing_column_nodes_driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1005 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/60cf717201bc_add_standalone_ports_supported.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1089 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/2fb93ffd2af1_increase_node_name_length.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2225 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/1a59178ebdf6_add_volume_targets_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1222 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/1e1d5ace7dc6_add_inspection_started_at_and_.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2485 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/5ea1b0d310e_added_port_group_table_and_altered_ports.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      929 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3cb628139ea4_nodes_add_console_enabled.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1040 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/1d6951876d68_add_storage_interface_db_field_and_.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1440 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/48d6c242bb9b_add_node_tags.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1074 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3bea56f25597_add_unique_constraint_to_instance_uuid.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1022 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/242cc6a923b3_add_node_maintenance_reason.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1020 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3ae36a5f5131_add_logical_name.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2044 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/868cb606a74a_add_version_field_in_base_class.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1523 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/5674c57409b9_replace_nostate_with_available.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4331 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1022 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3d86a077a3f2_add_port_physical_network.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2057 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/daa1ba02d98_add_volume_connectors_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1009 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/dd34e1f1303b_add_resource_class_to_node.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1024 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/bb59b63f55a_add_node_driver_internal_info.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1385 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/c14cef6dfedf_populate_node_network_interface.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1192 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/10b163d4481e_add_port_portgroup_internal_info.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      349 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/script.py.mako
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      434 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic/README
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3680 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/migration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    49980 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/db/sqlalchemy/api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      975 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/db/sqlalchemy/alembic.ini
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      705 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/conf/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2325 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3160 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/irmc.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1178 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/redfish.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4491 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/agent.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2651 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/ipmi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3160 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1451 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6413 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/pxe.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2354 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/console.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1533 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/audit.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4610 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/deploy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      985 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/dhcp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1312 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/swift.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8312 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/conductor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2018 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/auth.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1250 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/metrics_statsd.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14838 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/default.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8279 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/glance.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1804 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3641 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/opts.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2255 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/oneview.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2090 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/cinder.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1102 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/service_catalog.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1771 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/cisco.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4123 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/ilo.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      928 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/database.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1032 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/drac.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      874 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/keystone.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2383 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conf/metrics.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4108 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/neutron.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conf/iscsi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic/conductor/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22392 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conductor/task_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conductor/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    45367 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conductor/rpcapi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27583 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conductor/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   147125 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conductor/manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7492 2019-04-26 15:39:32.000000 ironic-9.1.7/ironic/conductor/notification_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25452 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic/conductor/base_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3169 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/plugin.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2694 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/common_settings
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      704 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/files/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1731 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/files/apache-ironic-api.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      283 2019-04-26 15:39:32.000000 ironic-9.1.7/devstack/files/apache-ipxe-ironic.template
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      891 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/files/apache-ironic-api-redirect.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/files/debs/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1137 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/files/debs/ironic
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/files/hooks/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     2845 2019-04-26 15:39:32.000000 ironic-9.1.7/devstack/files/hooks/qemu.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/files/rpms/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      260 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/files/rpms/ironic
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/tools/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/tools/ironic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/tools/ironic/templates/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2278 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/tools/ironic/templates/vm.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      128 2019-04-26 15:39:32.000000 ironic-9.1.7/devstack/tools/ironic/templates/brbm.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      424 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/tools/ironic/templates/tftpd-xinetd.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/tools/ironic/scripts/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4802 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/tools/ironic/scripts/configure-vm.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1053 2019-04-26 15:39:32.000000 ironic-9.1.7/devstack/tools/ironic/scripts/cleanup-node.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1091 2019-04-26 15:39:32.000000 ironic-9.1.7/devstack/tools/ironic/scripts/setup-network.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4451 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/tools/ironic/scripts/create-node.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/lib/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    91921 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/lib/ironic
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/devstack/upgrade/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     6625 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/upgrade/resources.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1466 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/upgrade/settings
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      454 2019-04-26 15:39:32.000000 ironic-9.1.7/devstack/upgrade/shutdown.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4485 2019-04-26 15:39:36.000000 ironic-9.1.7/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/common/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/common/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1421 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/common/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4739 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/common/waiters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/services/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9344 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/v1/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/v1/json/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/v1/json/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23377 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/services/baremetal/v1/json/baremetal_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      607 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24349 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1599 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/tests/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9593 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_volume_connector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1731 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_api_discovery.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      993 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/api_microversion_fixture.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8863 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_nodestates.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2123 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_drivers.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18808 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_ports_negative.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14778 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_ports.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3431 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_chassis.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17215 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_nodes.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3278 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_portgroups.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13094 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9093 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/ironic_standalone/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/ironic_standalone/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5228 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/ironic_standalone/test_basic_ops.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8134 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/baremetal_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5786 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/test_baremetal_multitenancy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6125 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/test_baremetal_boot_from_volume.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6027 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/test_baremetal_basic_ops.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13089 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/tests/scenario/baremetal_standalone_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5315 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1909 2019-04-26 15:39:36.000000 ironic-9.1.7/ironic_tempest_plugin/clients.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3375 2019-04-26 15:39:36.000000 ironic-9.1.7/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 15:41:44.000000 ironic-9.1.7/zuul.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1644 2019-04-26 15:39:36.000000 ironic-9.1.7/zuul.d/project.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6006 2019-04-26 15:39:36.000000 ironic-9.1.7/zuul.d/legacy-ironic-jobs.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8085 2019-04-26 15:41:44.000000 ironic-9.1.7/setup.cfg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-04-26 15:39:32.000000 ironic-9.1.7/LICENSE
```

### Comparing `ironic-9.1.6/ironic/objects/notification.py` & `ironic-9.1.7/ironic/objects/notification.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/conductor.py` & `ironic-9.1.7/ironic/objects/conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/volume_connector.py` & `ironic-9.1.7/ironic/objects/volume_connector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/indirection.py` & `ironic-9.1.7/ironic/objects/indirection.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/port.py` & `ironic-9.1.7/ironic/objects/port.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/base.py` & `ironic-9.1.7/ironic/objects/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/__init__.py` & `ironic-9.1.7/ironic/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/chassis.py` & `ironic-9.1.7/ironic/objects/chassis.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/node.py` & `ironic-9.1.7/ironic/objects/node.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/volume_target.py` & `ironic-9.1.7/ironic/objects/volume_target.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/portgroup.py` & `ironic-9.1.7/ironic/objects/portgroup.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/objects/fields.py` & `ironic-9.1.7/ironic/objects/fields.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/api.py` & `ironic-9.1.7/ironic/db/api.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/migration.py` & `ironic-9.1.7/ironic/db/migration.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/1e1d5ace7dc6_add_inspection_started_at_and_.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/1e1d5ace7dc6_add_inspection_started_at_and_.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3ae36a5f5131_add_logical_name.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3ae36a5f5131_add_logical_name.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/f6fdb920c182_set_pxe_enabled_true.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/f6fdb920c182_set_pxe_enabled_true.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/1d6951876d68_add_storage_interface_db_field_and_.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/1d6951876d68_add_storage_interface_db_field_and_.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/31baaf680d2b_add_node_instance_info.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/31baaf680d2b_add_node_instance_info.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/487deb87cc9d_add_conductor_affinity_and_online.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/487deb87cc9d_add_conductor_affinity_and_online.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/dbefd6bdaa2c_add_default_column_to_.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/dbefd6bdaa2c_add_default_column_to_.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3d86a077a3f2_add_port_physical_network.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3d86a077a3f2_add_port_physical_network.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/242cc6a923b3_add_node_maintenance_reason.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/242cc6a923b3_add_node_maintenance_reason.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3cb628139ea4_nodes_add_console_enabled.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3cb628139ea4_nodes_add_console_enabled.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/21b331f883ef_add_provision_updated_at.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/21b331f883ef_add_provision_updated_at.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/868cb606a74a_add_version_field_in_base_class.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/868cb606a74a_add_version_field_in_base_class.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/2353895ecfae_add_conductor_hardware_interfaces_table.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/2353895ecfae_add_conductor_hardware_interfaces_table.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/493d8f27f235_add_portgroup_configuration_fields.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/493d8f27f235_add_portgroup_configuration_fields.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/daa1ba02d98_add_volume_connectors_table.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/daa1ba02d98_add_volume_connectors_table.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/789acc877671_add_raid_config.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/789acc877671_add_raid_config.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/e294876e8028_add_node_network_interface.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/e294876e8028_add_node_network_interface.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/1a59178ebdf6_add_volume_targets_table.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/1a59178ebdf6_add_volume_targets_table.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/60cf717201bc_add_standalone_ports_supported.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/60cf717201bc_add_standalone_ports_supported.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/2fb93ffd2af1_increase_node_name_length.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/2fb93ffd2af1_increase_node_name_length.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/5674c57409b9_replace_nostate_with_available.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/5674c57409b9_replace_nostate_with_available.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/3bea56f25597_add_unique_constraint_to_instance_uuid.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/3bea56f25597_add_unique_constraint_to_instance_uuid.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/4f399b21ae71_add_node_clean_step.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/4f399b21ae71_add_node_clean_step.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/bb59b63f55a_add_node_driver_internal_info.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/bb59b63f55a_add_node_driver_internal_info.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/c14cef6dfedf_populate_node_network_interface.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/c14cef6dfedf_populate_node_network_interface.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/5ea1b0d310e_added_port_group_table_and_altered_ports.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/5ea1b0d310e_added_port_group_table_and_altered_ports.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/48d6c242bb9b_add_node_tags.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/48d6c242bb9b_add_node_tags.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/10b163d4481e_add_port_portgroup_internal_info.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/10b163d4481e_add_port_portgroup_internal_info.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/516faf1bb9b1_resizing_column_nodes_driver.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/516faf1bb9b1_resizing_column_nodes_driver.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/dd34e1f1303b_add_resource_class_to_node.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/dd34e1f1303b_add_resource_class_to_node.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/versions/bcdd431ba0bf_add_fields_for_all_interfaces.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/versions/bcdd431ba0bf_add_fields_for_all_interfaces.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic/env.py` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/api.py` & `ironic-9.1.7/ironic/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/models.py` & `ironic-9.1.7/ironic/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/migration.py` & `ironic-9.1.7/ironic/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/db/sqlalchemy/alembic.ini` & `ironic-9.1.7/ironic/db/sqlalchemy/alembic.ini`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/snmp.py` & `ironic-9.1.7/ironic/drivers/snmp.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/pxe.py` & `ironic-9.1.7/ironic/drivers/pxe.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/hardware_type.py` & `ironic-9.1.7/ironic/drivers/hardware_type.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/redfish.py` & `ironic-9.1.7/ironic/drivers/redfish.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/utils.py` & `ironic-9.1.7/ironic/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/power.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/common.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/console.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/console.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/inspect.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/vendor.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/vendor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/boot.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/boot.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/management.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ilo/firmware_processor.py` & `ironic-9.1.7/ironic/drivers/modules/ilo/firmware_processor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/image_cache.py` & `ironic-9.1.7/ironic/drivers/modules/image_cache.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/network/common.py` & `ironic-9.1.7/ironic/drivers/modules/network/common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/network/flat.py` & `ironic-9.1.7/ironic/drivers/modules/network/flat.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/network/noop.py` & `ironic-9.1.7/ironic/drivers/modules/network/noop.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/network/neutron.py` & `ironic-9.1.7/ironic/drivers/modules/network/neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/console_utils.py` & `ironic-9.1.7/ironic/drivers/modules/console_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/snmp.py` & `ironic-9.1.7/ironic/drivers/modules/snmp.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/pxe_config.template` & `ironic-9.1.7/ironic/drivers/modules/pxe_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/pxe.py` & `ironic-9.1.7/ironic/drivers/modules/pxe.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/elilo_efi_pxe_config.template` & `ironic-9.1.7/ironic/drivers/modules/elilo_efi_pxe_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/pxe_grub_config.template` & `ironic-9.1.7/ironic/drivers/modules/pxe_grub_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/irmc/power.py` & `ironic-9.1.7/ironic/drivers/modules/irmc/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/irmc/common.py` & `ironic-9.1.7/ironic/drivers/modules/irmc/common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/irmc/inspect.py` & `ironic-9.1.7/ironic/drivers/modules/irmc/inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/irmc/boot.py` & `ironic-9.1.7/ironic/drivers/modules/irmc/boot.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/irmc/management.py` & `ironic-9.1.7/ironic/drivers/modules/irmc/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/storage/noop.py` & `ironic-9.1.7/ironic/drivers/modules/storage/noop.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/storage/cinder.py` & `ironic-9.1.7/ironic/drivers/modules/storage/cinder.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/agent_base_vendor.py` & `ironic-9.1.7/ironic/drivers/modules/agent_base_vendor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/cimc/power.py` & `ironic-9.1.7/ironic/drivers/modules/cimc/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/cimc/common.py` & `ironic-9.1.7/ironic/drivers/modules/cimc/common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/cimc/management.py` & `ironic-9.1.7/ironic/drivers/modules/cimc/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ipmitool.py` & `ironic-9.1.7/ironic/drivers/modules/ipmitool.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ucs/power.py` & `ironic-9.1.7/ironic/drivers/modules/ucs/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ucs/helper.py` & `ironic-9.1.7/ironic/drivers/modules/ucs/helper.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ucs/management.py` & `ironic-9.1.7/ironic/drivers/modules/ucs/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/iscsi_deploy.py` & `ironic-9.1.7/ironic/drivers/modules/iscsi_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,17 @@
 DISK_LAYOUT_PARAMS = ('root_gb', 'swap_mb', 'ephemeral_gb')
 
 
 @image_cache.cleanup(priority=50)
 class InstanceImageCache(image_cache.ImageCache):
 
     def __init__(self):
+        master_path = CONF.pxe.instance_master_path or None
         super(self.__class__, self).__init__(
-            CONF.pxe.instance_master_path,
+            master_path,
             # MiB -> B
             cache_size=CONF.pxe.image_cache_size * 1024 * 1024,
             # min -> sec
             cache_ttl=CONF.pxe.image_cache_ttl * 60)
 
 
 def _get_image_dir_path(node_uuid):
```

### Comparing `ironic-9.1.6/ironic/drivers/modules/redfish/power.py` & `ironic-9.1.7/ironic/drivers/modules/redfish/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/redfish/utils.py` & `ironic-9.1.7/ironic/drivers/modules/redfish/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/redfish/management.py` & `ironic-9.1.7/ironic/drivers/modules/redfish/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/agent.py` & `ironic-9.1.7/ironic/drivers/modules/agent.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/power.py` & `ironic-9.1.7/ironic/drivers/modules/drac/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/job.py` & `ironic-9.1.7/ironic/drivers/modules/drac/job.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/common.py` & `ironic-9.1.7/ironic/drivers/modules/drac/common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/raid.py` & `ironic-9.1.7/ironic/drivers/modules/drac/raid.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/inspect.py` & `ironic-9.1.7/ironic/drivers/modules/drac/inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         properties = {}
 
         try:
             properties['memory_mb'] = sum(
                 [memory.size_mb for memory in client.list_memory()])
             cpus = client.list_cpus()
             if cpus:
-                properties['cpus'] = len(cpus)
+                properties['cpus'] = sum(
+                    [self._calculate_cpus(cpu) for cpu in cpus])
                 properties['cpu_arch'] = 'x86_64' if cpus[0].arch64 else 'x86'
 
             virtual_disks = client.list_virtual_disks()
             root_disk = self._guess_root_disk(virtual_disks)
             if root_disk:
                 properties['local_gb'] = int(root_disk.size_mb / units.Ki)
             else:
@@ -144,7 +145,19 @@
                                      megabytes.
         :returns: root disk.
         """
         disks.sort(key=lambda disk: disk.size_mb)
         for disk in disks:
             if disk.size_mb >= min_size_required_mb:
                 return disk
+
+    def _calculate_cpus(self, cpu):
+        """Find actual CPU count.
+
+        :param cpu: Pass cpu.
+
+        :returns: returns total cpu count.
+        """
+        if cpu.ht_enabled:
+            return cpu.cores * 2
+        else:
+            return cpu.cores
```

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/management.py` & `ironic-9.1.7/ironic/drivers/modules/drac/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/bios.py` & `ironic-9.1.7/ironic/drivers/modules/drac/bios.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/drac/vendor_passthru.py` & `ironic-9.1.7/ironic/drivers/modules/drac/vendor_passthru.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/boot.ipxe` & `ironic-9.1.7/ironic/drivers/modules/boot.ipxe`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/noop.py` & `ironic-9.1.7/ironic/drivers/modules/noop.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/deploy_utils.py` & `ironic-9.1.7/ironic/drivers/modules/deploy_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/fake.py` & `ironic-9.1.7/ironic/drivers/modules/fake.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/inspector.py` & `ironic-9.1.7/ironic/drivers/modules/inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/agent_client.py` & `ironic-9.1.7/ironic/drivers/modules/agent_client.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/oneview/power.py` & `ironic-9.1.7/ironic/drivers/modules/oneview/power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/oneview/common.py` & `ironic-9.1.7/ironic/drivers/modules/oneview/common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/oneview/inspect.py` & `ironic-9.1.7/ironic/drivers/modules/oneview/inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/oneview/deploy.py` & `ironic-9.1.7/ironic/drivers/modules/oneview/deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/oneview/management.py` & `ironic-9.1.7/ironic/drivers/modules/oneview/management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/oneview/deploy_utils.py` & `ironic-9.1.7/ironic/drivers/modules/oneview/deploy_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/modules/ipxe_config.template` & `ironic-9.1.7/ironic/drivers/modules/ipxe_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/base.py` & `ironic-9.1.7/ironic/drivers/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/ipmi.py` & `ironic-9.1.7/ironic/drivers/ipmi.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/oneview.py` & `ironic-9.1.7/ironic/drivers/oneview.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/ilo.py` & `ironic-9.1.7/ironic/drivers/ilo.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/drac.py` & `ironic-9.1.7/ironic/drivers/drac.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/cisco_ucs.py` & `ironic-9.1.7/ironic/drivers/cisco_ucs.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/fake_hardware.py` & `ironic-9.1.7/ironic/drivers/fake_hardware.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/agent.py` & `ironic-9.1.7/ironic/drivers/agent.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/irmc.py` & `ironic-9.1.7/ironic/drivers/irmc.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/fake.py` & `ironic-9.1.7/ironic/drivers/fake.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/raid_config_schema.json` & `ironic-9.1.7/ironic/drivers/raid_config_schema.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/drivers/generic.py` & `ironic-9.1.7/ironic/drivers/generic.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/glance.py` & `ironic-9.1.7/ironic/conf/glance.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/snmp.py` & `ironic-9.1.7/ironic/conf/snmp.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/audit.py` & `ironic-9.1.7/ironic/conf/audit.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/pxe.py` & `ironic-9.1.7/ironic/conf/pxe.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                default='/var/lib/ironic/images/',
                help=_('On the ironic-conductor node, directory where images '
                       'are stored on disk.')),
     cfg.StrOpt('instance_master_path',
                default='/var/lib/ironic/master_images',
                help=_('On the ironic-conductor node, directory where master '
                       'instance images are stored on disk. '
-                      'Setting to <None> disables image caching.')),
+                      'Setting to the empty string disables image caching.')),
     cfg.IntOpt('image_cache_size',
                default=20480,
                help=_('Maximum size (in MiB) of cache for master images, '
                       'including those in use.')),
     # 10080 here is 1 week - 60*24*7. It is entirely arbitrary in the absence
     # of a facility to disable the ttl entirely.
     cfg.IntOpt('image_cache_ttl',
```

### Comparing `ironic-9.1.6/ironic/conf/redfish.py` & `ironic-9.1.7/ironic/conf/redfish.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/conductor.py` & `ironic-9.1.7/ironic/conf/conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/api.py` & `ironic-9.1.7/ironic/conf/api.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/console.py` & `ironic-9.1.7/ironic/conf/console.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/ipmi.py` & `ironic-9.1.7/ironic/conf/ipmi.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/oneview.py` & `ironic-9.1.7/ironic/conf/oneview.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/__init__.py` & `ironic-9.1.7/ironic/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/swift.py` & `ironic-9.1.7/ironic/conf/swift.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/ilo.py` & `ironic-9.1.7/ironic/conf/ilo.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/drac.py` & `ironic-9.1.7/ironic/conf/drac.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/deploy.py` & `ironic-9.1.7/ironic/conf/deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/service_catalog.py` & `ironic-9.1.7/ironic/conf/service_catalog.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/default.py` & `ironic-9.1.7/ironic/conf/default.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/agent.py` & `ironic-9.1.7/ironic/conf/agent.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/metrics_statsd.py` & `ironic-9.1.7/ironic/conf/metrics_statsd.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/dhcp.py` & `ironic-9.1.7/ironic/conf/dhcp.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/iscsi.py` & `ironic-9.1.7/ironic/conf/iscsi.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/opts.py` & `ironic-9.1.7/ironic/conf/opts.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/metrics.py` & `ironic-9.1.7/ironic/conf/metrics.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/auth.py` & `ironic-9.1.7/ironic/conf/auth.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/irmc.py` & `ironic-9.1.7/ironic/conf/irmc.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/cinder.py` & `ironic-9.1.7/ironic/conf/cinder.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/keystone.py` & `ironic-9.1.7/ironic/conf/keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/inspector.py` & `ironic-9.1.7/ironic/conf/inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/cisco.py` & `ironic-9.1.7/ironic/conf/cisco.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/neutron.py` & `ironic-9.1.7/ironic/conf/neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conf/database.py` & `ironic-9.1.7/ironic/conf/database.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/config.py` & `ironic-9.1.7/ironic/api/config.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/hooks.py` & `ironic-9.1.7/ironic/api/hooks.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/middleware/__init__.py` & `ironic-9.1.7/ironic/api/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/middleware/auth_token.py` & `ironic-9.1.7/ironic/api/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/middleware/parsable_error.py` & `ironic-9.1.7/ironic/api/middleware/parsable_error.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/app.wsgi` & `ironic-9.1.7/ironic/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/root.py` & `ironic-9.1.7/ironic/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/base.py` & `ironic-9.1.7/ironic/api/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/link.py` & `ironic-9.1.7/ironic/api/controllers/link.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/state.py` & `ironic-9.1.7/ironic/api/controllers/v1/state.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/volume.py` & `ironic-9.1.7/ironic/api/controllers/v1/volume.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/volume_connector.py` & `ironic-9.1.7/ironic/api/controllers/v1/volume_connector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/collection.py` & `ironic-9.1.7/ironic/api/controllers/v1/collection.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/utils.py` & `ironic-9.1.7/ironic/api/controllers/v1/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/types.py` & `ironic-9.1.7/ironic/api/controllers/v1/types.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/port.py` & `ironic-9.1.7/ironic/api/controllers/v1/port.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/__init__.py` & `ironic-9.1.7/ironic/api/controllers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/notification_utils.py` & `ironic-9.1.7/ironic/api/controllers/v1/notification_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/chassis.py` & `ironic-9.1.7/ironic/api/controllers/v1/chassis.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/node.py` & `ironic-9.1.7/ironic/api/controllers/v1/node.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/volume_target.py` & `ironic-9.1.7/ironic/api/controllers/v1/volume_target.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/ramdisk.py` & `ironic-9.1.7/ironic/api/controllers/v1/ramdisk.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/portgroup.py` & `ironic-9.1.7/ironic/api/controllers/v1/portgroup.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/versions.py` & `ironic-9.1.7/ironic/api/controllers/v1/versions.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/controllers/v1/driver.py` & `ironic-9.1.7/ironic/api/controllers/v1/driver.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/expose.py` & `ironic-9.1.7/ironic/api/expose.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/api/app.py` & `ironic-9.1.7/ironic/api/app.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/cmd/dbsync.py` & `ironic-9.1.7/ironic/cmd/dbsync.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/cmd/conductor.py` & `ironic-9.1.7/ironic/cmd/conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/cmd/api.py` & `ironic-9.1.7/ironic/cmd/api.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/cmd/__init__.py` & `ironic-9.1.7/ironic/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conductor/manager.py` & `ironic-9.1.7/ironic/conductor/manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conductor/base_manager.py` & `ironic-9.1.7/ironic/conductor/base_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conductor/utils.py` & `ironic-9.1.7/ironic/conductor/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,16 +355,18 @@
 
     :param task: a TaskManager instance.
     """
     last_error = (_("Timeout reached while cleaning the node. Please "
                     "check if the ramdisk responsible for the cleaning is "
                     "running on the node. Failed on step %(step)s.") %
                   {'step': task.node.clean_step})
-    cleaning_error_handler(task, msg=last_error,
-                           set_fail_state=True)
+    # NOTE(rloo): this is called from the periodic task for cleanwait timeouts,
+    # via the task manager's process_event(). The node has already been moved
+    # to CLEANFAIL, so the error handler doesn't need to set the fail state.
+    cleaning_error_handler(task, msg=last_error, set_fail_state=False)
 
 
 def cleaning_error_handler(task, msg, tear_down_cleaning=True,
                            set_fail_state=True):
     """Put a failed node in CLEANFAIL and maintenance."""
     node = task.node
     if node.provision_state in (
@@ -389,15 +391,15 @@
         try:
             task.driver.deploy.tear_down_cleaning(task)
         except Exception as e:
             msg = ('Failed to tear down cleaning on node %(uuid)s, '
                    'reason: %(err)s' % {'err': e, 'uuid': node.uuid})
             LOG.exception(msg)
 
-    if set_fail_state:
+    if set_fail_state and node.provision_state != states.CLEANFAIL:
         target_state = states.MANAGEABLE if manual_clean else None
         task.process_event('fail', target_state=target_state)
 
 
 def spawn_cleaning_error_handler(e, node):
     """Handle spawning error for node cleaning."""
     if isinstance(e, exception.NoFreeConductorWorker):
```

### Comparing `ironic-9.1.6/ironic/conductor/rpcapi.py` & `ironic-9.1.7/ironic/conductor/rpcapi.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conductor/notification_utils.py` & `ironic-9.1.7/ironic/conductor/notification_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/conductor/task_manager.py` & `ironic-9.1.7/ironic/conductor/task_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/version.py` & `ironic-9.1.7/ironic/version.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/profiler.py` & `ironic-9.1.7/ironic/common/profiler.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/exception.py` & `ironic-9.1.7/ironic/common/exception.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/service.py` & `ironic-9.1.7/ironic/common/service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/release_mappings.py` & `ironic-9.1.7/ironic/common/release_mappings.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/config.py` & `ironic-9.1.7/ironic/common/config.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/raid.py` & `ironic-9.1.7/ironic/common/raid.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/utils.py` & `ironic-9.1.7/ironic/common/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/rpc_service.py` & `ironic-9.1.7/ironic/common/rpc_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/swift.py` & `ironic-9.1.7/ironic/common/swift.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/context.py` & `ironic-9.1.7/ironic/common/context.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/dhcp_factory.py` & `ironic-9.1.7/ironic/common/dhcp_factory.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/image_service.py` & `ironic-9.1.7/ironic/common/image_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/boot_devices.py` & `ironic-9.1.7/ironic/common/boot_devices.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/states.py` & `ironic-9.1.7/ironic/common/states.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/rpc.py` & `ironic-9.1.7/ironic/common/rpc.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/cinder.py` & `ironic-9.1.7/ironic/common/cinder.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/keystone.py` & `ironic-9.1.7/ironic/common/keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/policy.py` & `ironic-9.1.7/ironic/common/policy.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/wsgi_service.py` & `ironic-9.1.7/ironic/common/wsgi_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/i18n.py` & `ironic-9.1.7/ironic/common/i18n.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/fsm.py` & `ironic-9.1.7/ironic/common/fsm.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/network.py` & `ironic-9.1.7/ironic/common/network.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/glance_service/service.py` & `ironic-9.1.7/ironic/common/glance_service/service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/glance_service/service_utils.py` & `ironic-9.1.7/ironic/common/glance_service/service_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/glance_service/v2/image_service.py` & `ironic-9.1.7/ironic/common/glance_service/v2/image_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/glance_service/v1/image_service.py` & `ironic-9.1.7/ironic/common/glance_service/v1/image_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/glance_service/base_image_service.py` & `ironic-9.1.7/ironic/common/glance_service/base_image_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/images.py` & `ironic-9.1.7/ironic/common/images.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/neutron.py` & `ironic-9.1.7/ironic/common/neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/driver_factory.py` & `ironic-9.1.7/ironic/common/driver_factory.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/hash_ring.py` & `ironic-9.1.7/ironic/common/hash_ring.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/common/pxe_utils.py` & `ironic-9.1.7/ironic/common/pxe_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/dhcp/base.py` & `ironic-9.1.7/ironic/dhcp/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/dhcp/none.py` & `ironic-9.1.7/ironic/dhcp/none.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/dhcp/neutron.py` & `ironic-9.1.7/ironic/dhcp/neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_objects.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_objects.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_fields.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_fields.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_chassis.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_chassis.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/utils.py` & `ironic-9.1.7/ironic/tests/unit/objects/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_volume_target.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_volume_target.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_conductor.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_volume_connector.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_volume_connector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_port.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_port.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_portgroup.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_portgroup.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_node.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_node.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/objects/test_notification.py` & `ironic-9.1.7/ironic/tests/unit/objects/test_notification.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/stubs.py` & `ironic-9.1.7/ironic/tests/unit/stubs.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_ports.py` & `ironic-9.1.7/ironic/tests/unit/db/test_ports.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_portgroups.py` & `ironic-9.1.7/ironic/tests/unit/db/test_portgroups.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_chassis.py` & `ironic-9.1.7/ironic/tests/unit/db/test_chassis.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/utils.py` & `ironic-9.1.7/ironic/tests/unit/db/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_conductor.py` & `ironic-9.1.7/ironic/tests/unit/db/test_conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_volume_connectors.py` & `ironic-9.1.7/ironic/tests/unit/db/test_volume_connectors.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/base.py` & `ironic-9.1.7/ironic/tests/unit/db/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_volume_targets.py` & `ironic-9.1.7/ironic/tests/unit/db/test_volume_targets.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_node_tags.py` & `ironic-9.1.7/ironic/tests/unit/db/test_node_tags.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_api.py` & `ironic-9.1.7/ironic/tests/unit/db/test_api.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/test_nodes.py` & `ironic-9.1.7/ironic/tests/unit/db/test_nodes.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/test_types.py` & `ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/test_migrations.py` & `ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/test_migrations.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/db/sqlalchemy/test_api.py` & `ironic-9.1.7/ironic/tests/unit/db/sqlalchemy/test_api.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/third_party_driver_mock_specs.py` & `ironic-9.1.7/ironic/tests/unit/drivers/third_party_driver_mock_specs.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/pxe_config.template` & `ironic-9.1.7/ironic/tests/unit/drivers/pxe_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_ipmi.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/elilo_efi_pxe_config.template` & `ironic-9.1.7/ironic/tests/unit/drivers/elilo_efi_pxe_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/pxe_grub_config.template` & `ironic-9.1.7/ironic/tests/unit/drivers/pxe_grub_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_pxe.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_pxe.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_base.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_redfish.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_redfish.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_snmp.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_snmp.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_console.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_console.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_boot.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_boot.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_inspect.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_common.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_firmware_processor.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_firmware_processor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ilo/test_vendor.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ilo/test_vendor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_agent_base_vendor.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_agent_base_vendor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_noop.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_noop.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_noop.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_noop.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_neutron.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_flat.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_flat.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/network/test_common.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/network/test_common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_agent_client.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_agent_client.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_image_cache.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_image_cache.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_console_utils.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_console_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_pxe.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_pxe.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_boot.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_boot.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_inspect.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/test_common.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/test_common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ok.xml` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ok.xml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ng.xml` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/irmc/fake_sensors_data_ng.xml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/storage/test_cinder.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/storage/test_cinder.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_snmp.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_snmp.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/cimc/test_common.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/cimc/test_common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/ucs/test_helper.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/ucs/test_helper.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_agent.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_agent.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/redfish/test_utils.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/redfish/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_bios.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_bios.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_periodic_task.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_periodic_task.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_raid.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_raid.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/utils.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_inspect.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_inspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                  'vt_enabled': True,
                  'arch64': True},
                 {'id': 'CPU.Socket.2',
                  'cores': 6,
                  'speed': 2400,
                  'model': 'Intel(R) Xeon(R) CPU E5-2620 v3 @ 2.40GHz',
                  'state': 'ok',
-                 'ht_enabled': True,
+                 'ht_enabled': False,
                  'turbo_enabled': True,
                  'vt_enabled': True,
                  'arch64': True}]
         virtual_disks = [
             {'id': 'Disk.Virtual.0:RAID.Integrated.1-1',
              'name': 'disk 0',
              'description': 'Virtual Disk 0 on Integrated RAID Controller 1',
@@ -141,15 +141,15 @@
     @mock.patch.object(drac_common, 'get_drac_client', spec_set=True,
                        autospec=True)
     @mock.patch.object(objects.Port, 'create', spec_set=True, autospec=True)
     def test_inspect_hardware(self, mock_port_create, mock_get_drac_client):
         expected_node_properties = {
             'memory_mb': 32768,
             'local_gb': 1116,
-            'cpus': 2,
+            'cpus': 18,
             'cpu_arch': 'x86_64'}
         mock_client = mock.Mock()
         mock_get_drac_client.return_value = mock_client
         mock_client.list_memory.return_value = self.memory
         mock_client.list_cpus.return_value = self.cpus
         mock_client.list_virtual_disks.return_value = self.virtual_disks
         mock_client.list_nics.return_value = self.nics
@@ -184,15 +184,15 @@
                        autospec=True)
     @mock.patch.object(objects.Port, 'create', spec_set=True, autospec=True)
     def test_inspect_hardware_no_virtual_disk(self, mock_port_create,
                                               mock_get_drac_client):
         expected_node_properties = {
             'memory_mb': 32768,
             'local_gb': 279,
-            'cpus': 2,
+            'cpus': 18,
             'cpu_arch': 'x86_64'}
         mock_client = mock.Mock()
         mock_get_drac_client.return_value = mock_client
         mock_client.list_memory.return_value = self.memory
         mock_client.list_cpus.return_value = self.cpus
         mock_client.list_virtual_disks.return_value = []
         mock_client.list_physical_disks.return_value = self.physical_disks
@@ -229,15 +229,15 @@
                        autospec=True)
     @mock.patch.object(objects.Port, 'create', spec_set=True, autospec=True)
     def test_inspect_hardware_with_existing_ports(self, mock_port_create,
                                                   mock_get_drac_client):
         expected_node_properties = {
             'memory_mb': 32768,
             'local_gb': 1116,
-            'cpus': 2,
+            'cpus': 18,
             'cpu_arch': 'x86_64'}
         mock_client = mock.Mock()
         mock_get_drac_client.return_value = mock_client
         mock_client.list_memory.return_value = self.memory
         mock_client.list_cpus.return_value = self.cpus
         mock_client.list_virtual_disks.return_value = self.virtual_disks
         mock_client.list_nics.return_value = self.nics
@@ -255,7 +255,23 @@
     def test__guess_root_disk(self):
         with task_manager.acquire(self.context, self.node.uuid,
                                   shared=True) as task:
             root_disk = task.driver.inspect._guess_root_disk(
                 self.physical_disks)
 
             self.assertEqual(285888, root_disk.size_mb)
+
+    def test__calculate_cpus(self):
+        with task_manager.acquire(self.context, self.node.uuid,
+                                  shared=True) as task:
+            cpu = task.driver.inspect._calculate_cpus(
+                self.cpus[0])
+
+            self.assertEqual(12, cpu)
+
+    def test__calculate_cpus_without_ht_enabled(self):
+        with task_manager.acquire(self.context, self.node.uuid,
+                                  shared=True) as task:
+            cpu = task.driver.inspect._calculate_cpus(
+                self.cpus[1])
+
+            self.assertEqual(6, cpu)
```

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_common.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/drac/test_job.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/drac/test_job.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_deploy_utils.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_deploy_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_iscsi_deploy.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_iscsi_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1005,7 +1005,33 @@
             mock_get_deploy_image_info.assert_called_with(task.node)
             set_dhcp_provider_mock.assert_called_once_with()
             clean_dhcp_mock.assert_called_once_with(task)
         for path in ([self.kernel_path, self.image_path, self.config_path]
                      + self.files):
             self.assertFalse(os.path.exists(path),
                              '%s is not expected to exist' % path)
+
+
+class InstanceImageCacheTestCase(db_base.DbTestCase):
+    @mock.patch.object(fileutils, 'ensure_tree')
+    def test_with_master_path(self, mock_ensure_tree):
+        self.config(instance_master_path='/fake/path', group='pxe')
+        self.config(image_cache_size=500, group='pxe')
+        self.config(image_cache_ttl=30, group='pxe')
+
+        cache = iscsi_deploy.InstanceImageCache()
+
+        mock_ensure_tree.assert_called_once_with('/fake/path')
+        self.assertEqual(500 * 1024 * 1024, cache._cache_size)
+        self.assertEqual(30 * 60, cache._cache_ttl)
+
+    @mock.patch.object(fileutils, 'ensure_tree')
+    def test_without_master_path(self, mock_ensure_tree):
+        self.config(instance_master_path='', group='pxe')
+        self.config(image_cache_size=500, group='pxe')
+        self.config(image_cache_ttl=30, group='pxe')
+
+        cache = iscsi_deploy.InstanceImageCache()
+
+        mock_ensure_tree.assert_not_called()
+        self.assertEqual(500 * 1024 * 1024, cache._cache_size)
+        self.assertEqual(30 * 60, cache._cache_ttl)
```

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_power.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_power.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_management.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_management.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_inspect.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_deploy.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_deploy_utils.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_deploy_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/oneview/test_common.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/oneview/test_common.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_ipmitool.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_ipmitool.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/modules/test_inspector.py` & `ironic-9.1.7/ironic/tests/unit/drivers/modules/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_irmc.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_irmc.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/__init__.py` & `ironic-9.1.7/ironic/tests/unit/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_ilo.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_ilo.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_generic.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_generic.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config_boot_from_volume_no_volumes.template` & `ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config_boot_from_volume_no_volumes.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/boot.ipxe` & `ironic-9.1.7/ironic/tests/unit/drivers/boot.ipxe`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_utils.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_cisco.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_cisco.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/third_party_driver_mocks.py` & `ironic-9.1.7/ironic/tests/unit/drivers/third_party_driver_mocks.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config_boot_from_volume.template` & `ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config_boot_from_volume.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_fake.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_fake.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_oneview.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_oneview.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/test_drac.py` & `ironic-9.1.7/ironic/tests/unit/drivers/test_drac.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config_timeout.template` & `ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config_timeout.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/drivers/ipxe_config.template` & `ironic-9.1.7/ironic/tests/unit/drivers/ipxe_config.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conf/test_auth.py` & `ironic-9.1.7/ironic/tests/unit/conf/test_auth.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_base.py` & `ironic-9.1.7/ironic/tests/unit/api/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_ospmiddleware.py` & `ironic-9.1.7/ironic/tests/unit/api/test_ospmiddleware.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_acl.py` & `ironic-9.1.7/ironic/tests/unit/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/utils.py` & `ironic-9.1.7/ironic/tests/unit/api/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/base.py` & `ironic-9.1.7/ironic/tests/unit/api/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_audit.py` & `ironic-9.1.7/ironic/tests/unit/api/test_audit.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_hooks.py` & `ironic-9.1.7/ironic/tests/unit/api/test_hooks.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_middleware.py` & `ironic-9.1.7/ironic/tests/unit/api/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_versions.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_versions.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_ramdisk.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_ramdisk.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_drivers.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_drivers.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_ports.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_ports.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_portgroups.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_portgroups.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_chassis.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_chassis.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_volume_connectors.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_volume_connectors.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_volume_targets.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_volume_targets.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_volume.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_volume.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_types.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_types.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_expose.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_expose.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_utils.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_nodes.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_nodes.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_root.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_root.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/v1/test_notification_utils.py` & `ironic-9.1.7/ironic/tests/unit/api/v1/test_notification_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/api/test_root.py` & `ironic-9.1.7/ironic/tests/unit/api/test_root.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/__init__.py` & `ironic-9.1.7/ironic/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/cmd/test_conductor.py` & `ironic-9.1.7/ironic/tests/unit/cmd/test_conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/cmd/test_dbsync.py` & `ironic-9.1.7/ironic/tests/unit/cmd/test_dbsync.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test_base_manager.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test_base_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test_manager.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test_task_manager.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/mgr_utils.py` & `ironic-9.1.7/ironic/tests/unit/conductor/mgr_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test_utils.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1112,15 +1112,15 @@
         conductor_utils.cleanup_cleanwait_timeout(self.task)
 
         mock_error_handler.assert_called_once_with(
             self.task,
             msg="Timeout reached while cleaning the node. Please "
                 "check if the ramdisk responsible for the cleaning is "
                 "running on the node. Failed on step {}.",
-            set_fail_state=True)
+            set_fail_state=False)
 
     def test_cleanup_cleanwait_timeout(self):
         self.node.provision_state = states.CLEANFAIL
         target = 'baz'
         self.node.target_provision_state = target
         self.node.driver_internal_info = {}
         self.node.clean_step = {'key': 'val'}
@@ -1129,36 +1129,50 @@
                        "running on the node. Failed on step {'key': 'val'}.")
         self.node.driver_internal_info = {
             'cleaning_reboot': True,
             'clean_step_index': 0}
         conductor_utils.cleanup_cleanwait_timeout(self.task)
         self.assertEqual({}, self.node.clean_step)
         self.assertNotIn('clean_step_index', self.node.driver_internal_info)
-        self.task.process_event.assert_called_once_with('fail',
-                                                        target_state=None)
+        self.assertFalse(self.task.process_event.called)
         self.assertTrue(self.node.maintenance)
         self.assertEqual(clean_error, self.node.maintenance_reason)
 
-    def test_cleaning_error_handler(self):
-        self.node.provision_state = states.CLEANING
+    def _test_cleaning_error_handler(self, prov_state=states.CLEANING):
+        self.node.provision_state = prov_state
         target = 'baz'
         self.node.target_provision_state = target
-        self.node.driver_internal_info = {}
+        self.node.clean_step = {'key': 'val'}
+        self.node.driver_internal_info = {
+            'cleaning_reboot': True,
+            'clean_step_index': 0}
         msg = 'error bar'
         conductor_utils.cleaning_error_handler(self.task, msg)
         self.node.save.assert_called_once_with()
         self.assertEqual({}, self.node.clean_step)
         self.assertNotIn('clean_step_index', self.node.driver_internal_info)
         self.assertEqual(msg, self.node.last_error)
         self.assertTrue(self.node.maintenance)
         self.assertEqual(msg, self.node.maintenance_reason)
         driver = self.task.driver.deploy
         driver.tear_down_cleaning.assert_called_once_with(self.task)
-        self.task.process_event.assert_called_once_with('fail',
-                                                        target_state=None)
+        if prov_state == states.CLEANFAIL:
+            self.assertFalse(self.task.process_event.called)
+        else:
+            self.task.process_event.assert_called_once_with('fail',
+                                                            target_state=None)
+
+    def test_cleaning_error_handler(self):
+        self._test_cleaning_error_handler()
+
+    def test_cleaning_error_handler_cleanwait(self):
+        self._test_cleaning_error_handler(prov_state=states.CLEANWAIT)
+
+    def test_cleaning_error_handler_cleanfail(self):
+        self._test_cleaning_error_handler(prov_state=states.CLEANFAIL)
 
     def test_cleaning_error_handler_manual(self):
         target = states.MANAGEABLE
         self.node.target_provision_state = target
         conductor_utils.cleaning_error_handler(self.task, 'foo')
         self.task.process_event.assert_called_once_with('fail',
                                                         target_state=target)
```

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test__mgr_utils.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test__mgr_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test_rpcapi.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/conductor/test_notification_utils.py` & `ironic-9.1.7/ironic/tests/unit/conductor/test_notification_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_keystone.py` & `ironic-9.1.7/ironic/tests/unit/common/test_keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_states.py` & `ironic-9.1.7/ironic/tests/unit/common/test_states.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_driver_factory.py` & `ironic-9.1.7/ironic/tests/unit/common/test_driver_factory.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_hash_ring.py` & `ironic-9.1.7/ironic/tests/unit/common/test_hash_ring.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_neutron.py` & `ironic-9.1.7/ironic/tests/unit/common/test_neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_release_mappings.py` & `ironic-9.1.7/ironic/tests/unit/common/test_release_mappings.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_image_service.py` & `ironic-9.1.7/ironic/tests/unit/common/test_image_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_rpc.py` & `ironic-9.1.7/ironic/tests/unit/common/test_rpc.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_rpc_service.py` & `ironic-9.1.7/ironic/tests/unit/common/test_rpc_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_exception.py` & `ironic-9.1.7/ironic/tests/unit/common/test_exception.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_fsm.py` & `ironic-9.1.7/ironic/tests/unit/common/test_fsm.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_images.py` & `ironic-9.1.7/ironic/tests/unit/common/test_images.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_raid.py` & `ironic-9.1.7/ironic/tests/unit/common/test_raid.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_pxe_utils.py` & `ironic-9.1.7/ironic/tests/unit/common/test_pxe_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_wsgi_service.py` & `ironic-9.1.7/ironic/tests/unit/common/test_wsgi_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_cinder.py` & `ironic-9.1.7/ironic/tests/unit/common/test_cinder.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_glance_service.py` & `ironic-9.1.7/ironic/tests/unit/common/test_glance_service.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_network.py` & `ironic-9.1.7/ironic/tests/unit/common/test_network.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_policy.py` & `ironic-9.1.7/ironic/tests/unit/common/test_policy.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_utils.py` & `ironic-9.1.7/ironic/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_context.py` & `ironic-9.1.7/ironic/tests/unit/common/test_context.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/common/test_swift.py` & `ironic-9.1.7/ironic/tests/unit/common/test_swift.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/dhcp/test_factory.py` & `ironic-9.1.7/ironic/tests/unit/dhcp/test_factory.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/dhcp/test_neutron.py` & `ironic-9.1.7/ironic/tests/unit/dhcp/test_neutron.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/policy_fixture.py` & `ironic-9.1.7/ironic/tests/unit/policy_fixture.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/unit/raid_constants.py` & `ironic-9.1.7/ironic/tests/unit/raid_constants.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/tests/base.py` & `ironic-9.1.7/ironic/tests/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/locale/ko_KR/LC_MESSAGES/ironic-log-critical.po` & `ironic-9.1.7/ironic/locale/ko_KR/LC_MESSAGES/ironic-log-critical.po`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/locale/pt_BR/LC_MESSAGES/ironic-log-critical.po` & `ironic-9.1.7/ironic/locale/pt_BR/LC_MESSAGES/ironic-log-critical.po`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/locale/ja/LC_MESSAGES/ironic.po` & `ironic-9.1.7/ironic/locale/ja/LC_MESSAGES/ironic.po`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/locale/ja/LC_MESSAGES/ironic-log-critical.po` & `ironic-9.1.7/ironic/locale/ja/LC_MESSAGES/ironic-log-critical.po`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/locale/fr/LC_MESSAGES/ironic-log-info.po` & `ironic-9.1.7/ironic/locale/fr/LC_MESSAGES/ironic-log-info.po`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic/locale/fr/LC_MESSAGES/ironic-log-critical.po` & `ironic-9.1.7/ironic/locale/fr/LC_MESSAGES/ironic-log-critical.po`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/driver-requirements.txt` & `ironic-9.1.7/driver-requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-redfish-tinyipa/run.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -132,15 +132,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=1"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-agent_ipmitool-tinyipa-multinode/run.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -62,15 +62,15 @@
     - shell:
         cmd: |
           cat << 'EOF' >> ironic-extra-vars
             export DEVSTACK_GATE_OS_TEST_TIMEOUT=2400
           # networking-generic-switch requires sudo to execute ovs-vsctl commands
           export DEVSTACK_GATE_REMOVE_STACK_SUDO=0
           export PROJECTS="openstack/networking-generic-switch $PROJECTS"
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin networking-generic-switch git://git.openstack.org/openstack/networking-generic-switch"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin networking-generic-switch https://git.openstack.org/openstack/networking-generic-switch"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_USE_LINK_LOCAL=True"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"OVS_PHYSICAL_BRIDGE=brbm"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"PHYSICAL_NETWORK=mynetwork"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_PROVISION_NETWORK_NAME=ironic-provision"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_PROVISION_SUBNET_PREFIX=10.0.5.0/24"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_PROVISION_SUBNET_GATEWAY=10.0.5.1"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"Q_PLUGIN=ml2"
@@ -163,15 +163,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=7"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-pxe_ipmitool-postgres/run.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -150,15 +150,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=1"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-bfv/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-bfv/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -145,15 +145,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=3"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-inspector/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-inspector/run.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -61,15 +61,15 @@
     - shell:
         cmd: |
           cat << 'EOF' >> ironic-extra-vars
             export PROJECTS="openstack/ironic-inspector $PROJECTS"
           export PROJECTS="openstack/python-ironic-inspector-client $PROJECTS"
           export DEVSTACK_GATE_IRONIC_INSPECTOR=1
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic-inspector git://git.openstack.org/openstack/ironic-inspector"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic-inspector https://git.openstack.org/openstack/ironic-inspector"
 
           # use tempest plugin
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"TEMPEST_PLUGINS+=' /opt/stack/new/ironic-tempest-plugin'"
 
           export IRONIC_INSPECTOR_AUTO_DISCOVERY=0
           if [ "$IRONIC_INSPECTOR_AUTO_DISCOVERY" == "1" ]; then
                # discovery test requires sudo for iptables and virsh
@@ -164,15 +164,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=1"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic/run.yaml` & `ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -155,15 +155,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=7"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/ironic-dsvm-standalone/run.yaml` & `ironic-9.1.7/playbooks/legacy/ironic-dsvm-standalone/run.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -61,15 +61,15 @@
           export OVERRIDE_ENABLED_SERVICES="g-api,g-reg,q-agt,q-dhcp,q-l3,q-svc,key,mysql,rabbit,ir-api,ir-cond,s-account,s-container,s-object,s-proxy,tempest"
 
           export BRANCH_OVERRIDE="{{ zuul.override_checkout | default('default') }}"
           if [ "$BRANCH_OVERRIDE" != "default" ] ; then
               export OVERRIDE_ZUUL_BRANCH=$BRANCH_OVERRIDE
           fi
 
-          export DEVSTACK_LOCAL_CONFIG="enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG="enable_plugin ironic https://git.openstack.org/openstack/ironic"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=6"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_DEPLOY_DRIVER=agent_ipmitool"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"SWIFT_ENABLE_TEMPURLS=True"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"SWIFT_TEMPURL_KEY=secretkey"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_ENABLED_DRIVERS=fake,agent_ipmitool,pxe_ipmitool"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_AUTOMATED_CLEAN_ENABLED=False"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_USE_MOD_WSGI=True"
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-partition-uefi-pxe_ipmitool-tinyipa/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -132,15 +132,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=1"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-agent_ipmitool-tinyipa/run.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -128,15 +128,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=1"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/run.yaml` & `ironic-9.1.7/playbooks/legacy/grenade-dsvm-ironic-multinode-multitenant/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -70,15 +70,15 @@
     - shell:
         cmd: |
           cat << 'EOF' >> ironic-extra-vars
             export DEVSTACK_GATE_OS_TEST_TIMEOUT=2400
           # networking-generic-switch requires sudo to execute ovs-vsctl commands
           export DEVSTACK_GATE_REMOVE_STACK_SUDO=0
           export PROJECTS="openstack/networking-generic-switch $PROJECTS"
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin networking-generic-switch git://git.openstack.org/openstack/networking-generic-switch"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin networking-generic-switch https://git.openstack.org/openstack/networking-generic-switch"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_USE_LINK_LOCAL=True"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"OVS_PHYSICAL_BRIDGE=brbm"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"PHYSICAL_NETWORK=mynetwork"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_PROVISION_NETWORK_NAME=ironic-provision"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_PROVISION_SUBNET_PREFIX=10.0.5.0/24"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_PROVISION_SUBNET_GATEWAY=10.0.5.1"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"Q_PLUGIN=ml2"
@@ -193,15 +193,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=7"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/run.yaml` & `ironic-9.1.7/playbooks/legacy/tempest-dsvm-ironic-ipa-wholedisk-bios-pxe_snmp-tinyipa/run.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
@@ -132,15 +132,15 @@
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"IRONIC_VM_COUNT=1"
 
           # Ensure the ironic-vars-EARLY file exists
           touch ironic-vars-early
           # Pull in the EARLY variables injected by the optional builders
           source ironic-vars-early
 
-          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic git://git.openstack.org/openstack/ironic"
+          export DEVSTACK_LOCAL_CONFIG+=$'\n'"enable_plugin ironic https://git.openstack.org/openstack/ironic"
 
           # Ensure the ironic-EXTRA-vars file exists
           touch ironic-extra-vars
           # Pull in the EXTRA variables injected by the optional builders
           source ironic-extra-vars
 
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
```

### Comparing `ironic-9.1.6/README.rst` & `ironic-9.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ChangeLog` & `ironic-9.1.7/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+9.1.7
+-----
+
+* Revert "Fix OOB introspection to use pxe\_enabled flag in idrac driver"
+* Replace openstack.org git:// URLs with https://
+* Fix CPU count returned by introspection in Ironic iDRAC driver
+* Fix OOB introspection to use pxe\_enabled flag in idrac driver
+* Allow disabling instance image cache
+* Temporarily mark multinode job non-voting
+* Don't fail when node is in CLEANFAIL state
+
 9.1.6
 -----
 
 * Remove wrong install-guide-jobs in zuul setup
 * import zuul job settings from project-config
 * Fix iDRAC hardware type does not work with UEFI
 * Fix error when deleting a non-existent port
```

### Comparing `ironic-9.1.6/test-requirements.txt` & `ironic-9.1.7/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/Vagrantfile` & `ironic-9.1.7/Vagrantfile`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/AUTHORS` & `ironic-9.1.7/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 He Yongli <yongli.he@intel.com>
 Hieu LE <hieulq@vn.fujitsu.com>
 Hironori Shiina <shiina.hironori@jp.fujitsu.com>
 Honza Pokorny <honza@redhat.com>
 Hugo Nicodemos <hugonicodemos@gmail.com>
 Hugo Nicodemos <nicodemos@lsd.ufcg.edu.br>
 IWAMOTO Toshihiro <iwamoto@valinux.co.jp>
+Ian Wienand <iwienand@redhat.com>
 Igor Kalnitsky <igor@kalnitsky.org>
 Ihar Hrachyshka <ihrachys@redhat.com>
 Ilya Etingof <etingof@gmail.com>
 Ilya Pekelny <ipekelny@mirantis.com>
 Imre Farkas <ifarkas@redhat.com>
 Ionut Balutoiu <ibalutoiu@cloudbasesolutions.com>
 Jacek Tomasiak <jacek.tomasiak@gmail.com>
@@ -254,26 +255,28 @@
 Pádraig Brady <pbrady@redhat.com>
 R-Vaishnavi <itsvaishnavi@gmail.com>
 Rafi Khardalian <rafi@metacloud.com>
 Rakesh H S <rh-s@hp.com>
 Ramakrishnan G <rameshg87@gmail.com>
 Ramamani Yeleswarapu <ramamani.yeleswarapu@intel.com>
 Ricardo Araújo Santos <ricardo@lsd.ufcg.edu.br>
+Riccardo Pittau <elfosardo@gmail.com>
 Richard Pioso <richard.pioso@dell.com>
 Rick Harris <rconradharris@gmail.com>
 Robert Collins <rbtcollins@hp.com>
 Robert Collins <robertc@robertcollins.net>
 Rohan Kanade <openstack@rohankanade.com>
 Rohan Kanade <rohan.kanade@izeltech.com>
 Roman Bogorodskiy <rbogorodskiy@mirantis.com>
 Roman Dashevsky <dashevsky@selectel.ru>
 Roman Podoliaka <rpodolyaka@mirantis.com>
 Roman Prykhodchenko <me@romcheg.me>
 Roman Prykhodchenko <rprikhodchenko@mirantis.com>
 Ruby Loo <opensrloo@gmail.com>
+Ruby Loo <rloo@oath.com>
 Ruby Loo <rloo@yahoo-inc.com>
 Ruby Loo <ruby.loo@intel.com>
 Russell Bryant <rbryant@redhat.com>
 Russell Haering <russellhaering@gmail.com>
 Ryan Bridges <rybridges@oath.com>
 SHIGEMATSU Mitsuhiro <shigematsu.mitsuhiro@lab.ntt.co.jp>
 Sam Betts <sam@code-smash.net>
@@ -369,14 +372,15 @@
 anascko <ovoshchana@mirantis.com>
 baiyuan <bybai@cn.ibm.com>
 bin yu <froyo.bin@gmail.com>
 chenghang <cheng.hang@99cloud.net>
 chenglch <chenglch@cn.ibm.com>
 daz <dazzachan@yahoo.com.au>
 dekehn <dekehn@gmail.com>
+digambar <digambarpatil15@yahoo.co.in>
 divakar-padiyar-nandavar <divakar.padiyar-nandavar@hp.com>
 dparalen <vetrisko@gmail.com>
 ericxiett <eric_xiett@163.com>
 fpxie <fpxie@fiberhome.com>
 gaoxiaoyong <gaoxiaoyong@cn.fujitsu.com>
 gaozx <zxgao@fiberhome.com>
 gecong1973 <ge.cong@zte.com.cn>
```

### Comparing `ironic-9.1.6/ironic.egg-info/entry_points.txt` & `ironic-9.1.7/ironic.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic.egg-info/SOURCES.txt` & `ironic-9.1.7/ironic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -849,14 +849,15 @@
 releasenotes/notes/change-updated-at-object-field-a74466f7c4541072.yaml
 releasenotes/notes/check-dynamic-allocation-enabled-e94f3b8963b114d0.yaml
 releasenotes/notes/check-for-whole-disk-image-uefi-3bf2146588de2423.yaml
 releasenotes/notes/check_protocol_for_ironic_api-32f35c93a140d3ae.yaml
 releasenotes/notes/clean-nodes-stuck-in-cleaning-on-startup-443823ea4f937965.yaml
 releasenotes/notes/cleaning-retry-fix-89a5d0e65920a064.yaml
 releasenotes/notes/cleanup-provision-ports-before-retry-ec3c89c193766d70.yaml
+releasenotes/notes/cleanwait_timeout_fail-4323ba7d4d4da3e6.yaml
 releasenotes/notes/clear-hung-iscsi-sessions-d3b55c4c65fa4c8b.yaml
 releasenotes/notes/clear-node-target-power-state-de1f25be46d3e6d7.yaml
 releasenotes/notes/clear-target-stable-states-4545602d7aed9898.yaml
 releasenotes/notes/collect-deployment-logs-2ec1634847c3f6a5.yaml
 releasenotes/notes/conductor_early_import-fd29fa8b89089977.yaml
 releasenotes/notes/conf-debug-ipa-1d75e2283ca83395.yaml
 releasenotes/notes/config-drive-support-for-whole-disk-images-in-iscsi-deploy-0193c5222a7cd129.yaml
@@ -904,20 +905,22 @@
 releasenotes/notes/fix-api-node-name-updates-f3813295472795be.yaml
 releasenotes/notes/fix-baremetal-admin-user-not-neutron-admin-f163df90ab520dad.yaml
 releasenotes/notes/fix-boot-from-volume-for-iscsi-deploy-60bc0790ada62b26.yaml
 releasenotes/notes/fix-boot-from-volume-for-iscsi-deploy-71c1f2905498c50d.yaml
 releasenotes/notes/fix-bug-1675529-479357c217819420.yaml
 releasenotes/notes/fix-clean-steps-not-running-0d065cb022bc0419.yaml
 releasenotes/notes/fix-cleaning-spawn-error-60b60281f3be51c2.yaml
+releasenotes/notes/fix-cpu-count-8904a4e1a24456f4.yaml
 releasenotes/notes/fix-cve-2016-4985-b62abae577025365.yaml
 releasenotes/notes/fix-dir-permissions-bc56e83a651bbdb0.yaml
 releasenotes/notes/fix-disk-identifier-overwrite-42b33a5a0f7742d8.yaml
 releasenotes/notes/fix-get-deploy-info-port.yaml
 releasenotes/notes/fix-ilo-drivers-log-message-c3c64c1ca0a0bca8.yaml
 releasenotes/notes/fix-ilo-firmware-update-swift-path-with-pseudo-folder-0660345510ec0bb4.yaml
+releasenotes/notes/fix-instance-master-path-config-fa524c907a7888e5.yaml
 releasenotes/notes/fix-ipa-ephemeral-partition-1f1e020727a49078.yaml
 releasenotes/notes/fix-ipmi-numeric-password-75e080aa8bdfb9a2.yaml
 releasenotes/notes/fix-ipmitool-console-empty-password-a8edc5e2a1a7daf6.yaml
 releasenotes/notes/fix-ipxe-macro-4ae8bc4fe82e8f19.yaml
 releasenotes/notes/fix-ipxe-template-for-whole-disk-image-943da0311ca7aeb5.yaml
 releasenotes/notes/fix-keystone-parameters-cdb93576d7e7885b.yaml
 releasenotes/notes/fix-mac-address-48060f9e2847a38c.yaml
```

### Comparing `ironic-9.1.6/ironic.egg-info/requires.txt` & `ironic-9.1.7/ironic.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic.egg-info/PKG-INFO` & `ironic-9.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ironic
-Version: 9.1.6
+Version: 9.1.7
 Summary: OpenStack Bare Metal Provisioning
 Home-page: https://docs.openstack.org/ironic/latest/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `ironic-9.1.6/devstack/settings` & `ironic-9.1.7/devstack/settings`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/plugin.sh` & `ironic-9.1.7/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/common_settings` & `ironic-9.1.7/devstack/common_settings`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/files/apache-ironic-api-redirect.template` & `ironic-9.1.7/devstack/files/apache-ironic-api-redirect.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/files/hooks/qemu.py` & `ironic-9.1.7/devstack/files/hooks/qemu.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/files/apache-ironic-api.template` & `ironic-9.1.7/devstack/files/apache-ironic-api.template`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/files/debs/ironic` & `ironic-9.1.7/devstack/files/debs/ironic`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/upgrade/settings` & `ironic-9.1.7/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/upgrade/upgrade.sh` & `ironic-9.1.7/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/upgrade/resources.sh` & `ironic-9.1.7/devstack/upgrade/resources.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/tools/ironic/templates/vm.xml` & `ironic-9.1.7/devstack/tools/ironic/templates/vm.xml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/tools/ironic/scripts/setup-network.sh` & `ironic-9.1.7/devstack/tools/ironic/scripts/setup-network.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/tools/ironic/scripts/configure-vm.py` & `ironic-9.1.7/devstack/tools/ironic/scripts/configure-vm.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/tools/ironic/scripts/create-node.sh` & `ironic-9.1.7/devstack/tools/ironic/scripts/create-node.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/tools/ironic/scripts/cleanup-node.sh` & `ironic-9.1.7/devstack/tools/ironic/scripts/cleanup-node.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/devstack/lib/ironic` & `ironic-9.1.7/devstack/lib/ironic`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/cli/ironic-dbsync.rst` & `ironic-9.1.7/doc/source/cli/ironic-dbsync.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/configuration/sample-config.rst` & `ironic-9.1.7/doc/source/configuration/sample-config.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/enabling-drivers.rst` & `ironic-9.1.7/doc/source/install/enabling-drivers.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/install-ubuntu.rst` & `ironic-9.1.7/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/conf.py` & `ironic-9.1.7/doc/source/install/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/enabling-https.rst` & `ironic-9.1.7/doc/source/install/enabling-https.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/troubleshooting.rst` & `ironic-9.1.7/doc/source/install/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-tenant-networks.rst` & `ironic-9.1.7/doc/source/install/configure-tenant-networks.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-ipmi.rst` & `ironic-9.1.7/doc/source/install/configure-ipmi.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/install-obs.rst` & `ironic-9.1.7/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-glance-images.rst` & `ironic-9.1.7/doc/source/install/configure-glance-images.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/configure-ironic-api.rst` & `ironic-9.1.7/doc/source/install/include/configure-ironic-api.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/configure-ironic-api-mod_wsgi.rst` & `ironic-9.1.7/doc/source/install/include/configure-ironic-api-mod_wsgi.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/common-configure.rst` & `ironic-9.1.7/doc/source/install/include/common-configure.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/disk-label.rst` & `ironic-9.1.7/doc/source/install/include/disk-label.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/root-device-hints.rst` & `ironic-9.1.7/doc/source/install/include/root-device-hints.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/common-prerequisites.rst` & `ironic-9.1.7/doc/source/install/include/common-prerequisites.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/configure-ironic-conductor.rst` & `ironic-9.1.7/doc/source/install/include/configure-ironic-conductor.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/local-boot-partition-images.rst` & `ironic-9.1.7/doc/source/install/include/local-boot-partition-images.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/boot-mode.rst` & `ironic-9.1.7/doc/source/install/include/boot-mode.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/kernel-boot-parameters.rst` & `ironic-9.1.7/doc/source/install/include/kernel-boot-parameters.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/notifications.rst` & `ironic-9.1.7/doc/source/install/include/notifications.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/include/trusted-boot.rst` & `ironic-9.1.7/doc/source/install/include/trusted-boot.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-identity.rst` & `ironic-9.1.7/doc/source/install/configure-identity.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/standalone.rst` & `ironic-9.1.7/doc/source/install/standalone.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/deploy-ramdisk.rst` & `ironic-9.1.7/doc/source/install/deploy-ramdisk.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/enrollment.rst` & `ironic-9.1.7/doc/source/install/enrollment.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/install-rdo.rst` & `ironic-9.1.7/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/get_started.rst` & `ironic-9.1.7/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-glance-swift.rst` & `ironic-9.1.7/doc/source/install/configure-glance-swift.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-nova-flavors.rst` & `ironic-9.1.7/doc/source/install/configure-nova-flavors.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-pxe.rst` & `ironic-9.1.7/doc/source/install/configure-pxe.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-networking.rst` & `ironic-9.1.7/doc/source/install/configure-networking.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-compute.rst` & `ironic-9.1.7/doc/source/install/configure-compute.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configdrive.rst` & `ironic-9.1.7/doc/source/install/configdrive.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/configure-cleaning.rst` & `ironic-9.1.7/doc/source/install/configure-cleaning.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/install/index.rst` & `ironic-9.1.7/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/conf.py` & `ironic-9.1.7/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/deployment_architecture_2.png` & `ironic-9.1.7/doc/source/images/deployment_architecture_2.png`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/logical_architecture.png` & `ironic-9.1.7/doc/source/images/logical_architecture.png`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/states.svg` & `ironic-9.1.7/doc/source/images/states.svg`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/conceptual_architecture.png` & `ironic-9.1.7/doc/source/images/conceptual_architecture.png`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/deployment_steps.png` & `ironic-9.1.7/doc/source/images/deployment_steps.png`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/sample_trace_details.svg` & `ironic-9.1.7/doc/source/images/sample_trace_details.svg`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images/sample_trace.svg` & `ironic-9.1.7/doc/source/images/sample_trace.svg`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/user/index.rst` & `ironic-9.1.7/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/images_src/deployment_steps.svg` & `ironic-9.1.7/doc/source/images_src/deployment_steps.svg`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/code-contribution-guide.rst` & `ironic-9.1.7/doc/source/contributor/code-contribution-guide.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/governance.rst` & `ironic-9.1.7/doc/source/contributor/governance.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/vendor-passthru.rst` & `ironic-9.1.7/doc/source/contributor/vendor-passthru.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/dev-quickstart.rst` & `ironic-9.1.7/doc/source/contributor/dev-quickstart.rst`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     RABBIT_PASSWORD=password
     SERVICE_PASSWORD=password
     SERVICE_TOKEN=password
     SWIFT_HASH=password
     SWIFT_TEMPURL_KEY=password
 
     # Enable Ironic plugin
-    enable_plugin ironic git://git.openstack.org/openstack/ironic
+    enable_plugin ironic https://git.openstack.org/openstack/ironic
 
     # Enable Neutron which is required by Ironic and disable nova-network.
     disable_service n-net
     disable_service n-novnc
     enable_service q-svc
     enable_service q-agt
     enable_service q-dhcp
@@ -545,15 +545,15 @@
       sudo -u qemu touch $HOME/ironic-bm-logs/test.log
       # on Ubuntu
       sudo -u libvirt-qemu touch $HOME/ironic-bm-logs/test.log
 
 .. note::
     To check out an in-progress patch for testing, you can add a Git ref to the ``enable_plugin`` line. For instance::
 
-      enable_plugin ironic git://git.openstack.org/openstack/ironic refs/changes/46/295946/15
+      enable_plugin ironic https://git.openstack.org/openstack/ironic refs/changes/46/295946/15
 
     For a patch in review, you can find the ref to use by clicking the
     "Download" button in Gerrit. You can also specify a different git repo, or
     a branch or tag::
 
       enable_plugin ironic https://github.com/openstack/ironic stable/kilo
```

### Comparing `ironic-9.1.6/doc/source/contributor/webapi.rst` & `ironic-9.1.7/doc/source/contributor/webapi.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/ironic-multitenant-networking.rst` & `ironic-9.1.7/doc/source/contributor/ironic-multitenant-networking.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/webapi-version-history.rst` & `ironic-9.1.7/doc/source/contributor/webapi-version-history.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/drivers.rst` & `ironic-9.1.7/doc/source/contributor/drivers.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/osprofiler-support.rst` & `ironic-9.1.7/doc/source/contributor/osprofiler-support.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/architecture.rst` & `ironic-9.1.7/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/ironic-boot-from-volume.rst` & `ironic-9.1.7/doc/source/contributor/ironic-boot-from-volume.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 These connectors can be used to connect volumes created by cinder. The detailed
 description for DevStack is at :ref:`deploy_devstack`.
 
 ::
 
     [[local|localrc]]
 
-    enable_plugin ironic git://git.openstack.org/openstack/ironic
+    enable_plugin ironic https://git.openstack.org/openstack/ironic
 
     IRONIC_STORAGE_INTERFACE=cinder
 
     # Credentials
     ADMIN_PASSWORD=password
     DATABASE_PASSWORD=password
     RABBIT_PASSWORD=password
```

### Comparing `ironic-9.1.6/doc/source/contributor/releasing.rst` & `ironic-9.1.7/doc/source/contributor/releasing.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/notifications.rst` & `ironic-9.1.7/doc/source/contributor/notifications.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/faq.rst` & `ironic-9.1.7/doc/source/contributor/faq.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/third-party-ci.rst` & `ironic-9.1.7/doc/source/contributor/third-party-ci.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/index.rst` & `ironic-9.1.7/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/contributor/states.rst` & `ironic-9.1.7/doc/source/contributor/states.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/index.rst` & `ironic-9.1.7/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/radosgw.rst` & `ironic-9.1.7/doc/source/admin/radosgw.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/multitenancy.rst` & `ironic-9.1.7/doc/source/admin/multitenancy.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/troubleshooting.rst` & `ironic-9.1.7/doc/source/admin/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/console.rst` & `ironic-9.1.7/doc/source/admin/console.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/cimc.rst` & `ironic-9.1.7/doc/source/admin/drivers/cimc.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/oneview.rst` & `ironic-9.1.7/doc/source/admin/drivers/oneview.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/ipmitool.rst` & `ironic-9.1.7/doc/source/admin/drivers/ipmitool.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/ipa.rst` & `ironic-9.1.7/doc/source/admin/drivers/ipa.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/ilo.rst` & `ironic-9.1.7/doc/source/admin/drivers/ilo.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/snmp.rst` & `ironic-9.1.7/doc/source/admin/drivers/snmp.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/ucs.rst` & `ironic-9.1.7/doc/source/admin/drivers/ucs.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/redfish.rst` & `ironic-9.1.7/doc/source/admin/drivers/redfish.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/pxe.rst` & `ironic-9.1.7/doc/source/admin/drivers/pxe.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers/irmc.rst` & `ironic-9.1.7/doc/source/admin/drivers/irmc.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/cleaning.rst` & `ironic-9.1.7/doc/source/admin/cleaning.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/drivers.rst` & `ironic-9.1.7/doc/source/admin/drivers.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/inspection.rst` & `ironic-9.1.7/doc/source/admin/inspection.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/security.rst` & `ironic-9.1.7/doc/source/admin/security.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/raid.rst` & `ironic-9.1.7/doc/source/admin/raid.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/report.txt` & `ironic-9.1.7/doc/source/admin/report.txt`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/upgrade-guide.rst` & `ironic-9.1.7/doc/source/admin/upgrade-guide.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/notifications.rst` & `ironic-9.1.7/doc/source/admin/notifications.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/adoption.rst` & `ironic-9.1.7/doc/source/admin/adoption.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/boot-from-volume.rst` & `ironic-9.1.7/doc/source/admin/boot-from-volume.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/gmr.rst` & `ironic-9.1.7/doc/source/admin/gmr.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/index.rst` & `ironic-9.1.7/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/portgroups.rst` & `ironic-9.1.7/doc/source/admin/portgroups.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/api-audit-support.rst` & `ironic-9.1.7/doc/source/admin/api-audit-support.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/metrics.rst` & `ironic-9.1.7/doc/source/admin/metrics.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/doc/source/admin/upgrade-to-hardware-types.rst` & `ironic-9.1.7/doc/source/admin/upgrade-to-hardware-types.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/LICENSE` & `ironic-9.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/requirements.txt` & `ironic-9.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/vagrant.yaml` & `ironic-9.1.7/vagrant.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/setup.py` & `ironic-9.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/zuul.d/legacy-ironic-jobs.yaml` & `ironic-9.1.7/zuul.d/legacy-ironic-jobs.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/etc/ironic/rootwrap.d/ironic-lib.filters` & `ironic-9.1.7/etc/ironic/rootwrap.d/ironic-lib.filters`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/etc/ironic/api_audit_map.conf.sample` & `ironic-9.1.7/etc/ironic/api_audit_map.conf.sample`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/etc/ironic/policy.json.sample` & `ironic-9.1.7/etc/ironic/policy.json.sample`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/etc/ironic/rootwrap.conf` & `ironic-9.1.7/etc/ironic/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/etc/ironic/ironic.conf.sample` & `ironic-9.1.7/etc/ironic/ironic.conf.sample`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/etc/apache2/ironic` & `ironic-9.1.7/etc/apache2/ironic`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/source/conf.py` & `ironic-9.1.7/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/source/liberty.rst` & `ironic-9.1.7/releasenotes/source/liberty.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/ipa-streams-raw-images-1010327b0dad763c.yaml` & `ironic-9.1.7/releasenotes/notes/ipa-streams-raw-images-1010327b0dad763c.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/mask-configdrive-contents-77fc557d6bc63b2b.yaml` & `ironic-9.1.7/releasenotes/notes/mask-configdrive-contents-77fc557d6bc63b2b.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/shred-final-overwrite-with-zeros-50b5ba5b19c0da27.yaml` & `ironic-9.1.7/releasenotes/notes/shred-final-overwrite-with-zeros-50b5ba5b19c0da27.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/erase-devices-metadata-config-f39b6ca415a87757.yaml` & `ironic-9.1.7/releasenotes/notes/erase-devices-metadata-config-f39b6ca415a87757.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/no-root-device-as-kernel-param-5e5326acae7b77a4.yaml` & `ironic-9.1.7/releasenotes/notes/no-root-device-as-kernel-param-5e5326acae7b77a4.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/newton-driver-deprecations-e40369be37203057.yaml` & `ironic-9.1.7/releasenotes/notes/newton-driver-deprecations-e40369be37203057.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/rely-on-standalone-ports-supported-8153e1135787828b.yaml` & `ironic-9.1.7/releasenotes/notes/rely-on-standalone-ports-supported-8153e1135787828b.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/enable-osprofiler-support-e3839b0fa90d3831.yaml` & `ironic-9.1.7/releasenotes/notes/enable-osprofiler-support-e3839b0fa90d3831.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/bug-1694645-57289200e35bd883.yaml` & `ironic-9.1.7/releasenotes/notes/bug-1694645-57289200e35bd883.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/port-physical-network-a7009dc514353796.yaml` & `ironic-9.1.7/releasenotes/notes/port-physical-network-a7009dc514353796.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/added-redfish-driver-00ff5e3f7e9d6ee8.yaml` & `ironic-9.1.7/releasenotes/notes/added-redfish-driver-00ff5e3f7e9d6ee8.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-agent-erase-fallback-b07613a7042fe236.yaml` & `ironic-9.1.7/releasenotes/notes/add-agent-erase-fallback-b07613a7042fe236.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-snmp-inspection-support-e68fd6d57cb33846.yaml` & `ironic-9.1.7/releasenotes/notes/add-snmp-inspection-support-e68fd6d57cb33846.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/lookup-heartbeat-f9772521d12a0549.yaml` & `ironic-9.1.7/releasenotes/notes/lookup-heartbeat-f9772521d12a0549.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/remove-deprecated-dhcp-provider-methods-582742f3000be3c7.yaml` & `ironic-9.1.7/releasenotes/notes/remove-deprecated-dhcp-provider-methods-582742f3000be3c7.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/deprecate-dhcp-update-mac-address-f12a4959432c8e20.yaml` & `ironic-9.1.7/releasenotes/notes/deprecate-dhcp-update-mac-address-f12a4959432c8e20.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/configdrive-support-using-ceph-radosgw-8c6f7b8bede2077c.yaml` & `ironic-9.1.7/releasenotes/notes/configdrive-support-using-ceph-radosgw-8c6f7b8bede2077c.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/security_groups-b57a5d6c30c2fae4.yaml` & `ironic-9.1.7/releasenotes/notes/security_groups-b57a5d6c30c2fae4.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/multi-arch-deploy-bcf840107fc94bef.yaml` & `ironic-9.1.7/releasenotes/notes/multi-arch-deploy-bcf840107fc94bef.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/volume-connector-and-target-api-dd172f121ab3af8e.yaml` & `ironic-9.1.7/releasenotes/notes/volume-connector-and-target-api-dd172f121ab3af8e.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/remove-agent-passthru-432b18e6c430cee6.yaml` & `ironic-9.1.7/releasenotes/notes/remove-agent-passthru-432b18e6c430cee6.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/ipxe-use-swift-5ccf490daab809cc.yaml` & `ironic-9.1.7/releasenotes/notes/ipxe-use-swift-5ccf490daab809cc.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/resources-crud-notifications-70cba9f761da3afe.yaml` & `ironic-9.1.7/releasenotes/notes/resources-crud-notifications-70cba9f761da3afe.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-vif-attach-detach-support-99eca43eea6e5a30.yaml` & `ironic-9.1.7/releasenotes/notes/add-vif-attach-detach-support-99eca43eea6e5a30.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/new_capabilities-5241619c4b46a460.yaml` & `ironic-9.1.7/releasenotes/notes/new_capabilities-5241619c4b46a460.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-choice-to-some-options-9fb327c48e6bfda1.yaml` & `ironic-9.1.7/releasenotes/notes/add-choice-to-some-options-9fb327c48e6bfda1.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/net-names-b8a36aa30659ce2f.yaml` & `ironic-9.1.7/releasenotes/notes/net-names-b8a36aa30659ce2f.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/resource-classes-1bf903547236a473.yaml` & `ironic-9.1.7/releasenotes/notes/resource-classes-1bf903547236a473.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/implement-policy-in-code-cbb0216ef5f8224f.yaml` & `ironic-9.1.7/releasenotes/notes/implement-policy-in-code-cbb0216ef5f8224f.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-db-deadlock-handling-6bc10076537f3727.yaml` & `ironic-9.1.7/releasenotes/notes/add-db-deadlock-handling-6bc10076537f3727.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/bug-1506657-3bcb4ef46623124d.yaml` & `ironic-9.1.7/releasenotes/notes/bug-1506657-3bcb4ef46623124d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/fix-bug-1675529-479357c217819420.yaml` & `ironic-9.1.7/releasenotes/notes/fix-bug-1675529-479357c217819420.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/active-node-creation-a41c9869c966c82b.yaml` & `ironic-9.1.7/releasenotes/notes/active-node-creation-a41c9869c966c82b.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/idrac-hardware-type-54383960af3459d0.yaml` & `ironic-9.1.7/releasenotes/notes/idrac-hardware-type-54383960af3459d0.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/drac-raid-interface-f4c02b1c4fb37e2d.yaml` & `ironic-9.1.7/releasenotes/notes/drac-raid-interface-f4c02b1c4fb37e2d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add_portgroup_support-7d5c6663bb00684a.yaml` & `ironic-9.1.7/releasenotes/notes/add_portgroup_support-7d5c6663bb00684a.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/multitenant-networking-0a13c4aba252573e.yaml` & `ironic-9.1.7/releasenotes/notes/multitenant-networking-0a13c4aba252573e.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/collect-deployment-logs-2ec1634847c3f6a5.yaml` & `ironic-9.1.7/releasenotes/notes/collect-deployment-logs-2ec1634847c3f6a5.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/remove-most-unsupported-049f3401c2554a3c.yaml` & `ironic-9.1.7/releasenotes/notes/remove-most-unsupported-049f3401c2554a3c.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/dynamic-driver-list-show-apis-235e9fca26fc580d.yaml` & `ironic-9.1.7/releasenotes/notes/dynamic-driver-list-show-apis-235e9fca26fc580d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-node-resource-class-c31e26df4196293e.yaml` & `ironic-9.1.7/releasenotes/notes/add-node-resource-class-c31e26df4196293e.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/ilo-inconsistent-default-boot-mode-ef5a7c56372f89f1.yaml` & `ironic-9.1.7/releasenotes/notes/ilo-inconsistent-default-boot-mode-ef5a7c56372f89f1.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/futurist-e9c55699f479f97a.yaml` & `ironic-9.1.7/releasenotes/notes/futurist-e9c55699f479f97a.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/ilo-hardware-type-48fd1c8bccd70659.yaml` & `ironic-9.1.7/releasenotes/notes/ilo-hardware-type-48fd1c8bccd70659.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-agent-proxy-support-790e629634ca2eb7.yaml` & `ironic-9.1.7/releasenotes/notes/add-agent-proxy-support-790e629634ca2eb7.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/irmc-add-clean-step-reset-bios-config-a8bed625670b7fdf.yaml` & `ironic-9.1.7/releasenotes/notes/irmc-add-clean-step-reset-bios-config-a8bed625670b7fdf.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/refactor-ironic-lib-22939896d8d46a77.yaml` & `ironic-9.1.7/releasenotes/notes/refactor-ironic-lib-22939896d8d46a77.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/bug-1702158-79bf57bd4d8087b6.yaml` & `ironic-9.1.7/releasenotes/notes/bug-1702158-79bf57bd4d8087b6.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/fix-cve-2016-4985-b62abae577025365.yaml` & `ironic-9.1.7/releasenotes/notes/fix-cve-2016-4985-b62abae577025365.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-dynamic-allocation-feature-2fd6b4df7943f178.yaml` & `ironic-9.1.7/releasenotes/notes/add-dynamic-allocation-feature-2fd6b4df7943f178.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/keystone-auth-3155762c524e44df.yaml` & `ironic-9.1.7/releasenotes/notes/keystone-auth-3155762c524e44df.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/oslopolicy-scripts-bdcaeaf7dd9ce2ac.yaml` & `ironic-9.1.7/releasenotes/notes/oslopolicy-scripts-bdcaeaf7dd9ce2ac.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/drac-migrate-to-dracclient-2bd8a6d1dd3fdc69.yaml` & `ironic-9.1.7/releasenotes/notes/drac-migrate-to-dracclient-2bd8a6d1dd3fdc69.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/notify-node-storage-interface-7fd07ee7ee71cd22.yaml` & `ironic-9.1.7/releasenotes/notes/notify-node-storage-interface-7fd07ee7ee71cd22.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/pike-prelude-815f73ba4ad59f97.yaml` & `ironic-9.1.7/releasenotes/notes/pike-prelude-815f73ba4ad59f97.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/remove-deprecated-dhcp-provider-method-89926a8f0f4793a4.yaml` & `ironic-9.1.7/releasenotes/notes/remove-deprecated-dhcp-provider-method-89926a8f0f4793a4.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/create-on-conductor-c1c52a1f022c4048.yaml` & `ironic-9.1.7/releasenotes/notes/create-on-conductor-c1c52a1f022c4048.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/resource-class-change-563797d5a3c35683.yaml` & `ironic-9.1.7/releasenotes/notes/resource-class-change-563797d5a3c35683.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/remove-agent-passthru-complete-a6b2df65b95889d5.yaml` & `ironic-9.1.7/releasenotes/notes/remove-agent-passthru-complete-a6b2df65b95889d5.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/add-cisco-ucs-hardware-types-ee597ff0416f158f.yaml` & `ironic-9.1.7/releasenotes/notes/add-cisco-ucs-hardware-types-ee597ff0416f158f.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/pike-upgrade-fix-85091d0320ed273a.yaml` & `ironic-9.1.7/releasenotes/notes/pike-upgrade-fix-85091d0320ed273a.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/idrac-uefi-boot-mode-86f4694b4247a1ca.yaml` & `ironic-9.1.7/releasenotes/notes/idrac-uefi-boot-mode-86f4694b4247a1ca.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/amt-driver-wake-up-0880ed85476968be.yaml` & `ironic-9.1.7/releasenotes/notes/amt-driver-wake-up-0880ed85476968be.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/ocata-summary-a70f995cb3b18e18.yaml` & `ironic-9.1.7/releasenotes/notes/ocata-summary-a70f995cb3b18e18.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/fix-rpc-exceptions-12c70eb6ba177e39.yaml` & `ironic-9.1.7/releasenotes/notes/fix-rpc-exceptions-12c70eb6ba177e39.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/releasenotes/notes/node-storage-interface-api-1d6e217303bd53ff.yaml` & `ironic-9.1.7/releasenotes/notes/node-storage-interface-api-1d6e217303bd53ff.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/tox.ini` & `ironic-9.1.7/tox.ini`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-chassis.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-chassis.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-drivers.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-drivers.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-vifs.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-vifs.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-portgroups.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-portgroups.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/conf.py` & `ironic-9.1.7/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-volume.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-volume.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-portgroups.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-portgroups.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-versions.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-versions.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-node-management.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-node-management.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-portgroups-ports.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-portgroups-ports.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/parameters.yaml` & `ironic-9.1.7/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-volume.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-volume.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-ports.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-ports.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-nodes-ports.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-nodes-ports.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-node-passthru.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-node-passthru.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/index.rst` & `ironic-9.1.7/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-driver-passthru.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-driver-passthru.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/baremetal-api-v1-misc.inc` & `ironic-9.1.7/api-ref/source/baremetal-api-v1-misc.inc`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-target-list-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-target-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-create-response.json` & `ironic-9.1.7/api-ref/source/samples/node-create-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/nodes-list-details-response.json` & `ironic-9.1.7/api-ref/source/samples/nodes-list-details-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-target-create-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-target-create-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/lookup-node-response.json` & `ironic-9.1.7/api-ref/source/samples/lookup-node-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/chassis-list-details-response.json` & `ironic-9.1.7/api-ref/source/samples/chassis-list-details-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/api-v1-root-response.json` & `ironic-9.1.7/api-ref/source/samples/api-v1-root-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/drivers-list-response.json` & `ironic-9.1.7/api-ref/source/samples/drivers-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/portgroup-update-response.json` & `ironic-9.1.7/api-ref/source/samples/portgroup-update-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-list-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-target-list-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-target-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/drivers-list-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/drivers-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/api-root-response.json` & `ironic-9.1.7/api-ref/source/samples/api-root-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/nodes-list-response.json` & `ironic-9.1.7/api-ref/source/samples/nodes-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/chassis-update-response.json` & `ironic-9.1.7/api-ref/source/samples/chassis-update-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/port-list-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/port-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-update-driver-info-response.json` & `ironic-9.1.7/api-ref/source/samples/node-update-driver-info-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-show-response.json` & `ironic-9.1.7/api-ref/source/samples/node-show-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-connector-create-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-connector-create-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/chassis-show-response.json` & `ironic-9.1.7/api-ref/source/samples/chassis-show-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-target-update-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-target-update-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-volume-connector-list-response.json` & `ironic-9.1.7/api-ref/source/samples/node-volume-connector-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-connector-update-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-connector-update-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-volume-target-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/node-volume-target-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/port-update-response.json` & `ironic-9.1.7/api-ref/source/samples/port-update-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/portgroup-list-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/portgroup-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-connector-list-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-connector-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/portgroup-create-response.json` & `ironic-9.1.7/api-ref/source/samples/portgroup-create-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-port-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/portgroup-port-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/port-create-response.json` & `ironic-9.1.7/api-ref/source/samples/port-create-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-volume-list-response.json` & `ironic-9.1.7/api-ref/source/samples/node-volume-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-volume-connector-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/node-volume-connector-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-portgroup-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/node-portgroup-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/driver-property-response.json` & `ironic-9.1.7/api-ref/source/samples/driver-property-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/node-volume-target-list-response.json` & `ironic-9.1.7/api-ref/source/samples/node-volume-target-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/volume-connector-list-response.json` & `ironic-9.1.7/api-ref/source/samples/volume-connector-list-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/portgroup-port-detail-response.json` & `ironic-9.1.7/api-ref/source/samples/node-port-detail-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/driver-logical-disk-properties-response.json` & `ironic-9.1.7/api-ref/source/samples/driver-logical-disk-properties-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/source/samples/driver-get-response.json` & `ironic-9.1.7/api-ref/source/samples/driver-get-response.json`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/api-ref/regenerate-samples.sh` & `ironic-9.1.7/api-ref/regenerate-samples.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/manager.py` & `ironic-9.1.7/ironic_tempest_plugin/manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/README.rst` & `ironic-9.1.7/ironic_tempest_plugin/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/config.py` & `ironic-9.1.7/ironic_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/common/utils.py` & `ironic-9.1.7/ironic_tempest_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/common/waiters.py` & `ironic-9.1.7/ironic_tempest_plugin/common/waiters.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/services/baremetal/base.py` & `ironic-9.1.7/ironic_tempest_plugin/services/baremetal/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/services/baremetal/v1/json/baremetal_client.py` & `ironic-9.1.7/ironic_tempest_plugin/services/baremetal/v1/json/baremetal_client.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/plugin.py` & `ironic-9.1.7/ironic_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_nodestates.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_nodestates.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_drivers.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_drivers.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_ports.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_ports.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_ports_negative.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_ports_negative.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_portgroups.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_portgroups.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_chassis.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_chassis.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_volume_target.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_volume_target.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/base.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/base.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/api_microversion_fixture.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/api_microversion_fixture.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_volume_connector.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_volume_connector.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_nodes.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_nodes.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/api/admin/test_api_discovery.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/api/admin/test_api_discovery.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/scenario/baremetal_manager.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/scenario/baremetal_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/scenario/ironic_standalone/test_basic_ops.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/scenario/ironic_standalone/test_basic_ops.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/scenario/test_baremetal_basic_ops.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/scenario/test_baremetal_basic_ops.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/scenario/test_baremetal_multitenancy.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/scenario/test_baremetal_multitenancy.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/scenario/test_baremetal_boot_from_volume.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/scenario/test_baremetal_boot_from_volume.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/tests/scenario/baremetal_standalone_manager.py` & `ironic-9.1.7/ironic_tempest_plugin/tests/scenario/baremetal_standalone_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/ironic_tempest_plugin/clients.py` & `ironic-9.1.7/ironic_tempest_plugin/clients.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/PKG-INFO` & `ironic-9.1.7/ironic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ironic
-Version: 9.1.6
+Version: 9.1.7
 Summary: OpenStack Bare Metal Provisioning
 Home-page: https://docs.openstack.org/ironic/latest/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `ironic-9.1.6/tools/states_to_dot.py` & `ironic-9.1.7/tools/states_to_dot.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/tools/run_bashate.sh` & `ironic-9.1.7/tools/run_bashate.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/tools/check-releasenotes.py` & `ironic-9.1.7/tools/check-releasenotes.py`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/tools/config/ironic-config-generator.conf` & `ironic-9.1.7/tools/config/ironic-config-generator.conf`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/tools/config/check_uptodate.sh` & `ironic-9.1.7/tools/config/check_uptodate.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/tools/test-setup.sh` & `ironic-9.1.7/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `ironic-9.1.6/setup.cfg` & `ironic-9.1.7/setup.cfg`

 * *Files identical despite different names*

