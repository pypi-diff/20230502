# Comparing `tmp/ragraph-1.17.0.tar.gz` & `tmp/ragraph-1.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragraph-1.17.0.tar", max compression
+gzip compressed data, was "ragraph-1.17.1.tar", max compression
```

## Comparing `ragraph-1.17.0.tar` & `ragraph-1.17.1.tar`

### file list

```diff
@@ -1,136 +1,135 @@
--rw-r--r--   0        0        0    35400 2023-02-27 11:09:53.858232 ragraph-1.17.0/LICENSE.rst
--rw-r--r--   0        0        0     1850 2023-02-27 11:09:53.858232 ragraph-1.17.0/README.rst
--rw-r--r--   0        0        0     2128 2023-02-27 11:09:53.862233 ragraph-1.17.0/pyproject.toml
--rw-r--r--   0        0        0       72 2023-02-27 11:09:53.862233 ragraph-1.17.0/ragraph/__init__.py
--rw-r--r--   0        0        0      100 2023-02-27 11:09:53.862233 ragraph-1.17.0/ragraph/analysis/__init__.py
--rw-r--r--   0        0        0    20082 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/_classes.py
--rw-r--r--   0        0        0     7917 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/_utils.py
--rw-r--r--   0        0        0     1142 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/bus/__init__.py
--rw-r--r--   0        0        0     3743 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/bus/_gamma.py
--rw-r--r--   0        0        0     1613 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/cluster/__init__.py
--rw-r--r--   0        0        0    13797 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/cluster/_markov.py
--rw-r--r--   0        0        0     3444 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/cluster/_tarjan.py
--rw-r--r--   0        0        0      503 2023-02-27 11:09:53.863233 ragraph-1.17.0/ragraph/analysis/comparison/__init__.py
--rw-r--r--   0        0        0     5580 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/comparison/_delta.py
--rw-r--r--   0        0        0     4708 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/comparison/_sigma.py
--rw-r--r--   0        0        0     1752 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/comparison/utils.py
--rw-r--r--   0        0        0    19910 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/compatibility/__init__.py
--rw-r--r--   0        0        0     2735 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/compatibility/bdd.py
--rw-r--r--   0        0        0     1227 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/heuristics/__init__.py
--rw-r--r--   0        0        0     3368 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/heuristics/_johnson.py
--rw-r--r--   0        0        0     5187 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/heuristics/_markov_gamma.py
--rw-r--r--   0        0        0     1787 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/__init__.py
--rw-r--r--   0        0        0    11025 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/_axis.py
--rw-r--r--   0        0        0     5227 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/_genetic.py
--rw-r--r--   0        0        0     3024 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/_markov.py
--rw-r--r--   0        0        0      840 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/_name.py
--rw-r--r--   0        0        0     3773 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/_scc_tearing.py
--rw-r--r--   0        0        0     1713 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/_tarjan.py
--rw-r--r--   0        0        0     7133 2023-02-27 11:09:53.864233 ragraph-1.17.0/ragraph/analysis/sequence/metrics.py
--rw-r--r--   0        0        0     5256 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/analysis/sequence/utils.py
--rw-r--r--   0        0        0     1336 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/analysis/similarity/__init__.py
--rw-r--r--   0        0        0     3036 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/analysis/similarity/_jaccard.py
--rw-r--r--   0        0        0     9582 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/analysis/similarity/_similarity.py
--rw-r--r--   0        0        0     1830 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/analysis/similarity/utils.py
--rw-r--r--   0        0        0     9979 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/colors/__init__.py
--rw-r--r--   0        0        0     5320 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/colors/cubehelix.py
--rw-r--r--   0        0        0      774 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/colors/utils.py
--rw-r--r--   0        0        0     1663 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/datasets/__init__.py
--rw-r--r--   0        0        0      673 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/datasets/aircraft_engine/__init__.py
--rw-r--r--   0        0        0    28938 2023-02-27 11:09:53.865233 ragraph-1.17.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
--rw-r--r--   0        0        0      977 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
--rw-r--r--   0        0        0     1035 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_integral/__init__.py
--rw-r--r--   0        0        0     1364 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
--rw-r--r--   0        0        0      352 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
--rw-r--r--   0        0        0     1048 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_mix/__init__.py
--rw-r--r--   0        0        0     2264 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
--rw-r--r--   0        0        0      352 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
--rw-r--r--   0        0        0     1043 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_modular/__init__.py
--rw-r--r--   0        0        0     2722 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
--rw-r--r--   0        0        0      351 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
--rw-r--r--   0        0        0      813 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/climate_control/__init__.py
--rw-r--r--   0        0        0     5778 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/climate_control/climate_control_edges.csv
--rw-r--r--   0        0        0      632 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/climate_control/climate_control_nodes.csv
--rw-r--r--   0        0        0      374 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/climate_control_mg/__init__.py
--rw-r--r--   0        0        0     5778 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
--rw-r--r--   0        0        0     1441 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
--rw-r--r--   0        0        0      460 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/compatibility/__init__.py
--rw-r--r--   0        0        0      564 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/compatibility/compatibility_edges.csv
--rw-r--r--   0        0        0       83 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/compatibility/compatibility_nodes.csv
--rw-r--r--   0        0        0      431 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/design/__init__.py
--rw-r--r--   0        0        0      872 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/design/design_edges.csv
--rw-r--r--   0        0        0      384 2023-02-27 11:09:53.866233 ragraph-1.17.0/ragraph/datasets/design/design_nodes.csv
--rw-r--r--   0        0        0       57 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/eefde_lock/__init__.py
--rw-r--r--   0        0        0    24347 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/eefde_lock/eefde_lock_edges.csv
--rw-r--r--   0        0        0     1047 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv
--rw-r--r--   0        0        0      998 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/elevator175/__init__.py
--rw-r--r--   0        0        0   103961 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/elevator175/elevator175_edges.csv
--rw-r--r--   0        0        0     7255 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/elevator175/elevator175_nodes.csv
--rw-r--r--   0        0        0      995 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/elevator45/__init__.py
--rw-r--r--   0        0        0    29033 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/elevator45/elevator45_edges.csv
--rw-r--r--   0        0        0     1887 2023-02-27 11:09:53.867233 ragraph-1.17.0/ragraph/datasets/elevator45/elevator45_nodes.csv
--rw-r--r--   0        0        0     1148 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/esl/__init__.py
--rw-r--r--   0        0        0       75 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/esl/pump/__init__.py
--rw-r--r--   0        0        0     3523 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/esl/pump/pump.esl
--rw-r--r--   0        0        0     1868 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/ford_hood/__init__.py
--rw-r--r--   0        0        0    30483 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/ford_hood/ford_hood_edges.csv
--rw-r--r--   0        0        0     3339 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv
--rw-r--r--   0        0        0     1461 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/kodak3d/__init__.py
--rw-r--r--   0        0        0     6660 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/kodak3d/kodak3d_edges.csv
--rw-r--r--   0        0        0     1134 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv
--rw-r--r--   0        0        0      216 2023-02-27 11:09:53.868233 ragraph-1.17.0/ragraph/datasets/ledsip/__init__.py
--rw-r--r--   0        0        0   210027 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/ledsip/ledsip_edges.csv
--rw-r--r--   0        0        0    50840 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/ledsip/ledsip_nodes.csv
--rw-r--r--   0        0        0       74 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/localbus/__init__.py
--rw-r--r--   0        0        0      723 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/localbus/localbus_edges.csv
--rw-r--r--   0        0        0       27 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/localbus/localbus_nodes.csv
--rw-r--r--   0        0        0       76 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/overlap/__init__.py
--rw-r--r--   0        0        0      149 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/overlap/overlap_edges.csv
--rw-r--r--   0        0        0       15 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/overlap/overlap_nodes.csv
--rw-r--r--   0        0        0     3167 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/pathfinder/__init__.py
--rw-r--r--   0        0        0    17741 2023-02-27 11:09:53.869233 ragraph-1.17.0/ragraph/datasets/pathfinder/pathfinder_edges.csv
--rw-r--r--   0        0        0     1084 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv
--rw-r--r--   0        0        0      307 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/shaja8/__init__.py
--rw-r--r--   0        0        0      243 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/shaja8/shaja8_edges.csv
--rw-r--r--   0        0        0       21 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/shaja8/shaja8_nodes.csv
--rw-r--r--   0        0        0      224 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/similarity/__init__.py
--rw-r--r--   0        0        0      872 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/similarity/similarity_edges.csv
--rw-r--r--   0        0        0      360 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/similarity/similarity_nodes.csv
--rw-r--r--   0        0        0      253 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/tarjans8/__init__.py
--rw-r--r--   0        0        0      199 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/tarjans8/tarjans8_edges.csv
--rw-r--r--   0        0        0       21 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/tarjans8/tarjans8_nodes.csv
--rw-r--r--   0        0        0     1493 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/ucav/__init__.py
--rw-r--r--   0        0        0     5183 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/ucav/ucav_edges.csv
--rw-r--r--   0        0        0     1141 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/datasets/ucav/ucav_nodes.csv
--rw-r--r--   0        0        0     4372 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/edge.py
--rw-r--r--   0        0        0    23138 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/generic.py
--rw-r--r--   0        0        0    40199 2023-02-27 11:09:53.870233 ragraph-1.17.0/ragraph/graph.py
--rw-r--r--   0        0        0       80 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/__init__.py
--rw-r--r--   0        0        0    11987 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/archimate/__init__.py
--rw-r--r--   0        0        0    48350 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/archimate/archimate3_Model.xsd
--rw-r--r--   0        0        0      461 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/archimate/bare.xml
--rw-r--r--   0        0        0     8836 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/archimate/xml.xsd
--rw-r--r--   0        0        0     6759 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/canopy.py
--rw-r--r--   0        0        0    13974 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/csv.py
--rw-r--r--   0        0        0      243 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/esl.py
--rw-r--r--   0        0        0     4146 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/json.py
--rw-r--r--   0        0        0     5177 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/matrix.py
--rw-r--r--   0        0        0     1819 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/xml/XMI-Canonical.xsd
--rw-r--r--   0        0        0     9279 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/xml/__init__.py
--rw-r--r--   0        0        0      358 2023-02-27 11:09:53.871233 ragraph-1.17.0/ragraph/io/xml/bare.xml
--rw-r--r--   0        0        0     4332 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/io/xml/ragraph.xsd
--rw-r--r--   0        0        0     1276 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/io/yaml.py
--rw-r--r--   0        0        0     7922 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/node.py
--rw-r--r--   0        0        0     4337 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/__init__.py
--rw-r--r--   0        0        0      507 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/components/__init__.py
--rw-r--r--   0        0        0     1179 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/components/blank.py
--rw-r--r--   0        0        0     3878 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/components/labels.py
--rw-r--r--   0        0        0     9361 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/components/legend.py
--rw-r--r--   0        0        0    20900 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/components/piemap.py
--rw-r--r--   0        0        0     6829 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/components/tree.py
--rw-r--r--   0        0        0    28095 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/generic.py
--rw-r--r--   0        0        0     9817 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/svg.py
--rw-r--r--   0        0        0     9316 2023-02-27 11:09:53.872233 ragraph-1.17.0/ragraph/plot/utils.py
--rw-r--r--   0        0        0     3140 2023-02-27 11:09:53.873233 ragraph-1.17.0/ragraph/utils.py
--rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 ragraph-1.17.0/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 ragraph-1.17.0/PKG-INFO
+-rw-r--r--   0        0        0    35400 2023-05-02 10:06:24.073175 ragraph-1.17.1/LICENSE.rst
+-rw-r--r--   0        0        0     1781 2023-05-02 10:06:24.073175 ragraph-1.17.1/README.rst
+-rw-r--r--   0        0        0     2357 2023-05-02 10:06:24.076176 ragraph-1.17.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-05-02 10:06:24.076176 ragraph-1.17.1/ragraph/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-02 10:06:24.076176 ragraph-1.17.1/ragraph/analysis/__init__.py
+-rw-r--r--   0        0        0    19876 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/_classes.py
+-rw-r--r--   0        0        0     7901 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/_utils.py
+-rw-r--r--   0        0        0     1142 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/bus/__init__.py
+-rw-r--r--   0        0        0     3743 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/bus/_gamma.py
+-rw-r--r--   0        0        0     1613 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/cluster/__init__.py
+-rw-r--r--   0        0        0    13777 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/cluster/_markov.py
+-rw-r--r--   0        0        0     3438 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/cluster/_tarjan.py
+-rw-r--r--   0        0        0      503 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/__init__.py
+-rw-r--r--   0        0        0     5548 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/_delta.py
+-rw-r--r--   0        0        0     4722 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/_sigma.py
+-rw-r--r--   0        0        0     1706 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/comparison/utils.py
+-rw-r--r--   0        0        0    19484 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/compatibility/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-02 10:06:24.077175 ragraph-1.17.1/ragraph/analysis/compatibility/bdd.py
+-rw-r--r--   0        0        0     1227 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/heuristics/__init__.py
+-rw-r--r--   0        0        0     3368 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/heuristics/_johnson.py
+-rw-r--r--   0        0        0     5157 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/heuristics/_markov_gamma.py
+-rw-r--r--   0        0        0     1787 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/__init__.py
+-rw-r--r--   0        0        0    10956 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_axis.py
+-rw-r--r--   0        0        0     5226 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_genetic.py
+-rw-r--r--   0        0        0     3010 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_markov.py
+-rw-r--r--   0        0        0      840 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_name.py
+-rw-r--r--   0        0        0     3750 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_scc_tearing.py
+-rw-r--r--   0        0        0     1713 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/_tarjan.py
+-rw-r--r--   0        0        0     7133 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/metrics.py
+-rw-r--r--   0        0        0     5256 2023-05-02 10:06:24.078176 ragraph-1.17.1/ragraph/analysis/sequence/utils.py
+-rw-r--r--   0        0        0     1336 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/__init__.py
+-rw-r--r--   0        0        0     3036 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/_jaccard.py
+-rw-r--r--   0        0        0     9582 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/_similarity.py
+-rw-r--r--   0        0        0     1824 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/analysis/similarity/utils.py
+-rw-r--r--   0        0        0     9963 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/colors/__init__.py
+-rw-r--r--   0        0        0     5320 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/colors/cubehelix.py
+-rw-r--r--   0        0        0      774 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/colors/utils.py
+-rw-r--r--   0        0        0     1663 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/aircraft_engine/__init__.py
+-rw-r--r--   0        0        0    28938 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
+-rw-r--r--   0        0        0      977 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
+-rw-r--r--   0        0        0     1035 2023-05-02 10:06:24.079176 ragraph-1.17.1/ragraph/datasets/architecture_integral/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
+-rw-r--r--   0        0        0      352 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
+-rw-r--r--   0        0        0     1048 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_mix/__init__.py
+-rw-r--r--   0        0        0     2264 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
+-rw-r--r--   0        0        0      352 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
+-rw-r--r--   0        0        0     1043 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_modular/__init__.py
+-rw-r--r--   0        0        0     2722 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
+-rw-r--r--   0        0        0      351 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
+-rw-r--r--   0        0        0      813 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control/__init__.py
+-rw-r--r--   0        0        0     5778 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_edges.csv
+-rw-r--r--   0        0        0      632 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_nodes.csv
+-rw-r--r--   0        0        0      374 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control_mg/__init__.py
+-rw-r--r--   0        0        0     5778 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
+-rw-r--r--   0        0        0     1441 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
+-rw-r--r--   0        0        0      460 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/compatibility/__init__.py
+-rw-r--r--   0        0        0      564 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/compatibility/compatibility_edges.csv
+-rw-r--r--   0        0        0       83 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/compatibility/compatibility_nodes.csv
+-rw-r--r--   0        0        0      431 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/design/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/design/design_edges.csv
+-rw-r--r--   0        0        0      384 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/design/design_nodes.csv
+-rw-r--r--   0        0        0       57 2023-05-02 10:06:24.080176 ragraph-1.17.1/ragraph/datasets/eefde_lock/__init__.py
+-rw-r--r--   0        0        0    24347 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_edges.csv
+-rw-r--r--   0        0        0     1047 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv
+-rw-r--r--   0        0        0      998 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator175/__init__.py
+-rw-r--r--   0        0        0   103961 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_edges.csv
+-rw-r--r--   0        0        0     7255 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_nodes.csv
+-rw-r--r--   0        0        0      995 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator45/__init__.py
+-rw-r--r--   0        0        0    29033 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_edges.csv
+-rw-r--r--   0        0        0     1887 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_nodes.csv
+-rw-r--r--   0        0        0     1148 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/esl/__init__.py
+-rw-r--r--   0        0        0       75 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/esl/pump/__init__.py
+-rw-r--r--   0        0        0     3523 2023-05-02 10:06:24.081176 ragraph-1.17.1/ragraph/datasets/esl/pump/pump.esl
+-rw-r--r--   0        0        0     1868 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ford_hood/__init__.py
+-rw-r--r--   0        0        0    30483 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_edges.csv
+-rw-r--r--   0        0        0     3339 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_nodes.csv
+-rw-r--r--   0        0        0     1461 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/kodak3d/__init__.py
+-rw-r--r--   0        0        0     6660 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_edges.csv
+-rw-r--r--   0        0        0     1134 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_nodes.csv
+-rw-r--r--   0        0        0      216 2023-05-02 10:06:24.082176 ragraph-1.17.1/ragraph/datasets/ledsip/__init__.py
+-rw-r--r--   0        0        0   210027 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_edges.csv
+-rw-r--r--   0        0        0    50840 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_nodes.csv
+-rw-r--r--   0        0        0       74 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/localbus/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/localbus/localbus_edges.csv
+-rw-r--r--   0        0        0       27 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/localbus/localbus_nodes.csv
+-rw-r--r--   0        0        0       76 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/overlap/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/overlap/overlap_edges.csv
+-rw-r--r--   0        0        0       15 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/overlap/overlap_nodes.csv
+-rw-r--r--   0        0        0     3167 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/pathfinder/__init__.py
+-rw-r--r--   0        0        0    17741 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_edges.csv
+-rw-r--r--   0        0        0     1084 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_nodes.csv
+-rw-r--r--   0        0        0      307 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/shaja8/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/shaja8/shaja8_edges.csv
+-rw-r--r--   0        0        0       21 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/shaja8/shaja8_nodes.csv
+-rw-r--r--   0        0        0      224 2023-05-02 10:06:24.083176 ragraph-1.17.1/ragraph/datasets/similarity/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/similarity/similarity_edges.csv
+-rw-r--r--   0        0        0      360 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/similarity/similarity_nodes.csv
+-rw-r--r--   0        0        0      253 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/tarjans8/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/tarjans8/tarjans8_edges.csv
+-rw-r--r--   0        0        0       21 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/tarjans8/tarjans8_nodes.csv
+-rw-r--r--   0        0        0     1493 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/ucav/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/ucav/ucav_edges.csv
+-rw-r--r--   0        0        0     1141 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/datasets/ucav/ucav_nodes.csv
+-rw-r--r--   0        0        0     4372 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/edge.py
+-rw-r--r--   0        0        0    23032 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/generic.py
+-rw-r--r--   0        0        0    39432 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/graph.py
+-rw-r--r--   0        0        0       80 2023-05-02 10:06:24.084176 ragraph-1.17.1/ragraph/io/__init__.py
+-rw-r--r--   0        0        0    11755 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/__init__.py
+-rw-r--r--   0        0        0    48350 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/archimate3_Model.xsd
+-rw-r--r--   0        0        0      461 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/bare.xml
+-rw-r--r--   0        0        0     8836 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/archimate/xml.xsd
+-rw-r--r--   0        0        0     6745 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/canopy.py
+-rw-r--r--   0        0        0    13730 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/csv.py
+-rw-r--r--   0        0        0      229 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/esl.py
+-rw-r--r--   0        0        0     4146 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/json.py
+-rw-r--r--   0        0        0     5081 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/matrix.py
+-rw-r--r--   0        0        0     1819 2023-05-02 10:06:24.085176 ragraph-1.17.1/ragraph/io/xml/XMI-Canonical.xsd
+-rw-r--r--   0        0        0     9246 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/xml/__init__.py
+-rw-r--r--   0        0        0      358 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/xml/bare.xml
+-rw-r--r--   0        0        0     4332 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/xml/ragraph.xsd
+-rw-r--r--   0        0        0     1270 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/io/yaml.py
+-rw-r--r--   0        0        0     7862 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/node.py
+-rw-r--r--   0        0        0     4325 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/__init__.py
+-rw-r--r--   0        0        0      507 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/__init__.py
+-rw-r--r--   0        0        0     1178 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/blank.py
+-rw-r--r--   0        0        0     3822 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/labels.py
+-rw-r--r--   0        0        0     9115 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/legend.py
+-rw-r--r--   0        0        0    20779 2023-05-02 10:06:24.086176 ragraph-1.17.1/ragraph/plot/components/piemap.py
+-rw-r--r--   0        0        0     6765 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/components/tree.py
+-rw-r--r--   0        0        0    28046 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/generic.py
+-rw-r--r--   0        0        0     9811 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/svg.py
+-rw-r--r--   0        0        0     9274 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/plot/utils.py
+-rw-r--r--   0        0        0     3088 2023-05-02 10:06:24.087176 ragraph-1.17.1/ragraph/utils.py
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 ragraph-1.17.1/PKG-INFO
```

### Comparing `ragraph-1.17.0/LICENSE.rst` & `ragraph-1.17.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/README.rst` & `ragraph-1.17.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -14,52 +14,50 @@
 **********
 Quickstart
 **********
 
 Installation
 ============
 
-RaGraph can be installed using ``pip install ragraph`` for any Python version >=3.9. Or,
-for Poetry managed projects, use ``poetry add ragraph`` to add it as a dependency.
+RaGraph can be installed using ``pip install ragraph[all]`` for any Python version >=3.9. Or,
+for Poetry managed projects, use ``poetry add ragraph -E all`` to add it as a dependency.
 
 
 Using RaGraph
 =============
 
 RaGraph's primary use is working with Graph objects that contain Nodes and Eges between
 Nodes. See the `usage documentation <https://ragraph.ratio-case.nl/usage/index.html>`_
 for more info!
 
-
 ***************
 Developer guide
 ***************
 
 Python packaging information
 ============================
 
 This project is packaged using `poetry <https://python-poetry.org/>`_. Packaging
 information as well as dependencies are stored in `pyproject.toml <./pyproject.toml>`_.
 
-Installing the project and its development dependencies can be done using ``poetry install``.
-
-
-Invoke tasks
-============
-
-Most elemental maintenance tasks can be accomplished using
-[Invoke](https://www.pyinvoke.org/). After installing using ``poetry install`` and
-enabling the environment using ``poetry shell``, you can run all tasks using ``inv
-[taskname]`` or ``invoke [taskname]``. E.g. ``inv docs`` builds the documentation.
-
+Installing the project and its development dependencies can be done using ``poetry install -E all``.
 
 Versioning
 ==========
 
 This project uses `semantic versioning <https://semver.org>`_. Version increments are
 checked using `Raver <https://raver.ratio-case.nl>`_.
 
-
 Changelog
 =========
 
-Changelog format as described by https://keepachangelog.com/ has been adopted.
+Changelog format as described by https://keepachangelog.com/ has been adopted and can be reviewed `on this page <https://ragraph.ratio-case.nl/changelog.html>`.
+
+Tests
+=====
+
+Tests can be run using ``poetry run pytest``.
+
+Linting
+=======
+
+Linting config is included in `pyproject.toml <./pyproject.toml>`_ for both Black and Ruff.
```

### Comparing `ragraph-1.17.0/pyproject.toml` & `ragraph-1.17.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ragraph"
-version = "1.17.0"
+version = "1.17.1"
 description = "Ratio graph handling in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://ragraph.ratio-case.nl"
 readme = "README.rst"
-repository = "https://gitlab.com/ratio-case/python/ragraph"
-homepage = "https://gitlab.com/ratio-case/python/ragraph"
+repository = "https://gitlab.com/ratio-case-os/python/ragraph"
+homepage = "https://ragraph.ratio-case.nl"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dd = { version = "^0.5.7" }
 lxml = { version = "^4.8.0" }
 numpy = { version = "^1.22.3" }
 plotly = { version = "^5.7.0" }
@@ -25,34 +25,40 @@
 ratio-genetic-py = "^0.3.0"
 
 [tool.poetry.extras]
 esl = ["raesl"]
 plot = ["kaleido"]
 all = ["kaleido", "raesl"]
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.lint.dependencies]
 black = "*"
-invoke = "^1.7.1"
+raver = { version = "^3.0.1" }
+ruff = "^0.0.261"
+
+[tool.poetry.group.experiment.dependencies]
 jupyterlab = "^3"
 pandas = "^1.4.3"
-pydata-sphinx-theme = { version = "*" }
+
+[tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov = "*"
 pytest-doctestplus = "*"
+
+[tool.poetry.group.docs.dependencies]
+pydata-sphinx-theme = { version = "*" }
 pygments-csv-lexer = { version = "*" }
-raver = { version = "^3.0.1"}
 Sphinx = { version = "*" }
 sphinx-autoapi = { version = "*" }
 sphinx-copybutton = { version = "*" }
 sphinx-prompt = { version = "*" }
 sphinxcontrib-bibtex = { version = "*" }
 sphinxemoji = { version = "*" }
 
 [tool.black]
-line-length = 88
+line-length = 100
 target-version = ["py39"]
 
 [tool.pytest.ini_options]
 addopts = "-s --cov --cov-report xml:./.pytest_cache/coverage.xml --cov-report term-missing --doctest-plus --doctest-rst --basetemp ./tests/.temp"
 testpaths = ["docs", "tests"]
 markers = ["slow"]
 
@@ -72,9 +78,17 @@
 ]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 
 [tool.raver]
-ref = "origin/master"
+ref = "origin/main"
 changelog = "./docs/source/changelog.rst"
+
+[tool.ruff]
+line-length = 100
+select = [
+  "E",   # pycodestyle
+  "F",   # pyflakes
+]
+target-version = "py39"
```

### Comparing `ragraph-1.17.0/ragraph/analysis/_classes.py` & `ragraph-1.17.1/ragraph/analysis/_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,15 @@
     def __call__(self, value: Optional[List[str]] = None) -> List[Node]:
         if self.graph is None:
             raise ValueError("Graph must be set before cast is possible.")
         cast = NodeCast(self.graph)
         if value is None:
             root = cast(self.root)
             leafs = (
-                self.graph.leafs
-                if root is None
-                else [n for n in root.descendant_gen if n.is_leaf]
+                self.graph.leafs if root is None else [n for n in root.descendant_gen if n.is_leaf]
             )
         else:
             leafs = [n for n in (cast(leaf) for leaf in value) if n is not None]
         return leafs
 
 
 class MethodCast(Cast):
@@ -192,17 +190,15 @@
                 value = self.cast(value)
             except Exception:
                 raise ValueError(
                     f"Error while casting {self.name} value '{value}' using "
                     f"'{self.cast}' into a '{self.type}'."
                 )
         if self.enum is not None and value not in self.enum:
-            raise ValueError(
-                f"Value '{value}' is not allowed, try one of '{self.enum}'."
-            )
+            raise ValueError(f"Value '{value}' is not allowed, try one of '{self.enum}'.")
         if self.lower is not None:
             assert value > self.lower
         if self.upper is not None:
             assert value < self.upper
         return value
 
 
@@ -356,17 +352,15 @@
                 + f"function has '{sig.parameters.keys()}'. Difference: '{diff}'."
             )
 
         for pname, param in self.parameters.items():
             try:
                 f_param = sig.parameters[pname]
             except KeyError:
-                raise ValueError(
-                    f"Parameter {pname} is missing in the signature of '{func}'."
-                )
+                raise ValueError(f"Parameter {pname} is missing in the signature of '{func}'.")
 
             # Inherit default kwarg values.
             func.__annotations__[pname] = param.type
             if f_param.default != inspect._empty:
                 param.default = f_param.default
 
     def _apply_docstring(self, func: Callable):
@@ -407,16 +401,15 @@
     def log(self, msg: str, level: int = DEBUG):
         """Dispatch a logging message."""
         logger.log(level, f"{self.name}: \n{msg}\n")
 
 
 class BusAnalysis(Analysis):
     _default_parameters = {
-        p.name: p
-        for p in [graph, root, leafs, inherit, loops, edge_weights, names, safe]
+        p.name: p for p in [graph, root, leafs, inherit, loops, edge_weights, names, safe]
     }
     _returns = [
         "Detected bus nodes (or names thereof).",
         "Remaining nonbus nodes (or names thereof).",
     ]
 
     def wrap(self, func: Callable) -> Callable:
@@ -440,16 +433,15 @@
             leafs = kw["leafs"]
             if len(leafs) < 3:
                 self.log(f"Trivial case, too little nodes {len(leafs)} < 3.")
                 bus_leafs, nonbus_leafs = [], leafs
             # Nontrivial case, need to execute:
             else:
                 self.log(
-                    "Applying bus analysis to leafs "
-                    + f"'{[n.name for n in kw['leafs']]}'..."
+                    "Applying bus analysis to leafs " + f"'{[n.name for n in kw['leafs']]}'..."
                 )
                 bus_leafs, nonbus_leafs = func(**kw)
 
             # Postprocess results.
             bus_names = [n.name for n in bus_leafs]
             nonbus_names = [n.name for n in nonbus_leafs]
             self.log(f"BUS:    {bus_names}\nNONBUS: {nonbus_names}")
@@ -486,17 +478,15 @@
             if kw.get("safe", True):
                 self._parse_parameters(kw)
 
             # Create a deepcopy and update all nodal arguments to the new nodes.
             if not kw["inplace"]:
                 kw["graph"] = deepcopy(kw["graph"])
                 kw["leafs"] = [kw["graph"].node_dict[n.name] for n in kw["leafs"]]
-                kw["root"] = (
-                    kw["graph"].node_dict[kw["root"].name] if kw.get("root") else None
-                )
+                kw["root"] = kw["graph"].node_dict[kw["root"].name] if kw.get("root") else None
 
             # Trivial cases where there is nothing to cluster.
             if len(kw["leafs"]) < 2:
                 self.log("Trivial case, less than 2 nodes provided.")
                 graph = kw["graph"]
                 clusters = kw["leafs"]
 
@@ -508,17 +498,15 @@
                 # Cut leafs loose, but preserve root(s) if set.
                 for leaf in kw["leafs"]:
                     _utils.unset_parent(kw["graph"], leaf, roots)
 
                 # Execution
                 self.log("Applying cluster algorithm...")
                 graph, clusters = func(**kw)
-                self.log(
-                    f"Found {len(clusters)} clusters for {len(kw['leafs'])} leafs."
-                )
+                self.log(f"Found {len(clusters)} clusters for {len(kw['leafs'])} leafs.")
 
             # Postprocess results.
             if kw.get("root"):
                 self.log("Setting found clusters as children of root...")
                 _utils.set_children(graph, kw["root"], clusters)
                 clusters = [kw["root"]]
```

### Comparing `ragraph-1.17.0/ragraph/analysis/_utils.py` & `ragraph-1.17.1/ragraph/analysis/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         Created parent node.
     """
     if isinstance(children[0], str):
         parent_kind = graph.node_dict[children[0]].kind
     else:
         parent_kind = children[0].kind
     child_nodes = [
-        graph.node_dict[child] if isinstance(child, str) else child
-        for child in children
+        graph.node_dict[child] if isinstance(child, str) else child for child in children
     ]
     if "name" not in node_kwargs:
         if parent_kind:
             prefix = ".".join([parent_kind, prefix])
 
         node_kwargs["name"] = get_available_name(graph, prefix, lower)
     parent = Node(kind=parent_kind, **node_kwargs)
@@ -88,16 +87,15 @@
         recreation until the graph's hierarchy is complete. Inserting and moving nodes
         half-way a tree would have way too many implications for the edges.
     """
     new_parent_nodes = [
         graph.node_dict[node] if isinstance(node, str) else node for node in new_parents
     ]
     parent_sibling_nodes = [
-        graph.node_dict[node] if isinstance(node, str) else node
-        for node in parent_siblings
+        graph.node_dict[node] if isinstance(node, str) else node for node in parent_siblings
     ]
     assert set(new_parent_nodes).isdisjoint(
         parent_sibling_nodes
     ), "There should be no overlap between new parents and siblings."
 
     for i in new_parent_nodes:
         for j in new_parent_nodes:
```

### Comparing `ragraph-1.17.0/ragraph/analysis/bus/__init__.py` & `ragraph-1.17.1/ragraph/analysis/bus/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/bus/_gamma.py` & `ragraph-1.17.1/ragraph/analysis/bus/_gamma.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/cluster/__init__.py` & `ragraph-1.17.1/ragraph/analysis/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/cluster/_markov.py` & `ragraph-1.17.1/ragraph/analysis/cluster/_markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,15 @@
     symmetrize: bool = markov_params["symmetrize"],  # type: ignore
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, Union[List[Node], List[str]]]:
     assert leafs is not None
-    mat = graph.get_adjacency_matrix(
-        leafs, inherit=inherit, loops=loops, only=edge_weights
-    )
+    mat = graph.get_adjacency_matrix(leafs, inherit=inherit, loops=loops, only=edge_weights)
     assert isinstance(mat, np.ndarray)
     if symmetrize:
         mat = mat + mat.T  # Add transpose to get a guaranteed symmetrical matrix.
     tpm = calculate_tpm(mat, mu)
     if alpha > 1:  # Otherwise algorithm does nothing, then column max -> cluster ID.
         i = 0
 
@@ -227,17 +225,15 @@
         colsum = matrix.sum(0)
         to_prune = np.logical_and(matrix < threshold * colsum, matrix > 0)
 
     matrix = matrix / colsum
     return matrix
 
 
-def create_clusters(
-    graph: Graph, nodes: List[Node], cluster_ids: np.ndarray
-) -> List[Node]:
+def create_clusters(graph: Graph, nodes: List[Node], cluster_ids: np.ndarray) -> List[Node]:
     """Assign nodes in graph to new cluster nodes using a numbered array.
 
     Arguments:
         graph: Graph to add clusters into.
         nodes: Nodes that were clustered.
         cluster_ids: 1D array with numbered cluster assignment per node.
```

### Comparing `ragraph-1.17.0/ragraph/analysis/cluster/_tarjan.py` & `ragraph-1.17.1/ragraph/analysis/cluster/_tarjan.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,15 @@
             cluster_roots.append(parent)
         else:
             cluster_roots.append(children[0])
 
     return graph, cluster_roots
 
 
-def tarjans_scc_algorithm(
-    graph: Graph, nodes: List[Node], inherit: bool
-) -> List[List[Node]]:
+def tarjans_scc_algorithm(graph: Graph, nodes: List[Node], inherit: bool) -> List[List[Node]]:
     """Tarjan's strongly connected components algorithm.
 
     Arguments:
         graph: Graph to detect SCC's in (cycles).
         nodes: List of nodes (components) to detect SCC's for.
         inherit: Whether to take into account (inherit) edges between children during
             calculations.
```

### Comparing `ragraph-1.17.0/ragraph/analysis/comparison/_delta.py` & `ragraph-1.17.1/ragraph/analysis/comparison/_delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,17 +103,15 @@
         return self._unq_edges_b
 
     @property
     def cm_edges_ab(self) -> List[Edge]:
         """List of edges that are present in both graphs."""
         if self._cm_edges_ab is None:
             self._cm_edges_ab = [
-                edge
-                for edge in self.graph_a.edge_list
-                if edge not in set(self.unq_edges_a)
+                edge for edge in self.graph_a.edge_list if edge not in set(self.unq_edges_a)
             ]
         return self._cm_edges_ab
 
     @property
     def node_dict(self) -> Dict[str, Node]:
         """Dictionary from node name to Node object"""
         if self._node_dict is None:
```

### Comparing `ragraph-1.17.0/ragraph/analysis/comparison/_sigma.py` & `ragraph-1.17.1/ragraph/analysis/comparison/_sigma.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             of label occurrence) is calculated as edge weights. Defaults to fraction.
 
     Note:
         Graphs are compared on leaf node level. The resulting sigma or overlap is
         currently only calculated in terms of overlapping edge labels.
 
     Note:
-        Apart of label occurence, the overall edge occurence is also added as an Edge
-        weight, named `"_occurence"`. (The underscore prefix is added so it doesn't
+        Apart from label occurrence, the overall edge count is also added as an Edge
+        weight, named `"_count"`. (The underscore prefix is added so it doesn't
         collide with regular label names)
     """
 
     def __init__(self, graphs: List[Graph], mode: str = "fraction"):
         self.graphs = graphs
         self.mode = mode
 
@@ -70,15 +70,14 @@
 
     @property
     def nodes(self) -> List[Node]:
         """List of leaf nodes within the graph."""
         if not self._nodes:
             node_dict = {n.name: n for g in self.graphs for n in g.leafs}
             for n in node_dict.values():
-
                 self._nodes.append(
                     Node(
                         name=n.name,
                         kind=n.kind,
                         labels=n.labels,
                         weights=n.weights,
                         annotations=n.annotations,
@@ -106,15 +105,15 @@
 
             for key, edges in edge_dict.items():
                 self._edges.append(
                     Edge(
                         source=self.node_dict[key[0]],
                         target=self.node_dict[key[1]],
                         kind=key[2],
-                        labels=sorted(set([l for e in edges for l in e.labels])),
+                        labels=sorted(set([label for e in edges for label in e.labels])),
                         weights=self._get_edge_weights(edges),
                     )
                 )
 
         return self._edges
 
     @property
@@ -128,16 +127,16 @@
         return self._edge_dict
 
     def _get_edge_weights(self, edges: List[Edge]) -> Dict[str, Union[int, float]]:
         """Compute weights for edge in Sigma DSM from the provided list of edges."""
         weight_counts: Dict[str, Union[int, float]] = {"_count": len(edges)}
 
         for e in edges:
-            for l in e.labels:
-                weight_counts[l] = weight_counts.get(l, 0) + 1
+            for label in e.labels:
+                weight_counts[label] = weight_counts.get(label, 0) + 1
 
         div = 1 / len(self.graphs)
         return (
             weight_counts
             if self.mode == "absolute"
             else {key: value * div for key, value in weight_counts.items()}
         )
```

### Comparing `ragraph-1.17.0/ragraph/analysis/comparison/utils.py` & `ragraph-1.17.1/ragraph/analysis/comparison/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,15 @@
         a: Graph object.
         b: Graph object.
 
     Returns:
         List of unique leafs in Graph a.
     """
     return [
-        a.node_dict[n]
-        for n in a.node_dict.keys() - b.node_dict.keys()
-        if a.node_dict[n].is_leaf
+        a.node_dict[n] for n in a.node_dict.keys() - b.node_dict.keys() if a.node_dict[n].is_leaf
     ]
 
 
 def get_common_leafs(a: Graph, b: Graph, ue: List[Edge]) -> List[Node]:
     """Get common leafs in graph a and b
 
     Arguments:
@@ -31,17 +29,15 @@
       ue: List of unique edges.
 
     Returns:
       List of common leafs in graphs a and b.
     """
     # Shared leafs in both graphs, which do NOT participate in unique edges.
     common_leafs = [
-        a.node_dict[n]
-        for n in (a.node_dict.keys() & b.node_dict.keys())
-        if a.node_dict[n].is_leaf
+        a.node_dict[n] for n in (a.node_dict.keys() & b.node_dict.keys()) if a.node_dict[n].is_leaf
     ]
     return common_leafs
 
 
 def check_edge_equality(a: Edge, b: Edge) -> bool:
     """Checks if two edges are equal based on source, target, kind, labels.
 
@@ -66,11 +62,9 @@
     Arguments:
         a: Graph object.
         b: Graph object.
 
     Returns:
         List of unique edges in a.
     """
-    unq = [
-        ea for ea in a.edges if not any(check_edge_equality(ea, eb) for eb in b.edges)
-    ]
+    unq = [ea for ea in a.edges if not any(check_edge_equality(ea, eb) for eb in b.edges)]
     return unq
```

### Comparing `ragraph-1.17.0/ragraph/analysis/compatibility/__init__.py` & `ragraph-1.17.1/ragraph/analysis/compatibility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,21 @@
         variant: Variant node.
         weights: Optional list of weights to take into account.
         aggregation: Aggregation method, either "sum" or "product".
 
     Returns:
         Variant score.
     """
-    values = (
-        [variant.weights[k] for k in weights] if weights else variant.weights.values()
-    )
+    values = [variant.weights[k] for k in weights] if weights else variant.weights.values()
     if aggregation == "sum":
         return sum(values)
     return prod(values)
 
 
-def get_configuration_score(
-    variant_scores: Iterable[float], aggregation: str = "sum"
-) -> float:
+def get_configuration_score(variant_scores: Iterable[float], aggregation: str = "sum") -> float:
     """Score a configuration by aggregating variant scores by either taking the
     sum or product.
 
     Arguments:
         variant_scores: List of scores for all selected variants.
 
     Returns:
@@ -112,17 +108,15 @@
             or any(e.kind == compatibility_kind for e in graph[var2.name, var1.name])
         )
         if not compatible:
             return False
         incompatible = (
             False
             if incompatibility_kind is None
-            else any(
-                e.kind == incompatibility_kind for e in graph[var1.name, var2.name]
-            )
+            else any(e.kind == incompatibility_kind for e in graph[var1.name, var2.name])
             or any(e.kind == incompatibility_kind for e in graph[var2.name, var1.name])
         )
         return not incompatible
 
     return is_compatible
 
 
@@ -147,36 +141,24 @@
         raise ValueError("Applicability and inapplicability kind can't both be set.")
 
     def is_applicable(graph: Graph, element: Node, constraint: Node) -> bool:
         """Check whether these two nodes are compatible."""
         applicable = (
             True
             if applicability_kind is None
-            else any(
-                e.kind == applicability_kind
-                for e in graph[element.name, constraint.name]
-            )
-            or any(
-                e.kind == applicability_kind
-                for e in graph[constraint.name, element.name]
-            )
+            else any(e.kind == applicability_kind for e in graph[element.name, constraint.name])
+            or any(e.kind == applicability_kind for e in graph[constraint.name, element.name])
         )
         if not applicable:
             return False
         inapplicable = (
             False
             if inapplicability_kind is None
-            else any(
-                e.kind == inapplicability_kind
-                for e in graph[element.name, constraint.name]
-            )
-            or any(
-                e.kind == inapplicability_kind
-                for e in graph[constraint.name, element.name]
-            )
+            else any(e.kind == inapplicability_kind for e in graph[element.name, constraint.name])
+            or any(e.kind == inapplicability_kind for e in graph[constraint.name, element.name])
         )
         return not inapplicable
 
     return is_applicable
 
 
 def get_score_method(
@@ -249,27 +231,23 @@
     )
 
     def __init__(
         self,
         graph: Graph,
         variants: Dict[str, List[Node]],
         interface_method: Callable[[Graph, Node, Node], bool] = None,
-        compatibility_method: Callable[
-            [Graph, Node, Node], bool
-        ] = get_compatibility_method(
+        compatibility_method: Callable[[Graph, Node, Node], bool] = get_compatibility_method(
             compatibility_kind="compatibility", incompatibility_kind=None
         ),
         interface_compatibility: bool = True,
         score_method: Callable[[Tuple[Node, ...]], float] = get_score_method(
             variant_agg="sum", config_agg="sum", weights=None
         ),
         constraints: Optional[List[Node]] = None,
-        applicability_method: Callable[
-            [Graph, Node, Node], bool
-        ] = get_applicability_method(
+        applicability_method: Callable[[Graph, Node, Node], bool] = get_applicability_method(
             applicability_kind="applicability", inapplicability_kind=None
         ),
     ):
         self.graph = graph
         self.interface_method = interface_method
         self.compatibility_method = compatibility_method
         self.interface_compatibility = interface_compatibility
@@ -348,17 +326,15 @@
         return all(
             self.applicability_method(self.graph, variant, constraint)
             for constraint in self.constraints
         )
 
     def has_interface(self, var1: Node, var2: Node) -> bool:
         """Whether two variants have an interface that needs a compatibility check."""
-        return (self.interface_method is None) or self.interface_method(
-            self.graph, var1, var2
-        )
+        return (self.interface_method is None) or self.interface_method(self.graph, var1, var2)
 
     def is_compatible(self, var1: Node, var2: Node) -> bool:
         """Whether the two given variants are compatible according to
         :obj:`self.compatibility_method`
         """
 
         if self.interface_compatibility:
@@ -382,17 +358,15 @@
         Returns:
             Compatibility matrix as a list of lists or numpy array (if numpy is
             available).
         """
         variants = self._variants_list if variants is None else variants
         dim = len(variants)
         mat = (
-            np.zeros((dim, dim))
-            if HAVE_NUMPY
-            else [[0.0 for j in range(dim)] for i in range(dim)]
+            np.zeros((dim, dim)) if HAVE_NUMPY else [[0.0 for j in range(dim)] for i in range(dim)]
         )
         for i in range(dim):
             var1 = variants[i]
             for j in range(i + 1, dim):
                 if self.is_compatible(var1, variants[j]):
                     mat[i][j] = 1.0
                     mat[j][i] = 1.0
@@ -431,21 +405,17 @@
 
         Arguments:
             descending: Whether highest scores should go first.
 
         Returns:
             Sorted tuples of configurations and scores.
         """
-        return sorted(
-            self.yield_scored_configurations(), key=lambda x: x[-1], reverse=descending
-        )
+        return sorted(self.yield_scored_configurations(), key=lambda x: x[-1], reverse=descending)
 
-    def write_csv(
-        self, path: Union[str, Path], scored: bool = True, limit: int = -1
-    ) -> int:
+    def write_csv(self, path: Union[str, Path], scored: bool = True, limit: int = -1) -> int:
         """Write feasible configurations and optional scores to a CSV file."""
         path = Path(path)
         num = 0
         with open(path, mode="w+", encoding="utf-8") as f:
             f.write(";".join(self._elements))
 
         def append(content: str):
@@ -500,17 +470,15 @@
                             g[var2.name],
                             kind="compatibility",
                             labels=[],
                         )
                         if self.has_interface(var1, var2):
                             e1.labels.append("interface")
                             e1.labels.append(
-                                "compatible"
-                                if self.is_compatible(var1, var2)
-                                else "incompatible"
+                                "compatible" if self.is_compatible(var1, var2) else "incompatible"
                             )
                         else:
                             e1.labels.append("no interface")
                             e1.labels.append("compatible")
                             e1.weights["scale"] = 0.25
                         e2 = Edge(
                             g[var2.name],
```

### Comparing `ragraph-1.17.0/ragraph/analysis/compatibility/bdd.py` & `ragraph-1.17.1/ragraph/analysis/compatibility/bdd.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 def _yield_ranges(nums: List[int], start: int = 0) -> Generator[range, None, None]:
     """Generate matrix index ranges."""
     for i in nums:
         yield range(start, start + i)
         start += i
 
 
-def _recursive(
-    operation: str, bdd: _bdd.BDD, items: List[_bdd.Function]
-) -> _bdd.Function:
+def _recursive(operation: str, bdd: _bdd.BDD, items: List[_bdd.Function]) -> _bdd.Function:
     """Construct a recursive operation function over all items."""
     if len(items) == 1:
         return items[0]
     return bdd.apply(operation, items[0], _recursive(operation, bdd, items[1:]))
 
 
 def yield_feasible_configurations(
```

### Comparing `ragraph-1.17.0/ragraph/analysis/heuristics/__init__.py` & `ragraph-1.17.1/ragraph/analysis/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/heuristics/_johnson.py` & `ragraph-1.17.1/ragraph/analysis/heuristics/_johnson.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/heuristics/_markov_gamma.py` & `ragraph-1.17.1/ragraph/analysis/heuristics/_markov_gamma.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,13 +149,11 @@
                 bus.is_bus = True
 
         # Finished this root.
         checked_roots.append(local_root)
 
         # If local: move down a level.
         if not check_roots and local_buses:
-            check_roots = [
-                child for local_root in checked_roots for child in local_root.children
-            ]
+            check_roots = [child for local_root in checked_roots for child in local_root.children]
             checked_roots = []
 
     return graph, roots
```

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/__init__.py` & `ragraph-1.17.1/ragraph/analysis/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/_axis.py` & `ragraph-1.17.1/ragraph/analysis/sequence/_axis.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,15 @@
     roots = get_roots(nodes, root_cache, child_cache)
     roots.sort(key=lambda x: get_root_key(x, kind_order, sort_by_width, width_cache))
 
     # Sort by is_bus status with buses first, width second, if applicable.
     if sort_by_bus or sort_by_width:
         for parent in child_cache.keys():
             child_cache[parent].sort(
-                key=lambda x: get_sibling_key(
-                    x, sort_by_bus, sort_by_width, width_cache
-                )
+                key=lambda x: get_sibling_key(x, sort_by_bus, sort_by_width, width_cache)
             )
 
     # Complement width_cache for roots for completeness sake.
     if sort_by_width:
         for root in roots:
             width_cache[root] = sum(
                 width_cache.get(child, 1) for child in child_cache.get(root, [])
@@ -261,17 +259,15 @@
 
     Returns:
         Node width.
     """
     width_cache = dict() if width_cache is None else width_cache
     if node not in width_cache:
         if node.children:
-            width_cache[node] = sum(
-                get_width(child, width_cache) for child in node.children
-            )
+            width_cache[node] = sum(get_width(child, width_cache) for child in node.children)
         else:
             width_cache[node] = 1
     return width_cache[node]
 
 
 def get_root_key(
     node: Node,
@@ -343,10 +339,9 @@
     inherit: bool = True,
     loops: bool = False,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ):
-
     seq = get_axis_sequence(nodes, kinds, sort_by_bus, sort_by_width)  # type: ignore
     return graph, seq
```

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/_genetic.py` & `ragraph-1.17.1/ragraph/analysis/sequence/_genetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     edge_weights: Optional[List[str]] = None,
     loops: bool = False,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
-
     lineage = genetic_sequencing(
         graph,
         nodes,  # type: ignore
         n_chromosomes,  # type: ignore
         n_generations,  # type: ignore
         1,
         p_crossover,  # type: ignore
```

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/_markov.py` & `ragraph-1.17.1/ragraph/analysis/sequence/_markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,15 @@
     loops: bool = False,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
     assert nodes is not None
-    adj = graph.get_adjacency_matrix(
-        nodes=nodes, inherit=inherit, loops=loops, only=edge_weights
-    )
+    adj = graph.get_adjacency_matrix(nodes=nodes, inherit=inherit, loops=loops, only=edge_weights)
     assert isinstance(adj, np.ndarray)
 
     # Obtain node penalty scores.
     penalties = net_markov_flow_adjacency(adj, inf=inf, dep=dep, mu=mu, scale=scale)
 
     # Calculate final sequence.
     idxs = np.argsort(penalties)
```

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/_name.py` & `ragraph-1.17.1/ragraph/analysis/sequence/_name.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/_scc_tearing.py` & `ragraph-1.17.1/ragraph/analysis/sequence/_scc_tearing.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     loops: bool = False,
     edge_weights: Optional[List[str]] = None,
     inplace: bool = True,
     names: bool = False,
     safe: bool = True,
     **kwargs,
 ) -> Tuple[Graph, List[Node]]:
-
     sequence = scc_tearing_algorithm(
         graph, nodes, inherit, loops, decision, decision_args  # type: ignore
     )
     seq = list(sequence)
 
     return graph, seq
 
@@ -106,10 +105,8 @@
             continue
 
         # Pick node to tear.
         tear = decision(graph, scc, **decision_args)
         torn = scc.pop(tear)
         scc_tearing_analysis.log(f"torn '{torn.name}' from {[n.name for n in scc]}.")
         yield torn
-        yield from scc_tearing_algorithm(
-            graph, scc, inherit, loops, decision, decision_args
-        )
+        yield from scc_tearing_algorithm(graph, scc, inherit, loops, decision, decision_args)
```

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/_tarjan.py` & `ragraph-1.17.1/ragraph/analysis/sequence/_tarjan.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/metrics.py` & `ragraph-1.17.1/ragraph/analysis/sequence/metrics.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/sequence/utils.py` & `ragraph-1.17.1/ragraph/analysis/sequence/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/similarity/__init__.py` & `ragraph-1.17.1/ragraph/analysis/similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/similarity/_jaccard.py` & `ragraph-1.17.1/ragraph/analysis/similarity/_jaccard.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/similarity/_similarity.py` & `ragraph-1.17.1/ragraph/analysis/similarity/_similarity.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/analysis/similarity/utils.py` & `ragraph-1.17.1/ragraph/analysis/similarity/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 
     Returns:
         Object description function indicating check passings.
     """
     return lambda obj: [check(obj) for check in checks]
 
 
-def on_hasweights(
-    weights: List[str], threshold: float = 0.0
-) -> Callable[[Any], List[bool]]:
+def on_hasweights(weights: List[str], threshold: float = 0.0) -> Callable[[Any], List[bool]]:
     """Check whether an objects has certain weights above a threshold in its weights
     dictionary property.
 
     Arguments:
         weights: Keys to the :obj:`obj.weights` dictionary to check.
         threshold: Threshold to verify against.
```

### Comparing `ragraph-1.17.0/ragraph/colors/__init__.py` & `ragraph-1.17.1/ragraph/colors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,16 +321,15 @@
     if kind == "categorical":
         return [get_categorical(n_colors=n_colors)]
     elif kind == "sequential":
         if amount == 1:
             colormaps = [get_continuous(n_colors=n_colors)]
         else:
             colormaps = [
-                get_hue(n_colors=n_colors, hue=2.85 + 3 * i / amount)
-                for i in range(amount)
+                get_hue(n_colors=n_colors, hue=2.85 + 3 * i / amount) for i in range(amount)
             ]
     elif kind == "diverging":
         colormaps = [
             get_diverging_hues(
                 n_colors=n_colors,
                 lower_hue=0.95 - 1.0 * i / amount,
                 upper_hue=2.85 - 2 * i / amount,
```

### Comparing `ragraph-1.17.0/ragraph/colors/cubehelix.py` & `ragraph-1.17.1/ragraph/colors/cubehelix.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/colors/utils.py` & `ragraph-1.17.1/ragraph/colors/utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/__init__.py` & `ragraph-1.17.1/ragraph/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/aircraft_engine/__init__.py` & `ragraph-1.17.1/ragraph/datasets/aircraft_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv` & `ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/architecture_integral/__init__.py` & `ragraph-1.17.1/ragraph/datasets/architecture_integral/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv` & `ragraph-1.17.1/ragraph/datasets/architecture_integral/architecture_integral_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/architecture_mix/__init__.py` & `ragraph-1.17.1/ragraph/datasets/architecture_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv` & `ragraph-1.17.1/ragraph/datasets/architecture_mix/architecture_mix_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/architecture_modular/__init__.py` & `ragraph-1.17.1/ragraph/datasets/architecture_modular/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv` & `ragraph-1.17.1/ragraph/datasets/architecture_modular/architecture_modular_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/climate_control/__init__.py` & `ragraph-1.17.1/ragraph/datasets/climate_control/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/climate_control/climate_control_edges.csv` & `ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/climate_control/climate_control_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/climate_control/climate_control_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv` & `ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/compatibility/compatibility_edges.csv` & `ragraph-1.17.1/ragraph/datasets/compatibility/compatibility_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/design/design_edges.csv` & `ragraph-1.17.1/ragraph/datasets/design/design_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/eefde_lock/eefde_lock_edges.csv` & `ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/eefde_lock/eefde_lock_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/elevator175/__init__.py` & `ragraph-1.17.1/ragraph/datasets/elevator175/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/elevator175/elevator175_edges.csv` & `ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/elevator175/elevator175_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/elevator175/elevator175_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/elevator45/__init__.py` & `ragraph-1.17.1/ragraph/datasets/elevator45/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/elevator45/elevator45_edges.csv` & `ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/elevator45/elevator45_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/elevator45/elevator45_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/esl/__init__.py` & `ragraph-1.17.1/ragraph/datasets/esl/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/esl/pump/pump.esl` & `ragraph-1.17.1/ragraph/datasets/esl/pump/pump.esl`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ford_hood/__init__.py` & `ragraph-1.17.1/ragraph/datasets/ford_hood/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ford_hood/ford_hood_edges.csv` & `ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/ford_hood/ford_hood_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/kodak3d/__init__.py` & `ragraph-1.17.1/ragraph/datasets/kodak3d/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/kodak3d/kodak3d_edges.csv` & `ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/kodak3d/kodak3d_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ledsip/ledsip_edges.csv` & `ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ledsip/ledsip_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/ledsip/ledsip_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/localbus/localbus_edges.csv` & `ragraph-1.17.1/ragraph/datasets/localbus/localbus_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/pathfinder/__init__.py` & `ragraph-1.17.1/ragraph/datasets/pathfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/pathfinder/pathfinder_edges.csv` & `ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/pathfinder/pathfinder_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/similarity/similarity_edges.csv` & `ragraph-1.17.1/ragraph/datasets/similarity/similarity_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ucav/__init__.py` & `ragraph-1.17.1/ragraph/datasets/ucav/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ucav/ucav_edges.csv` & `ragraph-1.17.1/ragraph/datasets/ucav/ucav_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/datasets/ucav/ucav_nodes.csv` & `ragraph-1.17.1/ragraph/datasets/ucav/ucav_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/edge.py` & `ragraph-1.17.1/ragraph/edge.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/generic.py` & `ragraph-1.17.1/ragraph/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         """Get a mapping value."""
         if key in self._data:
             return self._data[key]
 
         if key in self._defaults:
             return self._defaults[key]
 
-        raise AttributeError(
-            f"Mapping does not contain a (default) value for key '{key}'."
-        )
+        raise AttributeError(f"Mapping does not contain a (default) value for key '{key}'.")
 
     def setter(self, value: Any):
         """Set a mapping value."""
         # Setting the mapping to None means resetting it to default.
         if value is None:
             self._data.pop(key, None)
             return
@@ -154,17 +152,15 @@
         See :obj:`self._check_allowed`.
         """
         if not key.startswith("_"):
             keys = set() if self._keys is None else self._keys
             keys = keys.union(self.keys())
             if key not in keys:
                 if self._protected:
-                    raise KeyError(
-                        f"Key or property '{key}' is not allowed. Only '{keys}'."
-                    )
+                    raise KeyError(f"Key or property '{key}' is not allowed. Only '{keys}'.")
                 else:
                     # Dynamically create a new field.
                     def stub(self):
                         f"""{key} mapping field."""
                         pass
 
                     stub.__name__ = key
@@ -188,17 +184,15 @@
             kwargs: Keyword arguments to update the set data with.
         """
         for arg in args:
             try:
                 for key, value in arg.items():
                     setattr(self, key, value)
             except AttributeError:
-                raise TypeError(
-                    f"Expected a dictionary or a Mapping. Found a {type(arg)}."
-                )
+                raise TypeError(f"Expected a dictionary or a Mapping. Found a {type(arg)}.")
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def __iter__(self):
         """Provide an iterator."""
         yield from self.items()
```

### Comparing `ragraph-1.17.0/ragraph/graph.py` & `ragraph-1.17.1/ragraph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,31 +256,25 @@
 
         If the node instance already exists in the graph, it is ignored.
 
         Arguments:
             node: Node to add.
         """
         if not isinstance(node, Node):
-            raise TypeError(
-                "%r is not an instance of Node but of %r." % (node, type(node))
-            )
+            raise TypeError("%r is not an instance of Node but of %r." % (node, type(node)))
 
         # Append own node if not exists.
         if node.name in self._nodes:
             if node == self._nodes[node.name]:
                 return
-            raise ValueError(
-                f"Another Node named '{node.name}' already exists in this Graph."
-            )
+            raise ValueError(f"Another Node named '{node.name}' already exists in this Graph.")
         if node.uuid in self.node_uuid_dict:
             if node == self.node_uuid_dict[node.uuid]:
                 return
-            raise ValueError(
-                f"Another Node with UUID '{node.uuid}' already exists in this Graph."
-            )
+            raise ValueError(f"Another Node with UUID '{node.uuid}' already exists in this Graph.")
         self._nodes[node.name] = node
         self.node_uuid_dict[node.uuid] = node
 
         # Append parent
         if self.add_parents and node.parent:
             self.add_node(node.parent)
 
@@ -392,17 +386,15 @@
         return self.get_weight_labels(self.node_gen)
 
     @property
     def edge_weight_labels(self) -> List[str]:
         """List of unique edge weight labels in the graph."""
         return self.get_weight_labels(self.edge_gen)
 
-    def get_weight_labels(
-        self, elements: Union[Iterable[Node], Iterable[Edge]]
-    ) -> List[str]:
+    def get_weight_labels(self, elements: Union[Iterable[Node], Iterable[Edge]]) -> List[str]:
         """Get an alphabetically sorted list of unique labels of node/edge weights."""
         labels: Set[str] = set()
         for elem in elements:
             labels.update(elem.weights.keys())
         return sorted(labels, key=str)
 
     @property
@@ -509,17 +501,15 @@
             sources: Source nodes.
             targets: Target nodes.
             inherit: Whether to include edges between descendants of given nodes.
             loops: Whether to include self-loop edges.
         """
         for source in sources:
             for target in targets:
-                yield from self.edges_between(
-                    source, target, inherit=inherit, loops=loops
-                )
+                yield from self.edges_between(source, target, inherit=inherit, loops=loops)
 
     def get_graph_slice(
         self,
         nodes: Optional[Iterable[Node]] = None,
         edges: Optional[Iterable[Edge]] = None,
         inherit: bool = False,
     ) -> "Graph":
@@ -534,30 +524,24 @@
                 between them (unless edges are explicitly specified).
 
         Note:
             This returns a deepcopy, so the copied nodes and edges do NOT share any
             changes! All parent and child nodes not in the list are excluded.
         """
         nodes = self.nodes if nodes is None else list(nodes)
-        edges = (
-            self.edges_between_all(nodes, nodes, inherit)
-            if edges is None
-            else list(edges)
-        )
+        edges = self.edges_between_all(nodes, nodes, inherit) if edges is None else list(edges)
 
         # Get a deepcopy to prevent changing nodes in the current graph instance.
         graph = deepcopy(Graph(nodes=nodes, edges=edges, add_children=inherit))
 
         # Reinstate relationships only between given nodes.
         graph_nodes = graph.nodes
         for node in graph_nodes:
             if node.parent:
-                node.parent = (
-                    graph[node.parent.name] if node.parent in graph.nodes else None
-                )
+                node.parent = graph[node.parent.name] if node.parent in graph.nodes else None
             node.children = [c for c in node.children if c in graph.nodes]
             if node.is_bus and not node.parent:
                 node.is_bus = False
 
         return graph
 
     def get_node_selection(
@@ -601,19 +585,15 @@
             List of selected edges.
         """
 
         nlist = nodes or self.get_node_selection(edge_kinds=edge_kinds)
         ekinds = edge_kinds or self.edge_kinds
         ekinds = sorted(set(ekinds))
 
-        return [
-            e
-            for e in self.edges_between_all(sources=nlist, targets=nlist)
-            if e.kind in ekinds
-        ]
+        return [e for e in self.edges_between_all(sources=nlist, targets=nlist) if e.kind in ekinds]
 
     def get_node_and_edge_selection(
         self,
         node_kinds: Optional[List[str]] = None,
         edge_kinds: Optional[List[str]] = None,
         depth: int = 2,
         selection_mode: str = "dependent",
@@ -643,17 +623,15 @@
             selection_mode=selection_mode,
         )
 
         edges = self.get_edge_selection(nodes=nodes, edge_kinds=edge_kinds)
 
         return nodes, edges
 
-    def get_hierarchy_dict(
-        self, roots: Optional[List[Node]] = None, levels: Optional[int] = None
-    ):
+    def get_hierarchy_dict(self, roots: Optional[List[Node]] = None, levels: Optional[int] = None):
         """Return a dictionary of the (partial) hierarchical node structure.
 
         Arguments:
             roots: Root nodes of the hierarchy to calculate.
             levels: Number of levels to include below the roots.
         """
         if roots is None:
@@ -687,17 +665,15 @@
 
         Returns:
             Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
             return a 2D nested list.
         """
         from ragraph.io.matrix import to_matrix
 
-        return to_matrix(
-            self, rows=nodes, cols=nodes, inherit=inherit, loops=loops, only=only
-        )
+        return to_matrix(self, rows=nodes, cols=nodes, inherit=inherit, loops=loops, only=only)
 
     def get_mapping_matrix(
         self,
         rows: Optional[Union[List[Node], List[str]]] = None,
         cols: Optional[Union[List[Node], List[str]]] = None,
         inherit: bool = False,
         loops: bool = False,
@@ -716,17 +692,15 @@
 
         Returns:
             Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
             return a 2D nested list.
         """
         from ragraph.io.matrix import to_matrix
 
-        return to_matrix(
-            self, rows=rows, cols=cols, inherit=inherit, loops=loops, only=only
-        )
+        return to_matrix(self, rows=rows, cols=cols, inherit=inherit, loops=loops, only=only)
 
     def get_ascii_art(
         self,
         nodes: Optional[List[Node]] = None,
         edge: str = "X",
         diag: str = "\u25A0",
         show: bool = True,
@@ -759,15 +733,14 @@
         topline = pad + "\u250C" + (dim - 1) * (ddd + "\u252C") + ddd + "\u2510"
         sepline = pad + "\u251C" + (dim - 1) * (ddd + "\u253C") + ddd + "\u2524"
         endline = pad + "\u2514" + (dim - 1) * (ddd + "\u2534") + ddd + "\u2518"
 
         lines = [topline]
 
         for i, tgt in enumerate(nodes):
-
             line = (maxlen - namelens[i]) * " " + tgt.name + "\u2525"
             for j, src in enumerate(nodes):
                 if i == j:
                     mark = diag
                 elif self._directed_edges.get(src.name, dict()).get(tgt.name, False):
                     mark = edge
                 else:
@@ -840,66 +813,50 @@
         consistent = True
 
         try:
             for node in self.node_list:
                 a = node
                 while a.parent:
                     if a.parent == node:
-                        raise ConsistencyError(
-                            "Node {} is in its own ancestors.".format(node)
-                        )
+                        raise ConsistencyError("Node {} is in its own ancestors.".format(node))
                     a = a.parent
                 ds = node.children
                 while ds:
                     if node in ds:
-                        raise ConsistencyError(
-                            "Node {} is in its own descendants.".format(node)
-                        )
+                        raise ConsistencyError("Node {} is in its own descendants.".format(node))
                     ds = [c for d in ds for c in d.children]
                 if node.parent and node.parent not in self.node_list:
                     raise ConsistencyError(
-                        "Node {}'s parent {} is missing in the graph.".format(
-                            node, node.parent
-                        )
+                        "Node {}'s parent {} is missing in the graph.".format(node, node.parent)
                     )
                 if node.parent and node not in node.parent.children:
                     raise ConsistencyError(
                         "Node {}'s does not occur in parent {}'s children.".format(
                             node, node.parent
                         )
                     )
                 for child in node.children:
                     if child not in self.node_list:
                         raise ConsistencyError(
-                            "Node {}'s child {} is missing in the graph.".format(
-                                node, child
-                            )
+                            "Node {}'s child {} is missing in the graph.".format(node, child)
                         )
                     if child.parent != node:
                         raise ConsistencyError(
-                            "Node {}'s child has a different parent {}.".format(
-                                node, child.parent
-                            )
+                            "Node {}'s child has a different parent {}.".format(node, child.parent)
                         )
                 if node.is_bus and not node.parent:
                     raise ConsistencyError(
-                        "Node {} is a bus node, but has no parent to be it for.".format(
-                            node
-                        )
+                        "Node {} is a bus node, but has no parent to be it for.".format(node)
                     )
 
             for edge in self.edge_list:
                 if edge.source.name not in self.node_dict:
-                    raise ConsistencyError(
-                        f"Edge source not in Graph: {repr(edge.source)}"
-                    )
+                    raise ConsistencyError(f"Edge source not in Graph: {repr(edge.source)}")
                 if edge.target.name not in self.node_dict:
-                    raise ConsistencyError(
-                        f"Edge target not in Graph: {repr(edge.source)}"
-                    )
+                    raise ConsistencyError(f"Edge target not in Graph: {repr(edge.source)}")
 
         except ConsistencyError as e:
             consistent = False
             if raise_error:
                 raise e
 
         return consistent
```

### Comparing `ragraph-1.17.0/ragraph/io/archimate/__init__.py` & `ragraph-1.17.1/ragraph/io/archimate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,16 @@
     Returns:
         Property definitions XML element.
 
     Note:
         Labels, Weight and Annotations all get their own prefixed properties.
     """
     propdefs = maker.propertyDefinitions(
-        maker.propertyDefinition(
-            maker.name("kind"), {"identifier": "kind", "type": "string"}
-        ),
-        maker.propertyDefinition(
-            maker.name("is_bus"), {"identifier": "is_bus", "type": "boolean"}
-        ),
+        maker.propertyDefinition(maker.name("kind"), {"identifier": "kind", "type": "string"}),
+        maker.propertyDefinition(maker.name("is_bus"), {"identifier": "is_bus", "type": "boolean"}),
     )
 
     for label in sorted(set(g.node_labels + g.edge_labels)):
         propdefs.append(
             maker.propertyDefinition(
                 maker.name(f"label: {label}"),
                 dict(identifier=f"_l_{label}", type="boolean"),
@@ -108,37 +104,29 @@
         Properties XML element.
     """
     props = maker.properties()
 
     props.append(maker.property(maker.value(obj.kind), propertyDefinitionRef="kind"))
 
     for i in sorted(obj.labels):
-        props.append(
-            maker.property(maker.value("true"), propertyDefinitionRef=f"_l_{i}")
-        )
+        props.append(maker.property(maker.value("true"), propertyDefinitionRef=f"_l_{i}"))
 
     for k in sorted(obj.weights.keys()):
         v = obj.weights[k]
-        props.append(
-            maker.property(maker.value(str(float(v))), propertyDefinitionRef=f"_w_{k}")
-        )
+        props.append(maker.property(maker.value(str(float(v))), propertyDefinitionRef=f"_w_{k}"))
 
     for k in sorted(obj.annotations.keys()):
         v = getattr(obj.annotations, k)
         if type(v) not in annot_types:
             continue
         t = annot_types[type(v)]
-        props.append(
-            maker.property(maker.value(str(v)), propertyDefinitionRef=f"_a_{t}_{k}")
-        )
+        props.append(maker.property(maker.value(str(v)), propertyDefinitionRef=f"_a_{t}_{k}"))
 
     if isinstance(obj, Node) and obj.is_bus:
-        props.append(
-            maker.property(maker.value("true"), propertyDefinitionRef="is_bus")
-        )
+        props.append(maker.property(maker.value("true"), propertyDefinitionRef="is_bus"))
 
     return props
 
 
 def _node_to_element(node: Node) -> etree.Element:
     """Convert a Node into an XML element.
 
@@ -160,25 +148,21 @@
     archi_type = getattr(node.annotations, "archimate", {}).get("type", "Node")
     archi_fields = {"identifier": _get_xmi_id(node, "_n_"), q_type: archi_type}
 
     # Archimate element properties (kind/labels/weights/annotations with a value)
     archi_properties = _get_properties(node)
 
     # Get documentation field if the respective annotation is found.
-    documentation = getattr(node.annotations, "archimate", {}).get(
-        "documentation", None
-    )
+    documentation = getattr(node.annotations, "archimate", {}).get("documentation", None)
 
     # Make element with or without documentation.
     if documentation is None:
         elem = maker.element(archi_name, archi_properties, archi_fields)
     else:
-        archi_docs = maker.documentation(
-            str(documentation).replace("\n", "\r\n"), {q_lang: "en"}
-        )
+        archi_docs = maker.documentation(str(documentation).replace("\n", "\r\n"), {q_lang: "en"})
         elem = maker.element(archi_name, archi_docs, archi_properties, archi_fields)
 
     return elem
 
 
 def _hierarchy_to_relationships(graph: Graph) -> Generator[etree.Element, None, None]:
     """Generate relationships of a Graph's Node hierarchy.
@@ -232,39 +216,31 @@
         q_type: archi_type,
     }
 
     # Archimate element properties (kind/labels/weights/annotations with a value)
     archi_properties = _get_properties(edge)
 
     # Get documentation field if the respective annotation is found.
-    documentation = getattr(edge.annotations, "archimate", {}).get(
-        "documentation", None
-    )
+    documentation = getattr(edge.annotations, "archimate", {}).get("documentation", None)
 
     # Make element with or without documentation.
     if documentation is None:
         elem = maker.relationship(
             archi_name,
             archi_properties,
             archi_fields,
         )
     else:
-        archi_docs = maker.documentation(
-            str(documentation).replace("\n", "\r\n"), {q_lang: "en"}
-        )
-        elem = maker.relationship(
-            archi_name, archi_docs, archi_properties, archi_fields
-        )
+        archi_docs = maker.documentation(str(documentation).replace("\n", "\r\n"), {q_lang: "en"})
+        elem = maker.relationship(archi_name, archi_docs, archi_properties, archi_fields)
 
     return elem
 
 
-def _expand_requirements_constraints(
-    node: Node, elems: etree.Element, rels: etree.Element
-):
+def _expand_requirements_constraints(node: Node, elems: etree.Element, rels: etree.Element):
     """Expand requirements and constraints so that they become an ApplicationFunction
     and Requirement/Constraint combination.
 
     Arguments:
         node: Nodes to expand.
         elems: XML element to append elements to.
         rels: XML element to append relationships to.
```

### Comparing `ragraph-1.17.0/ragraph/io/archimate/archimate3_Model.xsd` & `ragraph-1.17.1/ragraph/io/archimate/archimate3_Model.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/io/archimate/xml.xsd` & `ragraph-1.17.1/ragraph/io/archimate/xml.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/io/canopy.py` & `ragraph-1.17.1/ragraph/io/canopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,17 +195,15 @@
     opts.pop("$schema", None)
     opts["uuid"] = opts.pop("id", None)
     opts.pop("nodes", None)
     opts.pop("edges", None)
     graph = Graph(**opts)
     graph.nodes = [_decode_node(node_data) for node_data in data.get("nodes", [])]
     _decode_hierarchy(data, graph)
-    graph.edges = [
-        _decode_edge(edge_data, graph) for edge_data in data.get("edges", [])
-    ]
+    graph.edges = [_decode_edge(edge_data, graph) for edge_data in data.get("edges", [])]
     return graph
 
 
 def _decode_tab(data: Dict[str, Any]) -> Generator[Graph, None, None]:
     if isinstance(data.get("graph"), dict):
         yield _decode_graph(data["graph"])
```

### Comparing `ragraph-1.17.0/ragraph/io/csv.py` & `ragraph-1.17.1/ragraph/io/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,15 @@
 
     if nodes_path:
         node_dict = _load_nodes(nodes_path, csv_delimiter, iter_delimiter, node_weights)
     else:
         node_dict = _derive_nodes(edges_path, csv_delimiter)
 
     if edges_path:
-        edges = _load_edges(
-            edges_path, csv_delimiter, iter_delimiter, node_dict, edge_weights
-        )
+        edges = _load_edges(edges_path, csv_delimiter, iter_delimiter, node_dict, edge_weights)
     else:
         edges = []
 
     graph.add_parents = True
     graph.add_children = True
     graph.nodes = node_dict
     graph.edges = edges
@@ -132,17 +130,15 @@
         raise ValueError(
             "Nodes CSV file {} needs at least a 'name' column, found {}.".format(
                 str(fpath), columns
             )
         )
 
     wght_cols = node_weights
-    anno_cols = [
-        col for col in columns if col not in NODE_COLUMNS and col not in wght_cols
-    ]
+    anno_cols = [col for col in columns if col not in NODE_COLUMNS and col not in wght_cols]
 
     # Handle node names and annotations
     names = []
     nodes = []
     for row in rows:
         name = row["name"]
         anno = Annotations(**{col: row[col] for col in anno_cols})
@@ -171,19 +167,15 @@
         parent = row.get("parent", None)
         if parent:
             node.parent = node_dict[parent]
 
         children = row.get("children", [])
         if children:
             children_names = [n.strip() for n in children.split(iter_delimiter)]
-            children = [
-                node_dict[n]
-                for n in children_names
-                if node_dict[n] not in node.children
-            ]
+            children = [node_dict[n] for n in children_names if node_dict[n] not in node.children]
             node.children = node.children + children
 
         is_bus = row.get("is_bus", "false")
         if is_bus.strip().lower() == "true":
             node.is_bus = True
 
     return node_dict
@@ -248,23 +240,19 @@
 
     with Path(fpath).open(newline="") as f:
         reader = csv.DictReader(f, delimiter=csv_delimiter)
         columns = reader.fieldnames
         rows = [row for row in reader]
     if "source" not in columns or "target" not in columns:
         raise ValueError(
-            "Edges CSV file {} needs at least a 'source' and 'target' column.".format(
-                str(fpath)
-            )
+            "Edges CSV file {} needs at least a 'source' and 'target' column.".format(str(fpath))
         )
 
     wght_cols = edge_weights
-    anno_cols = [
-        col for col in columns if col not in EDGE_COLUMNS and col not in wght_cols
-    ]
+    anno_cols = [col for col in columns if col not in EDGE_COLUMNS and col not in wght_cols]
 
     edges = []
     for row in rows:
         if row.get("labels", None):
             row["labels"] = [s.strip() for s in row["labels"].split(iter_delimiter)]
         weights = {col: _convert_to_num(row[col]) for col in wght_cols}
         anno = Annotations(**{col: row[col] for col in anno_cols})
@@ -291,22 +279,18 @@
         csv_delimiter: CSV delimiter.
         iter_delimiter: Iterable delimiter (i.e. for children names list).
         use_uuid: Whether to export UUIDs, too.
     """
     # Weights column mapping
     wght_keys = [key for key in graph.node_weight_labels if key is not None]
     wght_map = {key: str(key) for key in wght_keys}
-    wght_map.update(
-        {key: str(key) + "_weight" for key in wght_keys if str(key) in NODE_COLUMNS}
-    )
+    wght_map.update({key: str(key) + "_weight" for key in wght_keys if str(key) in NODE_COLUMNS})
 
     # Annotations column mapping
-    anno_keys = sorted(
-        set([key for node in graph.node_list for key in node.annotations.keys()])
-    )
+    anno_keys = sorted(set([key for node in graph.node_list for key in node.annotations.keys()]))
     anno_map = {key: str(key) for key in anno_keys}
     anno_map.update(
         {
             key: str(key) + "_annotation"
             for key in anno_keys
             if str(key) in NODE_COLUMNS or str(key) in wght_map.values()
         }
@@ -368,22 +352,18 @@
         csv_delimiter: CSV delimiter.
         iter_delimiter: Iterable delimiter (i.e. for children names list).
         use_uuid: Whether to export UUIDs, too.
     """
     # Weights column mapping
     wght_keys = [key for key in graph.edge_weight_labels if key is not None]
     wght_map = {key: str(key) for key in wght_keys}
-    wght_map.update(
-        {key: str(key) + "_weight" for key in wght_keys if str(key) in EDGE_COLUMNS}
-    )
+    wght_map.update({key: str(key) + "_weight" for key in wght_keys if str(key) in EDGE_COLUMNS})
 
     # Annotations column mapping
-    anno_keys = sorted(
-        set([key for edge in graph.edge_list for key in edge.annotations.keys()])
-    )
+    anno_keys = sorted(set([key for edge in graph.edge_list for key in edge.annotations.keys()]))
     anno_map = {key: str(key) for key in anno_keys}
     anno_map.update(
         {
             key: str(key) + "_annotation"
             for key in anno_keys
             if str(key) in NODE_COLUMNS or str(key) in wght_map.values()
         }
@@ -441,14 +421,12 @@
             num = float(value)
             return num
         except ValueError:
             msg = " ".join(
                 [
                     "You are assigning a string as a weight property.",
                     "Please use a float, integer, or a Bool.",
-                    "A default value of 1.0 is used as a replacement for {}.".format(
-                        value
-                    ),
+                    "A default value of 1.0 is used as a replacement for {}.".format(value),
                 ]
             )
             warnings.warn(msg)
             return 1.0
```

### Comparing `ragraph-1.17.0/ragraph/io/json.py` & `ragraph-1.17.1/ragraph/io/json.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/io/matrix.py` & `ragraph-1.17.1/ragraph/io/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
     else:
         node_cols = _parse_labels(graph, cols)
 
     # Dimension check of matrix and labels.
     dim = (len(matrix), len(matrix[0]))
     labdim = (len(node_rows), len(node_cols))
     if dim != labdim:
-        raise ValueError(
-            f"Matrix dimensions {dim} do not agree with label dimensions {labdim}."
-        )
+        raise ValueError(f"Matrix dimensions {dim} do not agree with label dimensions {labdim}.")
 
     # Generate edges and return.
     edges = [
         Edge(
             source,
             target,
             name=f"{source.name}->{target.name}",
@@ -129,30 +127,25 @@
             sources = [source]
             targets = [target]
             if inherit:
                 sources.extend(source.descendants)
                 targets.extend(target.descendants)
 
             weight = sum(
-                [
-                    _get_weight(e, only=only)
-                    for e in graph.edges_between_all(sources, targets)
-                ]
+                [_get_weight(e, only=only) for e in graph.edges_between_all(sources, targets)]
             )
             matrix[row][col] = float(weight)
 
     return matrix
 
 
 def _parse_labels(graph: Graph, labels: Union[List[Node], List[str]]) -> List[Node]:
     """Parse matrix labels into a list of nodes."""
     nodes: List[Node] = [
-        label
-        if isinstance(label, Node)
-        else graph.node_dict.get(str(label), Node(str(label)))
+        label if isinstance(label, Node) else graph.node_dict.get(str(label), Node(str(label)))
         for label in labels
     ]
 
     for node in nodes:
         graph.add_node(node)  # Skips existing identical nodes.
 
     return nodes
```

### Comparing `ragraph-1.17.0/ragraph/io/xml/XMI-Canonical.xsd` & `ragraph-1.17.1/ragraph/io/xml/XMI-Canonical.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/io/xml/__init__.py` & `ragraph-1.17.1/ragraph/io/xml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """XML format support using the XML Metadata Interchange (XMI) standard."""
 import shutil
 import uuid as _uuid
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from lxml import etree
+
 from ragraph.edge import Edge
 from ragraph.generic import Annotations, Metadata
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 here = Path(__file__).parent
 schema_doc = etree.parse(str(here / "ragraph.xsd"))
@@ -36,17 +37,17 @@
 
     uuid = etree.SubElement(elem, "uuid")
     uuid.text = str(obj.uuid)
 
     kind = etree.SubElement(elem, "kind")
     kind.text = obj.kind
 
-    for l in obj.labels:
+    for lab in obj.labels:
         label = etree.SubElement(elem, "label")
-        label.text = l
+        label.text = lab
 
     for k, v in obj.weights.items():
         weight = etree.SubElement(elem, q_weight, attrib=dict(value=str(v)))
         weight.text = k
 
     elem.extend(_annotations_to_elements(obj.annotations))
 
@@ -189,17 +190,15 @@
 
     return annots
 
 
 def _elements_to_weights(elems: Iterable[etree.Element]) -> Dict[str, Any]:
     """Convert XML elements of rc:Weight type to a weights dictionary."""
     weights = {
-        e.text: float(e.attrib["value"])
-        if "." in e.attrib["value"]
-        else int(e.attrib["value"])
+        e.text: float(e.attrib["value"]) if "." in e.attrib["value"] else int(e.attrib["value"])
         for e in elems
     }
     return weights
 
 
 def _element_to_metadata(elem: etree.Element, obj: Metadata):
     """Extract metadata from element."""
@@ -219,17 +218,15 @@
     parent = elem.find("parent")
     if parent is not None:
         node._parent = parent.text
 
     node._children = [i.text for i in elem.findall("child")]
 
     node.is_bus = (
-        elem.find("is_bus").text.lower() == "true"
-        if elem.find("is_bus") is not None
-        else False
+        elem.find("is_bus").text.lower() == "true" if elem.find("is_bus") is not None else False
     )
 
     return node
 
 
 def _element_to_edge(elem: etree.Element, node_dict: Dict[str, Any]) -> Edge:
     """Convert an XML element to an Edge object."""
@@ -243,15 +240,15 @@
 def _resolve_node_references(node_dict: Dict[str, Node]):
     """Resolve parent/child nodal string references from names to nodes."""
     for k, v in node_dict.items():
         if isinstance(v._parent, str):
             v._parent = node_dict[v._parent]
         if v._children:
             if isinstance(v._children[0], str):
-                v._children = [node_dict[c] for c in v._children]
+                v._children = [node_dict[c] for c in v._children]  # type: ignore
 
 
 def from_xml(
     path: Optional[Union[str, Path]] = None,
     enc: Optional[str] = None,
     elem: Optional[etree.Element] = None,
     validate: bool = True,
@@ -275,17 +272,15 @@
     if path is not None:
         elem = etree.parse(str(Path(path))).getroot()
     elif enc is not None:
         elem = etree.fromstring(enc)
     elif elem is not None:
         assert isinstance(elem, etree._Element)
     else:
-        raise ValueError(
-            "At least one of the 'path', 'enc', or 'elem' arguments should be set."
-        )
+        raise ValueError("At least one of the 'path', 'enc', or 'elem' arguments should be set.")
 
     # Validate if required.
     if validate and not schema.validate(elem):
         raise ValueError(f"Schema validation failed: \n\n{schema.error_log}")
 
     # Find the Graph XML element.
     g = elem.find(f".//{q_graph}")
```

### Comparing `ragraph-1.17.0/ragraph/io/xml/ragraph.xsd` & `ragraph-1.17.1/ragraph/io/xml/ragraph.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.17.0/ragraph/io/yaml.py` & `ragraph-1.17.1/ragraph/io/yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from ruamel_yaml import YAML
 except ImportError:
     from ruamel.yaml import YAML
 
 yaml = YAML(typ="safe")
 
 
-def from_yaml(
-    path: Optional[Union[str, Path]] = None, enc: Optional[str] = None
-) -> Graph:
+def from_yaml(path: Optional[Union[str, Path]] = None, enc: Optional[str] = None) -> Graph:
     """Decode YAML file or string into a Graph.
 
     Arguments:
         path: YAML file path.
         enc: YAML encoded string.
 
     Returns:
```

### Comparing `ragraph-1.17.0/ragraph/node.py` & `ragraph-1.17.1/ragraph/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,17 +74,15 @@
         """Parent node. Defaults to `None`."""
         return self._parent
 
     @parent.setter
     def parent(self, value: Optional["Node"]):
         # Check type.
         if value is not None and not isinstance(value, Node):
-            raise TypeError(
-                "Parent should be of type {}, got {}.".format(Node, type(value))
-            )
+            raise TypeError("Parent should be of type {}, got {}.".format(Node, type(value)))
         previous = getattr(self, "_parent")
         if previous is not None:
             # Previous parent, need to unset first!
             previous._children.remove(self)
             self._parent = None
         if value is not None:
             # Re-set if value is not None.
@@ -113,17 +111,15 @@
         """Whether this node is a bus node for its parent."""
         return self._is_bus
 
     @is_bus.setter
     def is_bus(self, value: bool):
         value = bool(value)
         if value and not self._parent:
-            raise ValueError(
-                "Cannot be a bus without a parent to be it for. Set a parent first!"
-            )
+            raise ValueError("Cannot be a bus without a parent to be it for. Set a parent first!")
         self._is_bus = bool(value)
 
     @property
     def ancestors(self) -> List["Node"]:
         """Get all ancestors of this node."""
         return list(self.ancestor_gen)
```

### Comparing `ragraph-1.17.0/ragraph/plot/__init__.py` & `ragraph-1.17.1/ragraph/plot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,24 +112,20 @@
     grid = utils.get_mdm_grid(leafs=leafs, edges=edges, style=style)
 
     fig = utils.get_subplots(grid, style=style)
 
     return utils.process_fig(fig=fig, show=show, style=style)
 
 
-def delta_dsm(
-    g1: Graph, g2: Graph, *args, style: Style = Style(), **kwargs
-) -> go.Figure:
+def delta_dsm(g1: Graph, g2: Graph, *args, style: Style = Style(), **kwargs) -> go.Figure:
     """Get a delta-DSM plot between two Graph objects."""
     raise NotImplementedError()
 
 
-def sigma_dsm(
-    graphs: Iterable[Graph], *args, style: Style = Style(), **kwargs
-) -> go.Figure:
+def sigma_dsm(graphs: Iterable[Graph], *args, style: Style = Style(), **kwargs) -> go.Figure:
     """Get a sigma-DSM plot of any number of Graph objects."""
     raise NotImplementedError()
 
 
 def network(g: Graph, *args, style: Style = Style(), **kwargs) -> go.Figure:
     """Get a network plot of a Graph object."""
     raise NotImplementedError()
```

### Comparing `ragraph-1.17.0/ragraph/plot/components/blank.py` & `ragraph-1.17.1/ragraph/plot/components/blank.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     """Blank plot component
 
     Arguments:
         style: Plot style mapping.
     """
 
     def __init__(self, style=Style()):
-
         trace = go.Scatter(
             x=[0.5 * style.xstep],
             y=[0.5 * style.ystep],
             mode="markers",
             marker=dict(
                 line=dict(
                     color="#FFFFFF",
```

### Comparing `ragraph-1.17.0/ragraph/plot/components/labels.py` & `ragraph-1.17.1/ragraph/plot/components/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,20 @@
         elif style.labels.shorten:
             short_labels = [style.labels.shorten(label) for label in labels]
         else:
             short_labels = labels
 
         label_length = max(len(label) for label in short_labels)
         fontsize = (
-            int(0.6 * style.boxsize)
-            if style.labels.fontsize is None
-            else style.labels.fontsize
+            int(0.6 * style.boxsize) if style.labels.fontsize is None else style.labels.fontsize
         )
 
         if style.labels.textorientation == "vertical":
             height = (
-                label_length * fontsize * style.labels.fontaspectratio
-                + 0.3 * style.boxsize
+                label_length * fontsize * style.labels.fontaspectratio + 0.3 * style.boxsize
             )  # Text width plus 0.3 boxsize as margin.
 
             num = len(leafs)
             xmax = num * style.xstep
             width = xmax * style.boxsize
 
             xdata = [(i + 0.5) * style.xstep for i in range(num)]
@@ -67,16 +64,15 @@
                 range=[-0.5 * height / style.boxsize, 0.5 * height / style.boxsize],
                 scaleanchor="x",
                 scaleratio=1.0,
             )
         else:
             # Default option.
             width = (
-                label_length * fontsize * style.labels.fontaspectratio
-                + 0.5 * style.boxsize
+                label_length * fontsize * style.labels.fontaspectratio + 0.5 * style.boxsize
             )  # Text width plus 0.3 boxsize as margin.
 
             num = len(leafs)
             ymax = num * style.ystep
             height = ymax * style.boxsize
 
             xdata = num * [0.5 * width / style.boxsize]
```

### Comparing `ragraph-1.17.0/ragraph/plot/components/legend.py` & `ragraph-1.17.1/ragraph/plot/components/legend.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,18 @@
             # create categorical legend:
             categories = style.piemap.fields or get_legend_categories(
                 edges=edges, display=style.piemap.display
             )
 
             max_label_length = max(len(cat) for cat in categories)
             fontsize = (
-                int(0.6 * style.boxsize)
-                if style.legend.fontsize is None
-                else style.legend.fontsize
+                int(0.6 * style.boxsize) if style.legend.fontsize is None else style.legend.fontsize
             )
             width = (
-                max_label_length * fontsize * style.legend.fontaspectratio
-                + 1 * style.boxsize
+                max_label_length * fontsize * style.legend.fontaspectratio + 1 * style.boxsize
             )  # Text width plus 2 box sizes as margin.
 
             traces = get_categorical_legend_traces(categories=categories, style=style)
             xaxis, yaxis = deepcopy(style.legend.xaxis), deepcopy(style.legend.yaxis)
             num = len(categories)
             xaxis.update(
                 range=[0, (width / style.boxsize) * style.xstep],
@@ -62,17 +59,15 @@
             weight_labels = style.piemap.fields or get_legend_categories(
                 edges=edges, display="weight labels"
             )
 
             max_label_length = max(len(label) for label in weight_labels)
 
             fontsize = (
-                int(0.6 * style.boxsize)
-                if style.legend.fontsize is None
-                else style.legend.fontsize
+                int(0.6 * style.boxsize) if style.legend.fontsize is None else style.legend.fontsize
             )
 
             width = 2.5 * style.xstep * len(weight_labels) * style.boxsize
             xaxis.update(
                 range=[0, width / style.boxsize * style.xstep],
                 scaleanchor="y",
                 scaleratio=1.0,
@@ -104,19 +99,15 @@
     traces = []
     x0 = 0.5
     y0 = (len(categories) - 0.5) * style.ystep
 
     xdata = []
     ydata = []
 
-    fontsize = (
-        int(0.6 * style.boxsize)
-        if style.legend.fontsize is None
-        else style.legend.fontsize
-    )
+    fontsize = int(0.6 * style.boxsize) if style.legend.fontsize is None else style.legend.fontsize
 
     for idx, cat in enumerate(categories):
         y = y0 - idx * style.ystep
         color = style.palettes.get_categorical_color(idx, field=cat)
         traces.append(
             go.Scatter(
                 x=[x0],
@@ -201,33 +192,24 @@
                 marker=dict(size=0),
                 fillcolor=color,
                 line=dict(color=color),
                 showlegend=False,
             )
         )
 
-    fontsize = (
-        int(0.6 * style.boxsize)
-        if style.legend.fontsize is None
-        else style.legend.fontsize
-    )
+    fontsize = int(0.6 * style.boxsize) if style.legend.fontsize is None else style.legend.fontsize
 
     if style.legend.n_ticks >= 2:
         n = style.legend.n_ticks
         tick_step = (max_value - min_value) / (n - 1)
         traces.append(
             go.Scatter(
                 x=[x + 0.5 * style.xstep for step in range(n)],
-                y=[
-                    style.ystep + step * style.legend.height / (n - 1)
-                    for step in range(n)
-                ],
-                text=[
-                    "{:.1f}".format(min_value + step * tick_step) for step in range(n)
-                ],
+                y=[style.ystep + step * style.legend.height / (n - 1) for step in range(n)],
+                text=["{:.1f}".format(min_value + step * tick_step) for step in range(n)],
                 showlegend=False,
                 mode="text",
                 textfont=dict(
                     color=style.legend.fontcolor,
                     family=style.legend.fontfamily,
                     size=0.7 * fontsize,
                 ),
@@ -250,17 +232,15 @@
             ),
             hoverinfo="text",
         )
     )
     return traces
 
 
-def get_numerical_legend_traces(
-    edges: List[Edge], style: Style = Style()
-) -> List[go.Scatter]:
+def get_numerical_legend_traces(edges: List[Edge], style: Style = Style()) -> List[go.Scatter]:
     """Get traces for a numerical legend,
 
     Arguments:
         edges: List of edges that are displayed.
         style: Style object.
 
     Returns:
```

### Comparing `ragraph-1.17.0/ragraph/plot/components/piemap.py` & `ragraph-1.17.1/ragraph/plot/components/piemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from math import cos, pi, prod, sin
 from typing import Any, Dict, List, Tuple
 
 import plotly.graph_objs as go
+
 from ragraph import colors
 from ragraph.edge import Edge
 from ragraph.node import Node
 from ragraph.plot import svg
 from ragraph.plot.generic import Component, Style
 
 
@@ -74,17 +75,15 @@
             # Divide different node kinds by special lines.
             kind_shapes = _get_kind_shapes(rows, style)
 
         highlight_shapes = _get_highlight_shapes(rows, cols, style)
 
         # Combine all traces and shapes.
         traces = pie_traces
-        shapes = (
-            highlight_shapes + grid_shapes + pie_shapes + kind_shapes + hierarchy_shapes
-        )
+        shapes = highlight_shapes + grid_shapes + pie_shapes + kind_shapes + hierarchy_shapes
 
         dim = (len(rows), len(cols))
         xaxis, yaxis = deepcopy(style.piemap.xaxis), deepcopy(style.piemap.yaxis)
         xaxis.update(range=[0, dim[1]], scaleanchor="y", scaleratio=1.0)
         yaxis.update(range=[0, dim[0]])
 
         super().__init__(
@@ -108,22 +107,18 @@
     dim = (len(rows), len(cols))
 
     line = style.piemap.gridline
     xstep, ystep = style.xstep, style.ystep
 
     # Gridlines
     shapes = [
-        svg.get_line(
-            x0=0, x1=dim[1] * xstep, y0=i * ystep, y1=i * ystep, line=line
-        ).as_dict()
+        svg.get_line(x0=0, x1=dim[1] * xstep, y0=i * ystep, y1=i * ystep, line=line).as_dict()
         for i in range(dim[0] + 1)
     ] + [
-        svg.get_line(
-            x0=j * xstep, x1=j * xstep, y0=0, y1=dim[0] * ystep, line=line
-        ).as_dict()
+        svg.get_line(x0=j * xstep, x1=j * xstep, y0=0, y1=dim[0] * ystep, line=line).as_dict()
         for j in range(dim[1] + 1)
     ]
 
     if rows == cols:
         shapes += [
             svg.get_rectangle(
                 x0=i,
@@ -136,17 +131,15 @@
             ).as_dict()
             for i in range(dim[1])
         ]
 
     return shapes
 
 
-def _get_highlight_shapes(
-    rows: List[Node], cols: List[Node], style: Style
-) -> List[Dict[str, Any]]:
+def _get_highlight_shapes(rows: List[Node], cols: List[Node], style: Style) -> List[Dict[str, Any]]:
     """Get highlight bands for both rows and columns."""
     row_annot = (
         style.piemap.highlight_row_annotation
         if style.piemap.highlight_row_annotation
         else style.highlight_annotation
     )
     col_annot = (
@@ -247,17 +240,15 @@
             bundle = bundle_dict[source.name, target.name]
             if not bundle:
                 continue  # No edges here.
             field_values = fields_dict[source.name, target.name]
 
             # Equal angles if calculated else calculate relative ones.
             field_angles = (
-                _get_relative_angles(fields, field_values)
-                if equal_angles is None
-                else equal_angles
+                _get_relative_angles(fields, field_values) if equal_angles is None else equal_angles
             )
 
             # Get the scaled radius.
             radius = (
                 style.piemap.radius
                 if style.piemap.scale_weight is None
                 else style.piemap.radius
@@ -359,15 +350,15 @@
     if style_fields is not None:
         return style_fields
 
     display = style.piemap.display
     if display == "kinds":
         fields = set(e.kind for e in edges)
     elif display == "labels":
-        fields = set(l for e in edges for l in e.labels)
+        fields = set(label for e in edges for label in e.labels)
     elif display in {"weight labels", "weights"}:
         fields = set(wl for e in edges for wl in e.weights.keys())
     else:
         fields = set()
 
     return sorted(fields)
 
@@ -377,17 +368,15 @@
     if style.piemap.display == "weights":
         return
 
     if len(fields) > len(style.palettes.categorical):
         style.palettes.categorical = colors.get_categorical(len(fields))
 
 
-def _get_field_values(
-    edges: List[Edge], fields: List[str], style: Style
-) -> Dict[str, float]:
+def _get_field_values(edges: List[Edge], fields: List[str], style: Style) -> Dict[str, float]:
     """Get the field sums for the given edges according to the style."""
     field_map: Dict[str, float] = dict()
     if not edges:
         return field_map
 
     display = style.piemap.display
     if display == "kinds":
@@ -405,29 +394,25 @@
     elif display == "weight labels":
         field_map = {
             f: float(sum(f in e.weights for e in edges))
             for f in fields
             if sum(f in e.weights for e in edges)
         }
     elif display == "weights":
-        field_map = {
-            f: float(sum(e.weights.get(f, 0.0) for e in edges)) for f in fields
-        }
+        field_map = {f: float(sum(e.weights.get(f, 0.0) for e in edges)) for f in fields}
     else:
         field_map = dict(num=float(len(edges)))
     return field_map
 
 
 def _get_equal_angles(fields: List[str]) -> Dict[str, Tuple[float, float]]:
     """Get piechart angle dictionary."""
     delta = 2 * pi / len(fields)
     offset = pi / 2  # Start upright, then go clockwise for intuitive results.
-    return {
-        f: (offset - (i + 1) * delta, offset - i * delta) for i, f in enumerate(fields)
-    }
+    return {f: (offset - (i + 1) * delta, offset - i * delta) for i, f in enumerate(fields)}
 
 
 def _get_relative_angles(
     fields: List[str], sums: Dict[str, float]
 ) -> Dict[str, Tuple[float, float]]:
     """Get the field pie-chart angles given their value sums."""
     total = sum(abs(v) for v in sums.values())
@@ -653,7 +638,8 @@
         # Horizontal line.
         shapes.append(svg.get_line(x0=0, x1=dim, y0=y, y1=y, line=line).as_dict())
 
         # Vertical line.
         shapes.append(svg.get_line(x0=i, x1=i, y0=0, y1=dim, line=line).as_dict())
 
     return shapes
+    return shapes
```

### Comparing `ragraph-1.17.0/ragraph/plot/components/tree.py` & `ragraph-1.17.1/ragraph/plot/components/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,22 @@
         ancestors, depth, xdict, ydict = _get_data(leafs=leafs, style=style)
 
         node_trace = _get_node_trace(
             xdict=xdict,
             ydict=ydict,
             style=style,
         )
-        line_shapes = _get_line_shapes(
-            ancestors=ancestors, xdict=xdict, ydict=ydict, style=style
-        )
+        line_shapes = _get_line_shapes(ancestors=ancestors, xdict=xdict, ydict=ydict, style=style)
 
         # Calculating geometric boundaries.
         width = (depth + 1) * style.xstep * style.boxsize
         height = len(leafs) * style.ystep * style.boxsize
 
         xaxis, yaxis = deepcopy(style.tree.xaxis), deepcopy(style.tree.yaxis)
-        xaxis.update(
-            range=(-0.5, width / style.boxsize - 0.5), scaleanchor="y", scaleratio=1.0
-        )
+        xaxis.update(range=(-0.5, width / style.boxsize - 0.5), scaleanchor="y", scaleratio=1.0)
         yaxis.update(range=(0, height / style.boxsize))
 
         super().__init__(
             width=width,
             height=height,
             traces=[node_trace],
             shapes=line_shapes,
@@ -113,17 +109,15 @@
 
         parents = grandparents
         current_depth -= 1
 
     return processed_ancestors, tree_depth, xdict, ydict
 
 
-def _get_node_trace(
-    xdict: Dict[Node, float], ydict: Dict[Node, float], style: Style
-) -> go.Scatter:
+def _get_node_trace(xdict: Dict[Node, float], ydict: Dict[Node, float], style: Style) -> go.Scatter:
     """Get tree node trace from positional dictionaries. These are the 'dots'.
 
     Arguments:
       xdict: Dictionary of node to x position of tree nodes.
       ydict: Dictionary of node to y position of tree nodes.
       style: Plot style mapping.
 
@@ -215,13 +209,11 @@
         y = y1 + curve_delta
     elif y0 < y1:
         y = y1 - curve_delta
 
     x = x0 + curve_delta
 
     first_line = svg.get_line(x0=x0, x1=x0, y0=y0, y1=y, line=linestyle)
-    curve_line = svg.get_curvedline(
-        x0=x0, x1=x0, x2=x, y0=y, y1=y1, y2=y1, line=linestyle
-    )
+    curve_line = svg.get_curvedline(x0=x0, x1=x0, x2=x, y0=y, y1=y1, y2=y1, line=linestyle)
     second_line = svg.get_line(x0=x, x1=x1, y0=y1, y1=y1, line=linestyle)
 
     return [first_line, curve_line, second_line]
```

### Comparing `ragraph-1.17.0/ragraph/plot/generic.py` & `ragraph-1.17.1/ragraph/plot/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """RaGraph generic plotting classes such as :obj:`Component` and :obj:`Style`."""
 from copy import deepcopy
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from plotly import graph_objs as go
 from plotly.basedatatypes import BaseTraceType
+
 from ragraph import colors
 from ragraph.generic import Mapping, field
 from ragraph.plot import svg
 
 MODEBAR_BUTTONS = {
     "toImage",
     "sendDataToCloud",
@@ -248,17 +249,15 @@
         in the plot area. The :obj:`fields` argument is a filter on the possible
         values for that display mode. The :obj:`mode` argument then tunes how the wedges
         that make up the piecharts should be distributed. Most of the time, 'equal'
         gives the most predictable and clear results.
     """
 
     _defaults = dict(
-        busarea=svg.SVG(
-            fillcolor="rgba(150,150,150,0.2)", line=svg.Line(width=0), layer="below"
-        ),
+        busarea=svg.SVG(fillcolor="rgba(150,150,150,0.2)", line=svg.Line(width=0), layer="below"),
         clusterline=svg.Line(width=2, color="gray", dash="solid"),
         display="kinds",
         fields=None,
         gridline=svg.Line(color="#dfdfdf", width=2, dash="solid"),
         highlight_col_annotation=None,
         highlight_col_color=None,
         highlight_row_annotation=None,
@@ -473,17 +472,15 @@
         super().__init__(
             categorical=categorical,
             continuous=continuous,
             fields=fields,
             domains=domains,
         )
 
-    def get_categorical_palette(
-        self, field: Optional[str] = None
-    ) -> Union[str, List[str]]:
+    def get_categorical_palette(self, field: Optional[str] = None) -> Union[str, List[str]]:
         """Get a categorical color (palette). Might be an overridden color, colorlist,
         or the default palette for the given field."""
         palette = self.fields.get(field, self.categorical)
 
         # Handle when it's a dictionary/FieldPalette override.
         if isinstance(palette, dict) or isinstance(palette, FieldPalette):
             palette = palette.get("categorical", self.categorical)
@@ -895,15 +892,13 @@
     def xaxis(self) -> go.layout.XAxis:
         """Plotly X-axis options."""
 
     @field
     def yaxis(self) -> go.layout.YAxis:
         """Plotly Y-axis options."""
 
-    def get_figure(
-        self, style: Style = Style(), show: bool = True
-    ) -> Optional[go.Figure]:
+    def get_figure(self, style: Style = Style(), show: bool = True) -> Optional[go.Figure]:
         """Get a Plotly figure of this component alone."""
         from ragraph.plot.utils import get_subplots, process_fig
 
         fig = get_subplots([[self]], style=style)
         return process_fig(fig, style=style, show=show)
```

### Comparing `ragraph-1.17.0/ragraph/plot/svg.py` & `ragraph-1.17.1/ragraph/plot/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,17 +307,15 @@
 
     Returns:
         SVG shape mapping.
     """
     return SVG(type="rect", x0=x0, x1=x1, y0=y0, y1=y1, **kwargs)
 
 
-def get_wedge(
-    x: float, y: float, r: float, start_angle: float, end_angle: float, **kwargs
-) -> SVG:
+def get_wedge(x: float, y: float, r: float, start_angle: float, end_angle: float, **kwargs) -> SVG:
     """Get a wedge SVG mapping.
 
     Arguments:
         x: x position of the wedge center.
         y: y position of the wedge center.
         r: radius of the wedge.
         start_angle: Starting angle (radians) of the wedge.
```

### Comparing `ragraph-1.17.0/ragraph/plot/utils.py` & `ragraph-1.17.1/ragraph/plot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from ragraph.plot.components.labels import Labels
 from ragraph.plot.components.legend import Legend
 from ragraph.plot.components.piemap import PieMap
 from ragraph.plot.components.tree import Tree
 from ragraph.plot.generic import Component, Style
 
 
-def get_subplots(
-    components: List[List[Optional[Component]]], style=Style()
-) -> go.Figure:
+def get_subplots(components: List[List[Optional[Component]]], style=Style()) -> go.Figure:
     """Get a subplots :obj:`plotly.graph_objects.Figure` the given
 
     Arguments:
         components: Components to be laid out as subplots based on their width and
             height properties.
 
     Keyword arguments:
@@ -48,18 +46,15 @@
             default=1,
         )
         if any(col)
         else 1
         for col in components_t
     ]
 
-    widths = [
-        (x_max - x_min) * style.boxsize
-        for (x_max, x_min) in zip(max_x_ranges, min_x_ranges)
-    ]
+    widths = [(x_max - x_min) * style.boxsize for (x_max, x_min) in zip(max_x_ranges, min_x_ranges)]
 
     min_y_ranges = [
         min(
             [comp.yaxis.range[0] for comp in row if comp and comp.yaxis.range],
             default=0,
         )
         if any(row)
@@ -74,16 +69,15 @@
         )
         if any(row)
         else 1
         for row in components
     ]
 
     heights = [
-        (y_max - y_min) * style.boxsize
-        for (y_max, y_min) in zip(max_y_ranges, min_y_ranges)
+        (y_max - y_min) * style.boxsize for (y_max, y_min) in zip(max_y_ranges, min_y_ranges)
     ]
 
     fig = make_subplots(
         rows=rows,
         cols=cols,
         shared_xaxes=True,
         shared_yaxes=True,
@@ -138,17 +132,15 @@
             "height": sum(heights) + margin["t"] + margin["b"],
         }
     )
 
     return fig
 
 
-def process_fig(
-    fig: go.Figure, style: Style = Style(), show: bool = True
-) -> Optional[go.Figure]:
+def process_fig(fig: go.Figure, style: Style = Style(), show: bool = True) -> Optional[go.Figure]:
     """Show figure with config if :obj:`show` is set, otherwise return figure unchanged.
 
     Arguments:
         fig: Plotly figure.
         style: Style containing additional config.
         show: Whether to show the figure inline.
     """
```

### Comparing `ragraph-1.17.0/ragraph/utils.py` & `ragraph-1.17.1/ragraph/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,23 +70,15 @@
 
         if node.depth == depth - 1:
             yield from children
         else:
             yield from get_up_to_depth(children, depth)
 
 
-def is_dependent(
-    graph, lead_nodes: List[Node], node: Node, edge_kinds=Set[str]
-) -> bool:
+def is_dependent(graph, lead_nodes: List[Node], node: Node, edge_kinds=Set[str]) -> bool:
     """Check if a node is dependent on the lead node kind.
 
     E.g. an edge of the allowed kinds exists to or from the lead nodes.
     """
     return any(
-        True
-        for e in graph.edges_between_all(lead_nodes, [node])
-        if e.kind in edge_kinds
-    ) or any(
-        True
-        for e in graph.edges_between_all([node], lead_nodes)
-        if e.kind in edge_kinds
-    )
+        True for e in graph.edges_between_all(lead_nodes, [node]) if e.kind in edge_kinds
+    ) or any(True for e in graph.edges_between_all([node], lead_nodes) if e.kind in edge_kinds)
```

### Comparing `ragraph-1.17.0/PKG-INFO` & `ragraph-1.17.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ragraph
-Version: 1.17.0
+Version: 1.17.1
 Summary: Ratio graph handling in Python.
-Home-page: https://gitlab.com/ratio-case/python/ragraph
+Home-page: https://ragraph.ratio-case.nl
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +20,15 @@
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: plotly (>=5.7.0,<6.0.0)
 Requires-Dist: raesl ; extra == "esl" or extra == "all"
 Requires-Dist: ratio-genetic-py (>=0.3.0,<0.4.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Project-URL: Documentation, https://ragraph.ratio-case.nl
-Project-URL: Repository, https://gitlab.com/ratio-case/python/ragraph
+Project-URL: Repository, https://gitlab.com/ratio-case-os/python/ragraph
 Description-Content-Type: text/x-rst
 
 #######
 RaGraph
 #######
 
 RaGraph is a package to create, manipulate, and analyze graphs consisting of nodes and
@@ -43,53 +43,51 @@
 **********
 Quickstart
 **********
 
 Installation
 ============
 
-RaGraph can be installed using ``pip install ragraph`` for any Python version >=3.9. Or,
-for Poetry managed projects, use ``poetry add ragraph`` to add it as a dependency.
+RaGraph can be installed using ``pip install ragraph[all]`` for any Python version >=3.9. Or,
+for Poetry managed projects, use ``poetry add ragraph -E all`` to add it as a dependency.
 
 
 Using RaGraph
 =============
 
 RaGraph's primary use is working with Graph objects that contain Nodes and Eges between
 Nodes. See the `usage documentation <https://ragraph.ratio-case.nl/usage/index.html>`_
 for more info!
 
-
 ***************
 Developer guide
 ***************
 
 Python packaging information
 ============================
 
 This project is packaged using `poetry <https://python-poetry.org/>`_. Packaging
 information as well as dependencies are stored in `pyproject.toml <./pyproject.toml>`_.
 
-Installing the project and its development dependencies can be done using ``poetry install``.
-
-
-Invoke tasks
-============
-
-Most elemental maintenance tasks can be accomplished using
-[Invoke](https://www.pyinvoke.org/). After installing using ``poetry install`` and
-enabling the environment using ``poetry shell``, you can run all tasks using ``inv
-[taskname]`` or ``invoke [taskname]``. E.g. ``inv docs`` builds the documentation.
-
+Installing the project and its development dependencies can be done using ``poetry install -E all``.
 
 Versioning
 ==========
 
 This project uses `semantic versioning <https://semver.org>`_. Version increments are
 checked using `Raver <https://raver.ratio-case.nl>`_.
 
-
 Changelog
 =========
 
-Changelog format as described by https://keepachangelog.com/ has been adopted.
+Changelog format as described by https://keepachangelog.com/ has been adopted and can be reviewed `on this page <https://ragraph.ratio-case.nl/changelog.html>`.
+
+Tests
+=====
+
+Tests can be run using ``poetry run pytest``.
+
+Linting
+=======
+
+Linting config is included in `pyproject.toml <./pyproject.toml>`_ for both Black and Ruff.
```

