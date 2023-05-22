# Comparing `tmp/cim_graph-0.1.20230508194360a0.tar.gz` & `tmp/cim_graph-2023.5.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_graph-0.1.20230508194360a0.tar", max compression
+gzip compressed data, was "cim_graph-2023.5.1a0.tar", max compression
```

## Comparing `cim_graph-0.1.20230508194360a0.tar` & `cim_graph-2023.5.1a0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0     5141 2023-05-08 19:43:13.638811 cim_graph-0.1.20230508194360a0/README.md
--rw-r--r--   0        0        0        0 2023-05-08 19:43:13.638811 cim_graph-0.1.20230508194360a0/cimgraph/__init__.py
--rw-r--r--   0        0        0      105 2023-05-08 19:43:13.638811 cim_graph-0.1.20230508194360a0/cimgraph/data_profile/__init__.py
--rw-r--r--   0        0        0     9401 2023-05-08 19:43:13.638811 cim_graph-0.1.20230508194360a0/cimgraph/data_profile/cimext_2022/__init__.py
--rw-r--r--   0        0        0   370766 2023-05-08 19:43:13.638811 cim_graph-0.1.20230508194360a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
--rw-r--r--   0        0        0    24601 2023-05-08 19:43:13.638811 cim_graph-0.1.20230508194360a0/cimgraph/data_profile/rc4_2021/__init__.py
--rw-r--r--   0        0        0   835023 2023-05-08 19:43:13.642811 cim_graph-0.1.20230508194360a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
--rw-r--r--   0        0        0     1063 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/__init__.py
--rw-r--r--   0        0        0      353 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/blazegraph/__init__.py
--rw-r--r--   0        0        0     9114 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/blazegraph/blazegraph.py
--rw-r--r--   0        0        0     2797 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/blazegraph/query_parsers.py
--rw-r--r--   0        0        0    10318 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/gridappsd/__init__.py
--rw-r--r--   0        0        0     4226 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/__init__.py
--rw-r--r--   0        0        0     1492 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
--rw-r--r--   0        0        0     3711 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
--rw-r--r--   0        0        0     3156 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
--rw-r--r--   0        0        0     2646 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/analog.py
--rw-r--r--   0        0        0     1483 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/asset.py
--rw-r--r--   0        0        0      885 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py
--rw-r--r--   0        0        0     1491 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
--rw-r--r--   0        0        0     3141 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
--rw-r--r--   0        0        0     3046 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/breaker.py
--rw-r--r--   0        0        0     2795 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py
--rw-r--r--   0        0        0     5482 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
--rw-r--r--   0        0        0     2350 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py
--rw-r--r--   0        0        0     2672 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py
--rw-r--r--   0        0        0     2650 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/discrete.py
--rw-r--r--   0        0        0     3155 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
--rw-r--r--   0        0        0     2176 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
--rw-r--r--   0        0        0     2799 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/fuse.py
--rw-r--r--   0        0        0      995 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
--rw-r--r--   0        0        0     3961 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
--rw-r--r--   0        0        0     2973 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
--rw-r--r--   0        0        0     2881 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
--rw-r--r--   0        0        0     3615 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
--rw-r--r--   0        0        0     2446 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
--rw-r--r--   0        0        0     2585 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
--rw-r--r--   0        0        0     2444 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
--rw-r--r--   0        0        0     2831 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
--rw-r--r--   0        0        0     3956 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
--rw-r--r--   0        0        0     2101 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
--rw-r--r--   0        0        0     3294 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
--rw-r--r--   0        0        0     4090 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
--rw-r--r--   0        0        0     2366 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
--rw-r--r--   0        0        0     4137 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
--rw-r--r--   0        0        0     2813 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/recloser.py
--rw-r--r--   0        0        0     2668 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
--rw-r--r--   0        0        0     3314 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
--rw-r--r--   0        0        0     2801 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
--rw-r--r--   0        0        0     3015 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
--rw-r--r--   0        0        0     3688 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
--rw-r--r--   0        0        0     4996 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
--rw-r--r--   0        0        0     3020 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/terminal.py
--rw-r--r--   0        0        0     2415 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
--rw-r--r--   0        0        0     4453 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
--rw-r--r--   0        0        0     2648 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
--rw-r--r--   0        0        0     3122 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
--rw-r--r--   0        0        0     3765 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
--rw-r--r--   0        0        0     2604 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
--rw-r--r--   0        0        0     2280 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py
--rw-r--r--   0        0        0     2687 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
--rw-r--r--   0        0        0      386 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/models/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/models/distributed_model.py
--rw-r--r--   0        0        0     1715 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/models/model_parsers.py
--rw-r--r--   0        0        0     3171 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/models/secondary_area.py
--rw-r--r--   0        0        0     3738 2023-05-08 19:43:13.646812 cim_graph-0.1.20230508194360a0/cimgraph/models/switch_area.py
--rw-r--r--   0        0        0      757 2023-05-08 19:44:00.212192 cim_graph-0.1.20230508194360a0/pyproject.toml
--rw-r--r--   0        0        0     5810 1970-01-01 00:00:00.000000 cim_graph-0.1.20230508194360a0/PKG-INFO
+-rw-r--r--   0        0        0     5141 2023-05-22 23:10:05.718851 cim_graph-2023.5.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 23:10:05.718851 cim_graph-2023.5.1a0/cimgraph/__init__.py
+-rw-r--r--   0        0        0      105 2023-05-22 23:10:05.718851 cim_graph-2023.5.1a0/cimgraph/data_profile/__init__.py
+-rw-r--r--   0        0        0     9401 2023-05-22 23:10:05.718851 cim_graph-2023.5.1a0/cimgraph/data_profile/cimext_2022/__init__.py
+-rw-r--r--   0        0        0   370766 2023-05-22 23:10:05.722852 cim_graph-2023.5.1a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py
+-rw-r--r--   0        0        0    24601 2023-05-22 23:10:05.722852 cim_graph-2023.5.1a0/cimgraph/data_profile/rc4_2021/__init__.py
+-rw-r--r--   0        0        0   835023 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py
+-rw-r--r--   0        0        0     1063 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/__init__.py
+-rw-r--r--   0        0        0      353 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/blazegraph/__init__.py
+-rw-r--r--   0        0        0     9114 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/blazegraph/blazegraph.py
+-rw-r--r--   0        0        0     2797 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/blazegraph/query_parsers.py
+-rw-r--r--   0        0        0    10318 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4429 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/__init__.py
+-rw-r--r--   0        0        0     1492 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py
+-rw-r--r--   0        0        0     3711 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py
+-rw-r--r--   0        0        0     3156 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py
+-rw-r--r--   0        0        0     2646 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/analog.py
+-rw-r--r--   0        0        0     1483 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/asset.py
+-rw-r--r--   0        0        0      885 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py
+-rw-r--r--   0        0        0     1491 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py
+-rw-r--r--   0        0        0     3141 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py
+-rw-r--r--   0        0        0     3046 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/breaker.py
+-rw-r--r--   0        0        0     2795 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py
+-rw-r--r--   0        0        0     5482 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py
+-rw-r--r--   0        0        0     2350 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py
+-rw-r--r--   0        0        0     2672 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py
+-rw-r--r--   0        0        0     2650 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/discrete.py
+-rw-r--r--   0        0        0     3155 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py
+-rw-r--r--   0        0        0     2176 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py
+-rw-r--r--   0        0        0     2799 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/fuse.py
+-rw-r--r--   0        0        0      995 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py
+-rw-r--r--   0        0        0     3961 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py
+-rw-r--r--   0        0        0     3392 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator_phase.py
+-rw-r--r--   0        0        0     2973 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py
+-rw-r--r--   0        0        0     2881 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py
+-rw-r--r--   0        0        0     3615 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py
+-rw-r--r--   0        0        0     2446 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py
+-rw-r--r--   0        0        0     2585 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py
+-rw-r--r--   0        0        0     2444 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py
+-rw-r--r--   0        0        0     2831 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py
+-rw-r--r--   0        0        0     3956 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py
+-rw-r--r--   0        0        0     2101 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py
+-rw-r--r--   0        0        0     3294 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py
+-rw-r--r--   0        0        0     4090 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py
+-rw-r--r--   0        0        0     2366 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py
+-rw-r--r--   0        0        0     4137 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py
+-rw-r--r--   0        0        0     2813 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/recloser.py
+-rw-r--r--   0        0        0     2668 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py
+-rw-r--r--   0        0        0     3314 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py
+-rw-r--r--   0        0        0     3132 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/shunt_compensator_phase.py
+-rw-r--r--   0        0        0     2801 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py
+-rw-r--r--   0        0        0     3015 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py
+-rw-r--r--   0        0        0     3688 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py
+-rw-r--r--   0        0        0     4996 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py
+-rw-r--r--   0        0        0     3020 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/terminal.py
+-rw-r--r--   0        0        0     2415 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py
+-rw-r--r--   0        0        0     4453 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py
+-rw-r--r--   0        0        0     2648 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py
+-rw-r--r--   0        0        0     3122 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py
+-rw-r--r--   0        0        0     3765 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py
+-rw-r--r--   0        0        0     2604 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py
+-rw-r--r--   0        0        0     2280 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py
+-rw-r--r--   0        0        0     2687 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py
+-rw-r--r--   0        0        0      386 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/models/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/models/distributed_model.py
+-rw-r--r--   0        0        0     1715 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/models/model_parsers.py
+-rw-r--r--   0        0        0     3171 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/models/secondary_area.py
+-rw-r--r--   0        0        0     3738 2023-05-22 23:10:05.726852 cim_graph-2023.5.1a0/cimgraph/models/switch_area.py
+-rw-r--r--   0        0        0      747 2023-05-22 23:10:56.947916 cim_graph-2023.5.1a0/pyproject.toml
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 cim_graph-2023.5.1a0/PKG-INFO
```

### Comparing `cim_graph-0.1.20230508194360a0/README.md` & `cim_graph-2023.5.1a0/README.md`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/data_profile/cimext_2022/__init__.py` & `cim_graph-2023.5.1a0/cimgraph/data_profile/cimext_2022/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py` & `cim_graph-2023.5.1a0/cimgraph/data_profile/cimext_2022/gridappsd_cim_profile.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/data_profile/rc4_2021/__init__.py` & `cim_graph-2023.5.1a0/cimgraph/data_profile/rc4_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py` & `cim_graph-2023.5.1a0/cimgraph/data_profile/rc4_2021/gridappsd_cim_profile_rc4_2021.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/__init__.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/blazegraph/blazegraph.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/blazegraph/blazegraph.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/blazegraph/query_parsers.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/blazegraph/query_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/gridappsd/__init__.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/__init__.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #e
 import cimgraph.loaders.sparql.rc4_2021.energy_consumer as EnergyConsumerSPARQL
 import cimgraph.loaders.sparql.rc4_2021.energy_consumer_phase as EnergyConsumerPhaseSPARQL
 #f
 import cimgraph.loaders.sparql.rc4_2021.fuse as FuseSPARQL
 #l
 import cimgraph.loaders.sparql.rc4_2021.linear_shunt_compensator as LinearShuntCompensatorSPARQL
+import cimgraph.loaders.sparql.rc4_2021.linear_shunt_compensator_phase as LinearShuntCompensatorPhaseSPARQL
 import cimgraph.loaders.sparql.rc4_2021.load_break_switch as LoadBreakSwitchSPARQL
 #n
 import cimgraph.loaders.sparql.rc4_2021.no_load_test as NoLoadTestSPARQL
 #o
 import cimgraph.loaders.sparql.rc4_2021.overhead_wire_info as OverheadWireInfoSPARQL
 #p
 import cimgraph.loaders.sparql.rc4_2021.per_length_phase_impedance as PerLengthPhaseImpedanceSPARQL
@@ -42,14 +43,15 @@
 import cimgraph.loaders.sparql.rc4_2021.power_transformer_info as PowerTransformerInfoSPARQL
 #r
 import cimgraph.loaders.sparql.rc4_2021.ratio_tap_changer as RatioTapChangerSPARQL
 import cimgraph.loaders.sparql.rc4_2021.recloser as RecloserSPARQL
 #s
 import cimgraph.loaders.sparql.rc4_2021.sectionaliser as SectionaliserSPARQL
 import cimgraph.loaders.sparql.rc4_2021.short_circuit_test as ShortCircuitTestSPARQL
+import cimgraph.loaders.sparql.rc4_2021.shunt_compensator_phase as ShuntCompensatorPhaseSPARQL
 import cimgraph.loaders.sparql.rc4_2021.switch_phase as SwitchPhaseSPARQL
 import cimgraph.loaders.sparql.rc4_2021.synchronous_machine as SynchronousMachineSPARQL
 #t
 import cimgraph.loaders.sparql.rc4_2021.tap_changer_control as TapChangerControlSPARQL
 import cimgraph.loaders.sparql.rc4_2021.tape_shield_cable_info as TapeShieldCableInfoSPARQL
 import cimgraph.loaders.sparql.rc4_2021.terminal as TerminalSPARQL
 import cimgraph.loaders.sparql.rc4_2021.transformer_core_admittance as TransformerCoreAdmittanceSPARQL
```

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ac_dc_terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ac_line_segment_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/analog.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/analog.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/asset.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/asset.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/asset_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/base_voltage.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/battery_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/breaker.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/breaker.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/concentric_neutral_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/disconnector.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/discrete.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/discrete.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/energy_consumer_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/fuse.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/fuse.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/get_class_type.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/no_load_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/overhead_wire_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/per_length_phase_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/per_length_sequence_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/phase_impedance_data.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/photovoltaic_unit.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_electronics_connection_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_transformer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/power_transformer_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/recloser.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/recloser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/sectionaliser.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/short_circuit_test.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/switch_phase.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/tape_shield_cable_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/terminal.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/terminal.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_core_admittance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_end_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_mesh_impedance.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_end.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/transformer_tank_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/wire_position.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py` & `cim_graph-2023.5.1a0/cimgraph/loaders/sparql/rc4_2021/wire_spacing_info.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/models/distributed_model.py` & `cim_graph-2023.5.1a0/cimgraph/models/distributed_model.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/models/model_parsers.py` & `cim_graph-2023.5.1a0/cimgraph/models/model_parsers.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/models/secondary_area.py` & `cim_graph-2023.5.1a0/cimgraph/models/secondary_area.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/cimgraph/models/switch_area.py` & `cim_graph-2023.5.1a0/cimgraph/models/switch_area.py`

 * *Files identical despite different names*

### Comparing `cim_graph-0.1.20230508194360a0/pyproject.toml` & `cim_graph-2023.5.1a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cim-graph"
-version = "0.1.20230508194360a0"
+version = "2023.5.1a0"
 description = "CIM Graph"
 authors = ["C. Allwardt <3979063+craig8@users.noreply.github.com>"]
 packages = [
     { include = "cimgraph" }
 ]
 readme = "README.md"
```

### Comparing `cim_graph-0.1.20230508194360a0/PKG-INFO` & `cim_graph-2023.5.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-graph
-Version: 0.1.20230508194360a0
+Version: 2023.5.1a0
 Summary: CIM Graph
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

