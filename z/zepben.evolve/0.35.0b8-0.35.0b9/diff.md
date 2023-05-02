# Comparing `tmp/zepben.evolve-0.35.0b8-py3-none-any.whl.zip` & `tmp/zepben.evolve-0.35.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,304 +1,321 @@
-Zip file size: 395476 bytes, number of entries: 302
--rw-r--r--  2.0 unx    17077 b- defN 23-Jan-09 04:58 zepben/evolve/__init__.py
--rw-r--r--  2.0 unx     1387 b- defN 23-Jan-09 04:58 zepben/evolve/exceptions.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Jan-09 04:58 zepben/evolve/types.py
--rw-r--r--  2.0 unx     4576 b- defN 23-Jan-09 04:58 zepben/evolve/util.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/__init__.py
--rw-r--r--  2.0 unx     6640 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/database_reader.py
--rw-r--r--  2.0 unx     5803 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/database_writer.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/__init__.py
--rw-r--r--  2.0 unx     5319 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/base_cim_reader.py
--rw-r--r--  2.0 unx     2991 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/base_service_reader.py
--rw-r--r--  2.0 unx     4510 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/customer_cim_reader.py
--rw-r--r--  2.0 unx     1761 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/customer_service_reader.py
--rw-r--r--  2.0 unx     3245 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/diagram_cim_reader.py
--rw-r--r--  2.0 unx     1041 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/diagram_service_reader.py
--rw-r--r--  2.0 unx      733 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/metadata_collection_reader.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/metadata_entry_reader.py
--rw-r--r--  2.0 unx    68283 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/network_cim_reader.py
--rw-r--r--  2.0 unx    11437 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/network_service_reader.py
--rw-r--r--  2.0 unx     6872 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/readers/result_set.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/__init__.py
--rw-r--r--  2.0 unx     1009 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/column.py
--rw-r--r--  2.0 unx    11385 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/database_tables.py
--rw-r--r--  2.0 unx      403 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/exceptions.py
--rw-r--r--  2.0 unx     1164 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/metadata_tables.py
--rw-r--r--  2.0 unx     5820 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/sqlite_table.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/__init__.py
--rw-r--r--  2.0 unx     1484 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py
--rw-r--r--  2.0 unx     2295 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py
--rw-r--r--  2.0 unx     1561 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py
--rw-r--r--  2.0 unx     3547 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py
--rw-r--r--  2.0 unx     1696 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py
--rw-r--r--  2.0 unx     1435 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py
--rw-r--r--  2.0 unx     1409 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/__init__.py
--rw-r--r--  2.0 unx     2240 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py
--rw-r--r--  2.0 unx     8739 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py
--rw-r--r--  2.0 unx     5681 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/common_tables.py
--rw-r--r--  2.0 unx     1705 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py
--rw-r--r--  2.0 unx     1629 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py
--rw-r--r--  2.0 unx      494 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py
--rw-r--r--  2.0 unx     3669 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py
--rw-r--r--  2.0 unx     1995 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py
--rw-r--r--  2.0 unx     8308 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py
--rw-r--r--  2.0 unx     3113 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py
--rw-r--r--  2.0 unx     2454 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py
--rw-r--r--  2.0 unx     2581 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py
--rw-r--r--  2.0 unx     1205 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/__init__.py
--rw-r--r--  2.0 unx     1515 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/feeder_tables.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py
--rw-r--r--  2.0 unx      710 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py
--rw-r--r--  2.0 unx      458 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py
--rw-r--r--  2.0 unx    10492 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py
--rw-r--r--  2.0 unx     1845 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py
--rw-r--r--  2.0 unx     1659 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py
--rw-r--r--  2.0 unx     7441 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py
--rw-r--r--  2.0 unx     2114 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/__init__.py
--rw-r--r--  2.0 unx     5254 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/base_cim_writer.py
--rw-r--r--  2.0 unx     2995 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/base_service_writer.py
--rw-r--r--  2.0 unx     4748 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/customer_cim_writer.py
--rw-r--r--  2.0 unx     1393 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/customer_service_writer.py
--rw-r--r--  2.0 unx     2654 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/diagram_cim_writer.py
--rw-r--r--  2.0 unx     1004 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/diagram_service_writer.py
--rw-r--r--  2.0 unx      904 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/metadata_collection_writer.py
--rw-r--r--  2.0 unx     1257 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/metadata_entry_writer.py
--rw-r--r--  2.0 unx    65924 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/network_cim_writer.py
--rw-r--r--  2.0 unx     7983 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/network_service_writer.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jan-09 04:58 zepben/evolve/database/sqlite/writers/utils.py
--rw-r--r--  2.0 unx      309 b- defN 23-Jan-09 04:58 zepben/evolve/examples/__init__.py
--rw-r--r--  2.0 unx     6937 b- defN 23-Jan-09 04:58 zepben/evolve/examples/simple_node_breaker_feeder.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/__init__.py
--rw-r--r--  2.0 unx     7357 b- defN 23-Jan-09 04:58 zepben/evolve/model/phases.py
--rw-r--r--  2.0 unx     1502 b- defN 23-Jan-09 04:58 zepben/evolve/model/resistance_reactance.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/model/busbranch/__init__.py
--rw-r--r--  2.0 unx    47087 b- defN 23-Jan-09 04:58 zepben/evolve/model/busbranch/bus_branch.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/__init__.py
--rw-r--r--  2.0 unx     1398 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py
--rw-r--r--  2.0 unx     1445 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py
--rw-r--r--  2.0 unx     3555 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py
--rw-r--r--  2.0 unx     1877 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py
--rw-r--r--  2.0 unx      927 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py
--rw-r--r--  2.0 unx     5904 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py
--rw-r--r--  2.0 unx     3736 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py
--rw-r--r--  2.0 unx      860 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py
--rw-r--r--  2.0 unx     1287 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/__init__.py
--rw-r--r--  2.0 unx     4019 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/asset.py
--rw-r--r--  2.0 unx      845 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/asset_info.py
--rw-r--r--  2.0 unx      588 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py
--rw-r--r--  2.0 unx     3009 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/pole.py
--rw-r--r--  2.0 unx     1157 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/streetlight.py
--rw-r--r--  2.0 unx      635 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/assets/structure.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/common/__init__.py
--rw-r--r--  2.0 unx     1570 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/common/document.py
--rw-r--r--  2.0 unx     7841 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/common/location.py
--rw-r--r--  2.0 unx      531 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/common/organisation.py
--rw-r--r--  2.0 unx      838 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/common/organisation_role.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/customers/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/customers/customer.py
--rw-r--r--  2.0 unx     4260 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/customers/customer_agreement.py
--rw-r--r--  2.0 unx     1474 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/customers/customer_kind.py
--rw-r--r--  2.0 unx     3336 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/customers/pricing_structure.py
--rw-r--r--  2.0 unx      763 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/customers/tariff.py
--rw-r--r--  2.0 unx      244 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/__init__.py
--rw-r--r--  2.0 unx      244 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py
--rw-r--r--  2.0 unx     1859 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py
--rw-r--r--  2.0 unx     1250 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py
--rw-r--r--  2.0 unx      993 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py
--rw-r--r--  2.0 unx     1202 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/metering/__init__.py
--rw-r--r--  2.0 unx    11019 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/metering/metering.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/operations/__init__.py
--rw-r--r--  2.0 unx     3889 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61968/operations/operational_restriction.py
--rw-r--r--  2.0 unx      248 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/__init__.py
--rw-r--r--  2.0 unx      249 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py
--rw-r--r--  2.0 unx     1475 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py
--rw-r--r--  2.0 unx     1489 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py
--rw-r--r--  2.0 unx     1753 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py
--rw-r--r--  2.0 unx      811 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py
--rw-r--r--  2.0 unx      588 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/__init__.py
--rw-r--r--  2.0 unx      556 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/base_voltage.py
--rw-r--r--  2.0 unx     7135 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py
--rw-r--r--  2.0 unx     3645 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py
--rw-r--r--  2.0 unx      592 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py
--rw-r--r--  2.0 unx    14056 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/equipment.py
--rw-r--r--  2.0 unx    15618 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/equipment_container.py
--rw-r--r--  2.0 unx     6735 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/identified_object.py
--rw-r--r--  2.0 unx     1095 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/name.py
--rw-r--r--  2.0 unx     5023 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/name_type.py
--rw-r--r--  2.0 unx     6187 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/phase_code.py
--rw-r--r--  2.0 unx     1250 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py
--rw-r--r--  2.0 unx     6734 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/regions.py
--rw-r--r--  2.0 unx    10120 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/substation.py
--rw-r--r--  2.0 unx     6717 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/core/terminal.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py
--rw-r--r--  2.0 unx    10307 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py
--rw-r--r--  2.0 unx      748 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/domain/__init__.py
--rw-r--r--  2.0 unx    17065 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py
--rw-r--r--  2.0 unx     5374 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py
--rw-r--r--  2.0 unx      641 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/meas/__init__.py
--rw-r--r--  2.0 unx      963 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/meas/control.py
--rw-r--r--  2.0 unx      576 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/meas/iopoint.py
--rw-r--r--  2.0 unx     4294 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/meas/measurement.py
--rw-r--r--  2.0 unx     1753 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/meas/value.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/scada/__init__.py
--rw-r--r--  2.0 unx      737 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/scada/remote_control.py
--rw-r--r--  2.0 unx      587 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/scada/remote_point.py
--rw-r--r--  2.0 unx      734 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/scada/remote_source.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/__init__.py
--rw-r--r--  2.0 unx     2433 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py
--rw-r--r--  2.0 unx     1413 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/connectors.py
--rw-r--r--  2.0 unx      972 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py
--rw-r--r--  2.0 unx     7483 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py
--rw-r--r--  2.0 unx     6517 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/energy_source.py
--rw-r--r--  2.0 unx     1977 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py
--rw-r--r--  2.0 unx      492 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/line.py
--rw-r--r--  2.0 unx     1904 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/per_length.py
--rw-r--r--  2.0 unx      884 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py
--rw-r--r--  2.0 unx     9971 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py
--rw-r--r--  2.0 unx    24201 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py
--rw-r--r--  2.0 unx     3658 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py
--rw-r--r--  2.0 unx     1727 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py
--rw-r--r--  2.0 unx     6285 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/switch.py
--rw-r--r--  2.0 unx     2219 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py
--rw-r--r--  2.0 unx     1544 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/vector_group.py
--rw-r--r--  2.0 unx      786 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py
--rw-r--r--  2.0 unx      809 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py
--rw-r--r--  2.0 unx     2215 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py
--rw-r--r--  2.0 unx      248 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/infiec61970/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py
--rw-r--r--  2.0 unx     5385 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py
--rw-r--r--  2.0 unx     7542 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py
--rw-r--r--  2.0 unx     7636 b- defN 23-Jan-09 04:58 zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/__init__.py
--rw-r--r--  2.0 unx      960 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/__init__.py
--rw-r--r--  2.0 unx    17992 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/base_service.py
--rw-r--r--  2.0 unx    16620 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/base_service_comparator.py
--rw-r--r--  2.0 unx     1189 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/difference.py
--rw-r--r--  2.0 unx    20310 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/reference_resolvers.py
--rw-r--r--  2.0 unx    18922 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/resolver.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/meta/__init__.py
--rw-r--r--  2.0 unx      461 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/meta/data_source.py
--rw-r--r--  2.0 unx      804 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/meta/metadata_collection.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/translator/__init__.py
--rw-r--r--  2.0 unx     3395 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/translator/base_cim2proto.py
--rw-r--r--  2.0 unx     3994 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/translator/base_proto2cim.py
--rw-r--r--  2.0 unx     2924 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/translator/service_differences.py
--rw-r--r--  2.0 unx     1970 b- defN 23-Jan-09 04:58 zepben/evolve/services/common/translator/util.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/customer/__init__.py
--rw-r--r--  2.0 unx     1922 b- defN 23-Jan-09 04:58 zepben/evolve/services/customer/customer_service_comparator.py
--rw-r--r--  2.0 unx      501 b- defN 23-Jan-09 04:58 zepben/evolve/services/customer/customers.py
--rw-r--r--  2.0 unx     1044 b- defN 23-Jan-09 04:58 zepben/evolve/services/customer/translator/__init__.py
--rw-r--r--  2.0 unx     2760 b- defN 23-Jan-09 04:58 zepben/evolve/services/customer/translator/customer_cim2proto.py
--rw-r--r--  2.0 unx     3379 b- defN 23-Jan-09 04:58 zepben/evolve/services/customer/translator/customer_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/diagram/__init__.py
--rw-r--r--  2.0 unx     1486 b- defN 23-Jan-09 04:58 zepben/evolve/services/diagram/diagram_service_comparator.py
--rw-r--r--  2.0 unx     4598 b- defN 23-Jan-09 04:58 zepben/evolve/services/diagram/diagrams.py
--rw-r--r--  2.0 unx      508 b- defN 23-Jan-09 04:58 zepben/evolve/services/diagram/translator/__init__.py
--rw-r--r--  2.0 unx     2237 b- defN 23-Jan-09 04:58 zepben/evolve/services/diagram/translator/diagram_cim2proto.py
--rw-r--r--  2.0 unx     2463 b- defN 23-Jan-09 04:58 zepben/evolve/services/diagram/translator/diagram_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/measurement/__init__.py
--rw-r--r--  2.0 unx     1207 b- defN 23-Jan-09 04:58 zepben/evolve/services/measurement/measurements.py
--rw-r--r--  2.0 unx      261 b- defN 23-Jan-09 04:58 zepben/evolve/services/measurement/translator/__init__.py
--rw-r--r--  2.0 unx     1832 b- defN 23-Jan-09 04:58 zepben/evolve/services/measurement/translator/measurement_cim2proto.py
--rw-r--r--  2.0 unx     1951 b- defN 23-Jan-09 04:58 zepben/evolve/services/measurement/translator/measurement_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/__init__.py
--rw-r--r--  2.0 unx     6278 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/network_extensions.py
--rw-r--r--  2.0 unx    10634 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/network_service.py
--rw-r--r--  2.0 unx    37224 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/network_service_comparator.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/__init__.py
--rw-r--r--  2.0 unx     3654 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/find.py
--rw-r--r--  2.0 unx     5623 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/find_swer_equipment.py
--rw-r--r--  2.0 unx    16173 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/tracing.py
--rw-r--r--  2.0 unx     3395 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/util.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/__init__.py
--rw-r--r--  2.0 unx      775 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py
--rw-r--r--  2.0 unx     2394 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py
--rw-r--r--  2.0 unx     8420 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py
--rw-r--r--  2.0 unx     1162 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py
--rw-r--r--  2.0 unx     4223 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/connectivity_result.py
--rw-r--r--  2.0 unx     2671 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py
--rw-r--r--  2.0 unx     1212 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py
--rw-r--r--  2.0 unx     5162 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py
--rw-r--r--  2.0 unx     3872 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/phase_paths.py
--rw-r--r--  2.0 unx     9998 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py
--rw-r--r--  2.0 unx     2862 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py
--rw-r--r--  2.0 unx     7329 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py
--rw-r--r--  2.0 unx    10412 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py
--rw-r--r--  2.0 unx      583 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/__init__.py
--rw-r--r--  2.0 unx     5977 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py
--rw-r--r--  2.0 unx     5963 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py
--rw-r--r--  2.0 unx     3246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py
--rw-r--r--  2.0 unx     1477 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py
--rw-r--r--  2.0 unx     3990 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/direction_status.py
--rw-r--r--  2.0 unx     2546 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/feeder_direction.py
--rw-r--r--  2.0 unx     7410 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/remove_direction.py
--rw-r--r--  2.0 unx     6082 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/feeder/set_direction.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/__init__.py
--rw-r--r--  2.0 unx    10311 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/phase_inferrer.py
--rw-r--r--  2.0 unx     3342 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/phase_status.py
--rw-r--r--  2.0 unx     2628 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/phase_step.py
--rw-r--r--  2.0 unx     2014 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/phase_step_tracker.py
--rw-r--r--  2.0 unx     6251 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/phase_trace.py
--rw-r--r--  2.0 unx     5510 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/remove_phases.py
--rw-r--r--  2.0 unx    12798 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/phases/set_phases.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/__init__.py
--rw-r--r--  2.0 unx     1642 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/basic_tracker.py
--rw-r--r--  2.0 unx     3036 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/basic_traversal.py
--rw-r--r--  2.0 unx     6585 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py
--rw-r--r--  2.0 unx     5164 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/queue.py
--rw-r--r--  2.0 unx     1775 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/tracker.py
--rw-r--r--  2.0 unx     7479 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/traversals/traversal.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/tree/__init__.py
--rw-r--r--  2.0 unx     4454 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/tree/downstream_tree.py
--rw-r--r--  2.0 unx     1780 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/tree/tree_node.py
--rw-r--r--  2.0 unx     1167 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/tracing/tree/tree_node_tracker.py
--rw-r--r--  2.0 unx    20355 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/translator/__init__.py
--rw-r--r--  2.0 unx    55849 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/translator/network_cim2proto.py
--rw-r--r--  2.0 unx    67957 b- defN 23-Jan-09 04:58 zepben/evolve/services/network/translator/network_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/__init__.py
--rw-r--r--  2.0 unx      419 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/exceptions.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/__init__.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/consumer.py
--rw-r--r--  2.0 unx     3424 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/customer_consumer.py
--rw-r--r--  2.0 unx     3253 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/diagram_consumer.py
--rw-r--r--  2.0 unx    36489 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/network_consumer.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/hierarchy/__init__.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/get/hierarchy/data.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/grpc/__init__.py
--rw-r--r--  2.0 unx      801 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/grpc/auth_token_plugin.py
--rw-r--r--  2.0 unx     8113 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/grpc/connect.py
--rw-r--r--  2.0 unx     4020 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/grpc/grpc.py
--rw-r--r--  2.0 unx     4277 b- defN 23-Jan-09 04:58 zepben/evolve/streaming/grpc/grpc_channel_builder.py
--rw-r--r--  2.0 unx      245 b- defN 23-Jan-09 04:58 zepben/evolve/testing/__init__.py
--rw-r--r--  2.0 unx    20782 b- defN 23-Jan-09 04:58 zepben/evolve/testing/test_network_builder.py
--rw-r--r--  2.0 unx     3238 b- defN 23-Jan-09 04:58 zepben/evolve/testing/test_traversal.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Jan-09 05:01 zepben.evolve-0.35.0b8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2267 b- defN 23-Jan-09 05:01 zepben.evolve-0.35.0b8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-09 05:01 zepben.evolve-0.35.0b8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-09 05:01 zepben.evolve-0.35.0b8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    35109 b- defN 23-Jan-09 05:01 zepben.evolve-0.35.0b8.dist-info/RECORD
-302 files, 1397804 bytes uncompressed, 336454 bytes compressed:  75.9%
+Zip file size: 412388 bytes, number of entries: 319
+-rw-r--r--  2.0 unx    18234 b- defN 23-Jan-18 05:55 zepben/evolve/__init__.py
+-rw-r--r--  2.0 unx     1387 b- defN 23-Jan-18 05:55 zepben/evolve/exceptions.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jan-18 05:55 zepben/evolve/types.py
+-rw-r--r--  2.0 unx     4576 b- defN 23-Jan-18 05:55 zepben/evolve/util.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/__init__.py
+-rw-r--r--  2.0 unx     6688 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/database_reader.py
+-rw-r--r--  2.0 unx     5803 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/database_writer.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/__init__.py
+-rw-r--r--  2.0 unx     5319 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/base_cim_reader.py
+-rw-r--r--  2.0 unx     2991 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/base_service_reader.py
+-rw-r--r--  2.0 unx     4510 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/customer_cim_reader.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/customer_service_reader.py
+-rw-r--r--  2.0 unx     3245 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/diagram_cim_reader.py
+-rw-r--r--  2.0 unx     1041 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/diagram_service_reader.py
+-rw-r--r--  2.0 unx      733 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/metadata_collection_reader.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/metadata_entry_reader.py
+-rw-r--r--  2.0 unx    72711 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/network_cim_reader.py
+-rw-r--r--  2.0 unx    12259 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/network_service_reader.py
+-rw-r--r--  2.0 unx     6872 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/readers/result_set.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/__init__.py
+-rw-r--r--  2.0 unx     1009 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/column.py
+-rw-r--r--  2.0 unx    11816 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/database_tables.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/exceptions.py
+-rw-r--r--  2.0 unx     1164 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/metadata_tables.py
+-rw-r--r--  2.0 unx     5820 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/sqlite_table.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/__init__.py
+-rw-r--r--  2.0 unx     1484 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py
+-rw-r--r--  2.0 unx     1561 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py
+-rw-r--r--  2.0 unx     3547 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py
+-rw-r--r--  2.0 unx     1696 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py
+-rw-r--r--  2.0 unx     1435 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py
+-rw-r--r--  2.0 unx     1572 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py
+-rw-r--r--  2.0 unx     1409 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/__init__.py
+-rw-r--r--  2.0 unx     2240 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py
+-rw-r--r--  2.0 unx     9094 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py
+-rw-r--r--  2.0 unx     5681 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/common_tables.py
+-rw-r--r--  2.0 unx     1705 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py
+-rw-r--r--  2.0 unx     1629 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py
+-rw-r--r--  2.0 unx     4006 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py
+-rw-r--r--  2.0 unx     1995 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py
+-rw-r--r--  2.0 unx     8308 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py
+-rw-r--r--  2.0 unx     3113 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py
+-rw-r--r--  2.0 unx     2454 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py
+-rw-r--r--  2.0 unx     2581 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py
+-rw-r--r--  2.0 unx     2270 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py
+-rw-r--r--  2.0 unx     1205 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/__init__.py
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/feeder_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py
+-rw-r--r--  2.0 unx      710 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py
+-rw-r--r--  2.0 unx      458 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py
+-rw-r--r--  2.0 unx    10492 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py
+-rw-r--r--  2.0 unx     1845 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py
+-rw-r--r--  2.0 unx     7441 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py
+-rw-r--r--  2.0 unx     2114 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/__init__.py
+-rw-r--r--  2.0 unx     5263 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/base_cim_writer.py
+-rw-r--r--  2.0 unx     2995 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/base_service_writer.py
+-rw-r--r--  2.0 unx     4752 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/customer_cim_writer.py
+-rw-r--r--  2.0 unx     1393 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/customer_service_writer.py
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/diagram_cim_writer.py
+-rw-r--r--  2.0 unx     1004 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/diagram_service_writer.py
+-rw-r--r--  2.0 unx      904 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/metadata_collection_writer.py
+-rw-r--r--  2.0 unx     1257 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/metadata_entry_writer.py
+-rw-r--r--  2.0 unx    70327 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/network_cim_writer.py
+-rw-r--r--  2.0 unx     8395 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/network_service_writer.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jan-18 05:55 zepben/evolve/database/sqlite/writers/utils.py
+-rw-r--r--  2.0 unx      309 b- defN 23-Jan-18 05:55 zepben/evolve/examples/__init__.py
+-rw-r--r--  2.0 unx     6937 b- defN 23-Jan-18 05:55 zepben/evolve/examples/simple_node_breaker_feeder.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/__init__.py
+-rw-r--r--  2.0 unx     7357 b- defN 23-Jan-18 05:55 zepben/evolve/model/phases.py
+-rw-r--r--  2.0 unx     1502 b- defN 23-Jan-18 05:55 zepben/evolve/model/resistance_reactance.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/model/busbranch/__init__.py
+-rw-r--r--  2.0 unx    47076 b- defN 23-Jan-18 05:55 zepben/evolve/model/busbranch/bus_branch.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/__init__.py
+-rw-r--r--  2.0 unx     1398 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py
+-rw-r--r--  2.0 unx     1445 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py
+-rw-r--r--  2.0 unx     3555 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py
+-rw-r--r--  2.0 unx     1877 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py
+-rw-r--r--  2.0 unx      550 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py
+-rw-r--r--  2.0 unx     5904 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py
+-rw-r--r--  2.0 unx     3736 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py
+-rw-r--r--  2.0 unx      860 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py
+-rw-r--r--  2.0 unx     1287 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/__init__.py
+-rw-r--r--  2.0 unx     4019 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/asset.py
+-rw-r--r--  2.0 unx      845 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/asset_info.py
+-rw-r--r--  2.0 unx      588 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py
+-rw-r--r--  2.0 unx     3009 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/pole.py
+-rw-r--r--  2.0 unx     1157 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/streetlight.py
+-rw-r--r--  2.0 unx      635 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/assets/structure.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/common/__init__.py
+-rw-r--r--  2.0 unx     1570 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/common/document.py
+-rw-r--r--  2.0 unx     7841 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/common/location.py
+-rw-r--r--  2.0 unx      531 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/common/organisation.py
+-rw-r--r--  2.0 unx      838 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/common/organisation_role.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/customers/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/customers/customer.py
+-rw-r--r--  2.0 unx     4260 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/customers/customer_agreement.py
+-rw-r--r--  2.0 unx     1474 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/customers/customer_kind.py
+-rw-r--r--  2.0 unx     3336 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/customers/pricing_structure.py
+-rw-r--r--  2.0 unx      763 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/customers/tariff.py
+-rw-r--r--  2.0 unx      244 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/__init__.py
+-rw-r--r--  2.0 unx      244 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py
+-rw-r--r--  2.0 unx     1859 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py
+-rw-r--r--  2.0 unx     1250 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py
+-rw-r--r--  2.0 unx     1202 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/metering/__init__.py
+-rw-r--r--  2.0 unx    11019 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/metering/metering.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/operations/__init__.py
+-rw-r--r--  2.0 unx     3889 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61968/operations/operational_restriction.py
+-rw-r--r--  2.0 unx      248 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/__init__.py
+-rw-r--r--  2.0 unx      249 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py
+-rw-r--r--  2.0 unx     1475 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py
+-rw-r--r--  2.0 unx     1489 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py
+-rw-r--r--  2.0 unx     1753 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py
+-rw-r--r--  2.0 unx      588 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/__init__.py
+-rw-r--r--  2.0 unx      556 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/base_voltage.py
+-rw-r--r--  2.0 unx     7135 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py
+-rw-r--r--  2.0 unx     3645 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py
+-rw-r--r--  2.0 unx    14056 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/equipment.py
+-rw-r--r--  2.0 unx    15618 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/equipment_container.py
+-rw-r--r--  2.0 unx     6735 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/identified_object.py
+-rw-r--r--  2.0 unx     1095 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/name.py
+-rw-r--r--  2.0 unx     5023 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/name_type.py
+-rw-r--r--  2.0 unx     6187 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/phase_code.py
+-rw-r--r--  2.0 unx     1250 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py
+-rw-r--r--  2.0 unx     6734 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/regions.py
+-rw-r--r--  2.0 unx    10120 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/substation.py
+-rw-r--r--  2.0 unx     6717 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/core/terminal.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py
+-rw-r--r--  2.0 unx    10307 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py
+-rw-r--r--  2.0 unx      748 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/domain/__init__.py
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py
+-rw-r--r--  2.0 unx     5374 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py
+-rw-r--r--  2.0 unx      641 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/meas/__init__.py
+-rw-r--r--  2.0 unx      963 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/meas/control.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/meas/iopoint.py
+-rw-r--r--  2.0 unx     4294 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/meas/measurement.py
+-rw-r--r--  2.0 unx     1753 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/meas/value.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/protection/__init__.py
+-rw-r--r--  2.0 unx     1465 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/protection/current_relay.py
+-rw-r--r--  2.0 unx     4390 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/protection/protection_equipment.py
+-rw-r--r--  2.0 unx      816 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/protection/reclose_sequence.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/scada/__init__.py
+-rw-r--r--  2.0 unx      737 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/scada/remote_control.py
+-rw-r--r--  2.0 unx      587 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/scada/remote_point.py
+-rw-r--r--  2.0 unx      734 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/scada/remote_source.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/__init__.py
+-rw-r--r--  2.0 unx     2433 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/breaker.py
+-rw-r--r--  2.0 unx     1413 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/connectors.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/disconnector.py
+-rw-r--r--  2.0 unx      972 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py
+-rw-r--r--  2.0 unx     7483 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py
+-rw-r--r--  2.0 unx     6517 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/energy_source.py
+-rw-r--r--  2.0 unx     1977 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py
+-rw-r--r--  2.0 unx      595 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/fuse.py
+-rw-r--r--  2.0 unx      611 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/jumper.py
+-rw-r--r--  2.0 unx      492 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/line.py
+-rw-r--r--  2.0 unx      584 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py
+-rw-r--r--  2.0 unx     1904 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/per_length.py
+-rw-r--r--  2.0 unx      884 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py
+-rw-r--r--  2.0 unx     9971 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py
+-rw-r--r--  2.0 unx    24201 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py
+-rw-r--r--  2.0 unx     7168 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py
+-rw-r--r--  2.0 unx      582 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/recloser.py
+-rw-r--r--  2.0 unx     3658 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py
+-rw-r--r--  2.0 unx     1727 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py
+-rw-r--r--  2.0 unx     4955 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/switch.py
+-rw-r--r--  2.0 unx     2219 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py
+-rw-r--r--  2.0 unx     1544 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/vector_group.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py
+-rw-r--r--  2.0 unx      809 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py
+-rw-r--r--  2.0 unx     2215 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py
+-rw-r--r--  2.0 unx      248 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py
+-rw-r--r--  2.0 unx     5385 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py
+-rw-r--r--  2.0 unx     7542 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py
+-rw-r--r--  2.0 unx     7636 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py
+-rw-r--r--  2.0 unx      768 b- defN 23-Jan-18 05:55 zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/__init__.py
+-rw-r--r--  2.0 unx    17992 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/base_service.py
+-rw-r--r--  2.0 unx    16620 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/base_service_comparator.py
+-rw-r--r--  2.0 unx     1189 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/difference.py
+-rw-r--r--  2.0 unx    22265 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/reference_resolvers.py
+-rw-r--r--  2.0 unx    20018 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/resolver.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/meta/__init__.py
+-rw-r--r--  2.0 unx      461 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/meta/data_source.py
+-rw-r--r--  2.0 unx      804 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/meta/metadata_collection.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/translator/__init__.py
+-rw-r--r--  2.0 unx     3395 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/translator/base_cim2proto.py
+-rw-r--r--  2.0 unx     3994 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/translator/base_proto2cim.py
+-rw-r--r--  2.0 unx     2924 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/translator/service_differences.py
+-rw-r--r--  2.0 unx     2410 b- defN 23-Jan-18 05:55 zepben/evolve/services/common/translator/util.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/customer/__init__.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-Jan-18 05:55 zepben/evolve/services/customer/customer_service_comparator.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Jan-18 05:55 zepben/evolve/services/customer/customers.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Jan-18 05:55 zepben/evolve/services/customer/translator/__init__.py
+-rw-r--r--  2.0 unx     2760 b- defN 23-Jan-18 05:55 zepben/evolve/services/customer/translator/customer_cim2proto.py
+-rw-r--r--  2.0 unx     3379 b- defN 23-Jan-18 05:55 zepben/evolve/services/customer/translator/customer_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/diagram/__init__.py
+-rw-r--r--  2.0 unx     1486 b- defN 23-Jan-18 05:55 zepben/evolve/services/diagram/diagram_service_comparator.py
+-rw-r--r--  2.0 unx     4598 b- defN 23-Jan-18 05:55 zepben/evolve/services/diagram/diagrams.py
+-rw-r--r--  2.0 unx      508 b- defN 23-Jan-18 05:55 zepben/evolve/services/diagram/translator/__init__.py
+-rw-r--r--  2.0 unx     2237 b- defN 23-Jan-18 05:55 zepben/evolve/services/diagram/translator/diagram_cim2proto.py
+-rw-r--r--  2.0 unx     2463 b- defN 23-Jan-18 05:55 zepben/evolve/services/diagram/translator/diagram_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/measurement/__init__.py
+-rw-r--r--  2.0 unx     1207 b- defN 23-Jan-18 05:55 zepben/evolve/services/measurement/measurements.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Jan-18 05:55 zepben/evolve/services/measurement/translator/__init__.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Jan-18 05:55 zepben/evolve/services/measurement/translator/measurement_cim2proto.py
+-rw-r--r--  2.0 unx     1951 b- defN 23-Jan-18 05:55 zepben/evolve/services/measurement/translator/measurement_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/__init__.py
+-rw-r--r--  2.0 unx     6279 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/network_extensions.py
+-rw-r--r--  2.0 unx    10634 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/network_service.py
+-rw-r--r--  2.0 unx    39337 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/network_service_comparator.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/__init__.py
+-rw-r--r--  2.0 unx     3654 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/find.py
+-rw-r--r--  2.0 unx     5623 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/find_swer_equipment.py
+-rw-r--r--  2.0 unx    16173 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/tracing.py
+-rw-r--r--  2.0 unx     3395 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/util.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/__init__.py
+-rw-r--r--  2.0 unx      775 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py
+-rw-r--r--  2.0 unx     2394 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py
+-rw-r--r--  2.0 unx     8420 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py
+-rw-r--r--  2.0 unx     1162 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py
+-rw-r--r--  2.0 unx     4223 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/connectivity_result.py
+-rw-r--r--  2.0 unx     2671 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py
+-rw-r--r--  2.0 unx     5162 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py
+-rw-r--r--  2.0 unx     3872 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/phase_paths.py
+-rw-r--r--  2.0 unx     9998 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py
+-rw-r--r--  2.0 unx     2862 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py
+-rw-r--r--  2.0 unx     7329 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py
+-rw-r--r--  2.0 unx    10412 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/__init__.py
+-rw-r--r--  2.0 unx     5997 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py
+-rw-r--r--  2.0 unx     6053 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py
+-rw-r--r--  2.0 unx     3246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py
+-rw-r--r--  2.0 unx     1477 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py
+-rw-r--r--  2.0 unx     3990 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/direction_status.py
+-rw-r--r--  2.0 unx     2546 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/feeder_direction.py
+-rw-r--r--  2.0 unx     7410 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/remove_direction.py
+-rw-r--r--  2.0 unx     6082 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/feeder/set_direction.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/__init__.py
+-rw-r--r--  2.0 unx    10311 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/phase_inferrer.py
+-rw-r--r--  2.0 unx     3342 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/phase_status.py
+-rw-r--r--  2.0 unx     2628 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/phase_step.py
+-rw-r--r--  2.0 unx     2014 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/phase_step_tracker.py
+-rw-r--r--  2.0 unx     6251 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/phase_trace.py
+-rw-r--r--  2.0 unx     5510 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/remove_phases.py
+-rw-r--r--  2.0 unx    12798 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/phases/set_phases.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/__init__.py
+-rw-r--r--  2.0 unx     1642 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/basic_tracker.py
+-rw-r--r--  2.0 unx     2944 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/basic_traversal.py
+-rw-r--r--  2.0 unx     6585 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py
+-rw-r--r--  2.0 unx     5164 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/queue.py
+-rw-r--r--  2.0 unx     1775 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/tracker.py
+-rw-r--r--  2.0 unx     7479 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/traversals/traversal.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/tree/__init__.py
+-rw-r--r--  2.0 unx     4454 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/tree/downstream_tree.py
+-rw-r--r--  2.0 unx     1780 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/tree/tree_node.py
+-rw-r--r--  2.0 unx     1167 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/tracing/tree/tree_node_tracker.py
+-rw-r--r--  2.0 unx    21206 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/translator/__init__.py
+-rw-r--r--  2.0 unx    59797 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/translator/network_cim2proto.py
+-rw-r--r--  2.0 unx    72669 b- defN 23-Jan-18 05:55 zepben/evolve/services/network/translator/network_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/__init__.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/exceptions.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/__init__.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/consumer.py
+-rw-r--r--  2.0 unx     3424 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/customer_consumer.py
+-rw-r--r--  2.0 unx     3253 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/diagram_consumer.py
+-rw-r--r--  2.0 unx    36489 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/network_consumer.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/hierarchy/__init__.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/get/hierarchy/data.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/grpc/__init__.py
+-rw-r--r--  2.0 unx      801 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/grpc/auth_token_plugin.py
+-rw-r--r--  2.0 unx     8113 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/grpc/connect.py
+-rw-r--r--  2.0 unx     4020 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/grpc/grpc.py
+-rw-r--r--  2.0 unx     4277 b- defN 23-Jan-18 05:55 zepben/evolve/streaming/grpc/grpc_channel_builder.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-18 05:55 zepben/evolve/testing/__init__.py
+-rw-r--r--  2.0 unx    20782 b- defN 23-Jan-18 05:55 zepben/evolve/testing/test_network_builder.py
+-rw-r--r--  2.0 unx     3238 b- defN 23-Jan-18 05:55 zepben/evolve/testing/test_traversal.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-Jan-18 05:57 zepben.evolve-0.35.0b9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2267 b- defN 23-Jan-18 05:57 zepben.evolve-0.35.0b9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 05:57 zepben.evolve-0.35.0b9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 05:57 zepben.evolve-0.35.0b9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37171 b- defN 23-Jan-18 05:57 zepben.evolve-0.35.0b9.dist-info/RECORD
+319 files, 1451178 bytes uncompressed, 349866 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -93,14 +93,17 @@
 
 Filename: zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py
 Comment: 
 
+Filename: zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py
+Comment: 
+
 Filename: zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/iec61968/__init__.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py
@@ -144,14 +147,17 @@
 
 Filename: zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py
 Comment: 
 
+Filename: zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py
+Comment: 
+
 Filename: zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/__init__.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/feeder_tables.py
@@ -264,14 +270,17 @@
 
 Filename: zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py
@@ -339,14 +348,17 @@
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/__init__.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py
@@ -480,14 +492,26 @@
 
 Filename: zepben/evolve/model/cim/iec61970/base/meas/measurement.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/meas/value.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/protection/__init__.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/current_relay.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/protection_equipment.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/reclose_sequence.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/scada/__init__.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/scada/remote_control.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/scada/remote_point.py
@@ -498,44 +522,65 @@
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/__init__.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/breaker.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/connectors.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/disconnector.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/energy_source.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/fuse.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/wires/jumper.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/line.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/per_length.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/wires/recloser.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/switch.py
@@ -573,14 +618,20 @@
 
 Filename: zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py
+Comment: 
+
 Filename: zepben/evolve/services/__init__.py
 Comment: 
 
 Filename: zepben/evolve/services/common/__init__.py
 Comment: 
 
 Filename: zepben/evolve/services/common/base_service.py
@@ -885,23 +936,23 @@
 
 Filename: zepben/evolve/testing/test_network_builder.py
 Comment: 
 
 Filename: zepben/evolve/testing/test_traversal.py
 Comment: 
 
-Filename: zepben.evolve-0.35.0b8.dist-info/LICENSE
+Filename: zepben.evolve-0.35.0b9.dist-info/LICENSE
 Comment: 
 
-Filename: zepben.evolve-0.35.0b8.dist-info/METADATA
+Filename: zepben.evolve-0.35.0b9.dist-info/METADATA
 Comment: 
 
-Filename: zepben.evolve-0.35.0b8.dist-info/WHEEL
+Filename: zepben.evolve-0.35.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: zepben.evolve-0.35.0b8.dist-info/top_level.txt
+Filename: zepben.evolve-0.35.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: zepben.evolve-0.35.0b8.dist-info/RECORD
+Filename: zepben.evolve-0.35.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zepben/evolve/__init__.py

```diff
@@ -20,16 +20,18 @@
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.wire_material_kind import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import *
+from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_tank_info import *
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_construction_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_function_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infcommon.ratio import *
 from zepben.evolve.model.cim.iec61968.metering.metering import *
 from zepben.evolve.model.cim.iec61968.common.organisation import *
@@ -50,14 +52,17 @@
 from zepben.evolve.model.cim.iec61970.base.diagramlayout.orientation_kind import *
 from zepben.evolve.model.cim.iec61970.base.diagramlayout.diagram_style import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_point import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import *
 from zepben.evolve.model.cim.iec61970.base.domain.unit_symbol import *
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.current_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.reclose_sequence import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.battery_state_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.line import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import *
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import *
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import *
 from zepben.evolve.model.cim.iec61970.base.wires.vector_group import *
@@ -65,14 +70,21 @@
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import *
 from zepben.evolve.model.cim.iec61970.base.wires.phase_shunt_connection_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import *
 from zepben.evolve.model.cim.iec61970.base.wires.switch import *
+from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import *
+from zepben.evolve.model.cim.iec61970.base.wires.breaker import *
+from zepben.evolve.model.cim.iec61970.base.wires.disconnector import *
+from zepben.evolve.model.cim.iec61970.base.wires.fuse import *
+from zepben.evolve.model.cim.iec61970.base.wires.jumper import *
+from zepben.evolve.model.cim.iec61970.base.wires.load_break_switch import *
+from zepben.evolve.model.cim.iec61970.base.wires.recloser import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.single_phase_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.transformer_star_impedance import *
 from zepben.evolve.model.cim.iec61970.base.core.substation import *
 from zepben.evolve.model.cim.iec61970.base.core.terminal import *
 from zepben.evolve.model.cim.iec61970.base.core.equipment import *
@@ -86,14 +98,15 @@
 from zepben.evolve.model.cim.iec61970.base.core.equipment_container import *
 from zepben.evolve.model.cim.iec61970.base.core.connectivity_node import *
 from zepben.evolve.model.cim.iec61970.base.core.name import *
 from zepben.evolve.model.cim.iec61970.base.core.name_type import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.circuit import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.loop import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import *
+from zepben.evolve.model.cim.iec61970.infiec61970.protection.protection_kind import *
 from zepben.evolve.model.phases import *
 from zepben.evolve.model.resistance_reactance import *
 
 from zepben.evolve.services.network.tracing.traversals.tracker import *
 from zepben.evolve.services.network.tracing.traversals.basic_tracker import *
 from zepben.evolve.services.network.tracing.traversals.traversal import *
 from zepben.evolve.services.network.tracing.traversals.basic_traversal import *
@@ -189,23 +202,25 @@
 from zepben.evolve.database.sqlite.tables.associations.loop_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.circuit_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.customeragreements_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.equipment_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.usagepoints_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.assetorganisationroles_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.pricingstructure_association_tables import *
+from zepben.evolve.database.sqlite.tables.associations.protection_equipment_protected_switches import *
 from zepben.evolve.database.sqlite.tables.iec61968.common_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.customer_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.infiec61968.infassetinfo_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.metering_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.assetinfo_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.operations_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.meas_tables import *
+from zepben.evolve.database.sqlite.tables.iec61970.base.protection_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.scada_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.equivalent_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.auxiliaryequipment_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.diagramlayout_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.container_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.switch_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.energyconnection_tables import *
```

## zepben/evolve/database/sqlite/database_reader.py

```diff
@@ -34,15 +34,15 @@
         self._database_file = database_file
         self._get_connection = get_connection
         self._get_cursor = get_cursor
 
     _connection: Optional[Connection] = None
     _has_been_used = False
 
-    def load(
+    async def load(
         self,
         metadata_collection: MetadataCollection,
         network_service: NetworkService,
         diagram_service: DiagramService,
         customer_service: CustomerService
     ) -> bool:
         if not self._connect_database():
@@ -63,15 +63,15 @@
                      and DiagramServiceReader(get_cursor).load(diagram_service_reader) \
                      and CustomerServiceReader(get_cursor).load(customer_service_reader)
         except Exception as e:
             logger.error(f"Unable to load database: {str(e)}")
             self._close_connection()
             return False
 
-        return status and self._post_load(network_service)
+        return status and await self._post_load(network_service)
 
     def _connect_database(self) -> bool:
         if self._has_been_used:
             logger.error("You can only use the database reader once.")
             return False
 
         self._has_been_used = True
@@ -102,34 +102,34 @@
         try:
             self._connection.close()
         except Exception as e:
             logger.error(f"Failed to close connection to database: {str(e)}")
         finally:
             self._connection = None
 
-    def _post_load(self, network_service: NetworkService) -> bool:
+    async def _post_load(self, network_service: NetworkService) -> bool:
         #
         # NOTE: phase and direction tracing is not yet supported
         #
 
         logger.info("Applying feeder direction to network...")
-        tracing.set_direction().run(network_service)
+        await tracing.set_direction().run(network_service)
         logger.info("Feeder direction applied to network.")
 
         logger.info("Applying phases to network...")
-        tracing.set_phases().run(network_service)
-        tracing.phase_inferrer().run(network_service)
+        await tracing.set_phases().run(network_service)
+        await tracing.phase_inferrer().run(network_service)
         logger.info("Phasing applied to network.")
 
         logger.info("Assigning equipment to feeders...")
-        tracing.assign_equipment_to_feeders().run(network_service)
+        await tracing.assign_equipment_to_feeders().run(network_service)
         logger.info("Equipment assigned to feeders.")
 
         logger.info("Assigning equipment to LV feeders...")
-        tracing.assign_equipment_to_lv_feeders().run(network_service)
+        await tracing.assign_equipment_to_lv_feeders().run(network_service)
         logger.info("Equipment assigned to LV feeders.")
 
         logger.info("Validating primary sources vs feeders...")
         self._validate_sources(network_service)
         logger.info("Sources vs feeders validated.")
 
         self._close_connection()
```

## zepben/evolve/database/sqlite/readers/network_cim_reader.py

```diff
@@ -29,17 +29,18 @@
     TableLinearShuntCompensators, LinearShuntCompensator, PerLengthImpedance, TablePerLengthImpedances, PerLengthLineParameter, TablePerLengthLineParameters, \
     TablePerLengthSequenceImpedances, TablePowerElectronicsConnection, TablePowerElectronicsConnectionPhases, PowerElectronicsConnectionPhase, \
     TablePowerTransformers, PowerTransformer, VectorGroup, TablePowerTransformerEnds, PowerTransformerEnd, ProtectedSwitch, TableProtectedSwitches, \
     TableRatioTapChangers, RatioTapChanger, TransformerEnd, TableReclosers, Recloser, RegulatingCondEq, TableRegulatingCondEq, ShuntCompensator, \
     TableShuntCompensators, Switch, TableSwitches, TapChanger, TableTapChangers, TableTransformerEnds, TransformerStarImpedance, \
     TableTransformerStarImpedance, TableCircuits, Circuit, Loop, TableLoops, TableAssetOrganisationRolesAssets, TableEquipmentEquipmentContainers, \
     TableEquipmentOperationalRestrictions, TableEquipmentUsagePoints, TableUsagePointsEndDevices, TableCircuitsSubstations, TableCircuitsTerminals, \
-    TableLoopsSubstations, LoopSubstationRelationship, LvFeeder, TableLvFeeders, TablePotentialTransformers, PotentialTransformer, PotentialTransformerKind, \
-    PotentialTransformerInfo, Sensor, TableSensors, TableCurrentTransformers, CurrentTransformer, CurrentTransformerInfo, TableCurrentTransformerInfo, \
-    TablePotentialTransformerInfo
+    TablePotentialTransformers, PotentialTransformer, PotentialTransformerKind, PotentialTransformerInfo, Sensor, TableSensors, TableCurrentTransformers, \
+    CurrentTransformer, CurrentTransformerInfo, TableCurrentTransformerInfo, TablePotentialTransformerInfo, TableLoopsSubstations, LoopSubstationRelationship, \
+    LvFeeder, TableLvFeeders, CurrentRelayInfo, TableCurrentRelayInfo, SwitchInfo, TableSwitchInfo, ProtectionEquipment, TableProtectionEquipment, \
+    TableRecloseSequences, RecloseSequence, ProtectionKind, TableCurrentRelays, CurrentRelay, TableProtectionEquipmentProtectedSwitches
 
 __all__ = ["NetworkCIMReader"]
 
 
 class NetworkCIMReader(BaseCIMReader):
 
     # ************ IEC61968 ASSET INFO ************
@@ -103,14 +104,21 @@
         shunt_compensator_info.max_power_loss = rs.get_int(table.max_power_loss.query_index, None)
         shunt_compensator_info.rated_current = rs.get_int(table.rated_current.query_index, None)
         shunt_compensator_info.rated_reactive_power = rs.get_int(table.rated_reactive_power.query_index, None)
         shunt_compensator_info.rated_voltage = rs.get_int(table.rated_voltage.query_index, None)
 
         return self._load_asset_info(shunt_compensator_info, table, rs) and self._add_or_throw(shunt_compensator_info)
 
+    def load_switch_info(self, table: TableSwitchInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        switch_info = SwitchInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        switch_info.rated_interrupting_time = rs.get_double(table.rated_interrupting_time.query_index, None)
+
+        return self._load_asset_info(switch_info, table, rs) and self._add_or_throw(switch_info)
+
     def load_transformer_end_info(self, table: TableTransformerEndInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         transformer_end_info = TransformerEndInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         transformer_end_info.connection_kind = WindingConnection[rs.get_string(table.connection_kind.query_index)]
         transformer_end_info.emergency_s = rs.get_int(table.emergency_s.query_index, None)
         transformer_end_info.end_number = rs.get_int(table.end_number.query_index)
         transformer_end_info.insulation_u = rs.get_int(table.insulation_u.query_index, None)
@@ -267,14 +275,21 @@
             rs.get_string(table.state_or_province.query_index, "")
         )
 
         return None if town_detail.all_fields_null_or_empty() else town_detail
 
     # ************ IEC61968 infIEC61968 InfAssetInfo ************
 
+    def load_current_relay_info(self, table: TableCurrentRelayInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        current_relay_info = CurrentRelayInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        current_relay_info.curve_setting = rs.get_string(table.curve_setting.query_index, None)
+
+        return self._load_asset_info(current_relay_info, table, rs) and self._add_or_throw(current_relay_info)
+
     def load_current_transformer_info(self, table: TableCurrentTransformerInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         current_transformer_info = CurrentTransformerInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         current_transformer_info.accuracy_class = rs.get_string(table.accuracy_class.query_index, None)
         current_transformer_info.accuracy_limit = rs.get_double(table.accuracy_limit.query_index, None)
         current_transformer_info.core_count = rs.get_int(table.core_count.query_index, None)
         current_transformer_info.ct_class = rs.get_string(table.ct_class.query_index, None)
@@ -527,14 +542,44 @@
             measurement.remote_source.measurement = measurement
         measurement.terminal_mrid = rs.get_string(table.terminal_mrid.query_index, None)
         measurement.phases = PhaseCode[rs.get_string(table.phases.query_index)]
         measurement.unit_symbol = UnitSymbol[rs.get_string(table.unit_symbol.query_index)]
 
         return self._load_identified_object(measurement, table, rs)
 
+    # ************ IEC61970 Base Protection ************
+
+    def load_current_relay(self, table: TableCurrentRelays, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        current_relay = CurrentRelay(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        current_relay.current_limit_1 = rs.get_double(table.current_limit_1.query_index, None)
+        current_relay.inverse_time_flag = rs.get_boolean(table.inverse_time_flag.query_index, None)
+        current_relay.time_delay_1 = rs.get_double(table.time_delay_1.query_index, None)
+        current_relay.asset_info = self._ensure_get(rs.get_string(table.current_relay_info_mrid.query_index, None), WireInfo)
+
+        return self._load_protection_equipment(current_relay, table, rs) and self._add_or_throw(current_relay)
+
+    def _load_protection_equipment(self, protection_equipment: ProtectionEquipment, table: TableProtectionEquipment, rs: ResultSet) -> bool:
+        protection_equipment.relay_delay_time = rs.get_double(table.relay_delay_time.query_index, None)
+        protection_equipment.protection_kind = ProtectionKind[rs.get_string(table.protection_kind.query_index)]
+
+        return self._load_equipment(protection_equipment, table, rs)
+
+    def load_reclose_sequence(self, table: TableRecloseSequences, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        reclose_sequence = RecloseSequence(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        reclose_sequence.reclose_delay = rs.get_double(table.reclose_delay.query_index, None)
+        reclose_sequence.reclose_step = rs.get_int(table.reclose_step.query_index, None)
+
+        protected_switch_id = rs.get_string(table.protected_switch_mrid.query_index)
+        protected_switch = self._base_service.get(protected_switch_id, ProtectedSwitch)
+        protected_switch.add_reclose_sequence(reclose_sequence)
+
+        return self._load_identified_object(reclose_sequence, table, rs) and self._add_or_throw(reclose_sequence)
+
     # ************ IEC61970 BASE SCADA ************
 
     def load_remote_control(self, table: TableRemoteControls, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         remote_control = RemoteControl(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         remote_control.control = self._ensure_get(rs.get_string(table.control_mrid.query_index, None), Control)
         if remote_control.control is not None:
@@ -595,14 +640,16 @@
         )
 
         return self._load_conductor(ac_line_segment, table, rs) and self._add_or_throw(ac_line_segment)
 
     def load_breaker(self, table: TableBreakers, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         breaker = Breaker(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
+        breaker.in_transit_time = rs.get_double(table.in_transit_time.query_index, None)
+
         return self._load_protected_switch(breaker, table, rs) and self._add_or_throw(breaker)
 
     def load_load_break_switch(self, table: TableLoadBreakSwitches, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         load_break_switch = LoadBreakSwitch(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         return self._load_protected_switch(load_break_switch, table, rs) and self._add_or_throw(load_break_switch)
 
@@ -806,14 +853,16 @@
         power_transformer_end.rated_u = rs.get_int(table.rated_u.query_index, None)
         power_transformer_end.x = rs.get_double(table.x.query_index, None)
         power_transformer_end.x0 = rs.get_double(table.x0.query_index, None)
 
         return self._load_transformer_end(power_transformer_end, table, rs) and self._add_or_throw(power_transformer_end)
 
     def _load_protected_switch(self, protected_switch: ProtectedSwitch, table: TableProtectedSwitches, rs: ResultSet) -> bool:
+        protected_switch.breaking_capacity = rs.get_int(table.breaking_capacity.query_index, None)
+
         return self._load_switch(protected_switch, table, rs)
 
     def load_ratio_tap_changer(self, table: TableRatioTapChangers, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         ratio_tap_changer = RatioTapChanger(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         ratio_tap_changer.transformer_end = self._ensure_get(rs.get_string(table.transformer_end_mrid.query_index, None), TransformerEnd)
         if ratio_tap_changer.transformer_end is not None:
@@ -840,14 +889,17 @@
         shunt_compensator.nom_u = rs.get_int(table.nom_u.query_index, None)
         shunt_compensator.phase_connection = PhaseShuntConnectionKind[rs.get_string(table.phase_connection.query_index)]
         shunt_compensator.sections = rs.get_double(table.sections.query_index, None)
 
         return self._load_regulating_cond_eq(shunt_compensator, table, rs)
 
     def _load_switch(self, switch: Switch, table: TableSwitches, rs: ResultSet) -> bool:
+        switch.asset_info = self._ensure_get(rs.get_string(table.switch_info_mrid.query_index, None), SwitchInfo)
+
+        switch.rated_current = rs.get_int(table.rated_current.query_index, None)
         switch.set_normally_open(bool(rs.get_int(table.normal_open.query_index)))
         switch.set_open(bool(rs.get_int(table.open.query_index)))
 
         return self._load_conducting_equipment(switch, table, rs)
 
     def _load_tap_changer(self, tap_changer: TapChanger, table: TableTapChangers, rs: ResultSet) -> bool:
         tap_changer.control_enabled = rs.get_boolean(table.control_enabled.query_index)
@@ -1027,7 +1079,23 @@
             substation.add_loop(loop)
             loop.add_substation(substation)
         elif relationship == LoopSubstationRelationship.SUBSTATION_ENERGIZES_LOOP:
             substation.add_energized_loop(loop)
             loop.add_energizing_substation(substation)
 
         return True
+
+    def load_protection_equipment_protected_switch(self, table: TableProtectionEquipmentProtectedSwitches, rs: ResultSet,
+                                                   set_last_mrid: Callable[[str], str]) -> bool:
+        protection_equipment_mrid = set_last_mrid(rs.get_string(table.protection_equipment_mrid.query_index))
+        set_last_mrid(f"{protection_equipment_mrid}-to-UNKNOWN")
+
+        protected_switch_mrid = rs.get_string(table.protected_switch_mrid.query_index)
+        set_last_mrid(f"{protection_equipment_mrid}-to-{protected_switch_mrid}")
+
+        protection_equipment = self._base_service.get(protection_equipment_mrid, ProtectionEquipment)
+        protected_switch = self._base_service.get(protected_switch_mrid, ProtectedSwitch)
+
+        protection_equipment.add_protected_switch(protected_switch)
+        protected_switch.add_operated_by_protection_equipment(protection_equipment)
+
+        return True
```

## zepben/evolve/database/sqlite/readers/network_service_reader.py

```diff
@@ -11,15 +11,16 @@
     TablePowerElectronicsConnection, TablePowerElectronicsConnectionPhases, TableBatteryUnit, TablePhotoVoltaicUnit, TablePowerElectronicsWindUnit, \
     TableAcLineSegments, TableBreakers, TableLoadBreakSwitches, TableBusbarSections, TableDisconnectors, TableEnergyConsumers, TableEnergyConsumerPhases, \
     TableEnergySources, TableEnergySourcePhases, TableFuses, TableJumpers, TableJunctions, TableLinearShuntCompensators, TablePowerTransformers, \
     TableReclosers, TableTerminals, TableTransformerStarImpedance, TablePowerTransformerEnds, TableRatioTapChangers, TableFaultIndicators, TableFeeders, \
     TableLoops, TableCircuits, TablePositionPoints, TableLocationStreetAddresses, TableAssetOrganisationRolesAssets, TableUsagePointsEndDevices, \
     TableEquipmentUsagePoints, TableEquipmentOperationalRestrictions, TableEquipmentEquipmentContainers, TableCircuitsSubstations, TableCircuitsTerminals, \
     TableLoopsSubstations, TableControls, TableRemoteControls, TableRemoteSources, TableAnalogs, TableAccumulators, TableDiscretes, TableLvFeeders, \
-    TableCurrentTransformers, TablePotentialTransformers, TableCurrentTransformerInfo, TablePotentialTransformerInfo
+    TableCurrentTransformers, TablePotentialTransformers, TableCurrentTransformerInfo, TablePotentialTransformerInfo, TableCurrentRelayInfo, \
+    TableCurrentRelays, TableRecloseSequences, TableSwitchInfo, TableProtectionEquipmentProtectedSwitches
 from zepben.evolve.database.sqlite.readers.network_cim_reader import NetworkCIMReader
 
 __all__ = ["NetworkServiceReader"]
 
 
 class NetworkServiceReader(BaseServiceReader):
     """
@@ -33,15 +34,17 @@
         status = status and self._load_each(TableOverheadWireInfo, "overhead wire info", reader.load_overhead_wire_info)
         status = status and self._load_each(TablePowerTransformerInfo, "power transformer info", reader.load_power_transformer_info)
         status = status and self._load_each(TableTransformerTankInfo, "transformer tank info", reader.load_transformer_tank_info)
         status = status and self._load_each(TableNoLoadTests, "no load tests", reader.load_no_load_test)
         status = status and self._load_each(TableOpenCircuitTests, "open circuit tests", reader.load_open_circuit_test)
         status = status and self._load_each(TableShortCircuitTests, "short circuit tests", reader.load_short_circuit_test)
         status = status and self._load_each(TableShuntCompensatorInfo, "shunt compensator info", reader.load_shunt_compensator_info)
+        status = status and self._load_each(TableSwitchInfo, "switch info", reader.load_switch_info)
         status = status and self._load_each(TableTransformerEndInfo, "transformer end info", reader.load_transformer_end_info)
+        status = status and self._load_each(TableCurrentRelayInfo, "current relay info", reader.load_current_relay_info)
         status = status and self._load_each(TableCurrentTransformerInfo, "current transformer info", reader.load_current_transformer_info)
         status = status and self._load_each(TablePotentialTransformerInfo, "potential transformer info", reader.load_potential_transformer_info)
         status = status and self._load_each(TableLocations, "locations", reader.load_location)
         status = status and self._load_each(TableOrganisations, "organisations", reader.load_organisation)
         status = status and self._load_each(TableAssetOwners, "asset owners", reader.load_asset_owner)
         status = status and self._load_each(TablePoles, "poles", reader.load_pole)
         status = status and self._load_each(TableStreetlights, "streetlights", reader.load_streetlight)
@@ -65,14 +68,15 @@
         status = status and self._load_each(TableBatteryUnit, "battery unit", reader.load_battery_unit)
         status = status and self._load_each(TablePhotoVoltaicUnit, "photo voltaic unit", reader.load_photo_voltaic_unit)
         status = status and self._load_each(TablePowerElectronicsWindUnit, "power electronics wind unit", reader.load_power_electronics_wind_unit)
         status = status and self._load_each(TableAcLineSegments, "AC line segments", reader.load_ac_line_segment)
         status = status and self._load_each(TableBreakers, "breakers", reader.load_breaker)
         status = status and self._load_each(TableLoadBreakSwitches, "load break switches", reader.load_load_break_switch)
         status = status and self._load_each(TableBusbarSections, "busbar sections", reader.load_busbar_section)
+        status = status and self._load_each(TableCurrentRelays, "current relays", reader.load_current_relay)
         status = status and self._load_each(TableDisconnectors, "disconnectors", reader.load_disconnector)
         status = status and self._load_each(TableEnergyConsumers, "energy consumers", reader.load_energy_consumer)
         status = status and self._load_each(TableEnergyConsumerPhases, "energy consumer phases", reader.load_energy_consumer_phase)
         status = status and self._load_each(TableEnergySources, "energy sources", reader.load_energy_source)
         status = status and self._load_each(TableEnergySourcePhases, "energy source phases", reader.load_energy_source_phase)
         status = status and self._load_each(TableFuses, "fuses", reader.load_fuse)
         status = status and self._load_each(TableJumpers, "jumpers", reader.load_jumper)
@@ -106,20 +110,26 @@
             reader.load_equipment_operational_restriction
         )
         status = status and self._load_each(
             TableEquipmentEquipmentContainers,
             "equipment to equipment container associations",
             reader.load_equipment_equipment_container
         )
+        status = status and self._load_each(
+            TableProtectionEquipmentProtectedSwitches,
+            "protection equipment to protected switch associations",
+            reader.load_protection_equipment_protected_switch
+        )
         status = status and self._load_each(TableCircuitsSubstations, "circuit to substation associations", reader.load_circuit_substation)
         status = status and self._load_each(TableCircuitsTerminals, "circuit to terminal associations", reader.load_circuit_terminal)
         status = status and self._load_each(TableLoopsSubstations, "loop to substation associations", reader.load_loop_substation)
         status = status and self._load_each(TableControls, "controls", reader.load_control)
         status = status and self._load_each(TableRemoteControls, "remote controls", reader.load_remote_control)
         status = status and self._load_each(TableRemoteSources, "remote sources", reader.load_remote_source)
         status = status and self._load_each(TableAnalogs, "analogs", reader.load_analog)
         status = status and self._load_each(TableAccumulators, "accumulators", reader.load_accumulator)
         status = status and self._load_each(TableDiscretes, "discretes", reader.load_discrete)
+        status = status and self._load_each(TableRecloseSequences, "reclose sequences", reader.load_reclose_sequence)
 
         status = status and self.load_names(reader)
 
         return status
```

## zepben/evolve/database/sqlite/tables/database_tables.py

```diff
@@ -4,14 +4,15 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from sqlite3 import Cursor
 from typing import Dict, TypeVar, Type, Any, Optional
 
 from dataclassy import dataclass
 
+from zepben.evolve import TableProtectionEquipmentProtectedSwitches
 from zepben.evolve.database.sqlite.tables.associations.assetorganisationroles_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.circuit_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.customeragreements_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.equipment_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.loop_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.pricingstructure_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.usagepoints_association_tables import *
@@ -22,17 +23,18 @@
 from zepben.evolve.database.sqlite.tables.iec61968.customer_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.infiec61968.infassetinfo_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.metering_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.operations_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.auxiliaryequipment_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.diagramlayout_tables import *
-from zepben.evolve.database.sqlite.tables.iec61970.base.equivalent_tables import TableEquivalentBranches
+from zepben.evolve.database.sqlite.tables.iec61970.base.equivalent_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.infiec61970.feeder_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.meas_tables import *
+from zepben.evolve.database.sqlite.tables.iec61970.base.protection_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.scada_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.conductor_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.connector_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.energyconnection_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.generation.production_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.perlength_tables import *
 from zepben.evolve.database.sqlite.tables.iec61970.base.wires.switch_tables import *
@@ -60,14 +62,16 @@
         TableBusbarSections: TableBusbarSections(),
         TableCableInfo: TableCableInfo(),
         TableCircuits: TableCircuits(),
         TableCircuitsSubstations: TableCircuitsSubstations(),
         TableCircuitsTerminals: TableCircuitsTerminals(),
         TableConnectivityNodes: TableConnectivityNodes(),
         TableControls: TableControls(),
+        TableCurrentRelayInfo: TableCurrentRelayInfo(),
+        TableCurrentRelays: TableCurrentRelays(),
         TableCurrentTransformerInfo: TableCurrentTransformerInfo(),
         TableCurrentTransformers: TableCurrentTransformers(),
         TableCustomerAgreements: TableCustomerAgreements(),
         TableCustomerAgreementsPricingStructures: TableCustomerAgreementsPricingStructures(),
         TableCustomers: TableCustomers(),
         TableDiagramObjectPoints: TableDiagramObjectPoints(),
         TableDiagramObjects: TableDiagramObjects(),
@@ -114,24 +118,27 @@
         TablePowerElectronicsConnectionPhases: TablePowerElectronicsConnectionPhases(),
         TablePowerElectronicsWindUnit: TablePowerElectronicsWindUnit(),
         TablePowerTransformerEnds: TablePowerTransformerEnds(),
         TablePowerTransformerInfo: TablePowerTransformerInfo(),
         TablePowerTransformers: TablePowerTransformers(),
         TablePricingStructures: TablePricingStructures(),
         TablePricingStructuresTariffs: TablePricingStructuresTariffs(),
+        TableProtectionEquipmentProtectedSwitches: TableProtectionEquipmentProtectedSwitches(),
         TableRatioTapChangers: TableRatioTapChangers(),
         TableReclosers: TableReclosers(),
+        TableRecloseSequences: TableRecloseSequences(),
         TableRemoteControls: TableRemoteControls(),
         TableRemoteSources: TableRemoteSources(),
         TableShortCircuitTests: TableShortCircuitTests(),
         TableShuntCompensatorInfo: TableShuntCompensatorInfo(),
         TableSites: TableSites(),
         TableStreetlights: TableStreetlights(),
         TableSubGeographicalRegions: TableSubGeographicalRegions(),
         TableSubstations: TableSubstations(),
+        TableSwitchInfo: TableSwitchInfo(),
         TableTariffs: TableTariffs(),
         TableTerminals: TableTerminals(),
         TableTransformerEndInfo: TableTransformerEndInfo(),
         TableTransformerStarImpedance: TableTransformerStarImpedance(),
         TableTransformerTankInfo: TableTransformerTankInfo(),
         TableUsagePoints: TableUsagePoints(),
         TableUsagePointsEndDevices: TableUsagePointsEndDevices(),
```

## zepben/evolve/database/sqlite/tables/metadata_tables.py

```diff
@@ -9,15 +9,15 @@
 
 __all__ = ["TableVersion", "TableMetadataDataSources"]
 
 
 class TableVersion(SqliteTable):
     version: Column = None
 
-    SUPPORTED_VERSION = 44
+    SUPPORTED_VERSION = 45
 
     def __init__(self):
         self.version = self._create_column("version", "TEXT", Nullable.NOT_NULL)
 
     def name(self) -> str:
         return "version"
```

## zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py

```diff
@@ -5,15 +5,16 @@
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import TableAssetInfo
 
 __all__ = ["TablePowerTransformerInfo", "TableTransformerEndInfo", "TableTransformerTankInfo", "TableWireInfo", "TableCableInfo", "TableAssetInfo",
-           "TableOverheadWireInfo", "TableNoLoadTests", "TableOpenCircuitTests", "TableShortCircuitTests", "TableTransformerTest", "TableShuntCompensatorInfo"]
+           "TableOverheadWireInfo", "TableNoLoadTests", "TableOpenCircuitTests", "TableShortCircuitTests", "TableTransformerTest", "TableShuntCompensatorInfo",
+           "TableSwitchInfo"]
 
 
 # noinspection PyAbstractClass
 class TableTransformerTest(TableAssetInfo):
     base_power: Column = None
     temperature: Column = None
 
@@ -109,14 +110,25 @@
         self.rated_reactive_power = self._create_column("rated_reactive_power", "INTEGER", Nullable.NULL)
         self.rated_voltage = self._create_column("rated_voltage", "INTEGER", Nullable.NULL)
 
     def name(self) -> str:
         return "shunt_compensator_info"
 
 
+class TableSwitchInfo(TableAssetInfo):
+    rated_interrupting_time: Column = None
+
+    def __init__(self):
+        super(TableSwitchInfo, self).__init__()
+        self.rated_interrupting_time = self._create_column("rated_interrupting_time", "NUMBER", Nullable.NULL)
+
+    def name(self) -> str:
+        return "switch_info"
+
+
 class TableTransformerEndInfo(TableAssetInfo):
     connection_kind: Column = None
     emergency_s: Column = None
     end_number: Column = None
     insulation_u: Column = None
     phase_angle_clock: Column = None
     r: Column = None
```

## zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py

```diff
@@ -2,15 +2,26 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import TableAssetInfo
 
-__all__ = ["TableCurrentTransformerInfo", "TablePotentialTransformerInfo"]
+__all__ = ["TableCurrentRelayInfo", "TableCurrentTransformerInfo", "TablePotentialTransformerInfo"]
+
+
+class TableCurrentRelayInfo(TableAssetInfo):
+    curve_setting: Column = None
+
+    def __init__(self):
+        super(TableCurrentRelayInfo, self).__init__()
+        self.curve_setting = self._create_column("curve_setting", "TEXT", Nullable.NULL)
+
+    def name(self) -> str:
+        return "current_relay_info"
 
 
 class TableCurrentTransformerInfo(TableAssetInfo):
     accuracy_class: Column = None
     accuracy_limit: Column = None
     core_count: Column = None
     ct_class: Column = None
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py

```diff
@@ -9,32 +9,46 @@
 
 __all__ = ["TableSwitches", "TableProtectedSwitches", "TableFuses", "TableLoadBreakSwitches", "TableBreakers", "TableReclosers", "TableJumpers",
            "TableDisconnectors"]
 
 
 # noinspection PyAbstractClass
 class TableSwitches(TableConductingEquipment):
+    rated_current: Column = None
     normal_open: Column = None
     open: Column = None
+    switch_info_mrid: Column = None
 
     def __init__(self):
         super(TableSwitches, self).__init__()
+        self.rated_current = self._create_column("rated_current", "INTEGER", Nullable.NULL)
         self.normal_open = self._create_column("normal_open", "INTEGER", Nullable.NOT_NULL)
         self.open = self._create_column("open", "INTEGER", Nullable.NOT_NULL)
+        self.switch_info_mrid = self._create_column("switch_info_mrid", "TEXT", Nullable.NULL)
 
 
 # noinspection PyAbstractClass
 class TableProtectedSwitches(TableSwitches):
-    pass
+    breaking_capacity: Column = None
+
+    def __init__(self):
+        super(TableProtectedSwitches, self).__init__()
+        self.breaking_capacity = self._create_column("breaking_capacity", "INTEGER", Nullable.NULL)
 
 
 class TableBreakers(TableProtectedSwitches):
+    in_transit_time: Column = None
+
     def name(self) -> str:
         return "breakers"
 
+    def __init__(self):
+        super(TableBreakers, self).__init__()
+        self.in_transit_time = self._create_column("in_transit_time", "NUMBER", Nullable.NULL)
+
 
 class TableDisconnectors(TableSwitches):
     def name(self) -> str:
         return "disconnectors"
 
 
 class TableFuses(TableSwitches):
```

## zepben/evolve/database/sqlite/writers/base_cim_writer.py

```diff
@@ -33,63 +33,63 @@
     Helper methods for building insert statements. Note all fields need to be populated.
     """
 
     database_tables: DatabaseTables
     cursor: Cursor
     _failed_ids: Set[str] = set()
 
-    def _save_document(self, table: TableDocuments, insert: PreparedStatement, document: Document, description: str) -> bool:
-        insert.add_value(table.title.query_index, document.title)
-        # TODO: JVM seems to use Z as TZ offset (for UTC+0?) while python uses +HH:mm format. Need to investigate here
-        insert.add_value(table.created_date_time.query_index, f"{document.created_date_time.isoformat()}Z" if document.created_date_time else None)
-        insert.add_value(table.author_name.query_index, document.author_name)
-        insert.add_value(table.type.query_index, document.type)
-        insert.add_value(table.status.query_index, document.status)
-        insert.add_value(table.comment.query_index, document.comment)
-
-        return self.save_identified_object(table, insert, document, description)
-
     def save_organisation(self, organisation: Organisation) -> bool:
         table = self.database_tables.get_table(TableOrganisations)
         insert = self.database_tables.get_insert(TableOrganisations)
 
-        return self.save_identified_object(table, insert, organisation, "Organisation")
+        return self._save_identified_object(table, insert, organisation, "Organisation")
 
     def save_name_type(self, name_type: NameType) -> bool:
         table = self.database_tables.get_table(TableNameTypes)
         insert = self.database_tables.get_insert(TableNameTypes)
 
         insert.add_value(table.name_.query_index, name_type.name)
         insert.add_value(table.description.query_index, name_type.description)
 
-        return self.try_execute_single_update(insert, name_type.name, "name type")
+        return self._try_execute_single_update(insert, name_type.name, "name type")
 
     def save_name(self, name: Name) -> bool:
         table = self.database_tables.get_table(TableNames)
         insert = self.database_tables.get_insert(TableNames)
 
         insert.add_value(table.name_.query_index, name.name)
         insert.add_value(table.name_type_name.query_index, name.type.name)
         insert.add_value(table.identified_object_mrid.query_index, name.identified_object.mrid)
 
-        return self.try_execute_single_update(insert, name.name, "name")
+        return self._try_execute_single_update(insert, name.name, "name")
+
+    def _save_document(self, table: TableDocuments, insert: PreparedStatement, document: Document, description: str) -> bool:
+        insert.add_value(table.title.query_index, document.title)
+        # TODO: JVM seems to use Z as TZ offset (for UTC+0?) while python uses +HH:mm format. Need to investigate here
+        insert.add_value(table.created_date_time.query_index, f"{document.created_date_time.isoformat()}Z" if document.created_date_time else None)
+        insert.add_value(table.author_name.query_index, document.author_name)
+        insert.add_value(table.type.query_index, document.type)
+        insert.add_value(table.status.query_index, document.status)
+        insert.add_value(table.comment.query_index, document.comment)
+
+        return self._save_identified_object(table, insert, document, description)
 
-    def save_organisation_role(self, table: TableOrganisationRoles, insert: PreparedStatement, organisation_role: OrganisationRole, description: str) -> bool:
+    def _save_organisation_role(self, table: TableOrganisationRoles, insert: PreparedStatement, organisation_role: OrganisationRole, description: str) -> bool:
         insert.add_value(table.organisation_mrid.query_index, self._mrid_or_none(organisation_role.organisation))
-        return self.save_identified_object(table, insert, organisation_role, description)
+        return self._save_identified_object(table, insert, organisation_role, description)
 
-    def save_identified_object(self, table: TableIdentifiedObjects, insert: PreparedStatement, identified_object: IdentifiedObject, description: str) -> bool:
+    def _save_identified_object(self, table: TableIdentifiedObjects, insert: PreparedStatement, identified_object: IdentifiedObject, description: str) -> bool:
         insert.add_value(table.mrid.query_index, identified_object.mrid)
         insert.add_value(table.name_.query_index, identified_object.name)
         insert.add_value(table.description.query_index, identified_object.description)
         insert.add_value(table.num_diagram_objects.query_index, 0)  # Currently unused
 
-        return self.try_execute_single_update(insert, identified_object.mrid, description)
+        return self._try_execute_single_update(insert, identified_object.mrid, description)
 
-    def try_execute_single_update(self, query: PreparedStatement, mrid: str, description: str) -> bool:
+    def _try_execute_single_update(self, query: PreparedStatement, mrid: str, description: str) -> bool:
         """
         Execute an update on the database with the given `query`.
         Failures will be logged as warnings.
         `query` The PreparedStatement to execute.
         `mrid` The mRID of the relevant object that is being saved
         `description` A description of the type of object (e.g AcLineSegment)
         Returns True if the execute was successful, False otherwise.
```

## zepben/evolve/database/sqlite/writers/customer_cim_writer.py

```diff
@@ -27,15 +27,15 @@
     def save_customer(self, customer: Customer) -> bool:
         table = self.database_tables.get_table(TableCustomers)
         insert = self.database_tables.get_insert(TableCustomers)
 
         insert.add_value(table.kind.query_index, customer.kind.name)
         insert.add_value(table.num_end_devices.query_index, 0)  # Currently unused
 
-        return self.save_organisation_role(table, insert, customer, "Customer")
+        return self._save_organisation_role(table, insert, customer, "Customer")
 
     def save_customer_agreement(self, customer_agreement: CustomerAgreement) -> bool:
         table = self.database_tables.get_table(TableCustomerAgreements)
         insert = self.database_tables.get_insert(TableCustomerAgreements)
 
         status = True
         for ps in customer_agreement.pricing_structures:
@@ -65,18 +65,18 @@
     def save_customer_agreement_to_pricing_structure_association(self, customer_agreement: CustomerAgreement, pricing_structure: PricingStructure) -> bool:
         table = self.database_tables.get_table(TableCustomerAgreementsPricingStructures)
         insert = self.database_tables.get_insert(TableCustomerAgreementsPricingStructures)
 
         insert.add_value(table.customer_agreement_mrid.query_index, customer_agreement.mrid)
         insert.add_value(table.pricing_structure_mrid.query_index, pricing_structure.mrid)
 
-        return self.try_execute_single_update(insert, f"{customer_agreement.mrid}-to-{pricing_structure.mrid}",
-                                              "CustomerAgreement to PricingStructure association")
+        return self._try_execute_single_update(insert, f"{customer_agreement.mrid}-to-{pricing_structure.mrid}",
+                                               "CustomerAgreement to PricingStructure association")
 
     def save_pricing_structure_to_tariff_association(self, pricing_structure: PricingStructure, tariff: Tariff) -> bool:
         table = self.database_tables.get_table(TablePricingStructuresTariffs)
         insert = self.database_tables.get_insert(TablePricingStructuresTariffs)
 
         insert.add_value(table.pricing_structure_mrid.query_index, pricing_structure.mrid)
         insert.add_value(table.tariff_mrid.query_index, tariff.mrid)
 
-        return self.try_execute_single_update(insert, f"{pricing_structure.mrid}-to-{tariff.mrid}", "PricingStructure to Tariff association")
+        return self._try_execute_single_update(insert, f"{pricing_structure.mrid}-to-{tariff.mrid}", "PricingStructure to Tariff association")
```

## zepben/evolve/database/sqlite/writers/diagram_cim_writer.py

```diff
@@ -17,33 +17,33 @@
     def save_diagram(self, diagram: Diagram) -> bool:
         table = self.database_tables.get_table(TableDiagrams)
         insert = self.database_tables.get_insert(TableDiagrams)
 
         insert.add_value(table.diagram_style.query_index, diagram.diagram_style.name)
         insert.add_value(table.orientation_kind.query_index, diagram.orientation_kind.name)
 
-        return self.save_identified_object(table, insert, diagram, "diagram")
+        return self._save_identified_object(table, insert, diagram, "diagram")
 
     def save_diagram_object(self, diagram_object: DiagramObject) -> bool:
         table = self.database_tables.get_table(TableDiagramObjects)
         insert = self.database_tables.get_insert(TableDiagramObjects)
 
         status = True
         for sequence, point in enumerate(diagram_object.points):
             status = status and self.save_diagram_object_point(diagram_object, point, sequence)
         insert.add_value(table.identified_object_mrid.query_index, diagram_object.identified_object_mrid)
         insert.add_value(table.diagram_mrid.query_index, self._mrid_or_none(diagram_object.diagram))
         insert.add_value(table.style.query_index, diagram_object.style)
         insert.add_value(table.rotation.query_index, diagram_object.rotation)
 
-        return status and self.save_identified_object(table, insert, diagram_object, "diagram object")
+        return status and self._save_identified_object(table, insert, diagram_object, "diagram object")
 
     def save_diagram_object_point(self, diagram_object: DiagramObject, diagram_object_point: DiagramObjectPoint, sequence_number: int) -> bool:
         table = self.database_tables.get_table(TableDiagramObjectPoints)
         insert = self.database_tables.get_insert(TableDiagramObjectPoints)
 
         insert.add_value(table.diagram_object_mrid.query_index, diagram_object.mrid)
         insert.add_value(table.sequence_number.query_index, sequence_number)
         insert.add_value(table.x_position.query_index, diagram_object_point.x_position)
         insert.add_value(table.y_position.query_index, diagram_object_point.y_position)
 
-        return self.try_execute_single_update(insert, "{}-point{}".format(diagram_object.mrid, sequence_number), "diagram object point")
+        return self._try_execute_single_update(insert, "{}-point{}".format(diagram_object.mrid, sequence_number), "diagram object point")
```

## zepben/evolve/database/sqlite/writers/network_cim_writer.py

```diff
@@ -26,17 +26,19 @@
     TableNoLoadTests, TableTransformerTest, TransformerTest, ShortCircuitTest, TableShortCircuitTests, OpenCircuitTest, TableOpenCircuitTests, \
     PerLengthImpedance, TablePerLengthImpedances, TableAssetOrganisationRoles, AssetOwner, TableAssetOwners, TableStructures, Structure, Pole, TablePoles, \
     Streetlight, TableStreetlights, Location, TableLocations, TableLocationStreetAddressField, StreetAddress, TableLocationStreetAddresses, PositionPoint, \
     TablePositionPoints, TableStreetAddresses, TableTownDetails, TownDetail, StreetDetail, TableEndDevices, Meter, TableMeters, TableUsagePoints, \
     OperationalRestriction, TableOperationalRestrictions, TableFaultIndicators, TableAuxiliaryEquipment, AuxiliaryEquipment, FaultIndicator, \
     TableMeasurements, Measurement, Analog, TableAnalogs, Accumulator, TableAccumulators, Discrete, TableDiscretes, Control, TableControls, TableIoPoints, \
     IoPoint, TableRemotePoints, RemotePoint, RemoteControl, TableRemoteControls, RemoteSource, TableRemoteSources, ShuntCompensatorInfo, \
-    TableShuntCompensatorInfo, EquivalentBranch, EquivalentEquipment, Recloser, TableReclosers, TableEquipmentOperationalRestrictions, TableLvFeeders, LvFeeder, \
     CurrentTransformer, TableSensors, Sensor, TableCurrentTransformers, PotentialTransformer, TablePotentialTransformers, CurrentTransformerInfo, \
-    TableCurrentTransformerInfo, PotentialTransformerInfo, TablePotentialTransformerInfo
+    TableCurrentTransformerInfo, PotentialTransformerInfo, TablePotentialTransformerInfo, TableShuntCompensatorInfo, EquivalentBranch, EquivalentEquipment, \
+    Recloser, TableReclosers, TableEquipmentOperationalRestrictions, TableLvFeeders, LvFeeder, TableSwitchInfo, SwitchInfo, TableCurrentRelayInfo, \
+    CurrentRelayInfo, CurrentRelay, ProtectionEquipment, TableProtectionEquipment, RecloseSequence, TableCurrentRelays, TableRecloseSequences, \
+    TableProtectionEquipmentProtectedSwitches
 from zepben.evolve.database.sqlite.tables.iec61970.base.equivalent_tables import TableEquivalentBranches, TableEquivalentEquipment
 from zepben.evolve.database.sqlite.writers.base_cim_writer import BaseCIMWriter
 
 __all__ = ["NetworkCIMWriter"]
 
 
 class NetworkCIMWriter(BaseCIMWriter):
@@ -61,15 +63,15 @@
 
         return self._save_transformer_test(table, insert, no_load_test, "no load test")
 
     def _save_transformer_test(self, table: TableTransformerTest, insert: PreparedStatement, transformer_test: TransformerTest, description: str) -> bool:
         insert.add_value(table.base_power.query_index, transformer_test.base_power)
         insert.add_value(table.temperature.query_index, transformer_test.temperature)
 
-        return self.save_identified_object(table, insert, transformer_test, description)
+        return self._save_identified_object(table, insert, transformer_test, description)
 
     def save_short_circuit_test(self, short_circuit_test: ShortCircuitTest) -> bool:
         table = self.database_tables.get_table(TableShortCircuitTests)
         insert = self.database_tables.get_insert(TableShortCircuitTests)
 
         insert.add_value(table.current.query_index, short_circuit_test.current)
         insert.add_value(table.energised_end_step.query_index, short_circuit_test.energised_end_step)
@@ -91,14 +93,22 @@
         insert.add_value(table.max_power_loss.query_index, shunt_compensator_info.max_power_loss)
         insert.add_value(table.rated_current.query_index, shunt_compensator_info.rated_current)
         insert.add_value(table.rated_reactive_power.query_index, shunt_compensator_info.rated_reactive_power)
         insert.add_value(table.rated_voltage.query_index, shunt_compensator_info.rated_voltage)
 
         return self._save_asset_info(table, insert, shunt_compensator_info, "shunt compensator info")
 
+    def save_switch_info(self, switch_info: SwitchInfo) -> bool:
+        table = self.database_tables.get_table(TableSwitchInfo)
+        insert = self.database_tables.get_insert(TableSwitchInfo)
+
+        insert.add_value(table.rated_interrupting_time.query_index, switch_info.rated_interrupting_time)
+
+        return self._save_asset_info(table, insert, switch_info, "switch info")
+
     def save_open_circuit_test(self, open_circuit_test: OpenCircuitTest) -> bool:
         table = self.database_tables.get_table(TableOpenCircuitTests)
         insert = self.database_tables.get_insert(TableOpenCircuitTests)
 
         insert.add_value(table.energised_end_step.query_index, open_circuit_test.energised_end_step)
         insert.add_value(table.energised_end_voltage.query_index, open_circuit_test.energised_end_voltage)
         insert.add_value(table.open_end_step.query_index, open_circuit_test.open_end_step)
@@ -152,56 +162,53 @@
     def _save_wire_info(self, table: TableWireInfo, insert: PreparedStatement, wire_info: WireInfo, description: str) -> bool:
         insert.add_value(table.rated_current.query_index, wire_info.rated_current)
         insert.add_value(table.material.query_index, wire_info.material.name)
 
         return self._save_asset_info(table, insert, wire_info, description)
 
     def _save_asset_info(self, table: TableAssetInfo, insert: PreparedStatement, asset_info: AssetInfo, description: str) -> bool:
-        return self.save_identified_object(table, insert, asset_info, description)
+        return self._save_identified_object(table, insert, asset_info, description)
 
     # ************ IEC61968 ASSETS ************
 
     def _save_asset(self, table: TableAssets, insert: PreparedStatement, asset: Asset, description: str) -> bool:
         status = True
         insert.add_value(table.location_mrid.query_index, self._mrid_or_none(asset.location))
         for e in asset.organisation_roles:
             status = status and self._save_asset_organisation_role_to_asset_association(e, asset)
 
-        return status and self.save_identified_object(table, insert, asset, description)
+        return status and self._save_identified_object(table, insert, asset, description)
 
-    def save_asset_container(self, table: TableAssetContainers, insert: PreparedStatement, asset_container: AssetContainer, description: str) -> bool:
+    def _save_asset_container(self, table: TableAssetContainers, insert: PreparedStatement, asset_container: AssetContainer, description: str) -> bool:
         return self._save_asset(table, insert, asset_container, description)
 
-    def save_asset_info(self, table: TableAssetInfo, insert: PreparedStatement, asset_info: AssetInfo, description: str) -> bool:
-        return self.save_identified_object(table, insert, asset_info, description)
-
-    def save_asset_organisation_role(self,
-                                     table: TableAssetOrganisationRoles,
-                                     insert: PreparedStatement,
-                                     asset_organisation_role: AssetOrganisationRole,
-                                     description: str
-                                     ) -> bool:
-        return self.save_organisation_role(table, insert, asset_organisation_role, description)
+    def _save_asset_organisation_role(self,
+                                      table: TableAssetOrganisationRoles,
+                                      insert: PreparedStatement,
+                                      asset_organisation_role: AssetOrganisationRole,
+                                      description: str
+                                      ) -> bool:
+        return self._save_organisation_role(table, insert, asset_organisation_role, description)
 
     def save_asset_owner(self, asset_owner: AssetOwner) -> bool:
         table = self.database_tables.get_table(TableAssetOwners)
         insert = self.database_tables.get_insert(TableAssetOwners)
 
-        return self.save_asset_organisation_role(table, insert, asset_owner, "asset owner")
+        return self._save_asset_organisation_role(table, insert, asset_owner, "asset owner")
 
-    def save_structure(self, table: TableStructures, insert: PreparedStatement, structure: Structure, description: str) -> bool:
-        return self.save_asset_container(table, insert, structure, description)
+    def _save_structure(self, table: TableStructures, insert: PreparedStatement, structure: Structure, description: str) -> bool:
+        return self._save_asset_container(table, insert, structure, description)
 
     def save_pole(self, pole: Pole) -> bool:
         table = self.database_tables.get_table(TablePoles)
         insert = self.database_tables.get_insert(TablePoles)
 
         insert.add_value(table.classification.query_index, pole.classification)
 
-        return self.save_structure(table, insert, pole, "pole")
+        return self._save_structure(table, insert, pole, "pole")
 
     def save_streetlight(self, streetlight: Streetlight) -> bool:
         table = self.database_tables.get_table(TableStreetlights)
         insert = self.database_tables.get_insert(TableStreetlights)
 
         insert.add_value(table.pole_mrid.query_index, self._mrid_or_none(streetlight.pole))
         insert.add_value(table.light_rating.query_index, streetlight.light_rating)
@@ -230,48 +237,58 @@
         table = self.database_tables.get_table(TableLocations)
         insert = self.database_tables.get_insert(TableLocations)
 
         status = self.save_location_street_address(location, TableLocationStreetAddressField.mainAddress, location.main_address, "location main address")
         for sequence_number, point in enumerate(location.points):
             status = status and self.save_position_point(location, sequence_number, point)
 
-        return status and self.save_identified_object(table, insert, location, "location")
+        return status and self._save_identified_object(table, insert, location, "location")
 
     def save_location_street_address(self, location: Location, field: TableLocationStreetAddressField, street_address: StreetAddress, description: str) -> bool:
         if street_address is None:
             return True
 
         table = self.database_tables.get_table(TableLocationStreetAddresses)
         insert = self.database_tables.get_insert(TableLocationStreetAddresses)
 
         insert.add_value(table.location_mrid.query_index, location.mrid)
         insert.add_value(table.address_field.query_index, field.name)
 
-        return self.save_street_address(table, insert, street_address, "{}-{}".format(location.mrid, field), description)
+        return self._save_street_address(table, insert, street_address, "{}-{}".format(location.mrid, field), description)
 
     def save_position_point(self, location: Location, sequence_number: int, position_point: PositionPoint) -> bool:
         table = self.database_tables.get_table(TablePositionPoints)
         insert = self.database_tables.get_insert(TablePositionPoints)
 
         insert.add_value(table.location_mrid.query_index, location.mrid)
         insert.add_value(table.sequence_number.query_index, sequence_number)
         insert.add_value(table.x_position.query_index, position_point.x_position)
         insert.add_value(table.y_position.query_index, position_point.y_position)
 
-        return self.try_execute_single_update(insert, "{}-point{}".format(location.mrid, sequence_number), "position point")
+        return self._try_execute_single_update(insert, "{}-point{}".format(location.mrid, sequence_number), "position point")
 
-    def save_street_address(self, table: TableStreetAddresses, insert: PreparedStatement, street_address: StreetAddress, street_id: str,
-                            description: str) -> bool:
+    def _save_street_address(self, table: TableStreetAddresses, insert: PreparedStatement, street_address: StreetAddress, street_id: str,
+                             description: str) -> bool:
         insert.add_value(table.postal_code.query_index, street_address.postal_code)
         insert.add_value(table.po_box.query_index, street_address.po_box)
 
         self.insert_street_detail(table, insert, street_address.street_detail)
         self.insert_town_detail(table, insert, street_address.town_detail)
 
-        return self.try_execute_single_update(insert, street_id, description)
+        return self._try_execute_single_update(insert, street_id, description)
+
+    # ************ IEC61968 infIEC61968 InfAssetInfo ************
+
+    def save_current_relay_info(self, current_relay_info: CurrentRelayInfo) -> bool:
+        table = self.database_tables.get_table(TableCurrentRelayInfo)
+        insert = self.database_tables.get_insert(TableCurrentRelayInfo)
+
+        insert.add_value(table.curve_setting.query_index, current_relay_info.curve_setting)
+
+        return self._save_asset_info(table, insert, current_relay_info, "current relay info")
 
     # ************ IEC61968 infIEC61968 InfAssetInfo ************
 
     def save_current_transformer_info(self, current_transformer_info: CurrentTransformerInfo):
         table = self.database_tables.get_table(TableCurrentTransformerInfo)
         insert = self.database_tables.get_insert(TableCurrentTransformerInfo)
 
@@ -284,61 +301,60 @@
         insert.add_ratio(table.nominal_ratio_numerator.query_index, table.nominal_ratio_denominator.query_index, current_transformer_info.nominal_ratio)
         insert.add_value(table.primary_ratio.query_index, current_transformer_info.primary_ratio)
         insert.add_value(table.rated_current.query_index, current_transformer_info.rated_current)
         insert.add_value(table.secondary_fls_rating.query_index, current_transformer_info.secondary_fls_rating)
         insert.add_value(table.secondary_ratio.query_index, current_transformer_info.secondary_ratio)
         insert.add_value(table.usage.query_index, current_transformer_info.usage)
 
-        return self.save_asset_info(table, insert, current_transformer_info, "current transformer info")
+        return self._save_asset_info(table, insert, current_transformer_info, "current transformer info")
 
     def save_potential_transformer_info(self, potential_transformer_info: PotentialTransformerInfo):
         table = self.database_tables.get_table(TablePotentialTransformerInfo)
         insert = self.database_tables.get_insert(TablePotentialTransformerInfo)
 
         insert.add_value(table.accuracy_class.query_index, potential_transformer_info.accuracy_class)
         insert.add_ratio(table.nominal_ratio_numerator.query_index, table.nominal_ratio_denominator.query_index, potential_transformer_info.nominal_ratio)
         insert.add_value(table.primary_ratio.query_index, potential_transformer_info.primary_ratio)
         insert.add_value(table.pt_class.query_index, potential_transformer_info.pt_class)
         insert.add_value(table.rated_voltage.query_index, potential_transformer_info.rated_voltage)
         insert.add_value(table.secondary_ratio.query_index, potential_transformer_info.secondary_ratio)
 
-        return self.save_asset_info(table, insert, potential_transformer_info, "potential transformer info")
-
+        return self._save_asset_info(table, insert, potential_transformer_info, "potential transformer info")
 
     # ************ IEC61968 METERING ************
 
-    def save_end_device(self, table: TableEndDevices, insert: PreparedStatement, end_device: EndDevice, description: str) -> bool:
+    def _save_end_device(self, table: TableEndDevices, insert: PreparedStatement, end_device: EndDevice, description: str) -> bool:
         insert.add_value(table.customer_mrid.query_index, end_device.customer_mrid)
         insert.add_value(table.service_location_mrid.query_index, self._mrid_or_none(end_device.service_location))
 
         status = True
         for e in end_device.usage_points:
             status = status and self._save_usage_point_to_end_device_association(e, end_device)
 
-        return status and self.save_asset_container(table, insert, end_device, description)
+        return status and self._save_asset_container(table, insert, end_device, description)
 
     def save_meter(self, meter: Meter) -> bool:
         table = self.database_tables.get_table(TableMeters)
         insert = self.database_tables.get_insert(TableMeters)
 
-        return self.save_end_device(table, insert, meter, "meter")
+        return self._save_end_device(table, insert, meter, "meter")
 
     def save_usage_point(self, usage_point: UsagePoint) -> bool:
         table = self.database_tables.get_table(TableUsagePoints)
         insert = self.database_tables.get_insert(TableUsagePoints)
 
         insert.add_value(table.location_mrid.query_index, self._mrid_or_none(usage_point.usage_point_location))
         insert.add_value(table.is_virtual.query_index, int(usage_point.is_virtual))
         insert.add_value(table.connection_category.query_index, usage_point.connection_category)
 
         status = True
         for e in usage_point.equipment:
             status = status and self._save_equipment_to_usage_point_association(e, usage_point)
 
-        return status and self.save_identified_object(table, insert, usage_point, "usage point")
+        return status and self._save_identified_object(table, insert, usage_point, "usage point")
 
     # ************ IEC61968 OPERATIONS ************
 
     def save_operational_restriction(self, operational_restriction: OperationalRestriction) -> bool:
         table = self.database_tables.get_table(TableOperationalRestrictions)
         insert = self.database_tables.get_insert(TableOperationalRestrictions)
 
@@ -350,15 +366,15 @@
 
     # ************ IEC61970 AUXILIARY EQUIPMENT ************
 
     def save_auxiliary_equipment(self, table: TableAuxiliaryEquipment, insert: PreparedStatement, auxiliary_equipment: AuxiliaryEquipment,
                                  description: str) -> bool:
         insert.add_value(table.terminal_mrid.query_index, self._mrid_or_none(auxiliary_equipment.terminal))
 
-        return self.save_equipment(table, insert, auxiliary_equipment, description)
+        return self._save_equipment(table, insert, auxiliary_equipment, description)
 
     def save_current_transformer(self, current_transformer: CurrentTransformer) -> bool:
         table = self.database_tables.get_table(TableCurrentTransformers)
         insert = self.database_tables.get_insert(TableCurrentTransformers)
 
         insert.add_value(table.current_transformer_info_mrid.query_index, self._mrid_or_none(current_transformer.current_transformer_info))
         insert.add_value(table.core_burden.query_index, current_transformer.core_burden)
@@ -379,45 +395,45 @@
         insert.add_value(table.type.query_index, potential_transformer.type.short_name)
 
         return self.save_sensor(table, insert, potential_transformer, "potential transformer")
 
     def save_sensor(self, table: TableSensors, insert: PreparedStatement, sensor: Sensor, description: str) -> bool:
         return self.save_auxiliary_equipment(table, insert, sensor, description)
 
-    # ************ IEC6190 CORE ************
+    # ************ IEC6190 BASE CORE ************
 
     def _save_ac_dc_terminal(self, table: TableAcDcTerminals, insert: PreparedStatement,
                              ac_dc_terminal: AcDcTerminal, description: str) -> bool:
-        return self.save_identified_object(table, insert, ac_dc_terminal, description)
+        return self._save_identified_object(table, insert, ac_dc_terminal, description)
 
     def save_base_voltage(self, base_voltage: BaseVoltage) -> bool:
         table = self.database_tables.get_table(TableBaseVoltages)
         insert = self.database_tables.get_insert(TableBaseVoltages)
 
         insert.add_value(table.nominal_voltage.query_index, base_voltage.nominal_voltage)
 
-        return self.save_identified_object(table, insert, base_voltage, "base voltage")
+        return self._save_identified_object(table, insert, base_voltage, "base voltage")
 
     def _save_conducting_equipment(self, table: TableConductingEquipment, insert: PreparedStatement, conducting_equipment: ConductingEquipment,
                                    description: str) -> bool:
         insert.add_value(table.base_voltage_mrid.query_index, self._mrid_or_none(conducting_equipment.base_voltage))
 
-        return self.save_equipment(table, insert, conducting_equipment, description)
+        return self._save_equipment(table, insert, conducting_equipment, description)
 
     def save_connectivity_node(self, connectivity_node: ConnectivityNode) -> bool:
         table = self.database_tables.get_table(TableConnectivityNodes)
         insert = self.database_tables.get_insert(TableConnectivityNodes)
 
-        return self.save_identified_object(table, insert, connectivity_node, "connectivity node")
+        return self._save_identified_object(table, insert, connectivity_node, "connectivity node")
 
     def _save_connectivity_node_container(self, table: TableConnectivityNodeContainers, insert: PreparedStatement,
                                           connectivity_node_container: ConnectivityNodeContainer, description: str) -> bool:
         return self._save_power_system_resource(table, insert, connectivity_node_container, description)
 
-    def save_equipment(self, table: TableEquipment, insert: PreparedStatement, equipment: Equipment, description: str) -> bool:
+    def _save_equipment(self, table: TableEquipment, insert: PreparedStatement, equipment: Equipment, description: str) -> bool:
         insert.add_value(table.normally_in_service.query_index, int(equipment.normally_in_service))
         insert.add_value(table.in_service.query_index, int(equipment.in_service))
         status = True
         for e in equipment.containers:
             if not isinstance(e, Feeder):
                 status = status and self._save_equipment_to_equipment_container_association(equipment, e)
 
@@ -438,39 +454,39 @@
 
         return self._save_equipment_container(table, insert, feeder, "feeder")
 
     def save_geographical_region(self, geographical_region: GeographicalRegion) -> bool:
         table = self.database_tables.get_table(TableGeographicalRegions)
         insert = self.database_tables.get_insert(TableGeographicalRegions)
 
-        return self.save_identified_object(table, insert, geographical_region, "geographical region")
+        return self._save_identified_object(table, insert, geographical_region, "geographical region")
 
     def _save_power_system_resource(self,
                                     table: TablePowerSystemResources,
                                     insert: PreparedStatement,
                                     power_system_resource: PowerSystemResource,
                                     description: str) -> bool:
         insert.add_value(table.location_mrid.query_index, self._mrid_or_none(power_system_resource.location))
         insert.add_value(table.num_controls.query_index, 0)  # Currently unused
 
-        return self.save_identified_object(table, insert, power_system_resource, description)
+        return self._save_identified_object(table, insert, power_system_resource, description)
 
     def save_site(self, site: Site) -> bool:
         table = self.database_tables.get_table(TableSites)
         insert = self.database_tables.get_insert(TableSites)
 
         return self._save_equipment_container(table, insert, site, "site")
 
     def save_sub_geographical_region(self, sub_geographical_region: SubGeographicalRegion) -> bool:
         table = self.database_tables.get_table(TableSubGeographicalRegions)
         insert = self.database_tables.get_insert(TableSubGeographicalRegions)
 
         insert.add_value(table.geographical_region_mrid.query_index, self._mrid_or_none(sub_geographical_region.geographical_region))
 
-        return self.save_identified_object(table, insert, sub_geographical_region, "sub-geographical region")
+        return self._save_identified_object(table, insert, sub_geographical_region, "sub-geographical region")
 
     def save_substation(self, substation: Substation) -> bool:
         table = self.database_tables.get_table(TableSubstations)
         insert = self.database_tables.get_insert(TableSubstations)
 
         insert.add_value(table.sub_geographical_region_mrid.query_index, self._mrid_or_none(substation.sub_geographical_region))
 
@@ -483,15 +499,15 @@
         insert.add_value(table.conducting_equipment_mrid.query_index, self._mrid_or_none(terminal.conducting_equipment))
         insert.add_value(table.sequence_number.query_index, terminal.sequence_number)
         insert.add_value(table.connectivity_node_mrid.query_index, self._mrid_or_none(terminal.connectivity_node))
         insert.add_value(table.phases.query_index, terminal.phases.short_name)
 
         return self._save_ac_dc_terminal(table, insert, terminal, "terminal")
 
-    # ************ IEC61970 WIRES ************
+    # ************ IEC61970 BASE EQUIVALENTS ************
 
     def save_equivalent_branch(self, equivalent_branch: EquivalentBranch) -> bool:
         table = self.database_tables.get_table(TableEquivalentBranches)
         insert = self.database_tables.get_insert(TableEquivalentBranches)
 
         insert.add_value(table.negative_r12.query_index, equivalent_branch.negative_r12)
         insert.add_value(table.negative_r21.query_index, equivalent_branch.negative_r21)
@@ -512,56 +528,90 @@
 
         return self._save_equivalent_equipment(table, insert, equivalent_branch, "equivalent branch")
 
     def _save_equivalent_equipment(self, table: TableEquivalentEquipment, insert: PreparedStatement, equivalent_equipment: EquivalentEquipment,
                                    description: str) -> bool:
         return self._save_conducting_equipment(table, insert, equivalent_equipment, description)
 
-    def save_power_electronics_unit(self, table: TablePowerElectronicsUnit, insert: PreparedStatement, power_electronics_unit: PowerElectronicsUnit,
-                                    description: str) -> bool:
+    # ************ IEC61970 Base Protection ************
+
+    def save_current_relay(self, current_relay: CurrentRelay) -> bool:
+        table = self.database_tables.get_table(TableCurrentRelays)
+        insert = self.database_tables.get_insert(TableCurrentRelays)
+
+        insert.add_value(table.current_limit_1.query_index, current_relay.current_limit_1)
+        insert.add_value(table.inverse_time_flag.query_index, current_relay.inverse_time_flag)
+        insert.add_value(table.time_delay_1.query_index, current_relay.time_delay_1)
+        insert.add_value(table.current_relay_info_mrid.query_index, self._mrid_or_none(current_relay.current_relay_info))
+
+        return self._save_protection_equipment(table, insert, current_relay, "current relay")
+
+    def _save_protection_equipment(self, table: TableProtectionEquipment, insert: PreparedStatement, protection_equipment: ProtectionEquipment,
+                                   description: str) -> bool:
+        insert.add_value(table.relay_delay_time.query_index, protection_equipment.relay_delay_time)
+        insert.add_value(table.protection_kind.query_index, protection_equipment.protection_kind.short_name)
+
+        return self._save_equipment(table, insert, protection_equipment, description)
+
+    def _save_reclose_sequence(self, protected_switch: ProtectedSwitch, reclose_sequence: RecloseSequence) -> bool:
+        table = self.database_tables.get_table(TableRecloseSequences)
+        insert = self.database_tables.get_insert(TableRecloseSequences)
+
+        insert.add_value(table.protected_switch_mrid.query_index, protected_switch.mrid)
+        insert.add_value(table.reclose_delay.query_index, reclose_sequence.reclose_delay)
+        insert.add_value(table.reclose_step.query_index, reclose_sequence.reclose_step)
+
+        return self._save_identified_object(table, insert, reclose_sequence, "reclose sequence")
+
+    # ************ IEC61970 BASE WIRES ************
+
+    def _save_power_electronics_unit(self, table: TablePowerElectronicsUnit, insert: PreparedStatement, power_electronics_unit: PowerElectronicsUnit,
+                                     description: str) -> bool:
         insert.add_value(table.power_electronics_connection_mrid.query_index, self._mrid_or_none(power_electronics_unit.power_electronics_connection))
         insert.add_value(table.max_p.query_index, power_electronics_unit.max_p)
         insert.add_value(table.min_p.query_index, power_electronics_unit.min_p)
 
-        return self.save_equipment(table, insert, power_electronics_unit, description)
+        return self._save_equipment(table, insert, power_electronics_unit, description)
 
     def save_battery_unit(self, battery_unit: BatteryUnit) -> bool:
         table = self.database_tables.get_table(TableBatteryUnit)
         insert = self.database_tables.get_insert(TableBatteryUnit)
 
         insert.add_value(table.battery_state.query_index, battery_unit.battery_state.short_name)
         insert.add_value(table.rated_e.query_index, battery_unit.rated_e)
         insert.add_value(table.stored_e.query_index, battery_unit.stored_e)
 
-        return self.save_power_electronics_unit(table, insert, battery_unit, "battery unit")
+        return self._save_power_electronics_unit(table, insert, battery_unit, "battery unit")
 
     def save_photovoltaic_unit(self, photovoltaic_unit: PhotoVoltaicUnit) -> bool:
         table = self.database_tables.get_table(TablePhotoVoltaicUnit)
         insert = self.database_tables.get_insert(TablePhotoVoltaicUnit)
 
-        return self.save_power_electronics_unit(table, insert, photovoltaic_unit, "photo voltaic unit")
+        return self._save_power_electronics_unit(table, insert, photovoltaic_unit, "photo voltaic unit")
 
     def save_power_electronics_wind_unit(self, power_electronics_wind_unit: PowerElectronicsWindUnit) -> bool:
         table = self.database_tables.get_table(TablePowerElectronicsWindUnit)
         insert = self.database_tables.get_insert(TablePowerElectronicsWindUnit)
 
-        return self.save_power_electronics_unit(table, insert, power_electronics_wind_unit, "power electronics wind unit")
+        return self._save_power_electronics_unit(table, insert, power_electronics_wind_unit, "power electronics wind unit")
 
     def save_ac_line_segment(self, ac_line_segment: AcLineSegment) -> bool:
         table = self.database_tables.get_table(TableAcLineSegments)
         insert = self.database_tables.get_insert(TableAcLineSegments)
 
         insert.add_value(table.per_length_sequence_impedance_mrid.query_index, self._mrid_or_none(ac_line_segment.per_length_sequence_impedance))
 
         return self._save_conductor(table, insert, ac_line_segment, "AC line segment")
 
     def save_breaker(self, breaker: Breaker) -> bool:
         table = self.database_tables.get_table(TableBreakers)
         insert = self.database_tables.get_insert(TableBreakers)
 
+        insert.add_value(table.in_transit_time.query_index, breaker.in_transit_time)
+
         return self._save_protected_switch(table, insert, breaker, "breaker")
 
     def save_load_break_switch(self, load_break_switch: LoadBreakSwitch) -> bool:
         table = self.database_tables.get_table(TableLoadBreakSwitches)
         insert = self.database_tables.get_insert(TableLoadBreakSwitches)
 
         return self._save_protected_switch(table, insert, load_break_switch, "load break switch")
@@ -699,15 +749,15 @@
                                    per_length_sequence_impedance: PerLengthImpedance, description: str) -> bool:
         return self._save_per_length_line_parameter(table, insert, per_length_sequence_impedance, description)
 
     def _save_per_length_line_parameter(self, table: TablePerLengthLineParameters,
                                         insert: PreparedStatement,
                                         per_length_line_parameter: PerLengthLineParameter,
                                         description: str) -> bool:
-        return self.save_identified_object(table, insert, per_length_line_parameter, description)
+        return self._save_identified_object(table, insert, per_length_line_parameter, description)
 
     def save_per_length_sequence_impedance(self, per_length_sequence_impedance: PerLengthSequenceImpedance) -> bool:
         table = self.database_tables.get_table(TablePerLengthSequenceImpedances)
         insert = self.database_tables.get_insert(TablePerLengthSequenceImpedances)
 
         insert.add_value(table.r.query_index, per_length_sequence_impedance.r)
         insert.add_value(table.x.query_index, per_length_sequence_impedance.x)
@@ -776,15 +826,23 @@
         insert.add_value(table.rated_u.query_index, power_transformer_end.rated_u)
         insert.add_value(table.x.query_index, power_transformer_end.x)
         insert.add_value(table.x0.query_index, power_transformer_end.x0)
 
         return self._save_transformer_end(table, insert, power_transformer_end, "power transformer end")
 
     def _save_protected_switch(self, table: TableProtectedSwitches, insert: PreparedStatement, protected_switch: ProtectedSwitch, description: str) -> bool:
-        return self._save_switch(table, insert, protected_switch, description)
+        insert.add_value(table.breaking_capacity.query_index, protected_switch.breaking_capacity)
+
+        status = True
+        for rs in protected_switch.reclose_sequences:
+            status = status and self._save_reclose_sequence(protected_switch, rs)
+        for pe in protected_switch.operated_by_protection_equipment:
+            status = status and self._save_protection_equipment_protected_switch(pe, protected_switch)
+
+        return status and self._save_switch(table, insert, protected_switch, description)
 
     def save_ratio_tap_changer(self, ratio_tap_changer: RatioTapChanger) -> bool:
         table = self.database_tables.get_table(TableRatioTapChangers)
         insert = self.database_tables.get_insert(TableRatioTapChangers)
 
         insert.add_value(table.transformer_end_mrid.query_index, self._mrid_or_none(ratio_tap_changer.transformer_end))
         insert.add_value(table.step_voltage_increment.query_index, ratio_tap_changer.step_voltage_increment)
@@ -809,16 +867,18 @@
         insert.add_value(table.phase_connection.query_index, shunt_compensator.phase_connection.short_name)
         insert.add_value(table.sections.query_index, shunt_compensator.sections)
 
         return self._save_regulating_cond_eq(table, insert, shunt_compensator, description)
 
     def _save_switch(self, table: TableSwitches,
                      insert: PreparedStatement, switch: Switch, description: str) -> bool:
+        insert.add_value(table.rated_current.query_index, switch.rated_current)
         insert.add_value(table.normal_open.query_index, int(switch.is_normally_open()))
         insert.add_value(table.open.query_index, int(switch.is_open()))
+        insert.add_value(table.switch_info_mrid.query_index, self._mrid_or_none(switch.switch_info))
 
         return self._save_conducting_equipment(table, insert, switch, description)
 
     def _save_tap_changer(self, table: TableTapChangers, insert: PreparedStatement, tap_changer: TapChanger, description: str) -> bool:
         insert.add_value(table.control_enabled.query_index, tap_changer.control_enabled)
         insert.add_value(table.high_step.query_index, tap_changer.high_step)
         insert.add_value(table.low_step.query_index, tap_changer.low_step)
@@ -834,27 +894,27 @@
         insert.add_value(table.terminal_mrid.query_index, self._mrid_or_none(transformer_end.terminal))
         insert.add_value(table.base_voltage_mrid.query_index, self._mrid_or_none(transformer_end.base_voltage))
         insert.add_value(table.grounded.query_index, transformer_end.grounded)
         insert.add_value(table.r_ground.query_index, transformer_end.r_ground)
         insert.add_value(table.x_ground.query_index, transformer_end.x_ground)
         insert.add_value(table.star_impedance_mrid.query_index, self._mrid_or_none(transformer_end.star_impedance))
 
-        return self.save_identified_object(table, insert, transformer_end, description)
+        return self._save_identified_object(table, insert, transformer_end, description)
 
     def save_transformer_star_impedance(self, transformer_star_impedance: TransformerStarImpedance) -> bool:
         table = self.database_tables.get_table(TableTransformerStarImpedance)
         insert = self.database_tables.get_insert(TableTransformerStarImpedance)
 
         insert.add_value(table.r.query_index, transformer_star_impedance.r)
         insert.add_value(table.r0.query_index, transformer_star_impedance.r0)
         insert.add_value(table.x.query_index, transformer_star_impedance.x)
         insert.add_value(table.x0.query_index, transformer_star_impedance.x0)
         insert.add_value(table.transformer_end_info_mrid.query_index, self._mrid_or_none(transformer_star_impedance.transformer_end_info))
 
-        return self.save_identified_object(table, insert, transformer_star_impedance, "transformer star impedance")
+        return self._save_identified_object(table, insert, transformer_star_impedance, "transformer star impedance")
 
     # ************ IEC61970 InfIEC61970 ************
 
     def save_circuit(self, circuit: Circuit) -> bool:
         table = self.database_tables.get_table(TableCircuits)
         insert = self.database_tables.get_insert(TableCircuits)
 
@@ -873,154 +933,165 @@
         insert = self.database_tables.get_insert(TableLoops)
 
         status = True
         for sub in loop.energizing_substations:
             status = status and self._save_loop_to_substation_association(loop, sub, LoopSubstationRelationship.SUBSTATION_ENERGIZES_LOOP)
         for sub in loop.substations:
             status = status and self._save_loop_to_substation_association(loop, sub, LoopSubstationRelationship.LOOP_ENERGIZES_SUBSTATION)
-        return status and self.save_identified_object(table, insert, loop, "loop")
+        return status and self._save_identified_object(table, insert, loop, "loop")
 
     def save_lv_feeder(self, lv_feeder: LvFeeder) -> bool:
         table = self.database_tables.get_table(TableLvFeeders)
         insert = self.database_tables.get_insert(TableLvFeeders)
 
         insert.add_value(table.normal_head_terminal_mrid.query_index, self._mrid_or_none(lv_feeder.normal_head_terminal))
 
         return self._save_equipment_container(table, insert, lv_feeder, "lv_feeder")
 
     # ************ IEC61970 MEAS ************
 
-    def save_measurement(self, table: TableMeasurements, insert: PreparedStatement, measurement: Measurement, description: str) -> bool:
+    def _save_measurement(self, table: TableMeasurements, insert: PreparedStatement, measurement: Measurement, description: str) -> bool:
         insert.add_value(table.power_system_resource_mrid.query_index, measurement.power_system_resource_mrid)
         insert.add_value(table.remote_source_mrid.query_index, self._mrid_or_none(measurement.remote_source))
         insert.add_value(table.terminal_mrid.query_index, measurement.terminal_mrid)
         insert.add_value(table.phases.query_index, measurement.phases.short_name)
         insert.add_value(table.unit_symbol.query_index, measurement.unit_symbol.short_name)
 
-        return self.save_identified_object(table, insert, measurement, description)
+        return self._save_identified_object(table, insert, measurement, description)
 
     def save_analog(self, analog: Analog) -> bool:
         table = self.database_tables.get_table(TableAnalogs)
         insert = self.database_tables.get_insert(TableAnalogs)
 
         insert.add_value(table.positive_flow_in.query_index, analog.positive_flow_in)
 
-        return self.save_measurement(table, insert, analog, "analog")
+        return self._save_measurement(table, insert, analog, "analog")
 
     def save_accumulator(self, accumulator: Accumulator) -> bool:
         table = self.database_tables.get_table(TableAccumulators)
         insert = self.database_tables.get_insert(TableAccumulators)
 
-        return self.save_measurement(table, insert, accumulator, "accumulator")
+        return self._save_measurement(table, insert, accumulator, "accumulator")
 
     def save_discrete(self, discrete: Discrete) -> bool:
         table = self.database_tables.get_table(TableDiscretes)
         insert = self.database_tables.get_insert(TableDiscretes)
 
-        return self.save_measurement(table, insert, discrete, "discrete")
+        return self._save_measurement(table, insert, discrete, "discrete")
 
     def save_control(self, control: Control) -> bool:
         table = self.database_tables.get_table(TableControls)
         insert = self.database_tables.get_insert(TableControls)
 
         insert.add_value(table.power_system_resource_mrid.query_index, control.power_system_resource_mrid)
 
-        return self.save_io_point(table, insert, control, "control")
+        return self._save_io_point(table, insert, control, "control")
 
-    def save_io_point(self, table: TableIoPoints, insert: PreparedStatement, io_point: IoPoint, description: str) -> bool:
-        return self.save_identified_object(table, insert, io_point, description)
+    def _save_io_point(self, table: TableIoPoints, insert: PreparedStatement, io_point: IoPoint, description: str) -> bool:
+        return self._save_identified_object(table, insert, io_point, description)
 
     # ************ IEC61970 SCADA ************
 
     def save_remote_control(self, remote_control: RemoteControl) -> bool:
         table = self.database_tables.get_table(TableRemoteControls)
         insert = self.database_tables.get_insert(TableRemoteControls)
 
         insert.add_value(table.control_mrid.query_index, self._mrid_or_none(remote_control.control))
 
-        return self.save_remote_point(table, insert, remote_control, "remote control")
+        return self._save_remote_point(table, insert, remote_control, "remote control")
 
-    def save_remote_point(self, table: TableRemotePoints, insert: PreparedStatement, remote_point: RemotePoint, description: str) -> bool:
-        return self.save_identified_object(table, insert, remote_point, description)
+    def _save_remote_point(self, table: TableRemotePoints, insert: PreparedStatement, remote_point: RemotePoint, description: str) -> bool:
+        return self._save_identified_object(table, insert, remote_point, description)
 
     def save_remote_source(self, remote_source: RemoteSource) -> bool:
         table = self.database_tables.get_table(TableRemoteSources)
 
         insert = self.database_tables.get_insert(TableRemoteSources)
         insert.add_value(table.measurement_mrid.query_index, self._mrid_or_none(remote_source.measurement))
 
-        return self.save_remote_point(table, insert, remote_source, "remote source")
+        return self._save_remote_point(table, insert, remote_source, "remote source")
 
     # ************ ASSOCIATIONS ************
 
     def _save_asset_organisation_role_to_asset_association(self, asset_organisation_role: AssetOrganisationRole, asset: Asset) -> bool:
         table = self.database_tables.get_table(TableAssetOrganisationRolesAssets)
         insert = self.database_tables.get_insert(TableAssetOrganisationRolesAssets)
 
         insert.add_value(table.asset_organisation_role_mrid.query_index, asset_organisation_role.mrid)
         insert.add_value(table.asset_mrid.query_index, asset.mrid)
 
-        return self.try_execute_single_update(insert, f"{asset_organisation_role.mrid}-to-{asset.mrid}", "asset organisation role to asset association")
+        return self._try_execute_single_update(insert, f"{asset_organisation_role.mrid}-to-{asset.mrid}", "asset organisation role to asset association")
 
     def _save_usage_point_to_end_device_association(self, usage_point: UsagePoint, end_device: EndDevice) -> bool:
         table = self.database_tables.get_table(TableUsagePointsEndDevices)
         insert = self.database_tables.get_insert(TableUsagePointsEndDevices)
 
         insert.add_value(table.usage_point_mrid.query_index, usage_point.mrid)
         insert.add_value(table.end_device_mrid.query_index, end_device.mrid)
 
-        return self.try_execute_single_update(insert, f"{usage_point.mrid}-to-{end_device.mrid}", "usage point to end device association")
+        return self._try_execute_single_update(insert, f"{usage_point.mrid}-to-{end_device.mrid}", "usage point to end device association")
 
     def _save_equipment_to_usage_point_association(self, equipment: Equipment, usage_point: UsagePoint) -> bool:
         table = self.database_tables.get_table(TableEquipmentUsagePoints)
         insert = self.database_tables.get_insert(TableEquipmentUsagePoints)
 
         insert.add_value(table.equipment_mrid.query_index, equipment.mrid)
         insert.add_value(table.usage_point_mrid.query_index, usage_point.mrid)
 
-        return self.try_execute_single_update(insert, f"{equipment.mrid}-to-{usage_point.mrid}", "Equipment to UsagePoint association ")
+        return self._try_execute_single_update(insert, f"{equipment.mrid}-to-{usage_point.mrid}", "Equipment to UsagePoint association ")
 
     def _save_equipment_to_operational_restriction_association(self, equipment: Equipment, operational_restriction: OperationalRestriction) -> bool:
         table = self.database_tables.get_table(TableEquipmentOperationalRestrictions)
         insert = self.database_tables.get_insert(TableEquipmentOperationalRestrictions)
 
         insert.add_value(table.equipment_mrid.query_index, equipment.mrid)
         insert.add_value(table.operational_restriction_mrid.query_index, operational_restriction.mrid)
 
-        return self.try_execute_single_update(insert, f"{equipment.mrid}-to-{operational_restriction.mrid}", "equipment to operational restriction association")
+        return self._try_execute_single_update(insert, f"{equipment.mrid}-to-{operational_restriction.mrid}",
+                                               "equipment to operational restriction association")
 
     def _save_equipment_to_equipment_container_association(self, equipment: Equipment, equipment_container: EquipmentContainer) -> bool:
         table = self.database_tables.get_table(TableEquipmentEquipmentContainers)
         insert = self.database_tables.get_insert(TableEquipmentEquipmentContainers)
 
         insert.add_value(table.equipment_mrid.query_index, equipment.mrid)
         insert.add_value(table.equipment_container_mrid.query_index, equipment_container.mrid)
 
-        return self.try_execute_single_update(insert, f"{equipment.mrid}-to-{equipment_container.mrid}", "equipment to equipment container association")
+        return self._try_execute_single_update(insert, f"{equipment.mrid}-to-{equipment_container.mrid}", "equipment to equipment container association")
 
     def _save_circuit_to_substation_association(self, circuit: Circuit, substation: Substation) -> bool:
         table = self.database_tables.get_table(TableCircuitsSubstations)
         insert = self.database_tables.get_insert(TableCircuitsSubstations)
 
         insert.add_value(table.circuit_mrid.query_index, circuit.mrid)
         insert.add_value(table.substation_mrid.query_index, substation.mrid)
 
-        return self.try_execute_single_update(insert, f"{circuit.mrid}-to-{substation.mrid}", "circuit to substation association")
+        return self._try_execute_single_update(insert, f"{circuit.mrid}-to-{substation.mrid}", "circuit to substation association")
 
     def _save_circuit_to_terminal_association(self, circuit: Circuit, terminal: Terminal) -> bool:
         table = self.database_tables.get_table(TableCircuitsTerminals)
         insert = self.database_tables.get_insert(TableCircuitsTerminals)
 
         insert.add_value(table.circuit_mrid.query_index, circuit.mrid)
         insert.add_value(table.terminal_mrid.query_index, terminal.mrid)
 
-        return self.try_execute_single_update(insert, f"{circuit.mrid}-to-{terminal.mrid}", "circuit to terminal association")
+        return self._try_execute_single_update(insert, f"{circuit.mrid}-to-{terminal.mrid}", "circuit to terminal association")
 
     def _save_loop_to_substation_association(self, loop: Loop, substation: Substation, relationship: LoopSubstationRelationship) -> bool:
         table = self.database_tables.get_table(TableLoopsSubstations)
         insert = self.database_tables.get_insert(TableLoopsSubstations)
 
         insert.add_value(table.loop_mrid.query_index, loop.mrid)
         insert.add_value(table.substation_mrid.query_index, substation.mrid)
         insert.add_value(table.relationship.query_index, relationship.short_name)
 
-        return self.try_execute_single_update(insert, f"{loop.mrid}-to-{substation.mrid}", f"loop to substation association")
+        return self._try_execute_single_update(insert, f"{loop.mrid}-to-{substation.mrid}", f"loop to substation association")
+
+    def _save_protection_equipment_protected_switch(self, protection_equipment: ProtectionEquipment, protected_switch: ProtectedSwitch) -> bool:
+        table = self.database_tables.get_table(TableProtectionEquipmentProtectedSwitches)
+        insert = self.database_tables.get_insert(TableProtectionEquipmentProtectedSwitches)
+
+        insert.add_value(table.protection_equipment_mrid.query_index, protection_equipment.mrid)
+        insert.add_value(table.protected_switch_mrid.query_index, protected_switch.mrid)
+
+        return self._try_execute_single_update(insert, f"{protection_equipment.mrid}-to-{protected_switch.mrid}",
+                                               "protection equipment to protected switch association")
```

## zepben/evolve/database/sqlite/writers/network_service_writer.py

```diff
@@ -7,15 +7,15 @@
 from zepben.evolve import NetworkService, CableInfo, OverheadWireInfo, PowerTransformerInfo, TransformerTankInfo, NoLoadTest, OpenCircuitTest, \
     ShortCircuitTest, ShuntCompensatorInfo, TransformerEndInfo, AssetOwner, Pole, Streetlight, Location, Organisation, Meter, UsagePoint, \
     OperationalRestriction, FaultIndicator, BaseVoltage, ConnectivityNode, Feeder, GeographicalRegion, Site, SubGeographicalRegion, Substation, Terminal, \
     EquivalentBranch, PhotoVoltaicUnit, AcLineSegment, Breaker, LoadBreakSwitch, BusbarSection, Disconnector, EnergyConsumer, EnergyConsumerPhase, \
     EnergySource, EnergySourcePhase, Fuse, Jumper, Junction, LinearShuntCompensator, PerLengthSequenceImpedance, PowerElectronicsConnection, \
     PowerElectronicsConnectionPhase, PowerTransformer, PowerTransformerEnd, RatioTapChanger, Recloser, TransformerStarImpedance, Circuit, Loop, Analog, \
     Accumulator, Discrete, Control, RemoteControl, RemoteSource, BatteryUnit, PowerElectronicsWindUnit, LvFeeder, CurrentTransformerInfo, \
-    PotentialTransformerInfo, CurrentTransformer, PotentialTransformer
+    PotentialTransformerInfo, CurrentTransformer, PotentialTransformer, CurrentRelayInfo, CurrentRelay, SwitchInfo
 from zepben.evolve.database.sqlite.writers.base_service_writer import BaseServiceWriter
 from zepben.evolve.database.sqlite.writers.network_cim_writer import NetworkCIMWriter
 
 __all__ = ["NetworkServiceWriter"]
 
 
 class NetworkServiceWriter(BaseServiceWriter):
@@ -27,14 +27,15 @@
         status = status and self._save_all(service, OverheadWireInfo, writer.save_overhead_wire_info)
         status = status and self._save_all(service, PowerTransformerInfo, writer.save_power_transformer_info)
         status = status and self._save_all(service, TransformerTankInfo, writer.save_transformer_tank_info)
         status = status and self._save_all(service, NoLoadTest, writer.save_no_load_test)
         status = status and self._save_all(service, OpenCircuitTest, writer.save_open_circuit_test)
         status = status and self._save_all(service, ShortCircuitTest, writer.save_short_circuit_test)
         status = status and self._save_all(service, ShuntCompensatorInfo, writer.save_shunt_compensator_info)
+        status = status and self._save_all(service, SwitchInfo, writer.save_switch_info)
         status = status and self._save_all(service, TransformerEndInfo, writer.save_transformer_end_info)
         status = status and self._save_all(service, AssetOwner, writer.save_asset_owner)
         status = status and self._save_all(service, Pole, writer.save_pole)
         status = status and self._save_all(service, Streetlight, writer.save_streetlight)
         status = status and self._save_all(service, Location, writer.save_location)
         status = status and self._save_all_common(service, Organisation, writer.save_organisation)
         status = status and self._save_all(service, Meter, writer.save_meter)
@@ -83,9 +84,14 @@
         status = status and self._save_all(service, Control, writer.save_control)
         status = status and self._save_all(service, RemoteControl, writer.save_remote_control)
         status = status and self._save_all(service, RemoteSource, writer.save_remote_source)
         status = status and self._save_all(service, CurrentTransformerInfo, writer.save_current_transformer_info)
         status = status and self._save_all(service, PotentialTransformerInfo, writer.save_potential_transformer_info)
         status = status and self._save_all(service, CurrentTransformer, writer.save_current_transformer)
         status = status and self._save_all(service, PotentialTransformer, writer.save_potential_transformer)
+        status = status and self._save_all(service, CurrentRelayInfo, writer.save_current_relay_info)
+        status = status and self._save_all(service, CurrentRelay, writer.save_current_relay)
+
+        # Excluded:
+        #  - RecloseSequence: Saved via _save_protected_switch
 
         return status
```

## zepben/evolve/model/busbranch/bus_branch.py

```diff
@@ -5,15 +5,15 @@
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import abc
 from collections import Counter
 from dataclasses import dataclass, field
 from functools import reduce
 from typing import Set, Tuple, FrozenSet, Dict, Callable, Union, TypeVar, Any, List, Generic, Optional, Iterable
 
-from zepben.evolve import BasicTraversal, LifoQueue, Junction, BusbarSection, EquivalentBranch
+from zepben.evolve import BasicTraversal, Junction, BusbarSection, EquivalentBranch
 from zepben.evolve.model.cim.iec61970.base.core.conducting_equipment import ConductingEquipment
 from zepben.evolve.model.cim.iec61970.base.core.terminal import Terminal
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import AcLineSegment
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import EnergyConsumer
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import EnergySource
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import PowerElectronicsConnection
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import PowerTransformer, PowerTransformerEnd
```

## zepben/evolve/model/cim/iec61970/base/wires/switch.py

```diff
@@ -2,20 +2,24 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
+from typing import Optional, TYPE_CHECKING
+
 from zepben.evolve.model.cim.iec61970.base.core.conducting_equipment import ConductingEquipment
 from zepben.evolve.model.cim.iec61970.base.wires.single_phase_kind import SinglePhaseKind
+from zepben.evolve.util import require
 
-__all__ = ["Switch", "Breaker", "Disconnector", "Jumper", "Fuse", "ProtectedSwitch", "Recloser", "LoadBreakSwitch"]
+if TYPE_CHECKING:
+    from zepben.evolve import SwitchInfo
 
-from zepben.evolve.util import require
+__all__ = ["Switch"]
 
 
 def _calculate_open_state(current_state: int, is_open: bool, phase: SinglePhaseKind = None) -> int:
     require(phase != SinglePhaseKind.NONE and phase != SinglePhaseKind.INVALID,
             lambda: f"Invalid phase {phase} specified")
     if phase is None:
         return 0b1111 if is_open else 0
@@ -38,21 +42,37 @@
     All switches are two terminal devices including grounding switches.
 
     NOTE: The normal and currently open properties are implemented as an integer rather than a boolean to allow for the caching of
       measurement values if the switch is operating un-ganged. These values will cache the latest values from the measurement
       value for each phase of the switch.
     """
 
+    rated_current: Optional[int] = None
+    """The maximum continuous current carrying capacity in amps governed by the device material and construction. The attribute shall be a positive value."""
+
     _open: int = 0
     """Tells if the switch is considered open when used as input to topology processing."""
 
     _normally_open: int = 0
     """The attribute is used in cases when no Measurement for the status value is present. If the Switch has a status measurement the Discrete.normalValue 
     is expected to match with the Switch.normalOpen."""
 
+    @property
+    def switch_info(self) -> Optional[SwitchInfo]:
+        """Datasheet information for this Switch."""
+        return self.asset_info
+
+    @switch_info.setter
+    def switch_info(self, si: Optional[SwitchInfo]):
+        """
+        Set the :class:`SwitchInfo` for this :class:`Switch`
+        :param si: The SwitchInfo for this Switch
+        """
+        self.asset_info = si
+
     def is_normally_open(self, phase: SinglePhaseKind = None):
         """
         Check if the switch is normally open on `phase`.
 
         `phase` The `single_phase_kind.SinglePhaseKind` to check the normal status. A `phase` of `None` (default) checks if any phase is open.
         Returns True if `phase` is open in its normal state, False if it is closed
         """
@@ -94,64 +114,7 @@
         """
         `is_open` indicates if the phase(s) should be opened.
         `phase` the phase to set the current status. If set to None will default to all phases.
         Returns This `Switch` to be used fluently.
         """
         self._open = _calculate_open_state(self._open, is_open, phase)
         return self
-
-
-class ProtectedSwitch(Switch):
-    """
-    A ProtectedSwitch is a switching device that can be operated by ProtectionEquipment.
-    """
-    pass
-
-
-class Breaker(ProtectedSwitch):
-    """
-    A mechanical switching device capable of making, carrying, and breaking currents under normal circuit conditions
-    and also making, carrying for a specified time, and breaking currents under specified abnormal circuit conditions
-    e.g. those of short circuit.
-    """
-
-    def is_substation_breaker(self):
-        """Convenience function for detecting if this breaker is part of a substation. Returns true if this Breaker is associated with a Substation."""
-        return self.num_substations() > 0
-
-
-class Disconnector(Switch):
-    """
-    A manually operated or motor operated mechanical switching device used for changing the connections in a circuit,
-    or for isolating a circuit or equipment from a source of power. It is required to open or close circuits when
-    negligible current is broken or made.
-    """
-    pass
-
-
-class Fuse(Switch):
-    """
-    An overcurrent protective device with a circuit opening fusible part that is heated and severed by the passage of
-    overcurrent through it. A fuse is considered a switching device because it breaks current.
-    """
-    pass
-
-
-class Jumper(Switch):
-    """
-    A short section of conductor with negligible impedance which can be manually removed and replaced if the circuit is de-energized.
-    Note that zero-impedance branches can potentially be modeled by other equipment types.
-    """
-    pass
-
-
-class Recloser(ProtectedSwitch):
-    """
-    Pole-mounted fault interrupter with built-in phase and ground relays, current transformer (CT), and supplemental controls.
-    """
-    pass
-
-
-class LoadBreakSwitch(ProtectedSwitch):
-    """A mechanical switching device capable of making, carrying, and breaking currents under normal operating
-    conditions. """
-    pass
```

## zepben/evolve/services/common/reference_resolvers.py

```diff
@@ -6,29 +6,35 @@
 
 from __future__ import annotations
 
 from typing import Callable, Optional
 
 from dataclassy import dataclass
 
-from zepben.evolve import TransformerTankInfo, TransformerEndInfo, TransformerStarImpedance, NoLoadTest, ShortCircuitTest, OpenCircuitTest, ShuntCompensator, \
-    ShuntCompensatorInfo
+from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import NoLoadTest
+from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import OpenCircuitTest
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import PowerTransformerInfo
+from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import ShortCircuitTest
+from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import ShuntCompensatorInfo
+from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import SwitchInfo
+from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import TransformerEndInfo
+from zepben.evolve.model.cim.iec61968.assetinfo.transformer_tank_info import TransformerTankInfo
 from zepben.evolve.model.cim.iec61968.assetinfo.wire_info import WireInfo
 from zepben.evolve.model.cim.iec61968.assets.asset import Asset
 from zepben.evolve.model.cim.iec61968.assets.asset_organisation_role import AssetOrganisationRole
 from zepben.evolve.model.cim.iec61968.assets.pole import Pole
 from zepben.evolve.model.cim.iec61968.assets.streetlight import Streetlight
 from zepben.evolve.model.cim.iec61968.common.location import Location
 from zepben.evolve.model.cim.iec61968.common.organisation import Organisation
 from zepben.evolve.model.cim.iec61968.common.organisation_role import OrganisationRole
 from zepben.evolve.model.cim.iec61968.customers.customer import Customer
 from zepben.evolve.model.cim.iec61968.customers.customer_agreement import CustomerAgreement
 from zepben.evolve.model.cim.iec61968.customers.pricing_structure import PricingStructure
 from zepben.evolve.model.cim.iec61968.customers.tariff import Tariff
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import CurrentRelayInfo
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import CurrentTransformerInfo
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import PotentialTransformerInfo
 from zepben.evolve.model.cim.iec61968.metering.metering import EndDevice, UsagePoint
 from zepben.evolve.model.cim.iec61968.operations.operational_restriction import OperationalRestriction
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import AuxiliaryEquipment
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.current_transformer import CurrentTransformer
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.potential_transformer import PotentialTransformer
@@ -41,24 +47,31 @@
 from zepben.evolve.model.cim.iec61970.base.core.power_system_resource import PowerSystemResource
 from zepben.evolve.model.cim.iec61970.base.core.regions import GeographicalRegion, SubGeographicalRegion
 from zepben.evolve.model.cim.iec61970.base.core.substation import Substation
 from zepben.evolve.model.cim.iec61970.base.core.terminal import Terminal
 from zepben.evolve.model.cim.iec61970.base.diagramlayout.diagram_layout import Diagram, DiagramObject
 from zepben.evolve.model.cim.iec61970.base.meas.control import Control
 from zepben.evolve.model.cim.iec61970.base.meas.measurement import Measurement
+from zepben.evolve.model.cim.iec61970.base.protection.current_relay import CurrentRelay
+from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import ProtectionEquipment
+from zepben.evolve.model.cim.iec61970.base.protection.reclose_sequence import RecloseSequence
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import RemoteControl
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import RemoteSource
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import AcLineSegment, Conductor
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import EnergyConsumer, EnergyConsumerPhase
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import EnergySource
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import EnergySourcePhase
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import PowerElectronicsUnit
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import PerLengthSequenceImpedance
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import PowerElectronicsConnectionPhase, PowerElectronicsConnection
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import PowerTransformer, PowerTransformerEnd, RatioTapChanger, TransformerEnd
+from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import ProtectedSwitch
+from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import ShuntCompensator
+from zepben.evolve.model.cim.iec61970.base.wires.switch import Switch
+from zepben.evolve.model.cim.iec61970.base.wires.transformer_star_impedance import TransformerStarImpedance
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.circuit import Circuit
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.loop import Loop
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import LvFeeder
 
 __all__ = [
     "acls_to_plsi_resolver", "asset_to_asset_org_role_resolver", "asset_to_location_resolver", "pole_to_streetlight_resolver", "streetlight_to_pole_resolver",
     "aux_equip_to_term_resolver", "cond_equip_to_bv_resolver", "cond_equip_to_terminal_resolver", "conductor_to_wire_info_resolver",
@@ -71,15 +84,16 @@
     "sgr_to_gr_resolver", "sgr_to_sub_resolver", "sub_to_feeder_resolver", "sub_to_sgr_resolver", "sub_to_circuit_resolver", "sub_to_eloop_resolver",
     "sub_to_loop_resolver", "term_to_ce_resolver", "term_to_cn_resolver", "te_to_term_resolver", "te_to_bv_resolver", "te_to_rtc_resolver", "up_to_ed_resolver",
     "up_to_eq_resolver", "up_to_loc_resolver", "circuit_to_loop_resolver", "circuit_to_sub_resolver", "circuit_to_term_resolver", "loop_to_circuit_resolver",
     "loop_to_esub_resolver", "loop_to_sub_resolver", "BoundReferenceResolver", "ReferenceResolver", "UnresolvedReference", "tei_to_tti_resolver",
     "tti_to_tei_resolver", "tei_to_tsi_resolver", "tsi_to_tei_resolver", "te_to_tsi_resolver", "pti_to_tti_resolver", "peu_to_pec_resolver",
     "pec_to_peu_resolver", "pecphase_to_pec_resolver", "pec_to_pecphase_resolver", "tei_to_ee_nlt_resolver", "tei_to_ee_sct_resolver", "tei_to_ge_sct_resolver",
     "tei_to_oe_oct_resolver", "tei_to_ee_oct_resolver", "shunt_compensator_to_shunt_compensator_info_resolver", "lvfeeder_to_nht_resolver",
-    "lvfeeder_to_nef_resolver", "ct_to_cti_resolver", "vt_to_vti_resolver"
+    "lvfeeder_to_nef_resolver", "ct_to_cti_resolver", "vt_to_vti_resolver", "pe_to_ps_resolver", "ps_to_pe_resolver", "ps_to_rs_resolver",
+    "switch_to_switch_info_resolver", "current_relay_to_current_relay_info_resolver"
 ]
 
 
 @dataclass(frozen=True, eq=False, slots=True)
 class ReferenceResolver(object):
     from_class: type
     to_class: type
@@ -170,18 +184,22 @@
 aux_equip_to_term_resolver = ReferenceResolver(AuxiliaryEquipment, Terminal, lambda t, r: setattr(t, 'terminal', r))
 
 cond_equip_to_bv_resolver = ReferenceResolver(ConductingEquipment, BaseVoltage, lambda t, r: setattr(t, 'base_voltage', r))
 cond_equip_to_terminal_resolver = ReferenceResolver(ConductingEquipment, Terminal, _resolve_ce_term)
 
 conductor_to_wire_info_resolver = ReferenceResolver(Conductor, WireInfo, lambda t, r: setattr(t, 'asset_info', r))
 
+current_relay_to_current_relay_info_resolver = ReferenceResolver(CurrentRelay, CurrentRelayInfo, lambda t, r: setattr(t, 'asset_info', r))
+
 powertransformer_to_power_transformer_info_resolver = ReferenceResolver(PowerTransformer, PowerTransformerInfo, lambda t, r: setattr(t, 'asset_info', r))
 
 shunt_compensator_to_shunt_compensator_info_resolver = ReferenceResolver(ShuntCompensator, ShuntCompensatorInfo, lambda t, r: setattr(t, 'asset_info', r))
 
+switch_to_switch_info_resolver = ReferenceResolver(Switch, SwitchInfo, lambda t, r: setattr(t, 'asset_info', r))
+
 tei_to_tti_resolver = ReferenceResolver(TransformerEndInfo, TransformerTankInfo, lambda t, r: setattr(t, 'transformer_tank_info', r))
 
 tti_to_tei_resolver = ReferenceResolver(TransformerTankInfo, TransformerEndInfo, lambda t, r: t.add_transformer_end_info(r))
 
 tei_to_tsi_resolver = ReferenceResolver(TransformerEndInfo, TransformerStarImpedance, lambda t, r: setattr(t, 'transformer_star_impedance', r))
 
 tsi_to_tei_resolver = ReferenceResolver(TransformerStarImpedance, TransformerEndInfo, lambda t, r: setattr(t, 'transformer_end_info', r))
@@ -288,7 +306,11 @@
 tei_to_ge_sct_resolver = ReferenceResolver(TransformerEndInfo, ShortCircuitTest, lambda t, r: setattr(t, 'grounded_end_short_circuit_tests', r))
 tei_to_oe_oct_resolver = ReferenceResolver(TransformerEndInfo, OpenCircuitTest, lambda t, r: setattr(t, 'open_end_open_circuit_tests', r))
 tei_to_ee_oct_resolver = ReferenceResolver(TransformerEndInfo, OpenCircuitTest, lambda t, r: setattr(t, 'energised_end_open_circuit_tests', r))
 
 # To avoid confusion with PowerTransformer shortened as "pt", PotentialTransformer is shortened to "vt".
 ct_to_cti_resolver = ReferenceResolver(CurrentTransformer, CurrentTransformerInfo, lambda t, r: setattr(t, 'asset_info', r))
 vt_to_vti_resolver = ReferenceResolver(PotentialTransformer, PotentialTransformerInfo, lambda t, r: setattr(t, 'asset_info', r))
+
+pe_to_ps_resolver = ReferenceResolver(ProtectionEquipment, ProtectedSwitch, lambda t, r: t.add_protected_switch(r))
+ps_to_pe_resolver = ReferenceResolver(ProtectedSwitch, ProtectionEquipment, lambda t, r: t.add_operated_by_protection_equipment(r))
+ps_to_rs_resolver = ReferenceResolver(ProtectedSwitch, RecloseSequence, lambda t, r: t.add_reclose_sequence(r))
```

## zepben/evolve/services/common/resolver.py

```diff
@@ -7,15 +7,15 @@
 from __future__ import annotations
 
 from zepben.evolve import AcLineSegment, Asset, AuxiliaryEquipment, ConductingEquipment, Conductor, PowerTransformer, Pole, Streetlight, ConnectivityNode, \
     Control, Customer, CustomerAgreement, Diagram, DiagramObject, EndDevice, Equipment, EquipmentContainer, EnergyConsumer, EnergyConsumerPhase, EnergySource, \
     EnergySourcePhase, Feeder, GeographicalRegion, Measurement, OperationalRestriction, OrganisationRole, PowerSystemResource, PowerTransformerEnd, \
     PricingStructure, RatioTapChanger, RemoteControl, RemoteSource, SubGeographicalRegion, Substation, Terminal, TransformerEnd, UsagePoint, Circuit, Loop, \
     PowerElectronicsUnit, PowerElectronicsConnectionPhase, PowerElectronicsConnection, TransformerTankInfo, TransformerEndInfo, PowerTransformerInfo, \
-    TransformerStarImpedance, ShuntCompensator, LvFeeder, PotentialTransformer, CurrentTransformer
+    TransformerStarImpedance, ShuntCompensator, LvFeeder, PotentialTransformer, CurrentTransformer, ProtectionEquipment, ProtectedSwitch, Switch, CurrentRelay
 from zepben.evolve.services.common.reference_resolvers import *
 
 __all__ = ["per_length_sequence_impedance", "organisation_roles", "at_location", "ae_terminal", "ce_base_voltage", "ce_terminals",
            "asset_info", "streetlights", "pole", "cn_terminals", "remote_control", "agreements", "customer",
            "pricing_structures", "power_transformer_info",
            "diagram_objects", "diagram", "service_location", "ed_usage_points", "containers", "current_containers",
            "operational_restrictions",
@@ -25,15 +25,15 @@
            "psr_location", "ends", "power_transformer", "tariffs", "transformer_end", "control", "measurement",
            "geographical_region", "substations",
            "normal_energized_feeders", "sub_geographical_region", "conducting_equipment", "connectivity_node",
            "te_base_voltage", "ratio_tap_changer",
            "te_terminal", "end_devices", "up_equipment", "usage_point_location", "shunt_compensator_info",
            "transformer_end_info", "power_transformer_info_transformer_tank_info", "transformer_star_impedance",
            "star_impedance_transformer_end_info", "transformer_end_transformer_star_impedance", "normal_energized_lv_feeders",
-           "normal_energizing_feeders", "lv_feeder_normal_head_terminal", "normal_energizing_feeders"]
+           "normal_energizing_feeders", "lv_feeder_normal_head_terminal", "normal_energizing_feeders", "protected_switches"]
 
 
 def per_length_sequence_impedance(ac_line_segment: AcLineSegment):
     # noinspection PyArgumentList
     return BoundReferenceResolver(ac_line_segment, acls_to_plsi_resolver, None)
 
 
@@ -63,24 +63,34 @@
 
 
 def asset_info(conductor: Conductor) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(conductor, conductor_to_wire_info_resolver, None)
 
 
+def current_relay_info(cr: CurrentRelay) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(cr, current_relay_to_current_relay_info_resolver, None)
+
+
 def power_transformer_info(pt: PowerTransformer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(pt, powertransformer_to_power_transformer_info_resolver, None)
 
 
 def shunt_compensator_info(sc: ShuntCompensator) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(sc, shunt_compensator_to_shunt_compensator_info_resolver, None)
 
 
+def switch_info(switch: Switch) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(switch, switch_to_switch_info_resolver, None)
+
+
 def streetlights(p: Pole) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(p, pole_to_streetlight_resolver, streetlight_to_pole_resolver)
 
 
 def pole(streetlight: Streetlight) -> BoundReferenceResolver:
     # noinspection PyArgumentList
@@ -441,7 +451,22 @@
     # noinspection PyArgumentList
     return BoundReferenceResolver(current_transformer, ct_to_cti_resolver, None)
 
 
 def potential_transformer_info(potential_transformer: PotentialTransformer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(potential_transformer, vt_to_vti_resolver, None)
+
+
+def protected_switches(protection_equipment: ProtectionEquipment) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(protection_equipment, pe_to_ps_resolver, ps_to_pe_resolver)
+
+
+def operated_by_protection_equipment(protected_switch: ProtectedSwitch) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(protected_switch, ps_to_pe_resolver, pe_to_ps_resolver)
+
+
+def reclose_sequences(protected_switch: ProtectedSwitch) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(protected_switch, ps_to_rs_resolver, None)
```

## zepben/evolve/services/common/translator/util.py

```diff
@@ -1,19 +1,24 @@
 #  Copyright 2020 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
-from typing import Optional
+from typing import Optional, Dict
+
+# noinspection PyPackageRequirements
+# noinspection PyUnresolvedReferences
+# pylint: disable=import-error
+from google.protobuf.struct_pb2 import NullValue
 
 from zepben.protobuf.cim.iec61970.base.core.IdentifiedObject_pb2 import IdentifiedObject as PBIdentifiedObject
 
 __all__ = [
     "mrid_or_empty", "int_or_none", "uint_or_none", "float_or_none", "long_or_none", "str_or_none", "from_nullable_int", "from_nullable_uint",
-    "from_nullable_float", "from_nullable_long"
+    "from_nullable_float", "from_nullable_long", "nullable_bool_settings"
 ]
 
 #
 # NOTE: These values must be comparable using standard equality operators (i.e ==)
 #
 
 _UNKNOWN_FLOAT = float("-inf")
@@ -57,7 +62,17 @@
 
 def from_nullable_float(value: Optional[float]) -> float:
     return value if value is not None else _UNKNOWN_FLOAT
 
 
 def from_nullable_long(value: Optional[int]) -> int:
     return value if value is not None else _UNKNOWN_LONG
+
+
+def nullable_bool_settings(flag_name: str, value: Optional[bool]) -> Dict:
+    settings = {}
+    if value is None:
+        settings[f"{flag_name}Null"] = NullValue.NULL_VALUE
+    else:
+        settings[f"{flag_name}Set"] = value
+
+    return settings
```

## zepben/evolve/services/customer/customers.py

```diff
@@ -1,15 +1,13 @@
 #  Copyright 2020 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-from dataclassy import dataclass
-
 from zepben.evolve.services.common.base_service import BaseService
 
 __all__ = ["CustomerService"]
 
 
 class CustomerService(BaseService):
     """
```

## zepben/evolve/services/network/network_extensions.py

```diff
@@ -13,15 +13,15 @@
 from zepben.evolve.model.cim.iec61970.base.core.terminal import Terminal
 from zepben.evolve.model.cim.iec61970.base.core.phase_code import PhaseCode
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import Junction
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import EnergySource
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import PowerTransformer, PowerTransformerEnd
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import AcLineSegment
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import EnergyConsumer
-from zepben.evolve.model.cim.iec61970.base.wires.switch import Breaker
+from zepben.evolve.model.cim.iec61970.base.wires.breaker import Breaker
 from zepben.evolve.model.cim.iec61970.base.core.connectivity_node import ConnectivityNode
 from zepben.evolve.util import CopyableUUID
 
 __all__ = ["create_ac_line_segment", "create_two_winding_power_transformer", "create_energy_consumer",
            "create_energy_source", "create_bus", "create_breaker"]
```

## zepben/evolve/services/network/network_service_comparator.py

```diff
@@ -10,15 +10,16 @@
     TransformerTankInfo, TransformerTest, WireInfo, AssetOwner, Pole, Asset, Streetlight, Location, EndDevice, Meter, UsagePoint, OperationalRestriction, \
     AuxiliaryEquipment, FaultIndicator, BaseVoltage, ConductingEquipment, ConnectivityNode, Equipment, EquipmentContainer, Feeder, GeographicalRegion, \
     PowerSystemResource, Site, SubGeographicalRegion, Substation, Terminal, PowerElectronicsUnit, BatteryUnit, PhotoVoltaicUnit, PowerElectronicsWindUnit, \
     Breaker, LoadBreakSwitch, BusbarSection, Conductor, Disconnector, EnergyConsumer, EnergyConsumerPhase, EnergySource, EnergySourcePhase, Fuse, Jumper, \
     Junction, LinearShuntCompensator, PerLengthSequenceImpedance, PowerElectronicsConnection, PowerElectronicsConnectionPhase, PowerTransformer, \
     PowerTransformerEnd, RatioTapChanger, Recloser, RegulatingCondEq, ShuntCompensator, TapChanger, TransformerEnd, TransformerStarImpedance, Circuit, \
     Loop, SinglePhaseKind, ValueDifference, PhaseCode, Control, Measurement, Analog, Accumulator, Discrete, RemoteControl, RemoteSource, EquivalentBranch, \
-    Switch, ShuntCompensatorInfo, LvFeeder, CurrentTransformerInfo, PotentialTransformerInfo, CurrentTransformer, PotentialTransformer
+    Switch, ShuntCompensatorInfo, LvFeeder, CurrentTransformerInfo, PotentialTransformerInfo, CurrentTransformer, PotentialTransformer, SwitchInfo, \
+    CurrentRelayInfo, CurrentRelay, ProtectionEquipment, RecloseSequence, ProtectedSwitch
 from zepben.evolve.services.common.base_service_comparator import BaseServiceComparator
 from zepben.evolve.services.common.translator.service_differences import ObjectDifference
 
 
 @dataclass
 class NetworkServiceComparatorOptions:
     compare_terminals: bool = True
@@ -115,14 +116,21 @@
             ShuntCompensatorInfo.rated_current,
             ShuntCompensatorInfo.rated_reactive_power,
             ShuntCompensatorInfo.rated_voltage,
         )
 
         return self._compare_asset_info(diff)
 
+    def _compare_switch_info(self, source: SwitchInfo, target: SwitchInfo) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        self._compare_floats(diff, SwitchInfo.rated_interrupting_time)
+
+        return self._compare_asset_info(diff)
+
     def _compare_transformer_end_info(self, source: TransformerEndInfo, target: TransformerEndInfo) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_id_references(
             diff,
             TransformerEndInfo.transformer_star_impedance,
             TransformerEndInfo.energised_end_no_load_tests,
@@ -217,14 +225,21 @@
 
         return self._compare_identified_object(diff)
 
     #####################################
     # IEC61968 infIEC61968 InfAssetInfo #
     #####################################
 
+    def _compare_current_relay_info(self, source: CurrentRelayInfo, target: CurrentRelayInfo) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        self._compare_values(diff, CurrentRelayInfo.curve_setting)
+
+        return self._compare_asset_info(diff)
+
     def _compare_current_transformer_info(self, source: CurrentTransformerInfo, target: CurrentTransformerInfo) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_values(
             diff,
             CurrentTransformerInfo.accuracy_class,
             CurrentTransformerInfo.core_count,
@@ -499,14 +514,41 @@
 
     def _compare_measurement(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_values(diff, Measurement.power_system_resource_mrid, Measurement.unit_symbol, Measurement.phases, Measurement.terminal_mrid)
         self._compare_id_references(diff, Measurement.remote_source)
 
         return self._compare_identified_object(diff)
 
+    ############################
+    # IEC61970 Base Protection #
+    ############################
+
+    def _compare_current_relay(self, source: CurrentRelay, target: CurrentRelay) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        self._compare_values(diff, CurrentRelay.inverse_time_flag)
+        self._compare_floats(diff, CurrentRelay.current_limit_1, CurrentRelay.time_delay_1)
+
+        return self._compare_protection_equipment(diff)
+
+    def _compare_protection_equipment(self, diff: ObjectDifference) -> ObjectDifference:
+        self._compare_values(diff, ProtectionEquipment.protection_kind)
+        self._compare_floats(diff, ProtectionEquipment.relay_delay_time)
+        self._compare_id_reference_collections(diff, ProtectionEquipment.protected_switches)
+
+        return self._compare_equipment(diff)
+
+    def _compare_reclose_sequence(self, source: RecloseSequence, target: RecloseSequence) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        self._compare_values(diff, RecloseSequence.reclose_step)
+        self._compare_floats(diff, RecloseSequence.reclose_delay)
+
+        return self._compare_identified_object(diff)
+
     #######################
     # IEC61970 BASE SCADA #
     #######################
 
     def _compare_remote_control(self, source: RemoteControl, target: RemoteControl) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
@@ -555,15 +597,19 @@
         diff = ObjectDifference(source, target)
 
         self._compare_id_references(diff, AcLineSegment.per_length_sequence_impedance)
 
         return self._compare_conductor(diff)
 
     def _compare_breaker(self, source: Breaker, target: Breaker) -> ObjectDifference:
-        return self._compare_protected_switch(ObjectDifference(source, target))
+        diff = ObjectDifference(source, target)
+
+        self._compare_floats(diff, Breaker.in_transit_time)
+
+        return self._compare_protected_switch(diff)
 
     def _compare_busbar_section(self, source: BusbarSection, target: BusbarSection) -> ObjectDifference:
         return self._compare_connector(ObjectDifference(source, target))
 
     def _compare_conductor(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_floats(diff, Conductor.length)
 
@@ -711,15 +757,14 @@
         self._compare_floats(diff, PowerElectronicsConnectionPhase.p, PowerElectronicsConnectionPhase.q)
 
         return self._compare_power_system_resource(diff)
 
     def _compare_power_transformer(self, source: PowerTransformer, target: PowerTransformer) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
-        self._compare_id_references(diff, PowerTransformer.asset_info)
         self._compare_indexed_id_reference_collections(diff, PowerTransformer.ends)
         self._compare_values(diff, PowerTransformer.vector_group, PowerTransformer.construction_kind, PowerTransformer.function)
         self._compare_floats(diff, PowerTransformer.transformer_utilisation)
 
         return self._compare_conducting_equipment(diff)
 
     def _compare_power_transformer_end(self, source: PowerTransformerEnd, target: PowerTransformerEnd) -> ObjectDifference:
@@ -744,14 +789,17 @@
             PowerTransformerEnd.x,
             PowerTransformerEnd.x0
         )
 
         return self._compare_transformer_end(diff)
 
     def _compare_protected_switch(self, diff: ObjectDifference) -> ObjectDifference:
+        self._compare_values(diff, ProtectedSwitch.breaking_capacity)
+        self._compare_id_reference_collections(diff, ProtectedSwitch.reclose_sequences, ProtectedSwitch.operated_by_protection_equipment)
+
         return self._compare_switch(diff)
 
     def _compare_ratio_tap_changer(self, source: RatioTapChanger, target: RatioTapChanger) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_id_references(diff, RatioTapChanger.transformer_end)
         self._compare_floats(diff, RatioTapChanger.step_voltage_increment)
@@ -769,14 +817,15 @@
     def _compare_shunt_compensator(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_values(diff, ShuntCompensator.grounded, ShuntCompensator.nom_u, ShuntCompensator.phase_connection)
         self._compare_floats(diff, ShuntCompensator.sections)
 
         return self._compare_regulating_cond_eq(diff)
 
     def _compare_switch(self, diff: ObjectDifference) -> ObjectDifference:
+        self._compare_floats(diff, Switch.rated_current)
         self._add_if_different(diff, "isNormallyOpen", self._compare_open_status(diff, Switch.is_normally_open))
         self._add_if_different(diff, "isOpen", self._compare_open_status(diff, Switch.is_open))
 
         return self._compare_conducting_equipment(diff)
 
     def _compare_tap_changer(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_values(
```

## zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py

```diff
@@ -103,26 +103,26 @@
     async def _reached_lv(t: Terminal) -> bool:
         ce = t.conducting_equipment
         nominal_voltage = ce and ce.base_voltage and ce.base_voltage.nominal_voltage
         return nominal_voltage is not None and nominal_voltage < 1000
 
     async def _process_normal(self, terminal: Terminal, is_stopping: bool):
         # noinspection PyTypeChecker
-        self._process(terminal, ConductingEquipment.add_container, Feeder.add_equipment, is_stopping)
+        await self._process(terminal, ConductingEquipment.add_container, Feeder.add_equipment, is_stopping)
 
     async def _process_current(self, terminal: Terminal, is_stopping: bool):
         # noinspection PyTypeChecker
-        self._process(terminal, ConductingEquipment.add_current_container, Feeder.add_current_equipment, is_stopping)
+        await self._process(terminal, ConductingEquipment.add_current_container, Feeder.add_current_equipment, is_stopping)
 
-    def _process(
+    async def _process(
         self,
-        terminal: Optional[Terminal],
+        terminal: Terminal,
         assign_feeder_to_equip: Callable[[ConductingEquipment, EquipmentContainer], Any],
         assign_equip_to_feeder: Callable[[EquipmentContainer, ConductingEquipment], Any],
         is_stopping: bool
     ):
-        if is_stopping and (self._reached_lv(terminal) or self._reached_substation_transformer(terminal)):
+        if is_stopping and (await self._reached_lv(terminal) or await self._reached_substation_transformer(terminal)):
             return
 
         if terminal.conducting_equipment:
             assign_feeder_to_equip(terminal.conducting_equipment, self._active_feeder)
             assign_equip_to_feeder(self._active_feeder, terminal.conducting_equipment)
```

## zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py

```diff
@@ -1,14 +1,15 @@
 #  Copyright 2022 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Set, Callable, Optional, Awaitable, Any
 
+from zepben.evolve import BasicTraversal
 from zepben.evolve.model.cim.iec61970.base.core.conducting_equipment import ConductingEquipment
 from zepben.evolve.model.cim.iec61970.base.core.equipment_container import EquipmentContainer
 from zepben.evolve.model.cim.iec61970.base.core.terminal import Terminal
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import LvFeeder
 from zepben.evolve.services.network.network_service import NetworkService
 from zepben.evolve.services.network.tracing.feeder.associated_terminal_trace import new_normal_trace, new_current_trace, get_associated_terminals
 from zepben.evolve.services.network.tracing.traversals.traversal import Traversal
@@ -19,21 +20,21 @@
 class AssignToLvFeeders:
     """
     Convenience class that provides methods for assigning LV feeders on a `NetworkService`.
     Requires that a Feeder have a normalHeadTerminal with associated ConductingEquipment.
     This class is backed by a `BasicTraversal`.
     """
 
-    def __init__(self, _normal_traversal: Optional[Traversal[Terminal]] = None, _current_traversal: Optional[Traversal[Terminal]] = None):
-        self._normal_traversal: Traversal[Terminal] = _normal_traversal if _normal_traversal is not None else new_normal_trace()
+    def __init__(self, _normal_traversal: Optional[BasicTraversal[Terminal]] = None, _current_traversal: Optional[BasicTraversal[Terminal]] = None):
+        self._normal_traversal: BasicTraversal[Terminal] = _normal_traversal if _normal_traversal is not None else new_normal_trace()
         """
         The traversal used to trace the network in its normal state of the network.
         """
 
-        self._current_traversal: Traversal[Terminal] = _current_traversal if _current_traversal is not None else new_current_trace()
+        self._current_traversal: BasicTraversal[Terminal] = _current_traversal if _current_traversal is not None else new_current_trace()
         """
         The traversal used to trace the network in its current state of the network.
         """
 
         self._active_lv_feeder: Optional[LvFeeder] = None  # This will never be optional by the time it is used.
         """
         The LV feeder that is currently being processed.
@@ -73,15 +74,15 @@
         if not lv_feeder.normal_head_terminal:
             return
 
         await self._run_from_head_terminal(self._normal_traversal, lv_feeder.normal_head_terminal)
         await self._run_from_head_terminal(self._current_traversal, lv_feeder.normal_head_terminal)
 
     @staticmethod
-    async def _run_from_head_terminal(traversal: Traversal, head_terminal: Terminal):
+    async def _run_from_head_terminal(traversal: BasicTraversal[Terminal], head_terminal: Terminal):
         traversal.reset()
 
         traversal.tracker.visit(head_terminal)
         await traversal.apply_step_actions(head_terminal, False)
         traversal.process_queue.extend(get_associated_terminals(head_terminal))
 
         await traversal.run()
@@ -102,26 +103,26 @@
     async def _reached_hv(t: Terminal) -> bool:
         ce = t.conducting_equipment
         nominal_voltage = ce and ce.base_voltage and ce.base_voltage.nominal_voltage
         return nominal_voltage is not None and nominal_voltage >= 1000
 
     async def _process_normal(self, terminal: Terminal, is_stopping: bool):
         # noinspection PyTypeChecker
-        self._process(terminal, ConductingEquipment.add_container, LvFeeder.add_equipment, is_stopping)
+        await self._process(terminal, ConductingEquipment.add_container, LvFeeder.add_equipment, is_stopping)
 
     async def _process_current(self, terminal: Terminal, is_stopping: bool):
         # noinspection PyTypeChecker
-        self._process(terminal, ConductingEquipment.add_current_container, LvFeeder.add_current_equipment, is_stopping)
+        await self._process(terminal, ConductingEquipment.add_current_container, LvFeeder.add_current_equipment, is_stopping)
 
-    def _process(
+    async def _process(
         self,
-        terminal: Optional[Terminal],
+        terminal: Terminal,
         assign_lv_feeder_to_equip: Callable[[ConductingEquipment, EquipmentContainer], Any],
         assign_equip_to_lv_feeder: Callable[[EquipmentContainer, ConductingEquipment], Any],
         is_stopping: bool
     ):
-        if is_stopping and self._reached_hv(terminal):
+        if is_stopping and await self._reached_hv(terminal):
             return
 
         if terminal.conducting_equipment:
             assign_lv_feeder_to_equip(terminal.conducting_equipment, self._active_lv_feeder)
             assign_equip_to_lv_feeder(self._active_lv_feeder, terminal.conducting_equipment)
```

## zepben/evolve/services/network/tracing/traversals/basic_traversal.py

```diff
@@ -4,17 +4,16 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
 from typing import Callable, TypeVar
 
-from zepben.evolve import Traversal, BasicTracker
+from zepben.evolve import Traversal
 from zepben.evolve.services.network.tracing.traversals.queue import Queue, depth_first
-from zepben.evolve.services.network.tracing.traversals.tracker import Tracker
 
 __all__ = ["BasicTraversal"]
 T = TypeVar('T')
 
 
 class BasicTraversal(Traversal[T]):
     """
```

## zepben/evolve/services/network/translator/__init__.py

```diff
@@ -7,27 +7,29 @@
 from zepben.protobuf.cim.iec61968.assetinfo.CableInfo_pb2 import CableInfo
 from zepben.protobuf.cim.iec61968.assetinfo.NoLoadTest_pb2 import NoLoadTest
 from zepben.protobuf.cim.iec61968.assetinfo.OpenCircuitTest_pb2 import OpenCircuitTest
 from zepben.protobuf.cim.iec61968.assetinfo.OverheadWireInfo_pb2 import OverheadWireInfo
 from zepben.protobuf.cim.iec61968.assetinfo.PowerTransformerInfo_pb2 import PowerTransformerInfo
 from zepben.protobuf.cim.iec61968.assetinfo.ShortCircuitTest_pb2 import ShortCircuitTest
 from zepben.protobuf.cim.iec61968.assetinfo.ShuntCompensatorInfo_pb2 import ShuntCompensatorInfo
+from zepben.protobuf.cim.iec61968.assetinfo.SwitchInfo_pb2 import SwitchInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerEndInfo_pb2 import TransformerEndInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerTankInfo_pb2 import TransformerTankInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerTest_pb2 import TransformerTest
 from zepben.protobuf.cim.iec61968.assetinfo.WireInfo_pb2 import WireInfo
 from zepben.protobuf.cim.iec61968.assets.AssetContainer_pb2 import AssetContainer
 from zepben.protobuf.cim.iec61968.assets.AssetInfo_pb2 import AssetInfo
 from zepben.protobuf.cim.iec61968.assets.AssetOrganisationRole_pb2 import AssetOrganisationRole
 from zepben.protobuf.cim.iec61968.assets.AssetOwner_pb2 import AssetOwner
 from zepben.protobuf.cim.iec61968.assets.Asset_pb2 import Asset
 from zepben.protobuf.cim.iec61968.assets.Pole_pb2 import Pole
 from zepben.protobuf.cim.iec61968.assets.Streetlight_pb2 import Streetlight
 from zepben.protobuf.cim.iec61968.assets.Structure_pb2 import Structure
 from zepben.protobuf.cim.iec61968.common.Location_pb2 import Location
+from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentRelayInfo_pb2 import CurrentRelayInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentTransformerInfo_pb2 import CurrentTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.PotentialTransformerInfo_pb2 import PotentialTransformerInfo
 from zepben.protobuf.cim.iec61968.metering.EndDevice_pb2 import EndDevice
 from zepben.protobuf.cim.iec61968.metering.Meter_pb2 import Meter
 from zepben.protobuf.cim.iec61968.metering.UsagePoint_pb2 import UsagePoint
 from zepben.protobuf.cim.iec61968.operations.OperationalRestriction_pb2 import OperationalRestriction
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.AuxiliaryEquipment_pb2 import AuxiliaryEquipment
@@ -54,14 +56,17 @@
 from zepben.protobuf.cim.iec61970.base.equivalents.EquivalentEquipment_pb2 import EquivalentEquipment
 from zepben.protobuf.cim.iec61970.base.meas.Accumulator_pb2 import Accumulator
 from zepben.protobuf.cim.iec61970.base.meas.Analog_pb2 import Analog
 from zepben.protobuf.cim.iec61970.base.meas.Control_pb2 import Control
 from zepben.protobuf.cim.iec61970.base.meas.Discrete_pb2 import Discrete
 from zepben.protobuf.cim.iec61970.base.meas.IoPoint_pb2 import IoPoint
 from zepben.protobuf.cim.iec61970.base.meas.Measurement_pb2 import Measurement
+from zepben.protobuf.cim.iec61970.base.protection.CurrentRelay_pb2 import CurrentRelay
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionEquipment_pb2 import ProtectionEquipment
+from zepben.protobuf.cim.iec61970.base.protection.RecloseSequence_pb2 import RecloseSequence
 from zepben.protobuf.cim.iec61970.base.scada.RemoteControl_pb2 import RemoteControl
 from zepben.protobuf.cim.iec61970.base.scada.RemotePoint_pb2 import RemotePoint
 from zepben.protobuf.cim.iec61970.base.scada.RemoteSource_pb2 import RemoteSource
 from zepben.protobuf.cim.iec61970.base.wires.AcLineSegment_pb2 import AcLineSegment
 from zepben.protobuf.cim.iec61970.base.wires.Breaker_pb2 import Breaker
 from zepben.protobuf.cim.iec61970.base.wires.BusbarSection_pb2 import BusbarSection
 from zepben.protobuf.cim.iec61970.base.wires.Conductor_pb2 import Conductor
@@ -108,28 +113,30 @@
 CableInfo.mrid = lambda self: self.wi.mrid()
 NoLoadTest.mrid = lambda self: self.tt.mrid()
 OpenCircuitTest.mrid = lambda self: self.tt.mrid()
 OverheadWireInfo.mrid = lambda self: self.wi.mrid()
 PowerTransformerInfo.mrid = lambda self: self.ai.mrid()
 ShortCircuitTest.mrid = lambda self: self.tt.mrid()
 ShuntCompensatorInfo.mrid = lambda self: self.ai.mrid()
+SwitchInfo.mrid = lambda self: self.ai.mrid()
 TransformerEndInfo.mrid = lambda self: self.ai.mrid()
 TransformerTankInfo.mrid = lambda self: self.ai.mrid()
 TransformerTest.mrid = lambda self: self.io.mrid()
 TransformerStarImpedance.mrid = lambda self: self.io.mrid()
 WireInfo.mrid = lambda self: self.ai.mrid()
 Asset.mrid = lambda self: self.io.mrid()
 AssetContainer.mrid = lambda self: self.at.mrid()
 AssetInfo.mrid = lambda self: self.io.mrid()
 AssetOrganisationRole.mrid = lambda self: getattr(self, "or").mrid()
 AssetOwner.mrid = lambda self: self.aor.mrid()
 Pole.mrid = lambda self: self.st.mrid()
 Streetlight.mrid = lambda self: self.at.mrid()
 Structure.mrid = lambda self: self.ac.mrid()
 Location.mrid = lambda self: self.io.mrid()
+CurrentRelayInfo.mrid = lambda self: self.ai.mrid()
 CurrentTransformerInfo.mrid = lambda self: self.ai.mrid()
 PotentialTransformerInfo.mrid = lambda self: self.ai.mrid()
 EndDevice.mrid = lambda self: self.ac.mrid()
 Meter.mrid = lambda self: self.ed.mrid()
 UsagePoint.mrid = lambda self: self.io.mrid()
 OperationalRestriction.mrid = lambda self: self.doc.mrid()
 AuxiliaryEquipment.mrid = lambda self: self.eq.mrid()
@@ -156,14 +163,17 @@
 EquivalentEquipment.mrid = lambda self: self.ce.mrid()
 Accumulator.mrid = lambda self: self.measurement.mrid()
 Analog.mrid = lambda self: self.measurement.mrid()
 Discrete.mrid = lambda self: self.measurement.mrid()
 Control.mrid = lambda self: self.ip.mrid()
 IoPoint.mrid = lambda self: self.io.mrid()
 Measurement.mrid = lambda self: self.io.mrid()
+CurrentRelay.mrid = lambda self: self.pe.mrid()
+ProtectionEquipment.mrid = lambda self: self.eq.mrid()
+RecloseSequence.mrid = lambda self: self.io.mrid()
 RemoteControl.mrid = lambda self: self.rp.mrid()
 RemotePoint.mrid = lambda self: self.io.mrid()
 RemoteSource.mrid = lambda self: self.rp.mrid()
 BatteryUnit.mrid = lambda self: self.peu.mrid()
 PhotoVoltaicUnit.mrid = lambda self: self.peu.mrid()
 PowerElectronicsUnit.mrid = lambda self: self.eq.mrid()
 PowerElectronicsWindUnit.mrid = lambda self: self.peu.mrid()
@@ -301,15 +311,17 @@
 # per_length_sequence_impedance_mrid
 AcLineSegment.per_length_sequence_impedance_mrid = lambda self: getattr(self, "perLengthSequenceImpedanceMRID", None)
 
 # asset_info_mrid
 ConductingEquipment.asset_info_mrid = lambda self: self.eq.asset_info_mrid()
 Conductor.asset_info_mrid = lambda self: self.ce.asset_info_mrid()
 CurrentTransformer.asset_info_mrid = lambda self: self.sn.ae.eq.asset_info_mrid()
+CurrentRelay.asset_info_mrid = lambda self: self.pe.eq.asset_info_mrid()
 Equipment.asset_info_mrid = lambda self: self.psr.assetInfoMRID
 PotentialTransformer.asset_info_mrid = lambda self: self.sn.ae.eq.asset_info_mrid()
 PowerTransformer.asset_info_mrid = lambda self: self.ce.asset_info_mrid()
 ShuntCompensator.asset_info_mrid = lambda self: self.rce.ec.ce.asset_info_mrid()
+Switch.asset_info_mrid = lambda self: self.ce.asset_info_mrid()
 
 # ratio_tap_changer_mrid
 TransformerEnd.ratio_tap_changer_mrid = lambda self: getattr(self, "ratioTapChangerMRID", None)
 PowerTransformerEnd.ratio_tap_changer_mrid = lambda self: self.te.ratio_tap_changer_mrid()
```

## zepben/evolve/services/network/translator/network_cim2proto.py

```diff
@@ -6,14 +6,15 @@
 from zepben.protobuf.cim.iec61968.assetinfo.CableInfo_pb2 import CableInfo as PBCableInfo
 from zepben.protobuf.cim.iec61968.assetinfo.NoLoadTest_pb2 import NoLoadTest as PBNoLoadTest
 from zepben.protobuf.cim.iec61968.assetinfo.OpenCircuitTest_pb2 import OpenCircuitTest as PBOpenCircuitTest
 from zepben.protobuf.cim.iec61968.assetinfo.OverheadWireInfo_pb2 import OverheadWireInfo as PBOverheadWireInfo
 from zepben.protobuf.cim.iec61968.assetinfo.PowerTransformerInfo_pb2 import PowerTransformerInfo as PBPowerTransformerInfo
 from zepben.protobuf.cim.iec61968.assetinfo.ShortCircuitTest_pb2 import ShortCircuitTest as PBShortCircuitTest
 from zepben.protobuf.cim.iec61968.assetinfo.ShuntCompensatorInfo_pb2 import ShuntCompensatorInfo as PBShuntCompensatorInfo
+from zepben.protobuf.cim.iec61968.assetinfo.SwitchInfo_pb2 import SwitchInfo as PBSwitchInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerEndInfo_pb2 import TransformerEndInfo as PBTransformerEndInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerTankInfo_pb2 import TransformerTankInfo as PBTransformerTankInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerTest_pb2 import TransformerTest as PBTransformerTest
 from zepben.protobuf.cim.iec61968.assetinfo.WireInfo_pb2 import WireInfo as PBWireInfo
 from zepben.protobuf.cim.iec61968.assetinfo.WireMaterialKind_pb2 import WireMaterialKind as PBWireMaterialKind
 from zepben.protobuf.cim.iec61968.assets.AssetContainer_pb2 import AssetContainer as PBAssetContainer
 from zepben.protobuf.cim.iec61968.assets.AssetInfo_pb2 import AssetInfo as PBAssetInfo
@@ -25,28 +26,29 @@
 from zepben.protobuf.cim.iec61968.assets.Streetlight_pb2 import Streetlight as PBStreetlight
 from zepben.protobuf.cim.iec61968.assets.Structure_pb2 import Structure as PBStructure
 from zepben.protobuf.cim.iec61968.common.Location_pb2 import Location as PBLocation
 from zepben.protobuf.cim.iec61968.common.PositionPoint_pb2 import PositionPoint as PBPositionPoint
 from zepben.protobuf.cim.iec61968.common.StreetAddress_pb2 import StreetAddress as PBStreetAddress
 from zepben.protobuf.cim.iec61968.common.StreetDetail_pb2 import StreetDetail as PBStreetDetail
 from zepben.protobuf.cim.iec61968.common.TownDetail_pb2 import TownDetail as PBTownDetail
+from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentRelayInfo_pb2 import CurrentRelayInfo as PBCurrentRelayInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentTransformerInfo_pb2 import CurrentTransformerInfo as PBCurrentTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.PotentialTransformerInfo_pb2 import PotentialTransformerInfo as PBPotentialTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.TransformerConstructionKind_pb2 import TransformerConstructionKind as PBTransformerConstructionKind
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.TransformerFunctionKind_pb2 import TransformerFunctionKind as PBTransformerFunctionKind
 from zepben.protobuf.cim.iec61968.infiec61968.infcommon.Ratio_pb2 import Ratio as PBRatio
 from zepben.protobuf.cim.iec61968.metering.EndDevice_pb2 import EndDevice as PBEndDevice
 from zepben.protobuf.cim.iec61968.metering.Meter_pb2 import Meter as PBMeter
 from zepben.protobuf.cim.iec61968.metering.UsagePoint_pb2 import UsagePoint as PBUsagePoint
 from zepben.protobuf.cim.iec61968.operations.OperationalRestriction_pb2 import OperationalRestriction as PBOperationalRestriction
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.AuxiliaryEquipment_pb2 import AuxiliaryEquipment as PBAuxiliaryEquipment
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.CurrentTransformer_pb2 import CurrentTransformer as PBCurrentTransformer
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.FaultIndicator_pb2 import FaultIndicator as PBFaultIndicator
-from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.PotentialTransformer_pb2 import PotentialTransformer as PBPotentialTransformer
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.PotentialTransformerKind_pb2 import PotentialTransformerKind as PBPotentialTransformerKind
+from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.PotentialTransformer_pb2 import PotentialTransformer as PBPotentialTransformer
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.Sensor_pb2 import Sensor as PBSensor
 from zepben.protobuf.cim.iec61970.base.core.AcDcTerminal_pb2 import AcDcTerminal as PBAcDcTerminal
 from zepben.protobuf.cim.iec61970.base.core.BaseVoltage_pb2 import BaseVoltage as PBBaseVoltage
 from zepben.protobuf.cim.iec61970.base.core.ConductingEquipment_pb2 import ConductingEquipment as PBConductingEquipment
 from zepben.protobuf.cim.iec61970.base.core.ConnectivityNodeContainer_pb2 import ConnectivityNodeContainer as PBConnectivityNodeContainer
 from zepben.protobuf.cim.iec61970.base.core.ConnectivityNode_pb2 import ConnectivityNode as PBConnectivityNode
 from zepben.protobuf.cim.iec61970.base.core.EquipmentContainer_pb2 import EquipmentContainer as PBEquipmentContainer
@@ -64,14 +66,17 @@
 from zepben.protobuf.cim.iec61970.base.equivalents.EquivalentEquipment_pb2 import EquivalentEquipment as PBEquivalentEquipment
 from zepben.protobuf.cim.iec61970.base.meas.Accumulator_pb2 import Accumulator as PBAccumulator
 from zepben.protobuf.cim.iec61970.base.meas.Analog_pb2 import Analog as PBAnalog
 from zepben.protobuf.cim.iec61970.base.meas.Control_pb2 import Control as PBControl
 from zepben.protobuf.cim.iec61970.base.meas.Discrete_pb2 import Discrete as PBDiscrete
 from zepben.protobuf.cim.iec61970.base.meas.IoPoint_pb2 import IoPoint as PBIoPoint
 from zepben.protobuf.cim.iec61970.base.meas.Measurement_pb2 import Measurement as PBMeasurement
+from zepben.protobuf.cim.iec61970.base.protection.CurrentRelay_pb2 import CurrentRelay as PBCurrentRelay
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionEquipment_pb2 import ProtectionEquipment as PBProtectionEquipment
+from zepben.protobuf.cim.iec61970.base.protection.RecloseSequence_pb2 import RecloseSequence as PBRecloseSequence
 from zepben.protobuf.cim.iec61970.base.scada.RemoteControl_pb2 import RemoteControl as PBRemoteControl
 from zepben.protobuf.cim.iec61970.base.scada.RemotePoint_pb2 import RemotePoint as PBRemotePoint
 from zepben.protobuf.cim.iec61970.base.scada.RemoteSource_pb2 import RemoteSource as PBRemoteSource
 from zepben.protobuf.cim.iec61970.base.wires.AcLineSegment_pb2 import AcLineSegment as PBAcLineSegment
 from zepben.protobuf.cim.iec61970.base.wires.Breaker_pb2 import Breaker as PBBreaker
 from zepben.protobuf.cim.iec61970.base.wires.BusbarSection_pb2 import BusbarSection as PBBusbarSection
 from zepben.protobuf.cim.iec61970.base.wires.Conductor_pb2 import Conductor as PBConductor
@@ -112,32 +117,35 @@
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.BatteryUnit_pb2 import BatteryUnit as PBBatteryUnit
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.PhotoVoltaicUnit_pb2 import PhotoVoltaicUnit as PBPhotoVoltaicUnit
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.PowerElectronicsUnit_pb2 import PowerElectronicsUnit as PBPowerElectronicsUnit
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.PowerElectronicsWindUnit_pb2 import PowerElectronicsWindUnit as PBPowerElectronicsWindUnit
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.Circuit_pb2 import Circuit as PBCircuit
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.Loop_pb2 import Loop as PBLoop
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.LvFeeder_pb2 import LvFeeder as PBLvFeeder
+from zepben.protobuf.cim.iec61970.infiec61970.protection.ProtectionKind_pb2 import ProtectionKind as PBProtectionKind
 from zepben.protobuf.network.model.FeederDirection_pb2 import FeederDirection as PBFeederDirection
 
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import *
+from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_tank_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.wire_info import *
 from zepben.evolve.model.cim.iec61968.assets.asset import *
 from zepben.evolve.model.cim.iec61968.assets.asset_info import *
 from zepben.evolve.model.cim.iec61968.assets.asset_organisation_role import *
 from zepben.evolve.model.cim.iec61968.assets.pole import *
 from zepben.evolve.model.cim.iec61968.assets.streetlight import *
 from zepben.evolve.model.cim.iec61968.assets.structure import *
 from zepben.evolve.model.cim.iec61968.common.location import *
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infcommon.ratio import *
 from zepben.evolve.model.cim.iec61968.metering.metering import *
 from zepben.evolve.model.cim.iec61968.operations.operational_restriction import *
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import *
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.current_transformer import *
@@ -154,56 +162,68 @@
 from zepben.evolve.model.cim.iec61970.base.core.substation import *
 from zepben.evolve.model.cim.iec61970.base.core.terminal import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_branch import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_equipment import *
 from zepben.evolve.model.cim.iec61970.base.meas.control import *
 from zepben.evolve.model.cim.iec61970.base.meas.iopoint import *
 from zepben.evolve.model.cim.iec61970.base.meas.measurement import *
+from zepben.evolve.model.cim.iec61970.base.protection.current_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.reclose_sequence import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_point import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import *
+from zepben.evolve.model.cim.iec61970.base.wires.breaker import *
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import *
+from zepben.evolve.model.cim.iec61970.base.wires.disconnector import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import *
+from zepben.evolve.model.cim.iec61970.base.wires.fuse import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import *
+from zepben.evolve.model.cim.iec61970.base.wires.jumper import *
 from zepben.evolve.model.cim.iec61970.base.wires.line import *
+from zepben.evolve.model.cim.iec61970.base.wires.load_break_switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import *
+from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import *
+from zepben.evolve.model.cim.iec61970.base.wires.recloser import *
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.transformer_star_impedance import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.circuit import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.loop import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import *
-
 from zepben.evolve.services.common.translator.base_cim2proto import identified_object_to_pb, organisation_role_to_pb, document_to_pb
-from zepben.evolve.services.common.translator.util import mrid_or_empty, from_nullable_int, from_nullable_float, from_nullable_long, from_nullable_uint
+from zepben.evolve.services.common.translator.util import mrid_or_empty, from_nullable_int, from_nullable_float, from_nullable_long, from_nullable_uint, \
+    nullable_bool_settings
 
 __all__ = [
     "CimTranslationException", "cable_info_to_pb", "no_load_test_to_pb", "open_circuit_test_to_pb", "overhead_wire_info_to_pb", "power_transformer_info_to_pb",
-    "short_circuit_test_to_pb", "shunt_compensator_info_to_pb", "transformer_end_info_to_pb", "transformer_tank_info_to_pb", "transformer_test_to_pb",
-    "wire_info_to_pb", "asset_to_pb", "asset_container_to_pb", "asset_info_to_pb", "asset_organisation_role_to_pb", "asset_owner_to_pb", "pole_to_pb",
-    "streetlight_to_pb", "structure_to_pb", "location_to_pb", "position_point_to_pb", "street_address_to_pb", "town_detail_to_pb", "end_device_to_pb",
-    "meter_to_pb", "usage_point_to_pb", "operational_restriction_to_pb", "auxiliary_equipment_to_pb", "fault_indicator_to_pb", "ac_dc_terminal_to_pb",
-    "base_voltage_to_pb", "conducting_equipment_to_pb", "connectivity_node_to_pb", "connectivity_node_container_to_pb", "equipment_to_pb",
-    "equipment_container_to_pb", "feeder_to_pb", "geographical_region_to_pb", "power_system_resource_to_pb", "site_to_pb", "sub_geographical_region_to_pb",
-    "substation_to_pb", "terminal_to_pb", "equivalent_branch_to_pb", "equivalent_equipment_to_pb", "control_to_pb", "io_point_to_pb", "accumulator_to_pb",
-    "analog_to_pb", "discrete_to_pb", "measurement_to_pb", "remote_control_to_pb", "remote_point_to_pb", "remote_source_to_pb", "battery_unit_to_pb",
-    "photo_voltaic_unit_to_pb", "power_electronics_unit_to_pb", "power_electronics_wind_unit_to_pb", "ac_line_segment_to_pb", "breaker_to_pb",
-    "conductor_to_pb", "connector_to_pb", "disconnector_to_pb", "energy_connection_to_pb", "energy_consumer_to_pb", "energy_consumer_phase_to_pb",
-    "energy_source_to_pb", "energy_source_phase_to_pb", "fuse_to_pb", "jumper_to_pb", "junction_to_pb", "busbar_section_to_pb", "line_to_pb",
-    "linear_shunt_compensator_to_pb", "load_break_switch_to_pb", "per_length_line_parameter_to_pb", "per_length_impedance_to_pb",
-    "per_length_sequence_impedance_to_pb", "power_electronics_connection_to_pb", "power_electronics_connection_phase_to_pb", "power_transformer_to_pb",
-    "power_transformer_end_to_pb", "protected_switch_to_pb", "ratio_tap_changer_to_pb", "recloser_to_pb", "regulating_cond_eq_to_pb", "shunt_compensator_to_pb",
-    "switch_to_pb", "tap_changer_to_pb", "transformer_end_to_pb", "circuit_to_pb", "loop_to_pb", "lv_feeder_to_pb", "transformer_star_impedance_to_pb",
-    "current_transformer_info_to_pb", "potential_transformer_info_to_pb", "current_transformer_to_pb", "potential_transformer_to_pb"
+    "short_circuit_test_to_pb", "shunt_compensator_info_to_pb", "switch_info_to_pb", "transformer_end_info_to_pb", "transformer_tank_info_to_pb",
+    "transformer_test_to_pb", "wire_info_to_pb", "asset_to_pb", "asset_container_to_pb", "asset_info_to_pb", "asset_organisation_role_to_pb",
+    "asset_owner_to_pb", "pole_to_pb", "streetlight_to_pb", "structure_to_pb", "location_to_pb", "position_point_to_pb", "street_address_to_pb",
+    "street_detail_to_pb", "town_detail_to_pb", "current_relay_info_to_pb", "current_transformer_info_to_pb", "potential_transformer_info_to_pb",
+    "ratio_to_pb", "end_device_to_pb", "meter_to_pb", "usage_point_to_pb", "operational_restriction_to_pb", "auxiliary_equipment_to_pb",
+    "current_transformer_to_pb", "fault_indicator_to_pb", "potential_transformer_to_pb", "sensor_to_pb", "ac_dc_terminal_to_pb", "base_voltage_to_pb",
+    "conducting_equipment_to_pb", "connectivity_node_to_pb", "connectivity_node_container_to_pb", "equipment_to_pb", "equipment_container_to_pb",
+    "feeder_to_pb", "geographical_region_to_pb", "power_system_resource_to_pb", "site_to_pb", "sub_geographical_region_to_pb", "substation_to_pb",
+    "terminal_to_pb", "equivalent_branch_to_pb", "equivalent_equipment_to_pb", "accumulator_to_pb", "analog_to_pb", "control_to_pb", "discrete_to_pb",
+    "io_point_to_pb", "measurement_to_pb", "current_relay_to_pb", "protection_equipment_to_pb", "reclose_sequence_to_pb", "remote_control_to_pb",
+    "remote_point_to_pb", "remote_source_to_pb", "battery_unit_to_pb", "photo_voltaic_unit_to_pb", "power_electronics_unit_to_pb",
+    "power_electronics_wind_unit_to_pb", "ac_line_segment_to_pb", "breaker_to_pb", "conductor_to_pb", "connector_to_pb", "disconnector_to_pb",
+    "energy_connection_to_pb", "energy_consumer_to_pb", "energy_consumer_phase_to_pb", "energy_source_to_pb", "energy_source_phase_to_pb", "fuse_to_pb",
+    "jumper_to_pb", "junction_to_pb", "busbar_section_to_pb", "line_to_pb", "linear_shunt_compensator_to_pb", "load_break_switch_to_pb",
+    "per_length_line_parameter_to_pb", "per_length_impedance_to_pb", "per_length_sequence_impedance_to_pb", "power_electronics_connection_to_pb",
+    "power_electronics_connection_phase_to_pb", "power_transformer_to_pb", "power_transformer_end_to_pb", "protected_switch_to_pb", "ratio_tap_changer_to_pb",
+    "recloser_to_pb", "regulating_cond_eq_to_pb", "shunt_compensator_to_pb", "switch_to_pb", "tap_changer_to_pb", "transformer_end_to_pb",
+    "transformer_star_impedance_to_pb", "circuit_to_pb", "loop_to_pb", "lv_feeder_to_pb"
 ]
 
 
 def _get_or_none(getter, obj) -> object:
     return getter(obj) if obj else None
 
 
@@ -274,14 +294,21 @@
         maxPowerLoss=from_nullable_int(cim.max_power_loss),
         ratedCurrent=from_nullable_int(cim.rated_current),
         ratedReactivePower=from_nullable_int(cim.rated_reactive_power),
         ratedVoltage=from_nullable_int(cim.rated_voltage),
     )
 
 
+def switch_info_to_pb(cim: SwitchInfo) -> PBSwitchInfo:
+    return PBSwitchInfo(
+        ai=asset_info_to_pb(cim),
+        ratedInterruptingTime=from_nullable_float(cim.rated_interrupting_time)
+    )
+
+
 def transformer_end_info_to_pb(cim: TransformerEndInfo) -> PBTransformerEndInfo:
     return PBTransformerEndInfo(
         ai=asset_info_to_pb(cim),
         connectionKind=PBWindingConnection.Value(cim.connection_kind.short_name),
         emergencyS=from_nullable_int(cim.emergency_s),
         endNumber=from_nullable_int(cim.end_number),
         insulationU=from_nullable_int(cim.insulation_u),
@@ -326,14 +353,15 @@
 CableInfo.to_pb = cable_info_to_pb
 NoLoadTest.to_pb = no_load_test_to_pb
 OpenCircuitTest.to_pb = open_circuit_test_to_pb
 OverheadWireInfo.to_pb = overhead_wire_info_to_pb
 PowerTransformerInfo.to_pb = power_transformer_info_to_pb
 ShortCircuitTest.to_pb = short_circuit_test_to_pb
 ShuntCompensatorInfo.to_pb = shunt_compensator_info_to_pb
+SwitchInfo.to_pb = switch_info_to_pb
 TransformerEndInfo.to_pb = transformer_end_info_to_pb
 TransformerTankInfo.to_pb = transformer_tank_info_to_pb
 TransformerTest.to_pb = transformer_test_to_pb
 WireInfo.to_pb = wire_info_to_pb
 
 
 ###################
@@ -445,14 +473,21 @@
 TownDetail.to_pb = town_detail_to_pb
 
 
 #####################################
 # IEC61968 infIEC61968 InfAssetInfo #
 #####################################
 
+def current_relay_info_to_pb(cim: CurrentRelayInfo) -> PBCurrentRelayInfo:
+    return PBCurrentRelayInfo(
+        ai=asset_info_to_pb(cim),
+        curveSetting=cim.curve_setting
+    )
+
+
 def current_transformer_info_to_pb(cim: CurrentTransformerInfo) -> PBCurrentTransformerInfo:
     return PBCurrentTransformerInfo(
         ai=asset_info_to_pb(cim),
         accuracyClass=cim.accuracy_class,
         accuracyLimit=from_nullable_float(cim.accuracy_limit),
         coreCount=from_nullable_int(cim.core_count),
         ctClass=cim.ct_class,
@@ -475,14 +510,15 @@
         primaryRatio=from_nullable_float(cim.primary_ratio),
         ptClass=cim.pt_class,
         ratedVoltage=from_nullable_int(cim.rated_voltage),
         secondaryRatio=from_nullable_float(cim.secondary_ratio)
     )
 
 
+CurrentRelayInfo.to_pb = current_relay_info_to_pb
 CurrentTransformerInfo.to_pb = current_transformer_info_to_pb
 PotentialTransformerInfo.to_pb = potential_transformer_info_to_pb
 
 
 ##################################
 # IEC61968 infIEC61968 InfCommon #
 ##################################
@@ -782,14 +818,49 @@
 Analog.to_pb = analog_to_pb
 Control.to_pb = control_to_pb
 Discrete.to_pb = discrete_to_pb
 IoPoint.to_pb = io_point_to_pb
 Measurement.to_pb = measurement_to_pb
 
 
+############################
+# IEC61970 Base Protection #
+############################
+
+def current_relay_to_pb(cim: CurrentRelay) -> PBCurrentRelay:
+    return PBCurrentRelay(
+        pe=protection_equipment_to_pb(cim, True),
+        currentLimit1=from_nullable_float(cim.current_limit_1),
+        **nullable_bool_settings("inverseTimeFlag", cim.inverse_time_flag),
+        timeDelay1=from_nullable_float(cim.time_delay_1),
+    )
+
+
+def protection_equipment_to_pb(cim: ProtectionEquipment, include_asset_info: bool = False) -> PBProtectionEquipment:
+    return PBProtectionEquipment(
+        eq=equipment_to_pb(cim, include_asset_info),
+        relayDelayTime=from_nullable_float(cim.relay_delay_time),
+        protectionKind=PBProtectionKind.Value(cim.protection_kind.short_name),
+        protectedSwitchMRIDs=[str(io.mrid) for io in cim.protected_switches]
+    )
+
+
+def reclose_sequence_to_pb(cim: RecloseSequence) -> PBRecloseSequence:
+    return PBRecloseSequence(
+        io=identified_object_to_pb(cim),
+        recloseDelay=from_nullable_float(cim.reclose_delay),
+        recloseStep=from_nullable_int(cim.reclose_step)
+    )
+
+
+CurrentRelay.to_pb = current_relay_to_pb
+ProtectionEquipment.to_pb = protection_equipment_to_pb
+RecloseSequence.to_pb = reclose_sequence_to_pb
+
+
 #######################
 # IEC61970 BASE SCADA #
 #######################
 
 def remote_control_to_pb(cim: RemoteControl) -> PBRemoteControl:
     return PBRemoteControl(
         rp=remote_point_to_pb(cim),
@@ -857,15 +928,18 @@
     return PBAcLineSegment(
         cd=conductor_to_pb(cim),
         perLengthSequenceImpedanceMRID=mrid_or_empty(cim.per_length_sequence_impedance)
     )
 
 
 def breaker_to_pb(cim: Breaker) -> PBBreaker:
-    return PBBreaker(sw=protected_switch_to_pb(cim))
+    return PBBreaker(
+        sw=protected_switch_to_pb(cim),
+        inTransitTime=from_nullable_float(cim.in_transit_time)
+    )
 
 
 def conductor_to_pb(cim: Conductor) -> PBConductor:
     return PBConductor(
         ce=conducting_equipment_to_pb(cim, True),
         length=from_nullable_float(cim.length)
     )
@@ -1057,15 +1131,20 @@
         g=from_nullable_float(cim.g),
         g0=from_nullable_float(cim.g0),
         phaseAngleClock=from_nullable_int(cim.phase_angle_clock)
     )
 
 
 def protected_switch_to_pb(cim: ProtectedSwitch) -> PBProtectedSwitch:
-    return PBProtectedSwitch(sw=switch_to_pb(cim))
+    return PBProtectedSwitch(
+        sw=switch_to_pb(cim),
+        breakingCapacity=from_nullable_int(cim.breaking_capacity),
+        recloseSequenceMRIDs=[str(io.mrid) for io in cim.reclose_sequences],
+        operatedByProtectionEquipmentMRIDs=[str(io.mrid) for io in cim.operated_by_protection_equipment]
+    )
 
 
 def ratio_tap_changer_to_pb(cim: RatioTapChanger) -> PBRatioTapChanger:
     return PBRatioTapChanger(
         tc=tap_changer_to_pb(cim),
         transformerEndMRID=mrid_or_empty(cim.transformer_end),
         stepVoltageIncrement=from_nullable_float(cim.step_voltage_increment)
@@ -1091,15 +1170,16 @@
         nomU=from_nullable_int(cim.nom_u),
         phaseConnection=PBPhaseShuntConnectionKind.Enum.Value(cim.phase_connection.short_name)
     )
 
 
 def switch_to_pb(cim: Switch) -> PBSwitch:
     return PBSwitch(
-        ce=conducting_equipment_to_pb(cim),
+        ce=conducting_equipment_to_pb(cim, True),
+        ratedCurrent=from_nullable_uint(cim.rated_current),
         normalOpen=cim.get_normal_state(),
         open=cim.get_state()
     )
 
 
 def tap_changer_to_pb(cim: TapChanger) -> PBTapChanger:
     return PBTapChanger(
```

## zepben/evolve/services/network/translator/network_proto2cim.py

```diff
@@ -10,14 +10,15 @@
 from zepben.protobuf.cim.iec61968.assetinfo.CableInfo_pb2 import CableInfo as PBCableInfo
 from zepben.protobuf.cim.iec61968.assetinfo.NoLoadTest_pb2 import NoLoadTest as PBNoLoadTest
 from zepben.protobuf.cim.iec61968.assetinfo.OpenCircuitTest_pb2 import OpenCircuitTest as PBOpenCircuitTest
 from zepben.protobuf.cim.iec61968.assetinfo.OverheadWireInfo_pb2 import OverheadWireInfo as PBOverheadWireInfo
 from zepben.protobuf.cim.iec61968.assetinfo.PowerTransformerInfo_pb2 import PowerTransformerInfo as PBPowerTransformerInfo
 from zepben.protobuf.cim.iec61968.assetinfo.ShortCircuitTest_pb2 import ShortCircuitTest as PBShortCircuitTest
 from zepben.protobuf.cim.iec61968.assetinfo.ShuntCompensatorInfo_pb2 import ShuntCompensatorInfo as PBShuntCompensatorInfo
+from zepben.protobuf.cim.iec61968.assetinfo.SwitchInfo_pb2 import SwitchInfo as PBSwitchInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerEndInfo_pb2 import TransformerEndInfo as PBTransformerEndInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerTankInfo_pb2 import TransformerTankInfo as PBTransformerTankInfo
 from zepben.protobuf.cim.iec61968.assetinfo.TransformerTest_pb2 import TransformerTest as PBTransformerTest
 from zepben.protobuf.cim.iec61968.assetinfo.WireInfo_pb2 import WireInfo as PBWireInfo
 from zepben.protobuf.cim.iec61968.assets.AssetContainer_pb2 import AssetContainer as PBAssetContainer
 from zepben.protobuf.cim.iec61968.assets.AssetInfo_pb2 import AssetInfo as PBAssetInfo
 from zepben.protobuf.cim.iec61968.assets.AssetOrganisationRole_pb2 import AssetOrganisationRole as PBAssetOrganisationRole
@@ -27,14 +28,15 @@
 from zepben.protobuf.cim.iec61968.assets.Streetlight_pb2 import Streetlight as PBStreetlight
 from zepben.protobuf.cim.iec61968.assets.Structure_pb2 import Structure as PBStructure
 from zepben.protobuf.cim.iec61968.common.Location_pb2 import Location as PBLocation
 from zepben.protobuf.cim.iec61968.common.PositionPoint_pb2 import PositionPoint as PBPositionPoint
 from zepben.protobuf.cim.iec61968.common.StreetAddress_pb2 import StreetAddress as PBStreetAddress
 from zepben.protobuf.cim.iec61968.common.StreetDetail_pb2 import StreetDetail as PBStreetDetail
 from zepben.protobuf.cim.iec61968.common.TownDetail_pb2 import TownDetail as PBTownDetail
+from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentRelayInfo_pb2 import CurrentRelayInfo as PBCurrentRelayInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentTransformerInfo_pb2 import CurrentTransformerInfo as PBCurrentTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.PotentialTransformerInfo_pb2 import PotentialTransformerInfo as PBPotentialTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infcommon.Ratio_pb2 import Ratio as PBRatio
 from zepben.protobuf.cim.iec61968.metering.EndDevice_pb2 import EndDevice as PBEndDevice
 from zepben.protobuf.cim.iec61968.metering.Meter_pb2 import Meter as PBMeter
 from zepben.protobuf.cim.iec61968.metering.UsagePoint_pb2 import UsagePoint as PBUsagePoint
 from zepben.protobuf.cim.iec61968.operations.OperationalRestriction_pb2 import OperationalRestriction as PBOperationalRestriction
@@ -61,14 +63,17 @@
 from zepben.protobuf.cim.iec61970.base.equivalents.EquivalentEquipment_pb2 import EquivalentEquipment as PBEquivalentEquipment
 from zepben.protobuf.cim.iec61970.base.meas.Accumulator_pb2 import Accumulator as PBAccumulator
 from zepben.protobuf.cim.iec61970.base.meas.Analog_pb2 import Analog as PBAnalog
 from zepben.protobuf.cim.iec61970.base.meas.Control_pb2 import Control as PBControl
 from zepben.protobuf.cim.iec61970.base.meas.Discrete_pb2 import Discrete as PBDiscrete
 from zepben.protobuf.cim.iec61970.base.meas.IoPoint_pb2 import IoPoint as PBIoPoint
 from zepben.protobuf.cim.iec61970.base.meas.Measurement_pb2 import Measurement as PBMeasurement
+from zepben.protobuf.cim.iec61970.base.protection.CurrentRelay_pb2 import CurrentRelay as PBCurrentRelay
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionEquipment_pb2 import ProtectionEquipment as PBProtectionEquipment
+from zepben.protobuf.cim.iec61970.base.protection.RecloseSequence_pb2 import RecloseSequence as PBRecloseSequence
 from zepben.protobuf.cim.iec61970.base.scada.RemoteControl_pb2 import RemoteControl as PBRemoteControl
 from zepben.protobuf.cim.iec61970.base.scada.RemotePoint_pb2 import RemotePoint as PBRemotePoint
 from zepben.protobuf.cim.iec61970.base.scada.RemoteSource_pb2 import RemoteSource as PBRemoteSource
 from zepben.protobuf.cim.iec61970.base.wires.AcLineSegment_pb2 import AcLineSegment as PBAcLineSegment
 from zepben.protobuf.cim.iec61970.base.wires.Breaker_pb2 import Breaker as PBBreaker
 from zepben.protobuf.cim.iec61970.base.wires.BusbarSection_pb2 import BusbarSection as PBBusbarSection
 from zepben.protobuf.cim.iec61970.base.wires.Conductor_pb2 import Conductor as PBConductor
@@ -110,26 +115,28 @@
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.LvFeeder_pb2 import LvFeeder as PBLvFeeder
 
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import *
+from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_tank_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.wire_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.wire_material_kind import *
 from zepben.evolve.model.cim.iec61968.assets.asset import *
 from zepben.evolve.model.cim.iec61968.assets.asset_info import *
 from zepben.evolve.model.cim.iec61968.assets.asset_organisation_role import *
 from zepben.evolve.model.cim.iec61968.assets.pole import *
 from zepben.evolve.model.cim.iec61968.assets.streetlight import *
 from zepben.evolve.model.cim.iec61968.assets.structure import *
 from zepben.evolve.model.cim.iec61968.common.location import *
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_construction_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_function_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infcommon.ratio import *
 from zepben.evolve.model.cim.iec61968.metering.metering import *
 from zepben.evolve.model.cim.iec61968.operations.operational_restriction import *
@@ -151,66 +158,78 @@
 from zepben.evolve.model.cim.iec61970.base.core.terminal import *
 from zepben.evolve.model.cim.iec61970.base.domain.unit_symbol import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_branch import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_equipment import *
 from zepben.evolve.model.cim.iec61970.base.meas.control import *
 from zepben.evolve.model.cim.iec61970.base.meas.iopoint import *
 from zepben.evolve.model.cim.iec61970.base.meas.measurement import *
+from zepben.evolve.model.cim.iec61970.base.protection.current_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.reclose_sequence import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_point import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import *
+from zepben.evolve.model.cim.iec61970.base.wires.breaker import Breaker
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import *
+from zepben.evolve.model.cim.iec61970.base.wires.disconnector import Disconnector
 from zepben.evolve.model.cim.iec61970.base.wires.energy_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import *
+from zepben.evolve.model.cim.iec61970.base.wires.fuse import Fuse
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.battery_state_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import *
+from zepben.evolve.model.cim.iec61970.base.wires.jumper import Jumper
 from zepben.evolve.model.cim.iec61970.base.wires.line import *
+from zepben.evolve.model.cim.iec61970.base.wires.load_break_switch import LoadBreakSwitch
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import *
 from zepben.evolve.model.cim.iec61970.base.wires.phase_shunt_connection_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import *
+from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import ProtectedSwitch
+from zepben.evolve.model.cim.iec61970.base.wires.recloser import Recloser
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.single_phase_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.transformer_star_impedance import *
 from zepben.evolve.model.cim.iec61970.base.wires.vector_group import *
 from zepben.evolve.model.cim.iec61970.base.wires.winding_connection import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.circuit import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.loop import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import *
+from zepben.evolve.model.cim.iec61970.infiec61970.protection.protection_kind import *
 from zepben.evolve.model.phases import TracedPhases
 
 import zepben.evolve.services.common.resolver as resolver
 from zepben.evolve.services.common.translator.base_proto2cim import identified_object_to_cim, organisation_role_to_cim, document_to_cim
 from zepben.evolve.services.common.translator.util import int_or_none, float_or_none, long_or_none, str_or_none, uint_or_none
 from zepben.evolve.services.network.network_service import NetworkService
 from zepben.evolve.services.network.tracing.feeder.feeder_direction import FeederDirection
 
 __all__ = [
     "cable_info_to_cim", "no_load_test_to_cim", "open_circuit_test_to_cim", "overhead_wire_info_to_cim", "power_transformer_info_to_cim",
-    "short_circuit_test_to_cim", "shunt_compensator_info_to_cim", "transformer_end_info_to_cim", "transformer_tank_info_to_cim", "transformer_test_to_cim",
-    "wire_info_to_cim", "asset_to_cim", "asset_container_to_cim", "asset_info_to_cim", "asset_organisation_role_to_cim", "asset_owner_to_cim", "pole_to_cim",
-    "streetlight_to_cim", "structure_to_cim", "location_to_cim", "position_point_to_cim", "street_address_to_cim", "town_detail_to_cim", "end_device_to_cim",
-    "meter_to_cim", "usage_point_to_cim", "operational_restriction_to_cim", "auxiliary_equipment_to_cim", "fault_indicator_to_cim", "ac_dc_terminal_to_cim",
-    "base_voltage_to_cim", "conducting_equipment_to_cim", "connectivity_node_to_cim", "connectivity_node_container_to_cim", "equipment_to_cim",
-    "equipment_container_to_cim", "feeder_to_cim", "geographical_region_to_cim", "power_system_resource_to_cim", "site_to_cim",
-    "sub_geographical_region_to_cim", "substation_to_cim", "terminal_to_cim", "equivalent_branch_to_cim", "equivalent_equipment_to_cim", "accumulator_to_cim",
-    "analog_to_cim", "control_to_cim", "discrete_to_cim", "io_point_to_cim", "measurement_to_cim", "remote_control_to_cim", "remote_point_to_cim",
-    "remote_source_to_cim", "battery_unit_to_cim", "photo_voltaic_unit_to_cim", "power_electronics_unit_to_cim", "power_electronics_wind_unit_to_cim",
-    "ac_line_segment_to_cim", "breaker_to_cim", "conductor_to_cim", "connector_to_cim", "disconnector_to_cim", "energy_connection_to_cim",
-    "energy_consumer_to_cim", "energy_consumer_phase_to_cim", "energy_source_to_cim", "energy_source_phase_to_cim", "fuse_to_cim", "jumper_to_cim",
-    "junction_to_cim", "busbar_section_to_cim", "line_to_cim", "linear_shunt_compensator_to_cim", "load_break_switch_to_cim",
+    "short_circuit_test_to_cim", "shunt_compensator_info_to_cim", "switch_info_to_cim", "transformer_end_info_to_cim", "transformer_tank_info_to_cim",
+    "transformer_test_to_cim", "wire_info_to_cim", "asset_to_cim", "asset_container_to_cim", "asset_info_to_cim", "asset_organisation_role_to_cim",
+    "asset_owner_to_cim", "pole_to_cim", "streetlight_to_cim", "structure_to_cim", "location_to_cim", "position_point_to_cim", "street_address_to_cim",
+    "street_detail_to_cim", "town_detail_to_cim", "current_relay_info_to_cim", "current_transformer_info_to_cim", "potential_transformer_info_to_cim",
+    "ratio_to_cim", "end_device_to_cim", "meter_to_cim", "usage_point_to_cim", "operational_restriction_to_cim", "auxiliary_equipment_to_cim",
+    "current_transformer_to_cim", "fault_indicator_to_cim", "potential_transformer_to_cim", "sensor_to_cim", "ac_dc_terminal_to_cim", "base_voltage_to_cim",
+    "conducting_equipment_to_cim", "connectivity_node_to_cim", "connectivity_node_container_to_cim", "equipment_to_cim", "equipment_container_to_cim",
+    "feeder_to_cim", "geographical_region_to_cim", "power_system_resource_to_cim", "site_to_cim", "sub_geographical_region_to_cim", "substation_to_cim",
+    "terminal_to_cim", "equivalent_branch_to_cim", "equivalent_equipment_to_cim", "accumulator_to_cim", "analog_to_cim", "control_to_cim", "discrete_to_cim",
+    "io_point_to_cim", "measurement_to_cim", "current_relay_to_cim", "protection_equipment_to_cim", "reclose_sequence_to_cim", "remote_control_to_cim",
+    "remote_point_to_cim", "remote_source_to_cim", "battery_unit_to_cim", "photo_voltaic_unit_to_cim", "power_electronics_unit_to_cim",
+    "power_electronics_wind_unit_to_cim", "ac_line_segment_to_cim", "breaker_to_cim", "conductor_to_cim", "connector_to_cim", "disconnector_to_cim",
+    "energy_connection_to_cim", "energy_consumer_to_cim", "energy_consumer_phase_to_cim", "energy_source_to_cim", "energy_source_phase_to_cim", "fuse_to_cim",
+    "jumper_to_cim", "junction_to_cim", "busbar_section_to_cim", "line_to_cim", "linear_shunt_compensator_to_cim", "load_break_switch_to_cim",
     "per_length_line_parameter_to_cim", "per_length_impedance_to_cim", "per_length_sequence_impedance_to_cim", "power_electronics_connection_to_cim",
     "power_electronics_connection_phase_to_cim", "power_transformer_to_cim", "power_transformer_end_to_cim", "transformer_star_impedance_to_cim",
     "protected_switch_to_cim", "ratio_tap_changer_to_cim", "recloser_to_cim", "regulating_cond_eq_to_cim", "shunt_compensator_to_cim", "switch_to_cim",
-    "tap_changer_to_cim", "transformer_end_to_cim", "circuit_to_cim", "loop_to_cim", "lv_feeder_to_cim", "current_transformer_info_to_cim",
-    "potential_transformer_info_to_cim", "current_transformer_to_cim", "potential_transformer_to_cim"
+    "tap_changer_to_cim", "transformer_end_to_cim", "circuit_to_cim", "loop_to_cim", "lv_feeder_to_cim"
 ]
 
 
 #######################
 # IEC61968 ASSET INFO #
 #######################
 
@@ -300,14 +319,24 @@
         rated_voltage=int_or_none(pb.ratedVoltage),
     )
 
     asset_info_to_cim(pb.ai, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
+def switch_info_to_cim(pb: PBSwitchInfo, network_service: NetworkService) -> Optional[SwitchInfo]:
+    cim = SwitchInfo(
+        mrid=pb.mrid(),
+        rated_interrupting_time=float_or_none(pb.ratedInterruptingTime)
+    )
+
+    asset_info_to_cim(pb.ai, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
 def transformer_end_info_to_cim(pb: PBTransformerEndInfo, network_service: NetworkService) -> Optional[TransformerEndInfo]:
     # noinspection PyArgumentList
     cim = TransformerEndInfo(
         mrid=pb.mrid(),
         connection_kind=WindingConnection(pb.connectionKind),
         emergency_s=int_or_none(pb.emergencyS),
         end_number=pb.endNumber,
@@ -358,14 +387,15 @@
 PBCableInfo.to_cim = cable_info_to_cim
 PBNoLoadTest.to_cim = no_load_test_to_cim
 PBOpenCircuitTest.to_cim = open_circuit_test_to_cim
 PBOverheadWireInfo.to_cim = overhead_wire_info_to_cim
 PBPowerTransformerInfo.to_cim = power_transformer_info_to_cim
 PBShortCircuitTest.to_cim = short_circuit_test_to_cim
 PBShuntCompensatorInfo.to_cim = shunt_compensator_info_to_cim
+PBSwitchInfo.to_cim = switch_info_to_cim
 PBTransformerEndInfo.to_cim = transformer_end_info_to_cim
 PBTransformerTankInfo.to_cim = transformer_tank_info_to_cim
 PBTransformerTest.to_cim = transformer_test_to_cim
 PBWireInfo.to_cim = wire_info_to_cim
 
 
 ###################
@@ -387,15 +417,15 @@
 
 def asset_info_to_cim(pb: PBAssetInfo, cim: AssetInfo, network_service: NetworkService):
     identified_object_to_cim(pb.io, cim, network_service)
 
 
 def asset_organisation_role_to_cim(pb: PBAssetOrganisationRole, cim: AssetOrganisationRole,
                                    network_service: NetworkService):
-    organisation_role_to_cim(getattr(pb, 'or'), cim, network_service)
+    organisation_role_to_cim(getattr(pb, "or"), cim, network_service)
 
 
 def asset_owner_to_cim(pb: PBAssetOwner, network_service: NetworkService) -> Optional[AssetOwner]:
     # noinspection PyArgumentList
     cim = AssetOwner(mrid=pb.mrid())
 
     asset_organisation_role_to_cim(pb.aor, cim, network_service)
@@ -440,15 +470,15 @@
 
 
 ###################
 # IEC61968 COMMON #
 ###################
 
 def location_to_cim(pb: PBLocation, network_service: NetworkService) -> Optional[Location]:
-    cim = Location(mrid=pb.mrid(), main_address=street_address_to_cim(pb.mainAddress) if pb.HasField('mainAddress') else None)
+    cim = Location(mrid=pb.mrid(), main_address=street_address_to_cim(pb.mainAddress) if pb.HasField("mainAddress") else None)
 
     for point in pb.positionPoints:
         cim.add_point(position_point_to_cim(point))
 
     identified_object_to_cim(pb.io, cim, network_service)
     return cim if network_service.add(cim) else None
 
@@ -458,17 +488,17 @@
     return PositionPoint(pb.xPosition, pb.yPosition)
 
 
 def street_address_to_cim(pb: PBStreetAddress) -> Optional[StreetAddress]:
     # noinspection PyArgumentList
     return StreetAddress(
         postal_code=pb.postalCode,
-        town_detail=town_detail_to_cim(pb.townDetail) if pb.HasField('townDetail') else None,
+        town_detail=town_detail_to_cim(pb.townDetail) if pb.HasField("townDetail") else None,
         po_box=pb.poBox,
-        street_detail=street_detail_to_cim(pb.streetDetail) if pb.HasField('streetDetail') else None
+        street_detail=street_detail_to_cim(pb.streetDetail) if pb.HasField("streetDetail") else None
     )
 
 
 def street_detail_to_cim(pb: PBStreetDetail) -> Optional[StreetDetail]:
     # noinspection PyArgumentList
     return StreetDetail(
         building_name=pb.buildingName,
@@ -493,24 +523,34 @@
 PBTownDetail.to_cim = town_detail_to_cim
 
 
 #####################################
 # IEC61968 infIEC61968 InfAssetInfo #
 #####################################
 
+def current_relay_info_to_cim(pb: PBCurrentRelayInfo, network_service: NetworkService) -> Optional[CurrentRelayInfo]:
+    cim = CurrentRelayInfo(
+        mrid=pb.mrid(),
+        curve_setting=str_or_none(pb.curveSetting)
+    )
+
+    asset_info_to_cim(pb.ai, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
 def current_transformer_info_to_cim(pb: PBCurrentTransformerInfo, network_service: NetworkService) -> Optional[CurrentTransformerInfo]:
     cim = CurrentTransformerInfo(
         mrid=pb.mrid(),
         accuracy_class=str_or_none(pb.accuracyClass),
         accuracy_limit=float_or_none(pb.accuracyLimit),
         core_count=int_or_none(pb.coreCount),
         ct_class=str_or_none(pb.ctClass),
         knee_point_voltage=int_or_none(pb.kneePointVoltage),
-        max_ratio=ratio_to_cim(pb.maxRatio) if pb.HasField('maxRatio') else None,
-        nominal_ratio=ratio_to_cim(pb.nominalRatio) if pb.HasField('nominalRatio') else None,
+        max_ratio=ratio_to_cim(pb.maxRatio) if pb.HasField("maxRatio") else None,
+        nominal_ratio=ratio_to_cim(pb.nominalRatio) if pb.HasField("nominalRatio") else None,
         primary_ratio=float_or_none(pb.primaryRatio),
         rated_current=int_or_none(pb.ratedCurrent),
         secondary_fls_rating=int_or_none(pb.secondaryFlsRating),
         secondary_ratio=float_or_none(pb.secondaryRatio),
         usage=str_or_none(pb.usage)
     )
 
@@ -518,34 +558,36 @@
     return cim if network_service.add(cim) else None
 
 
 def potential_transformer_info_to_cim(pb: PBPotentialTransformerInfo, network_service: NetworkService) -> Optional[PotentialTransformerInfo]:
     cim = PotentialTransformerInfo(
         mrid=pb.mrid(),
         accuracy_class=str_or_none(pb.accuracyClass),
-        nominal_ratio=ratio_to_cim(pb.nominalRatio) if pb.HasField('nominalRatio') else None,
+        nominal_ratio=ratio_to_cim(pb.nominalRatio) if pb.HasField("nominalRatio") else None,
         primary_ratio=float_or_none(pb.primaryRatio),
         pt_class=str_or_none(pb.ptClass),
         rated_voltage=int_or_none(pb.ratedVoltage),
         secondary_ratio=float_or_none(pb.secondaryRatio)
     )
 
     asset_info_to_cim(pb.ai, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
+PBCurrentRelayInfo.to_cim = current_relay_info_to_cim
 PBCurrentTransformerInfo.to_cim = current_transformer_info_to_cim
 PBPotentialTransformerInfo.to_cim = potential_transformer_info_to_cim
 
 
 ##################################
 # IEC61968 infIEC61968 InfCommon #
 ##################################
 
 def ratio_to_cim(pb: PBRatio) -> Ratio:
+    # noinspection PyArgumentList
     return Ratio(pb.numerator, pb.denominator)
 
 
 PBRatio.to_cim = ratio_to_cim
 
 
 #####################
@@ -899,14 +941,58 @@
 PBAnalog.to_cim = analog_to_cim
 PBControl.to_cim = control_to_cim
 PBDiscrete.to_cim = discrete_to_cim
 PBIoPoint.to_cim = io_point_to_cim
 PBMeasurement.to_cim = measurement_to_cim
 
 
+############################
+# IEC61970 Base Protection #
+############################
+
+
+def current_relay_to_cim(pb: PBCurrentRelay, network_service: NetworkService) -> Optional[CurrentRelay]:
+    cim = CurrentRelay(
+        mrid=pb.mrid(),
+        current_limit_1=float_or_none(pb.currentLimit1),
+        inverse_time_flag=None if pb.HasField("inverseTimeFlagNull") else pb.inverseTimeFlagSet,
+        time_delay_1=float_or_none(pb.timeDelay1)
+    )
+
+    network_service.resolve_or_defer_reference(resolver.current_relay_info(cim), pb.asset_info_mrid())
+
+    protection_equipment_to_cim(pb.pe, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
+def protection_equipment_to_cim(pb: PBProtectionEquipment, cim: ProtectionEquipment, network_service: NetworkService):
+    cim.relay_delay_time = float_or_none(pb.relayDelayTime)
+    cim.protection_kind = ProtectionKind(pb.protectionKind)
+
+    for mrid in pb.protectedSwitchMRIDs:
+        network_service.resolve_or_defer_reference(resolver.protected_switches(cim), mrid)
+
+    equipment_to_cim(pb.eq, cim, network_service)
+
+
+def reclose_sequence_to_cim(pb: PBRecloseSequence, network_service: NetworkService):
+    cim = RecloseSequence(
+        mrid=pb.mrid(),
+        reclose_delay=float_or_none(pb.recloseDelay),
+        reclose_step=int_or_none(pb.recloseStep)
+    )
+
+    identified_object_to_cim(pb.io, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
+PBCurrentRelay.to_cim = current_relay_to_cim
+PBRecloseSequence.to_cim = reclose_sequence_to_cim
+
+
 #######################
 # IEC61970 BASE SCADA #
 #######################
 
 def remote_control_to_cim(pb: PBRemoteControl, network_service: NetworkService) -> Optional[RemoteControl]:
     # noinspection PyArgumentList
     cim = RemoteControl(mrid=pb.mrid())
@@ -991,15 +1077,18 @@
     network_service.resolve_or_defer_reference(resolver.per_length_sequence_impedance(cim), pb.perLengthSequenceImpedanceMRID)
 
     conductor_to_cim(pb.cd, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def breaker_to_cim(pb: PBBreaker, network_service: NetworkService) -> Optional[Breaker]:
-    cim = Breaker(mrid=pb.mrid())
+    cim = Breaker(
+        mrid=pb.mrid(),
+        in_transit_time=float_or_none(pb.inTransitTime)
+    )
 
     protected_switch_to_cim(pb.sw, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def conductor_to_cim(pb: PBConductor, cim: Conductor, network_service: NetworkService):
     cim.length = float_or_none(pb.length)
@@ -1267,14 +1356,22 @@
     network_service.resolve_or_defer_reference(resolver.star_impedance_transformer_end_info(cim), pb.transformerEndInfoMRID)
 
     identified_object_to_cim(pb.io, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def protected_switch_to_cim(pb: PBProtectedSwitch, cim: ProtectedSwitch, network_service: NetworkService):
+    cim.breaking_capacity = int_or_none(pb.breakingCapacity)
+
+    for mrid in pb.recloseSequenceMRIDs:
+        network_service.resolve_or_defer_reference(resolver.reclose_sequences(cim), mrid)
+
+    for mrid in pb.operatedByProtectionEquipmentMRIDs:
+        network_service.resolve_or_defer_reference(resolver.operated_by_protection_equipment(cim), mrid)
+
     switch_to_cim(pb.sw, cim, network_service)
 
 
 def ratio_tap_changer_to_cim(pb: PBRatioTapChanger, network_service: NetworkService) -> Optional[RatioTapChanger]:
     cim = RatioTapChanger(
         mrid=pb.mrid(),
         step_voltage_increment=float_or_none(pb.stepVoltageIncrement)
@@ -1306,14 +1403,16 @@
     cim.nom_u = int_or_none(pb.nomU)
     cim.phase_connection = PhaseShuntConnectionKind(pb.phaseConnection)
 
     regulating_cond_eq_to_cim(pb.rce, cim, network_service)
 
 
 def switch_to_cim(pb: PBSwitch, cim: Switch, network_service: NetworkService):
+    network_service.resolve_or_defer_reference(resolver.switch_info(cim), pb.asset_info_mrid())
+    cim.rated_current = uint_or_none(pb.ratedCurrent)
     cim.set_normally_open(pb.normalOpen)
     cim.set_open(pb.open)
 
     conducting_equipment_to_cim(pb.ce, cim, network_service)
 
 
 def tap_changer_to_cim(pb: PBTapChanger, cim: TapChanger, network_service: NetworkService):
```

## Comparing `zepben.evolve-0.35.0b8.dist-info/LICENSE` & `zepben.evolve-0.35.0b9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zepben.evolve-0.35.0b8.dist-info/METADATA` & `zepben.evolve-0.35.0b9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zepben.evolve
-Version: 0.35.0b8
+Version: 0.35.0b9
 Summary: Python SDK for interacting with the Evolve platform
 Home-page: https://github.com/zepben/evolve-sdk-python
 Author: Kurt Greaves
 Author-email: kurt.greaves@zepben.com
 License: MPL 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (<2.27.0,>=2.26.0)
-Requires-Dist: zepben.protobuf (==0.23.0b1)
+Requires-Dist: zepben.protobuf (==0.23.0b5)
 Requires-Dist: zepben.auth (==0.10.0b2)
 Requires-Dist: dataclassy (==0.6.2)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: mock (==4.0.3)
 Provides-Extra: test
 Requires-Dist: pytest (==7.1.2) ; extra == 'test'
 Requires-Dist: pytest-cov (==2.10.1) ; extra == 'test'
```

## Comparing `zepben.evolve-0.35.0b8.dist-info/RECORD` & `zepben.evolve-0.35.0b9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,100 @@
-zepben/evolve/__init__.py,sha256=HYkDB8RW_zGyJLHPLHoJiyfuoQ7dRdfCtwU8hCkmcE8,17077
+zepben/evolve/__init__.py,sha256=mtZy1JRGtdPFqTyo9yVfMl0q7ryhfB_V5M2SHBNcbWk,18234
 zepben/evolve/exceptions.py,sha256=4eUY0GFMFHIUsWQ1EvvZOVEGeOR9AQl6PCELScTKeVk,1387
 zepben/evolve/types.py,sha256=lzuvuOQqT8D5Cjc7l34OauIdf1K9Mz584rzZjN_W_ls,1132
 zepben/evolve/util.py,sha256=KsNJTqgt7il2DRfdj3mLgQX215uBU-oicX4kHEnEEc4,4576
 zepben/evolve/database/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
-zepben/evolve/database/sqlite/database_reader.py,sha256=tIN-Woh25EUIDopDqlykVkHtoWx6NX3qQfGSGM7ihiY,6640
+zepben/evolve/database/sqlite/database_reader.py,sha256=ZaD1RZZy7Che22ti0haHJ9XcWJcTIs2tVLNDYKh806w,6688
 zepben/evolve/database/sqlite/database_writer.py,sha256=jc4OHkokCf3gTMcZZEqiAZ-4d-6BaeS0Ruhg7mhHWkI,5803
 zepben/evolve/database/sqlite/readers/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/readers/base_cim_reader.py,sha256=Lo55R_8Z8zjKbpSriN_lezYZFb6ClCIdB9mJg1zaAD8,5319
 zepben/evolve/database/sqlite/readers/base_service_reader.py,sha256=rm1ZX7XrhGHPf8FitvKpwBFZl7XXAqINGQlo51ySaxM,2991
 zepben/evolve/database/sqlite/readers/customer_cim_reader.py,sha256=_7gCOhEWJlYD3fEXp9kBvNq__iCQGEXaH1zbEtn2j7M,4510
 zepben/evolve/database/sqlite/readers/customer_service_reader.py,sha256=3f0DSehd7gYyIdWvNwKYGDScyh5dqlIWfgpbixvyhfo,1761
 zepben/evolve/database/sqlite/readers/diagram_cim_reader.py,sha256=rvI-b0yTQ7Payjc2UXgw1O3a7IxT5Jp38PsRtdWNTYQ,3245
 zepben/evolve/database/sqlite/readers/diagram_service_reader.py,sha256=BnrYdlsMC7WQ-gli83k9xQe1JOvjdT2yzAVRnerXIoA,1041
 zepben/evolve/database/sqlite/readers/metadata_collection_reader.py,sha256=5GyXYWOPRH2jxdLMkHok8DnbrrlDZLgdHG8M_CF5FQw,733
 zepben/evolve/database/sqlite/readers/metadata_entry_reader.py,sha256=sSu4F65iKmNuONgRqJKPHI07aM4oHVd4r9PJhgiLnZ4,1088
-zepben/evolve/database/sqlite/readers/network_cim_reader.py,sha256=y8nnw3bKEWlKwspk6Nfbkx-XT89VuvgxZ3r2QpPgIe8,68283
-zepben/evolve/database/sqlite/readers/network_service_reader.py,sha256=T471089q-tUr7hJumGRij88cegeuyvEqJVVwxxySZ04,11437
+zepben/evolve/database/sqlite/readers/network_cim_reader.py,sha256=HVj2M6dDgZzbblB1AgPIH9lHV8SvTvALAL5VffCPM70,72711
+zepben/evolve/database/sqlite/readers/network_service_reader.py,sha256=3CqvDXA9qTNclIP_YWYMeM_V6xCceM6CW7d29g62k9U,12259
 zepben/evolve/database/sqlite/readers/result_set.py,sha256=Wzp-8JgO48Dus7RafGrq3J9-LcHqjqqHQU4ab3IWTtY,6872
 zepben/evolve/database/sqlite/tables/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/column.py,sha256=CV0qjq0yh2O_f6eifnPZonjYhSP9PhFHCvLpc876v6s,1009
-zepben/evolve/database/sqlite/tables/database_tables.py,sha256=WAielBf8LP2vpFleJVhFCk6sJ-nefLSVEZgLzANHaNA,11385
+zepben/evolve/database/sqlite/tables/database_tables.py,sha256=FjehDiIcnjOpj8W1wHjVPfS70pmIY5Si6ib5PZaSbHE,11816
 zepben/evolve/database/sqlite/tables/exceptions.py,sha256=pbvLh4ebcd4S8_KGo1V77zUJjDLXqd9ZJiFYSwa5-eg,403
-zepben/evolve/database/sqlite/tables/metadata_tables.py,sha256=D3OjCByGfD6NcBJRr8khvi7Rt1OaJno-cj7EEB7Bbjs,1164
+zepben/evolve/database/sqlite/tables/metadata_tables.py,sha256=uOCGQe_qJD8MrXeDYIvH8ybhXRcdPhAQgmMSpjSGbPM,1164
 zepben/evolve/database/sqlite/tables/sqlite_table.py,sha256=GVCX3LWMA05kb2wjwLk9GaBDBMzm5VBEQBwgmi8FTZw,5820
 zepben/evolve/database/sqlite/tables/associations/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py,sha256=JrwgezI7eBqSNzUC56C7XtNrLNed3vuon-ZNasL0IqU,1484
 zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py,sha256=vXNdgz_UYKZ2AyAzz4dpTvXD3D8zjKVeNvvTiJLYh04,2295
 zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py,sha256=Wisqd5Lqbwnl0zYet3OBZztQGnkoYRpkHbRQ4jrGpso,1561
 zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py,sha256=r2XCZD_wWu2ryjo2ih0nu1imdNDOMn-jy_FlkzR079Y,3547
 zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py,sha256=b5SNfGeLJ7m0m9tNRE7-fB7GdL8M5xDwyjPG1ersjys,1696
 zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py,sha256=Y5kDx5ojDr-pmq2I3Wny2wA3G7ghEW4AyH6H_i46NGE,1435
+zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py,sha256=8cm62CmmC17CvWBX00DgNV6zq8ad_DPk8Esefj3Lhm4,1572
 zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py,sha256=kxugBZD_Y3f7jbu4NY8M7uOg4YnvNyRehllwXEeKy9E,1409
 zepben/evolve/database/sqlite/tables/iec61968/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py,sha256=QOeJ9ICw6y3_oFEUE60gwp5b72bUlLwS2hqM2YfS_gE,2240
-zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py,sha256=bK4bB1OcYrPTpWRJt-iihaasRmrRqftTgV5bCpUNs1w,8739
+zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py,sha256=sQ_tZtEH2IS97R5V1lc0fRgq0jEOVDT35eCXFKI7b0E,9094
 zepben/evolve/database/sqlite/tables/iec61968/common_tables.py,sha256=gVgChRuntHugMfL-NfSjndazex49FlJM82YFLj8MJig,5681
 zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py,sha256=4N-p6nuyVbBgEtiAvZaspC-ue65LXKVobgI2M4JvFI0,1705
 zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py,sha256=s_3xvfHh_2_P-98MhOOsZKK195enG1-I_b0QgyKGlQU,1629
 zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py,sha256=Jf79k-2HdSFraxEFoondmHIzLZ7fsbLyCoZuhEhiJNA,494
 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py,sha256=qkHg6NMUq2sNLqFdkpbeQeYuYxDUJavrxlksDwVQdkY,3669
+zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py,sha256=pxAQzBtsftX7EfInh3qAK9XCLhJezkHCiDF3uV4NvOM,4006
 zepben/evolve/database/sqlite/tables/iec61970/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py,sha256=LIdAYBtwuElrgLuJ7UyiSAN1V92XN6KggqmH8K9PxRs,1995
 zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py,sha256=8bjlYmF_SpoABRC_BcXLM6m04hIw0vKrEdZdXTBfQpQ,8308
 zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py,sha256=IN3i52QSloZ_E_HVFc5o-jsNu3uRBIy7mb4foMrmTvE,3113
 zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py,sha256=1xhxCbHQQxeGC1v6SakyWr0ayWtivz72cfw-9NUayW0,2454
 zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py,sha256=NUBdg8d9q_SNgxgN3BQjZr7y7GR4w0rURHJtc8qvYeE,2581
+zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py,sha256=YRU6do-ypNBr8PBriuOB8IlkmYsciHI1LXRFIn7VfJw,2270
 zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py,sha256=XzhIia2eiLlM1jvi0HpSvCWaTS0aLdxlvxAjpELighI,1205
 zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/iec61970/base/infiec61970/feeder_tables.py,sha256=Z5OLCIrRoKAkD8jQpP44YDPRJpGBNJ23vSjXmRr-53Q,1515
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py,sha256=DGL5fdsMjAgm1mnO1IYw9JNIMbQ9gGcTG7moYwy2ieE,1226
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py,sha256=4riWaMbOcixTPpC3IwEBDx9FDziLcYADHh3qym8ycCM,710
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py,sha256=NsoWgpK5afTT_HtP2SucS2_8zN2RZONTK2aajwSsXCU,458
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py,sha256=g5Y8cMqY37LRjMpF1hrMic9ajgaYciC_15PSaBGUt80,10492
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py,sha256=gZktb4mRARMR-s57uQLXDAkd_hV8r4mquyKmyJEwBg4,1845
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py,sha256=Fb0neWGiiaq0AS_1QLpg2AfmkBE7nin5VcqvTWwRlFQ,1659
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py,sha256=ikzKzeOwNugsWSeEPE38FQYfHBMdROfjWMIJznAOEnI,2325
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py,sha256=27j5oShun8jKwEw-c6z94K3PM9t7RcOeP8XfV9Phf5E,7441
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py,sha256=EHqhrrCsctfG6yRzStnZUzKuuDemtNlgSvpfwLcLzqo,2114
 zepben/evolve/database/sqlite/writers/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
-zepben/evolve/database/sqlite/writers/base_cim_writer.py,sha256=LFty2oWq5jJGG5Eu29u70KD5-Fg-Gv9Q6dRr20BZHPs,5254
+zepben/evolve/database/sqlite/writers/base_cim_writer.py,sha256=UnC0bjgdV8pi8-mr25EhJqvAXIuo4ZZcddPyIgeHTsA,5263
 zepben/evolve/database/sqlite/writers/base_service_writer.py,sha256=_1YtEuglQcK6-EZV5voKB8staQ3B45EcY4NfVmq5VYc,2995
-zepben/evolve/database/sqlite/writers/customer_cim_writer.py,sha256=gusA9MWoqGM7IzyR3SxyG5tJxz4TduAYUurO2mx5nb4,4748
+zepben/evolve/database/sqlite/writers/customer_cim_writer.py,sha256=JcgS6cKChei6-zjY_i0DH-be-Eyg8wSsE_PNxOHqToM,4752
 zepben/evolve/database/sqlite/writers/customer_service_writer.py,sha256=5FFU4nDtHU9aeyDB8AE56SCJNrg5jVqEaIz9in1ckV4,1393
-zepben/evolve/database/sqlite/writers/diagram_cim_writer.py,sha256=2KCnECJmj0gmSlio-4BSDAHlEDu2Ar6vT4Rjdc0LoJ4,2654
+zepben/evolve/database/sqlite/writers/diagram_cim_writer.py,sha256=gt0zPfC4eF3kYdqow4PulN2MtzP_b9QvhFci2eybhRk,2657
 zepben/evolve/database/sqlite/writers/diagram_service_writer.py,sha256=pEjVWxXj36KAH-sbnfw4ZX1JlVV9iXLKlSAT2Tq2qJI,1004
 zepben/evolve/database/sqlite/writers/metadata_collection_writer.py,sha256=EKEM3xesMy9tNCkd_i1sQJf1nMH91gKJicMow-bKhjU,904
 zepben/evolve/database/sqlite/writers/metadata_entry_writer.py,sha256=3nepwz1lAJ_lUMqyccRPQDCNlqJjws11-xom80NmyC8,1257
-zepben/evolve/database/sqlite/writers/network_cim_writer.py,sha256=bXH2-Vmt4VzmdS6c9Fw92o3d5w_tVIjtSD0fMxc4WHc,65924
-zepben/evolve/database/sqlite/writers/network_service_writer.py,sha256=pFGjIPUXxw2kyMFHqvA9fVJUXnUU9nDH1NfRdvfCLqo,7983
+zepben/evolve/database/sqlite/writers/network_cim_writer.py,sha256=KYUvCGs_U13R8VoAt4woKfRj1dct8KpKi-Y_oyXYY0Y,70327
+zepben/evolve/database/sqlite/writers/network_service_writer.py,sha256=lYGOCSQl7sNUM9vAc9Er2XBh-cF_aCCJMt3VSLvfjjg,8395
 zepben/evolve/database/sqlite/writers/utils.py,sha256=9-LeN3lzAM-G5D2SMlIfce20GHvEe35DiBbgckTBdAg,1430
 zepben/evolve/examples/__init__.py,sha256=P2Sy6K493IiVzpnYbjqonBYlEb3K_MJnJXaF9gm6k6c,309
 zepben/evolve/examples/simple_node_breaker_feeder.py,sha256=ksaZsW-HmWhc0YvBq8nD_NopUOK7i9BIeITBTAhKffI,6937
 zepben/evolve/model/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/phases.py,sha256=06VmOb5-t7o6vPuyM11Uy9OLKSTSSEfdWNBnyIV8Z0g,7357
 zepben/evolve/model/resistance_reactance.py,sha256=O4Ix9qfPyV9Me_uj3JOA3UXCNO994mjratNkrENpAlg,1502
 zepben/evolve/model/busbranch/__init__.py,sha256=Z43kZuy6PMJMbDL-8XIPllgYW7_oCy9ofZuisQ1ykAA,245
-zepben/evolve/model/busbranch/bus_branch.py,sha256=AJt0a_8gKy3gzx2b1VwIBvGPvVYvR76AmRsHDq4dSng,47087
+zepben/evolve/model/busbranch/bus_branch.py,sha256=dqgCMteMo5Dd75LAQMQRltrwdTQe3PvzJ86I7XQogM4,47076
 zepben/evolve/model/cim/__init__.py,sha256=oULWHOZIcXpVDL0mPQ075LbasZvOOfJEN-vs9NDPRgg,245
 zepben/evolve/model/cim/iec61968/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61968/assetinfo/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py,sha256=cff2rPwtEEc9kXliADOsTRSJFvE4iOFYwhuG9VrzDyM,1398
 zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py,sha256=bb-fmOSyUhLm13s77WH9MIBFDaARdlRUUwVfqwAiDYU,1445
 zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py,sha256=u9w1vIxjyI7y9MEULKiGFOYSjXbuFtfNq75Ux3nZIqU,3555
 zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py,sha256=mD79R7L3g34QvIJrXhcFOKiLEM4DW7Yh9zmzheD_G_4,1877
 zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py,sha256=NK1lKM2B8cnfMmCpc4dFm2CVzIijF6Frjj3oa8xBmhM,927
+zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py,sha256=z_Sdq67hg36stoXMuA8RCwqg4js9bBxhF7EL-pcWVg4,550
 zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py,sha256=_Qgli4l-odOc-v4lJ6dJNzt034ZXL-zF9lj64wGwNio,5904
 zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py,sha256=Sc7YAzJ2CGCG21na1wdXtkSBSiUPipC3RB4AaCXi8-U,3736
 zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py,sha256=MJ-3CjqRR3LVz851qO7ETMoXRnXYgvWxu6kk7hBzf6U,860
 zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py,sha256=RjeRxug3NyoeeqVHQXxT2Y5bYt8QQHLoNkzhT6kZfKk,1287
 zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py,sha256=WxyuOYlowj7jv1G-FsKbUBKJ0I5IzA2t9rdGQ82fPtk,1015
 zepben/evolve/model/cim/iec61968/assets/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61968/assets/asset.py,sha256=f35lisRGU7DKABV8pFuzY8V3lWFUrOrlc8wJtgKAJYo,4019
@@ -109,14 +112,15 @@
 zepben/evolve/model/cim/iec61968/customers/customer.py,sha256=kUXD624TXS9NDEha1rjgIjMvT8PMJoza2duo5uQYDiY,3534
 zepben/evolve/model/cim/iec61968/customers/customer_agreement.py,sha256=nmBXk0rbm8ErmFalGfxJw_Ttwgr60fDAnfdyyfobmtc,4260
 zepben/evolve/model/cim/iec61968/customers/customer_kind.py,sha256=kpb5bdUi3DTH8vrZnec_N2o58GWUclNp5XE1zAj2jYQ,1474
 zepben/evolve/model/cim/iec61968/customers/pricing_structure.py,sha256=9Gzg3eGXF5-AUM0BQrGh2dD9aRQFUYERKxwlUIcUbCU,3336
 zepben/evolve/model/cim/iec61968/customers/tariff.py,sha256=b9V6q8sTtQSa3TmXK8c_i7H1PUJNUFTRBADS7uKujwE,763
 zepben/evolve/model/cim/iec61968/infiec61968/__init__.py,sha256=H2nCXHtt_ZNMXRpq7SAx7WEzEj0Wqom9eVCN4KyB_kM,244
 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py,sha256=H2nCXHtt_ZNMXRpq7SAx7WEzEj0Wqom9eVCN4KyB_kM,244
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py,sha256=gsVFxa_Bj0br72MaIa4qkMRcuwutpcBGQ9cdBHOSFPE,560
 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py,sha256=lR2WplhBxwfgCVyQflz0kmVrqq0OsHzNzAVDLe9gXdA,1859
 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py,sha256=_NJHZb91yrN-eQ_m9639qeHX5hJAblViY7rKhuXnfv0,1250
 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py,sha256=D1elpgov8T6IUA0VEXb-b5VFPKVu0O1MA7fxVjz8FkI,993
 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py,sha256=dsqM23VrHcG7Nm_H2eohV2FY3fzKSEvpZ58LOJJNBwQ,1098
 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py,sha256=nFdcikJb3FegBko35m1xxmjMmC3cZCaqr8ohypQJQIQ,245
 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py,sha256=wSQYWWKWEGcK7WTnTE9xznzunO-phHsxp9PKOnzmsZY,1202
 zepben/evolve/model/cim/iec61968/metering/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
@@ -156,63 +160,76 @@
 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py,sha256=og8fHISfLCaOTBzUOQgwnoWGluTh1LYwezNi1wvNkE0,5374
 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py,sha256=6eEdP1666-9qE7oyTvydC5QhJEg0S9TMiQq-WL6RkxQ,641
 zepben/evolve/model/cim/iec61970/base/meas/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61970/base/meas/control.py,sha256=yBbQ9Oxm0eVhY-aCZnrlswk0xwJj8yXe5ZuVssekBJk,963
 zepben/evolve/model/cim/iec61970/base/meas/iopoint.py,sha256=oYPZtF7oFcApvYyjfoKFW_yfuvVxyCE10XwedkdrBmo,576
 zepben/evolve/model/cim/iec61970/base/meas/measurement.py,sha256=En33kPBYFI3VMGtqsEKdH36wh31ZjqOziZFsm7ilOpw,4294
 zepben/evolve/model/cim/iec61970/base/meas/value.py,sha256=4oyA8p0zU_q5Y2ZvWTYyZUdnTGVztES3PV872BTXLX8,1753
+zepben/evolve/model/cim/iec61970/base/protection/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
+zepben/evolve/model/cim/iec61970/base/protection/current_relay.py,sha256=64KTDP4-uL7fCSDkNgT8ikVcj8CyOw5CBs0xT4fffmU,1465
+zepben/evolve/model/cim/iec61970/base/protection/protection_equipment.py,sha256=vrorBrCx-JmklbMJ7rIHcOHTV8u7GKD8Ad68UL9GilI,4390
+zepben/evolve/model/cim/iec61970/base/protection/reclose_sequence.py,sha256=OofXRx6Mi7TcGigSSmJOF_0VdtEa1zYXSxM-XXyhkYc,816
 zepben/evolve/model/cim/iec61970/base/scada/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61970/base/scada/remote_control.py,sha256=vde0kHMW9NPdnpsvjAOdzEPObmnHC7DTmosBe7OMEHQ,737
 zepben/evolve/model/cim/iec61970/base/scada/remote_point.py,sha256=24wo3YRkxMaQzdeb3eLFPZdqvanZaCsKNkufNBY9uzM,587
 zepben/evolve/model/cim/iec61970/base/scada/remote_source.py,sha256=pncg6tp9JG_0r2mFq54Nn8DF6DEYsQoJcbxYhdQSCb8,734
 zepben/evolve/model/cim/iec61970/base/wires/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py,sha256=9VmQ-knOX2yy1CtTKn0spn3uT3ixxQYLjgvag1sKj8U,2433
+zepben/evolve/model/cim/iec61970/base/wires/breaker.py,sha256=3yIPVniMxi_-gkuXr3sYGSA4Bw5FyNJzZlBXv_CbpL8,1385
 zepben/evolve/model/cim/iec61970/base/wires/connectors.py,sha256=LPl7YY--JBXjjbU85GDBJ4WrkzkW7gN4e-yXQy8VVFU,1413
+zepben/evolve/model/cim/iec61970/base/wires/disconnector.py,sha256=JiLxyuyRwGFAPhkpomXgEdIVOdXo7Vawvbc8pSByOFg,672
 zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py,sha256=IoarB8Xvd2k9C8oZ-9xj4z3plldb04qLFtkv8iQZKOo,972
 zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py,sha256=ij4feEpkVXTsavIiZZiQ43TjXUNZc0WerZeGsp6A3BY,7483
 zepben/evolve/model/cim/iec61970/base/wires/energy_source.py,sha256=GkpuLA5gCSUTdvW-fqkxbwAKAtCgKi2MX0JEb-d4QgQ,6517
 zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py,sha256=QRf_lrH-pahw1udd5RFLD22K2K_x3abrUDiz-zXtWZE,1977
+zepben/evolve/model/cim/iec61970/base/wires/fuse.py,sha256=SZ_8BLbz4z5vvp4mnSwEbG_iTgfUEgX9sZY3TScATlo,595
+zepben/evolve/model/cim/iec61970/base/wires/jumper.py,sha256=PzxemGQ2YS4h2gnk3lr1qVn-MXCiGH3ZkjF-ytUXyoY,611
 zepben/evolve/model/cim/iec61970/base/wires/line.py,sha256=trm1GyzU7eN3QXjmS1R6Mv9VbwwRkpI9mw7PEu8ltMI,492
+zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py,sha256=7lB4HR0YqckUkElrPCSOdMVbzp0a7DiIheqB2dnx68U,584
 zepben/evolve/model/cim/iec61970/base/wires/per_length.py,sha256=VrTl3pj8QAW_Vil6us9st7E1eI-k4-FeJhZeWDV_d84,1904
 zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py,sha256=BcqwbMq0r8Ly7HdVBLoyUA0creNLijKIfvzSaa_Tqhc,884
 zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py,sha256=pdj69iUtkvA-qSaMxp8TB7dez-2kMeZSJ33nEaSG0oM,9971
 zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py,sha256=97XYNYWq4OB8pi00VHAI3ucIzK5o-vPd9NnjueTEeBA,24201
+zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py,sha256=tLOxn89h2BedMfHwX_CvZ1T7G_ZDe_8nppJu32UAJxM,7168
+zepben/evolve/model/cim/iec61970/base/wires/recloser.py,sha256=qYsY9KpbSKpRO40ZSQ4B4kE9kpMP4iI0QSdI5O323gs,582
 zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py,sha256=yq_eWYHkjkjFxZ8sADBDv-XqtYwUXR9iaKS1fMhE1uU,3658
 zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py,sha256=T28hFSwfMvOfu5FHaaCc7diA-g2AxmWe9E1KlCEk7tg,1727
-zepben/evolve/model/cim/iec61970/base/wires/switch.py,sha256=MvQFlSm2d5CI_SrxmRoDqQ1OA2xnGBm6wFb3oH9D3N0,6285
+zepben/evolve/model/cim/iec61970/base/wires/switch.py,sha256=LGXCnv_MHPumP5xZHEPKubWvyIBpHgu1cMj_j-QRSwg,4955
 zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py,sha256=rdnILwNB2rbk2eh_kuJ3ZffeMR9xG_DFgC2h5z0Vbjc,2219
 zepben/evolve/model/cim/iec61970/base/wires/vector_group.py,sha256=S3pjZrMpLdimT2YTJfAgrQ3Zin93BG0A6K8Tc-R6K1s,1544
 zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py,sha256=6hShBWsMLC_TXZqZqVn2UyMKVBZE__curGTUYrkRKuY,786
 zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
 zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py,sha256=Qm3v3I2INonSvXapfBwMMAgV7nM735RXzJYhQ3en6KY,809
 zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py,sha256=AZGF-UN7X_zryAttflt94ZgYmi6_RiShHBfH790Ye98,2215
 zepben/evolve/model/cim/iec61970/infiec61970/__init__.py,sha256=gdyluJGv7VH5-tEpBgn43Qv92811qc1Xk45frJyQZms,248
 zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py,sha256=7BamRnWDlBnFA5PdijJlEc_wtQjap5cFWL8r0b1IDqw,5385
 zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py,sha256=PMtWsjKBO2q-DzHHqJcsrwIYNUmwzmOXe7zF861zfwM,7542
 zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py,sha256=IIuSzIf6RTnhO8GWTmEYaiRBVP3Grt10TB9uL4RAy6s,7636
+zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
+zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py,sha256=eQEYyQrzT6z-lSmz4vjN_rQy_4Ao7u_da6S-IuCKkYA,768
 zepben/evolve/services/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/common/__init__.py,sha256=36G32WG2TiQ9Y0iXXt9qlMB08ndzL7YRRGWnvCF3ilE,960
 zepben/evolve/services/common/base_service.py,sha256=vI0ZgThBay1ekr-6OfawHL7OqrnIB6ihBxKlwARo_Vk,17992
 zepben/evolve/services/common/base_service_comparator.py,sha256=FajIqULknyu9fqKdkV6kQe7wbsb_m7g_bqfHnecRhkg,16620
 zepben/evolve/services/common/difference.py,sha256=q-MrJgkt57YpkgK1CnxoXbgUCXHH84HPzr0Iy1S2j9s,1189
-zepben/evolve/services/common/reference_resolvers.py,sha256=8fY268WFEUowyDHEL7XZZMddxDfC4YHpbWB2XczOg0g,20310
-zepben/evolve/services/common/resolver.py,sha256=wrX5ADXe_gxyQsfEon1thSqtU_sDcOgMUut8QxJlsL8,18922
+zepben/evolve/services/common/reference_resolvers.py,sha256=h4DCZ0UHOOpMgPLyLLI5mdZE1f0Ts4OJBdTT8w-f_zY,22265
+zepben/evolve/services/common/resolver.py,sha256=zPTuYM3CEu4tDeCn7ZU7_utthKOLFOIDOZsSdc8OSC0,20018
 zepben/evolve/services/common/meta/__init__.py,sha256=Z43kZuy6PMJMbDL-8XIPllgYW7_oCy9ofZuisQ1ykAA,245
 zepben/evolve/services/common/meta/data_source.py,sha256=vbnymwi7Jg71Pa_mqX7aOhgoaQ1EygNKKpp2tvkxJYo,461
 zepben/evolve/services/common/meta/metadata_collection.py,sha256=84y5Qv7hKL4f7DSg1Yk_v-tEqcMYQywCqeK7_ogqpi0,804
 zepben/evolve/services/common/translator/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/common/translator/base_cim2proto.py,sha256=rygjaLxvKzBPEtOQxAGguZM1R_hcdMtQLLK_NM9Pspg,3395
 zepben/evolve/services/common/translator/base_proto2cim.py,sha256=ZL4u5WxmK3m1TKUD8hQ74wnSSfXovgv4JnSONRB57Ho,3994
 zepben/evolve/services/common/translator/service_differences.py,sha256=L4aivTqMeMUYwOyTff37Z0CgRgql7_JRGLhxqy3RXoY,2924
-zepben/evolve/services/common/translator/util.py,sha256=I94lEn_Mg7ujR9ihWJo9ew4v_REZA2lGIXgnsY63Oa8,1970
+zepben/evolve/services/common/translator/util.py,sha256=IRM4aLPRwUhMnx_cMZ226M-jbsa_5yiig1YMMv_Al8Y,2410
 zepben/evolve/services/customer/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/customer/customer_service_comparator.py,sha256=vBdElGq1ksEcjj1ZhBpNCfoIT2wu0z1mUIalqomp5Ss,1922
-zepben/evolve/services/customer/customers.py,sha256=By6BkySaZ5Gqh00ZkGQwCFQBLhZtpPlb3jNkXOu6BH0,501
+zepben/evolve/services/customer/customers.py,sha256=WIeP_NiW9sbZfwlcgu3exsjxxsC_ZaD4b6iSj4NmnNA,467
 zepben/evolve/services/customer/translator/__init__.py,sha256=SM-mlQwphX25z2C_RVjHGzcrJ5_01_PLyOBkcjgo-B8,1044
 zepben/evolve/services/customer/translator/customer_cim2proto.py,sha256=hd2hIcnzZGA9BJNmivGRy3W4ZkvTLBwIm5YQLBdNsRw,2760
 zepben/evolve/services/customer/translator/customer_proto2cim.py,sha256=AEadkXozPeCuPxiDIW-Mc7uMnvyXaR3YcmMTCvTytYw,3379
 zepben/evolve/services/diagram/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/diagram/diagram_service_comparator.py,sha256=jVxZ0dX01AmnArDsJgxMUFG6vwzupwI-YykB___trIE,1486
 zepben/evolve/services/diagram/diagrams.py,sha256=JTifVxdW9Fb7_IDPN2nyTFhoap4AnHu0SzAqCZUe998,4598
 zepben/evolve/services/diagram/translator/__init__.py,sha256=H3ub-XSA4dkdnaXqixbJ1tDdS1Vxq4p_YnC7LN4Rjqs,508
@@ -220,17 +237,17 @@
 zepben/evolve/services/diagram/translator/diagram_proto2cim.py,sha256=O_DE41o7OhPLyyFwqTxRcszrqrTv921xLsSR0GV62vE,2463
 zepben/evolve/services/measurement/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/measurement/measurements.py,sha256=57w12Pmyp2O_uZ_zjXA76WcbJqdrtIAR2rA3Majy8-Q,1207
 zepben/evolve/services/measurement/translator/__init__.py,sha256=Sk7Ii6qTO75bXSb-pt2AnOcEAlVwwQQ9qVSslZeZMGk,261
 zepben/evolve/services/measurement/translator/measurement_cim2proto.py,sha256=0ubggqVuZNEGs9oQDs3gfxSpqTHtuslZ3B6AIuzK-yc,1832
 zepben/evolve/services/measurement/translator/measurement_proto2cim.py,sha256=3fqGENBnGSKtdafvotnKdlujbN7jRdiViiy5SUAh1d8,1951
 zepben/evolve/services/network/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
-zepben/evolve/services/network/network_extensions.py,sha256=k1bJ02BSSy8X4Hxr81T0RpAOXoDfm7ETMKe8DJPXWnI,6278
+zepben/evolve/services/network/network_extensions.py,sha256=EqeEPaaWLGVfRI4No2erEm4V7gBu-bN0cRvwS9D4w9w,6279
 zepben/evolve/services/network/network_service.py,sha256=LN_Ejw_f3VIZAH0Z96iAIsQrY66Wa_6cAXksRHncaUc,10634
-zepben/evolve/services/network/network_service_comparator.py,sha256=eVzc0qeNB9BasbUjDE4KpbNq9Oa89ThH_Rk6YjVGIMM,37224
+zepben/evolve/services/network/network_service_comparator.py,sha256=QMlnG0BTA7iZbdjlE3LxEl9vRKihEKpa6iVbAZzyUt8,39337
 zepben/evolve/services/network/tracing/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/network/tracing/find.py,sha256=gialgfqckC5j1DsYaa76sQrtNf9H0R22zXgjvymogSQ,3654
 zepben/evolve/services/network/tracing/find_swer_equipment.py,sha256=M2K7cOSGS0qEZHt3WPOxPidUndJ7mmVT0ZDGE5UjeOo,5623
 zepben/evolve/services/network/tracing/tracing.py,sha256=CD6mE4BWJB9GtuK5yvFcQiw_zTtQhITgXQAq70D2hUg,16173
 zepben/evolve/services/network/tracing/util.py,sha256=eLfeC_jP38zkojhJsqcrZlG6w_HGKTHCxa1n9sGMr0s,3395
 zepben/evolve/services/network/tracing/connectivity/__init__.py,sha256=_CGeGWwIlS5myb1IUwG3wwAWx-Fp_VLLQV9yyl_hg6A,246
 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py,sha256=e9EddqibKjuW4rAKtwuLPm5mIb2C0HelImeebTSxV5w,775
@@ -244,16 +261,16 @@
 zepben/evolve/services/network/tracing/connectivity/phase_paths.py,sha256=THDO-ZlVSOQxoGSHJ7Whg7egBth6qu8OFyb7UaBJAN0,3872
 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py,sha256=egPsY3gZnL7j7rSa-86mQAYEOMWdOkcjdkTSCtw1pLA,9998
 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py,sha256=bWfgz_BbTT8AMam_WLnvinHotxF0oSF-Eney2hdgucY,2862
 zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py,sha256=HKrp8uNh66zNImWdFDwdAWu3asMC8XwLEFmDOSRfolI,7329
 zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py,sha256=1A4-T4huicJ3resrFYtTuSHlrFGUSUvyG4QLJvq1W8M,10412
 zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py,sha256=AxzphaAZUFR5DfZCxq7oBnwaMIHnH23Ojwcn020YzYs,583
 zepben/evolve/services/network/tracing/feeder/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
-zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py,sha256=mlXq0OOtSFyMfc3mn8WYx4PZq93_i29QN0xNf7lRf60,5977
-zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py,sha256=EdxG7OGgymkaE7fblCcbflaAsMPFyjA0YwxnCPx0LX8,5963
+zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py,sha256=UmHIu3cZYE6sVxVai9NY6txRMTbAg8joR1Mf3-52Dfw,5997
+zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py,sha256=lsBS1eEw-0E0JyGV-ii5ql8HBE-oPskEyjIarX0jOis,6053
 zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py,sha256=hYSr7fzPkX7IshyOBOexV5S9M-GOUbOnZsWK6xfU9MM,3246
 zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py,sha256=tgrBKqiugzTQGNLuoSa6ZBpRKNbGUsdrA7JUl-a8uCM,1477
 zepben/evolve/services/network/tracing/feeder/direction_status.py,sha256=J6GWPPBrn52hy__pl-tYH22UoYRUv-a31aHmn24pUsk,3990
 zepben/evolve/services/network/tracing/feeder/feeder_direction.py,sha256=JVA4IG638CAdsvC5Yo9ZE_AQ_cSjYKx3OTwEkBfdHwo,2546
 zepben/evolve/services/network/tracing/feeder/remove_direction.py,sha256=gkDquludJfepbNfj9PAwJA4xy7jv_d0GsCW6_pdmTn0,7410
 zepben/evolve/services/network/tracing/feeder/set_direction.py,sha256=zvjSrx9X1OFgB4ke744uIT2ZEMSxnVrWDyVaek4RroE,6082
 zepben/evolve/services/network/tracing/phases/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
@@ -262,26 +279,26 @@
 zepben/evolve/services/network/tracing/phases/phase_step.py,sha256=UOG_Prx4bav4-Gk9SvJgLbObj9ULCdEYgipYZo38v-s,2628
 zepben/evolve/services/network/tracing/phases/phase_step_tracker.py,sha256=7IXkTibDpMFv464hK_hjY-vffoCExR0Q47125Z8Y14U,2014
 zepben/evolve/services/network/tracing/phases/phase_trace.py,sha256=Tve85ez8gAslPAVPhH8h08iaKrmY7X0mNbXrr3RXRB8,6251
 zepben/evolve/services/network/tracing/phases/remove_phases.py,sha256=7DXCn198AmoSYv21Z2cXowb5iPgcAiimDqhCQVZtRcY,5510
 zepben/evolve/services/network/tracing/phases/set_phases.py,sha256=3FJzWW4t2ywtdLdZlFmCVlYrr2X3j3FyqbjBDkCdaGQ,12798
 zepben/evolve/services/network/tracing/traversals/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/services/network/tracing/traversals/basic_tracker.py,sha256=-c2qYBA0tuZAEEsj8GfaKSBXgFqbNqGBnSk5zfRO4fA,1642
-zepben/evolve/services/network/tracing/traversals/basic_traversal.py,sha256=STze-fNDRIjryboMjdtRKXxOzGbypIsbSKMY6o-8eYo,3036
+zepben/evolve/services/network/tracing/traversals/basic_traversal.py,sha256=GPS2KErwZYDXazDK0K1VD2yozF8dJ7OTcxU3PAb57yE,2944
 zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py,sha256=E1XXnSVX-3peCTVbiB4z539t_pU5opS5UgUIlF8HalU,6585
 zepben/evolve/services/network/tracing/traversals/queue.py,sha256=im_BL2OZoZtyI-jTatLpxSdy8Uoc18YXMMfiU_IO9UQ,5164
 zepben/evolve/services/network/tracing/traversals/tracker.py,sha256=9ujg-RnzMi8qNmwdOAM2fdAxI2LBEPF-ZGnN2uHJ7kw,1775
 zepben/evolve/services/network/tracing/traversals/traversal.py,sha256=or6bUr-U0L38QRLPulvd876j4Giv5sI4ok99yRnqZTU,7479
 zepben/evolve/services/network/tracing/tree/__init__.py,sha256=nFdcikJb3FegBko35m1xxmjMmC3cZCaqr8ohypQJQIQ,245
 zepben/evolve/services/network/tracing/tree/downstream_tree.py,sha256=p8FUwcJQ4VG3Z-9Bc1ev4vR4xYf1B_KpUDJ2B9pSxD0,4454
 zepben/evolve/services/network/tracing/tree/tree_node.py,sha256=sIj62B6Rffyz5imSdEwr-zRU-9J2NCMQP_WRbE0WVu0,1780
 zepben/evolve/services/network/tracing/tree/tree_node_tracker.py,sha256=BjZg6amIM7MfIIfrcsaswzhJ9ltu_fxtK5uKFDon130,1167
-zepben/evolve/services/network/translator/__init__.py,sha256=F-R_WzK7Z5rNv2MLgPBVBsB6hnHiQtuwCX59syA4cCA,20355
-zepben/evolve/services/network/translator/network_cim2proto.py,sha256=MS5_yyxCLe4UP-7K884rQxuG6WweETgxnTeivjMjGHU,55849
-zepben/evolve/services/network/translator/network_proto2cim.py,sha256=Nhfy3kI_W5c_gniR0_20E14ElnddxVeGqW3xfgN0tSw,67957
+zepben/evolve/services/network/translator/__init__.py,sha256=gD2FDuE9ST4gyd9T91pchFXkgtrA5Fesl_ZDe_gPflc,21206
+zepben/evolve/services/network/translator/network_cim2proto.py,sha256=ZCAD_JYDD5Meo5uMaq3yYOnBneNSLtyxjemNejxhIUw,59797
+zepben/evolve/services/network/translator/network_proto2cim.py,sha256=-xytCjgJka3IOhYwssN6IghWaoqd6HSaZ9FEi1iox5U,72669
 zepben/evolve/streaming/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/streaming/exceptions.py,sha256=YcB_uyMq6DA8hCMbAJRFwoHlq06a5_jRLd8Q7H6JZHA,419
 zepben/evolve/streaming/get/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/evolve/streaming/get/consumer.py,sha256=IjJ_YnJkPCkNumY6XamSw9wagKhJ58YGgPFeq7OCiu0,7682
 zepben/evolve/streaming/get/customer_consumer.py,sha256=mdIPk5g2sWDsnz3KqTjDxnsi8OAGQQVwaChlC_gVyy4,3424
 zepben/evolve/streaming/get/diagram_consumer.py,sha256=M0q6Ja5adiU4hpQt3l4_CuUbQ3qhRXbmbmJKC0gVICc,3253
 zepben/evolve/streaming/get/network_consumer.py,sha256=y-eLkbWk6c-nYnmrSy0dg_4_0TuACxPjRQizjnpnjLI,36489
@@ -291,12 +308,12 @@
 zepben/evolve/streaming/grpc/auth_token_plugin.py,sha256=6hQfWIwTb-BucccEurtZapfIukQuIBbwl_9nvVHTckw,801
 zepben/evolve/streaming/grpc/connect.py,sha256=2ov5B75i3tPestxA9oQGaEt5UsVt079HDI630qGZNio,8113
 zepben/evolve/streaming/grpc/grpc.py,sha256=gnvykcZbSSvyda_5iYfgljC1tDd1SB9LgXTZHMNYBuE,4020
 zepben/evolve/streaming/grpc/grpc_channel_builder.py,sha256=PZ6_xEAo_uFtv1d19Zxq7r7SxDhmAnTxaKv0JDp-QPA,4277
 zepben/evolve/testing/__init__.py,sha256=nFdcikJb3FegBko35m1xxmjMmC3cZCaqr8ohypQJQIQ,245
 zepben/evolve/testing/test_network_builder.py,sha256=4ij59LA2XuT_NaL8cjN4ZX3YU474XE6wKeF-zbZAKVI,20782
 zepben/evolve/testing/test_traversal.py,sha256=Czm2mHsAkakccYoPllGd9x6OWe7s6QuJ-bGtyzue0Yg,3238
-zepben.evolve-0.35.0b8.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
-zepben.evolve-0.35.0b8.dist-info/METADATA,sha256=YU2o7Pj_qAB5JtaBSX9ELbAiF6E6LOuVV4ftZPIlOeo,2267
-zepben.evolve-0.35.0b8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-zepben.evolve-0.35.0b8.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
-zepben.evolve-0.35.0b8.dist-info/RECORD,,
+zepben.evolve-0.35.0b9.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
+zepben.evolve-0.35.0b9.dist-info/METADATA,sha256=puzlqkLTBUWbg6-0ay_V67aB77tj-30OOMo2h6HTO3A,2267
+zepben.evolve-0.35.0b9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+zepben.evolve-0.35.0b9.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
+zepben.evolve-0.35.0b9.dist-info/RECORD,,
```

