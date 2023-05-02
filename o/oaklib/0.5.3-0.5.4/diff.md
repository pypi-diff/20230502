# Comparing `tmp/oaklib-0.5.3.tar.gz` & `tmp/oaklib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.3.tar", max compression
+gzip compressed data, was "oaklib-0.5.4.tar", max compression
```

## Comparing `oaklib-0.5.3.tar` & `oaklib-0.5.4.tar`

### file list

```diff
@@ -1,269 +1,269 @@
--rw-r--r--   0        0        0    11357 2023-04-22 04:11:21.568200 oaklib-0.5.3/LICENSE
--rw-r--r--   0        0        0     7241 2023-04-22 04:11:21.568200 oaklib-0.5.3/README.md
--rw-r--r--   0        0        0     1865 2023-04-22 04:12:10.052633 oaklib-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/__init__.py
--rw-r--r--   0        0        0   190704 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      115 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0      562 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      118 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4537 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12159 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5155 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    25704 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0     6615 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13328 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14564 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2023-04-22 04:11:21.692201 oaklib-0.5.3/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15768 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    32727 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3607 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    45533 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    17625 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-04-22 04:11:21.696201 oaklib-0.5.3/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5588 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5602 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5996 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0     3332 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2179 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1053 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30434 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16240 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2532 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1238 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    35620 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/rustsim/__init__.py
--rw-r--r--   0        0        0    14065 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/rustsim/rustsim_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    34101 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21451 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36699 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   105396 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3283 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-04-22 04:11:21.700201 oaklib-0.5.3/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    13406 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8817 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      977 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13280 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    18964 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     1386 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7833 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1301 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2179 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     1391 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     1090 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0      563 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1666 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      525 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1408 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     7511 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/resource.py
--rw-r--r--   0        0        0    14395 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    11026 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3054 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1540 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-04-22 04:11:21.704201 oaklib-0.5.3/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14443 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22274 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2676 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-04-22 04:11:21.708201 oaklib-0.5.3/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     9068 1970-01-01 00:00:00.000000 oaklib-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 19:59:30.568183 oaklib-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7241 2023-05-02 19:59:30.568183 oaklib-0.5.4/README.md
+-rw-r--r--   0        0        0     1883 2023-05-02 20:00:18.725214 oaklib-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-05-02 19:59:30.688186 oaklib-0.5.4/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   193630 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12159 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5155 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    36266 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    11740 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13328 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14564 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15768 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    45533 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    17625 2023-05-02 19:59:30.692186 oaklib-0.5.4/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5614 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5602 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5996 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0     4563 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2179 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1053 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.696186 oaklib-0.5.4/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30434 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16240 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2532 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1238 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    35620 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/rustsim/__init__.py
+-rw-r--r--   0        0        0    14065 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/rustsim/rustsim_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    34101 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21451 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36699 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   106198 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    20557 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8830 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      977 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13681 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    18964 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     2638 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-05-02 19:59:30.700186 oaklib-0.5.4/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7511 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2087 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7906 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1301 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2208 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1130 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1432 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8084 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/resource.py
+-rw-r--r--   0        0        0    14739 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3419 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1540 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14443 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22274 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-05-02 19:59:30.704186 oaklib-0.5.4/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 oaklib-0.5.4/PKG-INFO
```

### Comparing `oaklib-0.5.3/LICENSE` & `oaklib-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/README.md` & `oaklib-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/pyproject.toml` & `oaklib-0.5.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.3"
+version = "v0.5.4"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
-curies = "^0.4.0"
-nxontology = "^0.4.0"
-pronto = "^2.5.0"
+curies = ">=0.4.0"
+pronto = ">=2.5.0"
 SPARQLWrapper = "*"
-SQLAlchemy = "^1.4.32"
-linkml-runtime = "^1.2.15"
-networkx = "^2.7.1"
-sssom-schema = "^0.11.0"
-sssom = "^0.3.26"
-ratelimit = "^2.2.1"
-appdirs = "^1.4.4"
-semsql = "^0.3.1"
-lark = "^1.1.2"
-kgcl-schema = "^0.3.5"
-funowl = "^0.1.12"
+SQLAlchemy = ">=1.4.32"
+linkml-runtime = ">=1.2.15"
+networkx = ">=2.7.1"
+sssom-schema = ">=0.11.0"
+sssom = ">=0.3.26"
+ratelimit = ">=2.2.1"
+appdirs = ">=1.4.4"
+semsql = ">=0.3.1"
+lark = ">=1.1.2"
+kgcl-schema = ">=0.3.5"
+funowl = ">=0.1.12"
 gilda = {version = "^0.10.1", optional = true}
 kgcl-rdflib = "^0.3.0"
-pystow = "^0.5.0"
+pystow = ">=0.5.0"
 class-resolver = ">=0.4.2"
-ontoportal-client = "0.0.3"
-bioregistry = "^0.6.35"
-prefixmaps = "^0.1.2"
-ols-client = "^0.1.1"
-pandas = "^1.5.1"
-linkml-renderer = "^0.1.2"
-airium = "^0.2.5"
+ontoportal-client = ">=0.0.3"
+bioregistry = ">=0.6.35"
+prefixmaps = ">=0.1.2"
+ols-client = ">=0.1.1"
+linkml-renderer = ">=0.1.2"
+airium = ">=0.2.5"
 ndex2 = "^3.5.0"
 rustsim = ">=0.1.6"
-upsetplot = "^0.8.0"
 pysolr = "^3.9.0"
-eutils = "^0.6.0"
-
+eutils = ">=0.6.0"
+requests-cache = "^1.0.1"
+click = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
-jupyter = "^1.0.0"
+pandas = ">=1.5.1"
+jupyter = ">=1.0.0"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-click = ">=4.4.0"
 myst-parser = ">=1.0.0"
 linkml = "^1.2.14"
 sphinxcontrib-mermaid = "^0.8.1"
 sphinx-copybutton = "0.5.1"
 coverage = "^6.3.2"
```

### Comparing `oaklib-0.5.3/src/oaklib/cli.py` & `oaklib-0.5.4/src/oaklib/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,14 +840,18 @@
 @click.option("--associations-type", "-G", help="Syntax of associations input")
 @click.option(
     "--preferred-language", "-l", help="Preferred language for labels and lexical elements"
 )
 @click.option(
     "--other-languages", multiple=True, help="Additional languages for labels and lexical elements"
 )
+@click.option(
+    "--requests-cache-db",
+    help="If specified, all http requests will be cached to this sqlite file",
+)
 @input_option
 @input_type_option
 @add_option
 @click.option(
     "--merge/--no-merge",
     default=False,
     show_default=True,
@@ -863,14 +867,15 @@
     merge: bool,
     associations: List,
     associations_type: str,
     save_as: str,
     autosave: bool,
     named_prefix_map,
     metamodel_mappings,
+    requests_cache_db,
     prefix,
     import_depth: Optional[int],
     **kwargs,
 ):
     """Run the oaklib Command Line.
 
     A subcommand must be passed - for example: ancestors, terms, ...
@@ -890,14 +895,18 @@
         logger.setLevel(logging.DEBUG)
     elif verbose == 1:
         logger.setLevel(logging.INFO)
     else:
         logger.setLevel(logging.WARNING)
     if quiet:
         logger.setLevel(logging.ERROR)
+    if requests_cache_db:
+        import requests_cache
+
+        requests_cache.install_cache(requests_cache_db)
     resource = OntologyResource()
     resource.slug = input
     settings.autosave = autosave
     for k, v in kwargs.items():
         if v is not None:
             logging.info(f"Setting {k}={v}")
             setattr(settings, k, v)
@@ -4067,68 +4076,137 @@
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingCsvWriter)
     writer.autolabel = autolabel
     writer.output = output
     actual_predicates = _process_predicates_arg(predicates)
     actual_association_predicates = _process_predicates_arg(association_predicates)
-    if isinstance(impl, AssociationProviderInterface):
-        curies = list(query_terms_iterator(terms, impl))
-        qs_it = impl.associations(
-            curies,
-            predicates=actual_association_predicates,
-            subject_closure_predicates=actual_predicates,
-        )
-        qo_it = impl.associations(
-            objects=curies,
-            predicates=actual_association_predicates,
-            object_closure_predicates=actual_predicates,
-        )
+    if not isinstance(impl, AssociationProviderInterface):
+        raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+    curies = list(query_terms_iterator(terms, impl))
+    qs_it = impl.associations(
+        curies,
+        predicates=actual_association_predicates,
+        subject_closure_predicates=actual_predicates,
+    )
+    qo_it = impl.associations(
+        objects=curies,
+        predicates=actual_association_predicates,
+        object_closure_predicates=actual_predicates,
+    )
+    if terms_role is None or terms_role == SubjectOrObjectRole.SUBJECT.value:
+        it = qs_it
+    elif terms_role == SubjectOrObjectRole.OBJECT.value:
+        it = qo_it
+    else:
+        logging.info("Using query terms to query both subject and object")
+        it = chain(qs_it, qo_it)
+    has_relationships = defaultdict(bool)
+    for assoc in it:
         if terms_role is None or terms_role == SubjectOrObjectRole.SUBJECT.value:
-            it = qs_it
+            has_relationships[assoc.subject] = True
         elif terms_role == SubjectOrObjectRole.OBJECT.value:
-            it = qo_it
+            has_relationships[assoc.object] = True
         else:
-            logging.info("Using query terms to query both subject and object")
-            it = chain(qs_it, qo_it)
-        has_relationships = defaultdict(bool)
-        for assoc in it:
-            if terms_role is None or terms_role == SubjectOrObjectRole.SUBJECT.value:
-                has_relationships[assoc.subject] = True
-            elif terms_role == SubjectOrObjectRole.OBJECT.value:
-                has_relationships[assoc.object] = True
-            else:
-                has_relationships[assoc.subject] = True
-                has_relationships[assoc.object] = True
-            if if_absent and if_absent == IfAbsent.absent_only.value:
-                continue
-            writer.emit(
-                assoc,
-                label_fields=["subject", "predicate", "object"],
-            )
+            has_relationships[assoc.subject] = True
+            has_relationships[assoc.object] = True
         if if_absent and if_absent == IfAbsent.absent_only.value:
-            for curie in curies:
-                if not has_relationships[curie]:
-                    writer.emit(
-                        dict(subject=curie, predicate=None, object=None),
-                        label_fields=["subject", "predicate", "object"],
-                    )
-        if set_value:
-            if len(actual_predicates) != 1:
-                raise ValueError(f"predicates={actual_predicates}, expected exactly one")
-            pred = actual_predicates[0]
-            changes = []
-            for curie in curies:
-                changes.append(
-                    kgcl.EdgeCreation(id="x", subject=curie, predicate=pred, object=set_value)
+            continue
+        writer.emit(
+            assoc,
+            label_fields=["subject", "predicate", "object"],
+        )
+    if if_absent and if_absent == IfAbsent.absent_only.value:
+        for curie in curies:
+            if not has_relationships[curie]:
+                writer.emit(
+                    dict(subject=curie, predicate=None, object=None),
+                    label_fields=["subject", "predicate", "object"],
                 )
-            _apply_changes(impl, changes)
+    if set_value:
+        if len(actual_predicates) != 1:
+            raise ValueError(f"predicates={actual_predicates}, expected exactly one")
+        pred = actual_predicates[0]
+        changes = []
+        for curie in curies:
+            changes.append(
+                kgcl.EdgeCreation(id="x", subject=curie, predicate=pred, object=set_value)
+            )
+        _apply_changes(impl, changes)
 
-    else:
+
+@main.command()
+@output_option
+@predicates_option
+@autolabel_option
+@output_type_option
+@output_option
+@if_absent_option
+@set_value_option
+@click.option(
+    "--association-predicates",
+    help="A comma-separated list of predicates for the association relation",
+)
+@click.option(
+    "--terms-role",
+    "-Q",
+    type=click.Choice([x.value for x in SubjectOrObjectRole]),
+    default=SubjectOrObjectRole.OBJECT.value,
+    show_default=True,
+    help="How to interpret query terms.",
+)
+@click.argument("terms", nargs=-1)
+def associations_matrix(
+    terms,
+    predicates: str,
+    association_predicates: str,
+    terms_role: str,
+    autolabel: bool,
+    output_type: str,
+    output: str,
+    if_absent: bool,
+    set_value: str,
+):
+    """
+    Co-annotation matrix query.
+
+    Example:
+    """
+    impl = settings.impl
+    writer = _get_writer(output_type, impl, StreamingCsvWriter)
+    writer.autolabel = autolabel
+    writer.output = output
+    actual_predicates = _process_predicates_arg(predicates)
+    actual_association_predicates = _process_predicates_arg(association_predicates)
+    if not isinstance(impl, AssociationProviderInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+    if "@" in terms:
+        ix = terms.index("@")
+        logging.info(f"Splitting terms into two, position = {ix}")
+        curies1 = list(query_terms_iterator(terms[0:ix], impl))
+        curies2 = list(query_terms_iterator(terms[ix + 1 :], impl))
+    else:
+        curies1 = list(query_terms_iterator(terms, impl))
+        curies2 = list(curies1)
+    if terms_role != SubjectOrObjectRole.OBJECT.value:
+        raise NotImplementedError("terms-role not yet supported")
+    pairs_it = impl.association_pairwise_coassociations(
+        curies1=curies1,
+        curies2=curies2,
+        predicates=actual_association_predicates,
+        subject_closure_predicates=actual_predicates,
+    )
+    for pair in pairs_it:
+        # TODO: more elegant way to handle this
+        pair.associations_for_subjects_in_common = None
+        writer.emit(
+            pair,
+            label_fields=["object1", "object2"],
+        )
+    writer.finish()
 
 
 @main.command()
 @output_option
 @predicates_option
 @autolabel_option
 @output_type_option
@@ -4350,36 +4428,51 @@
 
 @main.command()
 @output_option
 @predicates_option
 @autolabel_option
 @output_type_option
 @output_option
+@click.option("--old-date", help="Old date, in YYYY-MM-DD format")
+@click.option("--new-date", help="Old date, in YYYY-MM-DD format")
 @click.option("-g", "--associations", help="associations")
 @click.option("-X", "--other-associations", help="other associations")
 @click.option(
     "--group-by",
     help="One of: publications; primary_knowledge_source",
 )
 def diff_associations(
     predicates: str,
     autolabel: bool,
     output_type: str,
     output: str,
     group_by: str,
     associations: str,
     other_associations: str,
+    **kwargs,
 ):
     """
-    Diffs two association sources. EXPERIMENTAL.
+    Diffs two association sources.
+
+    Example:
 
-    This functionality may move out of core
+        runoak -i sqlite:obo:go  -G gaf  diff-associations \
+           --old-date ${date1} --new-date ${date2} \
+           -g  "${download_dir}/${group}-${date1}.gaf" \
+           -X "${download_dir}/${group}-${date2}.gaf" \
+           --group-by publications -p i,p \
+           -o "${group}-diff-${date1}-to-${date2}.tsv
+
+    See https://w3id.org/oak/association for the diff data model.
+
+    NOTE: This functionality may move out of core
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingCsvWriter)
+    writer.heterogeneous_keys = True
     writer.autolabel = autolabel
     writer.output = output
     actual_predicates = _process_predicates_arg(predicates)
     logging.info(f"Fetching parser for {settings.associations_type}")
     association_parser = get_association_parser(settings.associations_type)
     if not isinstance(impl, AssociationProviderInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
@@ -4405,14 +4498,17 @@
                 assocs1, assocs2, actual_predicates
             )
         elif group_by:
             raise ValueError(f"Unknown group-by: {group_by}")
         else:
             changes = differ.calculate_change_objects(assocs1, assocs2, actual_predicates)
         for change in changes:
+            if kwargs:
+                for k, v in kwargs.items():
+                    setattr(change, k, v)
             writer.emit(change, label_fields=["old_object", "new_object"])
     writer.finish()
 
 
 @main.command()
 @click.option(
     "--cutoff",
```

### Comparing `oaklib-0.5.3/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.4/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.5.4/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.4/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.4/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.4/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.4/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.4/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.4/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.4/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/association.py` & `oaklib-0.5.4/src/oaklib/datamodels/similarity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-# Auto generated from association.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-18T12:40:46
-# Schema: association
+# Auto generated from similarity.yaml by pythongen.py version: 0.9.0
+# Generation date: 2023-04-10T09:38:53
+# Schema: similarity
 #
-# id: https://w3id.org/oak/association
-# description: A datamodel for representing generic associations. The core datamodel is broad, encompassing the W3
-#              Open Annotation data model as well as common ontology annotation data models using in the
-#              biosciences.
+# id: https://w3id.org/oak/similarity
+# description: A datamodel for representing semantic similarity between terms or lists of terms.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
 import sys
 from dataclasses import dataclass
 from typing import Any, ClassVar, Dict, List, Optional, Union
 
 from jsonasobj2 import JsonObj, as_dict
 from linkml_runtime.linkml_model.meta import (
     EnumDefinition,
     PermissibleValue,
     PvFormulaOptions,
 )
-from linkml_runtime.linkml_model.types import Boolean, String, Uriorcurie
+from linkml_runtime.linkml_model.types import Float, Integer, String, Uriorcurie
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.utils.dataclass_extensions_376 import (
     dataclasses_init_fn_with_kwargs,
 )
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
-from linkml_runtime.utils.metamodelcore import (
-    Bool,
-    URIorCURIE,
-    bnode,
-    empty_dict,
-    empty_list,
-)
+from linkml_runtime.utils.metamodelcore import URIorCURIE, bnode, empty_dict, empty_list
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.yamlutils import (
     YAMLRoot,
     extended_float,
     extended_int,
     extended_str,
 )
@@ -46,688 +38,681 @@
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
-BIOLINK = CurieNamespace("biolink", "https://w3id.org/biolink/vocab/")
 LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
-OA = CurieNamespace("oa", "http://www.w3.org/ns/oa#")
-ONTOASSOC = CurieNamespace("ontoassoc", "https://w3id.org/oak/association/")
-RDF = CurieNamespace("rdf", "http://example.org/UNKNOWN/rdf/")
-SSSOM = CurieNamespace("sssom", "https://w3id.org/sssom/")
-DEFAULT_ = ONTOASSOC
+OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
+PAV = CurieNamespace("pav", "http://purl.org/pav/")
+PROV = CurieNamespace("prov", "http://www.w3.org/ns/prov#")
+RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
+RDFS = CurieNamespace("rdfs", "http://www.w3.org/2000/01/rdf-schema#")
+SCHEMA = CurieNamespace("schema", "http://schema.org/")
+SH = CurieNamespace("sh", "https://w3id.org/shacl/")
+SIM = CurieNamespace("sim", "https://w3id.org/linkml/similarity/")
+SKOS = CurieNamespace("skos", "http://www.w3.org/2004/02/skos/core#")
+SSSOM = CurieNamespace("sssom", "http://w3id.org/sssom/")
+XSD = CurieNamespace("xsd", "http://www.w3.org/2001/XMLSchema#")
+DEFAULT_ = SIM
 
 
 # Types
+class ZeroToOne(Float):
+    type_class_uri = XSD.float
+    type_class_curie = "xsd:float"
+    type_name = "ZeroToOne"
+    type_model_uri = SIM.ZeroToOne
+
+
+class NonNegativeFloat(Float):
+    type_class_uri = XSD.float
+    type_class_curie = "xsd:float"
+    type_name = "NonNegativeFloat"
+    type_model_uri = SIM.NonNegativeFloat
+
+
+class NegativeLogValue(Float):
+    type_class_uri = XSD.float
+    type_class_curie = "xsd:float"
+    type_name = "NegativeLogValue"
+    type_model_uri = SIM.NegativeLogValue
+
+
+class ItemCount(Integer):
+    type_class_uri = XSD.integer
+    type_class_curie = "xsd:integer"
+    type_name = "ItemCount"
+    type_model_uri = SIM.ItemCount
+
 
 # Class references
+class TermInfoId(extended_str):
+    pass
 
 
-@dataclass
-class Association(YAMLRoot):
+class BestMatchMatchSource(extended_str):
+    pass
+
+
+class PairwiseSimilarity(YAMLRoot):
     """
-    A generic association between a thing (subject) and another thing (object).
+    Abstract grouping for representing individual pairwise similarities
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OA.Annotation
-    class_class_curie: ClassVar[str] = "oa:Annotation"
-    class_name: ClassVar[str] = "Association"
-    class_model_uri: ClassVar[URIRef] = ONTOASSOC.Association
-
-    subject: Optional[Union[str, URIorCURIE]] = None
-    predicate: Optional[Union[str, URIorCURIE]] = None
-    object: Optional[Union[str, URIorCURIE]] = None
-    property_values: Optional[
-        Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]
-    ] = empty_list()
-    subject_label: Optional[str] = None
-    predicate_label: Optional[str] = None
-    object_label: Optional[str] = None
-    publications: Optional[
-        Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
-    ] = empty_list()
-    primary_knowledge_source: Optional[Union[str, URIorCURIE]] = None
-    aggregator_knowledge_source: Optional[Union[str, URIorCURIE]] = None
-
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.subject is not None and not isinstance(self.subject, URIorCURIE):
-            self.subject = URIorCURIE(self.subject)
-
-        if self.predicate is not None and not isinstance(self.predicate, URIorCURIE):
-            self.predicate = URIorCURIE(self.predicate)
-
-        if self.object is not None and not isinstance(self.object, URIorCURIE):
-            self.object = URIorCURIE(self.object)
-
-        if not isinstance(self.property_values, list):
-            self.property_values = (
-                [self.property_values] if self.property_values is not None else []
-            )
-        self.property_values = [
-            v if isinstance(v, PropertyValue) else PropertyValue(**as_dict(v))
-            for v in self.property_values
-        ]
-
-        if self.subject_label is not None and not isinstance(self.subject_label, str):
-            self.subject_label = str(self.subject_label)
-
-        if self.predicate_label is not None and not isinstance(self.predicate_label, str):
-            self.predicate_label = str(self.predicate_label)
-
-        if self.object_label is not None and not isinstance(self.object_label, str):
-            self.object_label = str(self.object_label)
-
-        if not isinstance(self.publications, list):
-            self.publications = [self.publications] if self.publications is not None else []
-        self.publications = [
-            v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.publications
-        ]
-
-        if self.primary_knowledge_source is not None and not isinstance(
-            self.primary_knowledge_source, URIorCURIE
-        ):
-            self.primary_knowledge_source = URIorCURIE(self.primary_knowledge_source)
-
-        if self.aggregator_knowledge_source is not None and not isinstance(
-            self.aggregator_knowledge_source, URIorCURIE
-        ):
-            self.aggregator_knowledge_source = URIorCURIE(self.aggregator_knowledge_source)
-
-        super().__post_init__(**kwargs)
+    class_class_uri: ClassVar[URIRef] = SIM.PairwiseSimilarity
+    class_class_curie: ClassVar[str] = "sim:PairwiseSimilarity"
+    class_name: ClassVar[str] = "PairwiseSimilarity"
+    class_model_uri: ClassVar[URIRef] = SIM.PairwiseSimilarity
 
 
 @dataclass
-class NegatedAssociation(YAMLRoot):
+class TermPairwiseSimilarity(PairwiseSimilarity):
     """
-    A negated association between a thing (subject) and another thing (object).
+    A simple pairwise similarity between two atomic concepts/terms
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOASSOC.NegatedAssociation
-    class_class_curie: ClassVar[str] = "ontoassoc:NegatedAssociation"
-    class_name: ClassVar[str] = "NegatedAssociation"
-    class_model_uri: ClassVar[URIRef] = ONTOASSOC.NegatedAssociation
-
-    subject: Optional[Union[str, URIorCURIE]] = None
-    predicate: Optional[Union[str, URIorCURIE]] = None
-    object: Optional[Union[str, URIorCURIE]] = None
-    property_values: Optional[
-        Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]
-    ] = empty_list()
+    class_class_uri: ClassVar[URIRef] = SIM.TermPairwiseSimilarity
+    class_class_curie: ClassVar[str] = "sim:TermPairwiseSimilarity"
+    class_name: ClassVar[str] = "TermPairwiseSimilarity"
+    class_model_uri: ClassVar[URIRef] = SIM.TermPairwiseSimilarity
+
+    subject_id: Union[str, URIorCURIE] = None
     subject_label: Optional[str] = None
-    predicate_label: Optional[str] = None
+    subject_source: Optional[str] = None
+    object_id: Optional[Union[str, URIorCURIE]] = None
     object_label: Optional[str] = None
-    publications: Optional[
-        Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
-    ] = empty_list()
-    primary_knowledge_source: Optional[Union[str, URIorCURIE]] = None
-    aggregator_knowledge_source: Optional[Union[str, URIorCURIE]] = None
+    object_source: Optional[str] = None
+    ancestor_id: Optional[Union[str, URIorCURIE]] = None
+    ancestor_label: Optional[str] = None
+    ancestor_source: Optional[str] = None
+    object_information_content: Optional[Union[float, NegativeLogValue]] = None
+    subject_information_content: Optional[Union[float, NegativeLogValue]] = None
+    ancestor_information_content: Optional[Union[float, NegativeLogValue]] = None
+    jaccard_similarity: Optional[Union[float, ZeroToOne]] = None
+    dice_similarity: Optional[Union[float, ZeroToOne]] = None
+    phenodigm_score: Optional[Union[float, NonNegativeFloat]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.subject is not None and not isinstance(self.subject, URIorCURIE):
-            self.subject = URIorCURIE(self.subject)
-
-        if self.predicate is not None and not isinstance(self.predicate, URIorCURIE):
-            self.predicate = URIorCURIE(self.predicate)
-
-        if self.object is not None and not isinstance(self.object, URIorCURIE):
-            self.object = URIorCURIE(self.object)
-
-        if not isinstance(self.property_values, list):
-            self.property_values = (
-                [self.property_values] if self.property_values is not None else []
-            )
-        self.property_values = [
-            v if isinstance(v, PropertyValue) else PropertyValue(**as_dict(v))
-            for v in self.property_values
-        ]
+        if self._is_empty(self.subject_id):
+            self.MissingRequiredField("subject_id")
+        if not isinstance(self.subject_id, URIorCURIE):
+            self.subject_id = URIorCURIE(self.subject_id)
 
         if self.subject_label is not None and not isinstance(self.subject_label, str):
             self.subject_label = str(self.subject_label)
 
-        if self.predicate_label is not None and not isinstance(self.predicate_label, str):
-            self.predicate_label = str(self.predicate_label)
+        if self.subject_source is not None and not isinstance(self.subject_source, str):
+            self.subject_source = str(self.subject_source)
+
+        if self.object_id is not None and not isinstance(self.object_id, URIorCURIE):
+            self.object_id = URIorCURIE(self.object_id)
 
         if self.object_label is not None and not isinstance(self.object_label, str):
             self.object_label = str(self.object_label)
 
-        if not isinstance(self.publications, list):
-            self.publications = [self.publications] if self.publications is not None else []
-        self.publications = [
-            v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.publications
-        ]
-
-        if self.primary_knowledge_source is not None and not isinstance(
-            self.primary_knowledge_source, URIorCURIE
-        ):
-            self.primary_knowledge_source = URIorCURIE(self.primary_knowledge_source)
+        if self.object_source is not None and not isinstance(self.object_source, str):
+            self.object_source = str(self.object_source)
 
-        if self.aggregator_knowledge_source is not None and not isinstance(
-            self.aggregator_knowledge_source, URIorCURIE
-        ):
-            self.aggregator_knowledge_source = URIorCURIE(self.aggregator_knowledge_source)
+        if self.ancestor_id is not None and not isinstance(self.ancestor_id, URIorCURIE):
+            self.ancestor_id = URIorCURIE(self.ancestor_id)
 
-        super().__post_init__(**kwargs)
+        if self.ancestor_label is not None and not isinstance(self.ancestor_label, str):
+            self.ancestor_label = str(self.ancestor_label)
 
+        if self.ancestor_source is not None and not isinstance(self.ancestor_source, str):
+            self.ancestor_source = str(self.ancestor_source)
 
-@dataclass
-class PropertyValue(YAMLRoot):
-    """
-    A generic tag-value that can be associated with an association.
-    """
+        if self.object_information_content is not None and not isinstance(
+            self.object_information_content, NegativeLogValue
+        ):
+            self.object_information_content = NegativeLogValue(self.object_information_content)
 
-    _inherited_slots: ClassVar[List[str]] = []
+        if self.subject_information_content is not None and not isinstance(
+            self.subject_information_content, NegativeLogValue
+        ):
+            self.subject_information_content = NegativeLogValue(self.subject_information_content)
 
-    class_class_uri: ClassVar[URIRef] = ONTOASSOC.PropertyValue
-    class_class_curie: ClassVar[str] = "ontoassoc:PropertyValue"
-    class_name: ClassVar[str] = "PropertyValue"
-    class_model_uri: ClassVar[URIRef] = ONTOASSOC.PropertyValue
+        if self.ancestor_information_content is not None and not isinstance(
+            self.ancestor_information_content, NegativeLogValue
+        ):
+            self.ancestor_information_content = NegativeLogValue(self.ancestor_information_content)
 
-    predicate: Optional[Union[str, URIorCURIE]] = None
-    object: Optional[Union[str, URIorCURIE]] = None
+        if self.jaccard_similarity is not None and not isinstance(
+            self.jaccard_similarity, ZeroToOne
+        ):
+            self.jaccard_similarity = ZeroToOne(self.jaccard_similarity)
 
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.predicate is not None and not isinstance(self.predicate, URIorCURIE):
-            self.predicate = URIorCURIE(self.predicate)
+        if self.dice_similarity is not None and not isinstance(self.dice_similarity, ZeroToOne):
+            self.dice_similarity = ZeroToOne(self.dice_similarity)
 
-        if self.object is not None and not isinstance(self.object, URIorCURIE):
-            self.object = URIorCURIE(self.object)
+        if self.phenodigm_score is not None and not isinstance(
+            self.phenodigm_score, NonNegativeFloat
+        ):
+            self.phenodigm_score = NonNegativeFloat(self.phenodigm_score)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class RollupGroup(YAMLRoot):
+class TermSetPairwiseSimilarity(PairwiseSimilarity):
+    """
+    A simple pairwise similarity between two sets of concepts/terms
+    """
+
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOASSOC.RollupGroup
-    class_class_curie: ClassVar[str] = "ontoassoc:RollupGroup"
-    class_name: ClassVar[str] = "RollupGroup"
-    class_model_uri: ClassVar[URIRef] = ONTOASSOC.RollupGroup
-
-    group_object: Optional[Union[str, URIorCURIE]] = None
-    sub_groups: Optional[
-        Union[Union[dict, "RollupGroup"], List[Union[dict, "RollupGroup"]]]
-    ] = empty_list()
-    associations: Optional[
-        Union[Union[dict, Association], List[Union[dict, Association]]]
-    ] = empty_list()
+    class_class_uri: ClassVar[URIRef] = SIM.TermSetPairwiseSimilarity
+    class_class_curie: ClassVar[str] = "sim:TermSetPairwiseSimilarity"
+    class_name: ClassVar[str] = "TermSetPairwiseSimilarity"
+    class_model_uri: ClassVar[URIRef] = SIM.TermSetPairwiseSimilarity
+
+    subject_termset: Optional[
+        Union[Dict[Union[str, TermInfoId], Union[dict, "TermInfo"]], List[Union[dict, "TermInfo"]]]
+    ] = empty_dict()
+    object_termset: Optional[
+        Union[Dict[Union[str, TermInfoId], Union[dict, "TermInfo"]], List[Union[dict, "TermInfo"]]]
+    ] = empty_dict()
+    subject_best_matches: Optional[
+        Union[
+            Dict[Union[str, BestMatchMatchSource], Union[dict, "BestMatch"]],
+            List[Union[dict, "BestMatch"]],
+        ]
+    ] = empty_dict()
+    object_best_matches: Optional[
+        Union[
+            Dict[Union[str, BestMatchMatchSource], Union[dict, "BestMatch"]],
+            List[Union[dict, "BestMatch"]],
+        ]
+    ] = empty_dict()
+    average_score: Optional[float] = None
+    best_score: Optional[float] = None
+    metric: Optional[Union[str, URIorCURIE]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.group_object is not None and not isinstance(self.group_object, URIorCURIE):
-            self.group_object = URIorCURIE(self.group_object)
+        self._normalize_inlined_as_dict(
+            slot_name="subject_termset", slot_type=TermInfo, key_name="id", keyed=True
+        )
+
+        self._normalize_inlined_as_dict(
+            slot_name="object_termset", slot_type=TermInfo, key_name="id", keyed=True
+        )
+
+        self._normalize_inlined_as_dict(
+            slot_name="subject_best_matches",
+            slot_type=BestMatch,
+            key_name="match_source",
+            keyed=True,
+        )
+
+        self._normalize_inlined_as_dict(
+            slot_name="object_best_matches",
+            slot_type=BestMatch,
+            key_name="match_source",
+            keyed=True,
+        )
 
-        if not isinstance(self.sub_groups, list):
-            self.sub_groups = [self.sub_groups] if self.sub_groups is not None else []
-        self.sub_groups = [
-            v if isinstance(v, RollupGroup) else RollupGroup(**as_dict(v)) for v in self.sub_groups
-        ]
+        if self.average_score is not None and not isinstance(self.average_score, float):
+            self.average_score = float(self.average_score)
 
-        if not isinstance(self.associations, list):
-            self.associations = [self.associations] if self.associations is not None else []
-        self.associations = [
-            v if isinstance(v, Association) else Association(**as_dict(v))
-            for v in self.associations
-        ]
+        if self.best_score is not None and not isinstance(self.best_score, float):
+            self.best_score = float(self.best_score)
+
+        if self.metric is not None and not isinstance(self.metric, URIorCURIE):
+            self.metric = URIorCURIE(self.metric)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class ParserConfiguration(YAMLRoot):
+class TermInfo(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOASSOC.ParserConfiguration
-    class_class_curie: ClassVar[str] = "ontoassoc:ParserConfiguration"
-    class_name: ClassVar[str] = "ParserConfiguration"
-    class_model_uri: ClassVar[URIRef] = ONTOASSOC.ParserConfiguration
-
-    preserve_negated_associations: Optional[Union[bool, Bool]] = None
-    include_association_attributes: Optional[Union[bool, Bool]] = None
-    primary_knowledge_source: Optional[Union[str, URIorCURIE]] = None
-    aggregator_knowledge_source: Optional[Union[str, URIorCURIE]] = None
+    class_class_uri: ClassVar[URIRef] = SIM.TermInfo
+    class_class_curie: ClassVar[str] = "sim:TermInfo"
+    class_name: ClassVar[str] = "TermInfo"
+    class_model_uri: ClassVar[URIRef] = SIM.TermInfo
 
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.preserve_negated_associations is not None and not isinstance(
-            self.preserve_negated_associations, Bool
-        ):
-            self.preserve_negated_associations = Bool(self.preserve_negated_associations)
-
-        if self.include_association_attributes is not None and not isinstance(
-            self.include_association_attributes, Bool
-        ):
-            self.include_association_attributes = Bool(self.include_association_attributes)
+    id: Union[str, TermInfoId] = None
+    label: Optional[str] = None
 
-        if self.primary_knowledge_source is not None and not isinstance(
-            self.primary_knowledge_source, URIorCURIE
-        ):
-            self.primary_knowledge_source = URIorCURIE(self.primary_knowledge_source)
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, TermInfoId):
+            self.id = TermInfoId(self.id)
 
-        if self.aggregator_knowledge_source is not None and not isinstance(
-            self.aggregator_knowledge_source, URIorCURIE
-        ):
-            self.aggregator_knowledge_source = URIorCURIE(self.aggregator_knowledge_source)
+        if self.label is not None and not isinstance(self.label, str):
+            self.label = str(self.label)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class AssociationChange(YAMLRoot):
+class BestMatch(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOASSOC.AssociationChange
-    class_class_curie: ClassVar[str] = "ontoassoc:AssociationChange"
-    class_name: ClassVar[str] = "AssociationChange"
-    class_model_uri: ClassVar[URIRef] = ONTOASSOC.AssociationChange
-
-    summary_group: Optional[str] = None
-    publications: Optional[
-        Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
-    ] = empty_list()
-    publication_is_added: Optional[Union[bool, Bool]] = None
-    publication_is_deleted: Optional[Union[bool, Bool]] = None
-    subject: Optional[Union[str, URIorCURIE]] = None
-    old_predicate: Optional[Union[str, URIorCURIE]] = None
-    new_predicate: Optional[Union[str, URIorCURIE]] = None
-    old_object: Optional[Union[str, URIorCURIE]] = None
-    new_object: Optional[Union[str, URIorCURIE]] = None
-    old_object_obsolete: Optional[Union[bool, Bool]] = None
-    is_migration: Optional[Union[bool, Bool]] = None
-    is_generalization: Optional[Union[bool, Bool]] = None
-    is_specialization: Optional[Union[bool, Bool]] = None
-    is_creation: Optional[Union[bool, Bool]] = None
-    is_deletion: Optional[Union[bool, Bool]] = None
-    closure_predicates: Optional[
-        Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
-    ] = empty_list()
+    class_class_uri: ClassVar[URIRef] = SIM.BestMatch
+    class_class_curie: ClassVar[str] = "sim:BestMatch"
+    class_name: ClassVar[str] = "BestMatch"
+    class_model_uri: ClassVar[URIRef] = SIM.BestMatch
+
+    match_source: Union[str, BestMatchMatchSource] = None
+    score: float = None
+    similarity: Union[dict, TermPairwiseSimilarity] = None
+    match_source_label: Optional[str] = None
+    match_target: Optional[str] = None
+    match_target_label: Optional[str] = None
+    match_subsumer: Optional[Union[str, URIorCURIE]] = None
+    match_subsumer_label: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.summary_group is not None and not isinstance(self.summary_group, str):
-            self.summary_group = str(self.summary_group)
-
-        if not isinstance(self.publications, list):
-            self.publications = [self.publications] if self.publications is not None else []
-        self.publications = [
-            v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.publications
-        ]
-
-        if self.publication_is_added is not None and not isinstance(
-            self.publication_is_added, Bool
-        ):
-            self.publication_is_added = Bool(self.publication_is_added)
-
-        if self.publication_is_deleted is not None and not isinstance(
-            self.publication_is_deleted, Bool
-        ):
-            self.publication_is_deleted = Bool(self.publication_is_deleted)
-
-        if self.subject is not None and not isinstance(self.subject, URIorCURIE):
-            self.subject = URIorCURIE(self.subject)
-
-        if self.old_predicate is not None and not isinstance(self.old_predicate, URIorCURIE):
-            self.old_predicate = URIorCURIE(self.old_predicate)
-
-        if self.new_predicate is not None and not isinstance(self.new_predicate, URIorCURIE):
-            self.new_predicate = URIorCURIE(self.new_predicate)
-
-        if self.old_object is not None and not isinstance(self.old_object, URIorCURIE):
-            self.old_object = URIorCURIE(self.old_object)
-
-        if self.new_object is not None and not isinstance(self.new_object, URIorCURIE):
-            self.new_object = URIorCURIE(self.new_object)
-
-        if self.old_object_obsolete is not None and not isinstance(self.old_object_obsolete, Bool):
-            self.old_object_obsolete = Bool(self.old_object_obsolete)
-
-        if self.is_migration is not None and not isinstance(self.is_migration, Bool):
-            self.is_migration = Bool(self.is_migration)
+        if self._is_empty(self.match_source):
+            self.MissingRequiredField("match_source")
+        if not isinstance(self.match_source, BestMatchMatchSource):
+            self.match_source = BestMatchMatchSource(self.match_source)
+
+        if self._is_empty(self.score):
+            self.MissingRequiredField("score")
+        if not isinstance(self.score, float):
+            self.score = float(self.score)
+
+        if self._is_empty(self.similarity):
+            self.MissingRequiredField("similarity")
+        if not isinstance(self.similarity, TermPairwiseSimilarity):
+            self.similarity = TermPairwiseSimilarity(**as_dict(self.similarity))
+
+        if self.match_source_label is not None and not isinstance(self.match_source_label, str):
+            self.match_source_label = str(self.match_source_label)
+
+        if self.match_target is not None and not isinstance(self.match_target, str):
+            self.match_target = str(self.match_target)
 
-        if self.is_generalization is not None and not isinstance(self.is_generalization, Bool):
-            self.is_generalization = Bool(self.is_generalization)
+        if self.match_target_label is not None and not isinstance(self.match_target_label, str):
+            self.match_target_label = str(self.match_target_label)
 
-        if self.is_specialization is not None and not isinstance(self.is_specialization, Bool):
-            self.is_specialization = Bool(self.is_specialization)
+        if self.match_subsumer is not None and not isinstance(self.match_subsumer, URIorCURIE):
+            self.match_subsumer = URIorCURIE(self.match_subsumer)
 
-        if self.is_creation is not None and not isinstance(self.is_creation, Bool):
-            self.is_creation = Bool(self.is_creation)
-
-        if self.is_deletion is not None and not isinstance(self.is_deletion, Bool):
-            self.is_deletion = Bool(self.is_deletion)
-
-        if not isinstance(self.closure_predicates, list):
-            self.closure_predicates = (
-                [self.closure_predicates] if self.closure_predicates is not None else []
-            )
-        self.closure_predicates = [
-            v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.closure_predicates
-        ]
+        if self.match_subsumer_label is not None and not isinstance(self.match_subsumer_label, str):
+            self.match_subsumer_label = str(self.match_subsumer_label)
 
         super().__post_init__(**kwargs)
 
 
 # Enumerations
 
 
 # Slots
 class slots:
     pass
 
 
-slots.subject = Slot(
-    uri=RDF.subject,
-    name="subject",
-    curie=RDF.curie("subject"),
-    model_uri=ONTOASSOC.subject,
+slots.subject_id = Slot(
+    uri=SSSOM.subject_id,
+    name="subject_id",
+    curie=SSSOM.curie("subject_id"),
+    model_uri=SIM.subject_id,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Union[str, URIorCURIE],
 )
 
 slots.subject_label = Slot(
     uri=SSSOM.subject_label,
     name="subject_label",
     curie=SSSOM.curie("subject_label"),
-    model_uri=ONTOASSOC.subject_label,
+    model_uri=SIM.subject_label,
     domain=None,
     range=Optional[str],
 )
 
-slots.predicate = Slot(
-    uri=RDF.predicate,
-    name="predicate",
-    curie=RDF.curie("predicate"),
-    model_uri=ONTOASSOC.predicate,
-    domain=None,
-    range=Optional[Union[str, URIorCURIE]],
-)
-
-slots.predicate_label = Slot(
-    uri=SSSOM.predicate_label,
-    name="predicate_label",
-    curie=SSSOM.curie("predicate_label"),
-    model_uri=ONTOASSOC.predicate_label,
+slots.subject_source = Slot(
+    uri=SSSOM.subject_source,
+    name="subject_source",
+    curie=SSSOM.curie("subject_source"),
+    model_uri=SIM.subject_source,
     domain=None,
     range=Optional[str],
 )
 
-slots.object = Slot(
-    uri=RDF.object,
-    name="object",
-    curie=RDF.curie("object"),
-    model_uri=ONTOASSOC.object,
+slots.object_id = Slot(
+    uri=SSSOM.object_id,
+    name="object_id",
+    curie=SSSOM.curie("object_id"),
+    model_uri=SIM.object_id,
     domain=None,
     range=Optional[Union[str, URIorCURIE]],
 )
 
 slots.object_label = Slot(
     uri=SSSOM.object_label,
     name="object_label",
     curie=SSSOM.curie("object_label"),
-    model_uri=ONTOASSOC.object_label,
+    model_uri=SIM.object_label,
     domain=None,
     range=Optional[str],
 )
 
-slots.property_values = Slot(
-    uri=ONTOASSOC.property_values,
-    name="property_values",
-    curie=ONTOASSOC.curie("property_values"),
-    model_uri=ONTOASSOC.property_values,
+slots.object_source = Slot(
+    uri=SSSOM.object_source,
+    name="object_source",
+    curie=SSSOM.curie("object_source"),
+    model_uri=SIM.object_source,
     domain=None,
-    range=Optional[Union[Union[dict, PropertyValue], List[Union[dict, PropertyValue]]]],
+    range=Optional[str],
 )
 
-slots.group_object = Slot(
-    uri=RDF.object,
-    name="group_object",
-    curie=RDF.curie("object"),
-    model_uri=ONTOASSOC.group_object,
+slots.ancestor_id = Slot(
+    uri=SIM.ancestor_id,
+    name="ancestor_id",
+    curie=SIM.curie("ancestor_id"),
+    model_uri=SIM.ancestor_id,
     domain=None,
     range=Optional[Union[str, URIorCURIE]],
 )
 
-slots.sub_groups = Slot(
-    uri=ONTOASSOC.sub_groups,
-    name="sub_groups",
-    curie=ONTOASSOC.curie("sub_groups"),
-    model_uri=ONTOASSOC.sub_groups,
+slots.ancestor_label = Slot(
+    uri=SIM.ancestor_label,
+    name="ancestor_label",
+    curie=SIM.curie("ancestor_label"),
+    model_uri=SIM.ancestor_label,
     domain=None,
-    range=Optional[Union[Union[dict, RollupGroup], List[Union[dict, RollupGroup]]]],
+    range=Optional[str],
 )
 
-slots.associations = Slot(
-    uri=ONTOASSOC.associations,
-    name="associations",
-    curie=ONTOASSOC.curie("associations"),
-    model_uri=ONTOASSOC.associations,
+slots.ancestor_source = Slot(
+    uri=SIM.ancestor_source,
+    name="ancestor_source",
+    curie=SIM.curie("ancestor_source"),
+    model_uri=SIM.ancestor_source,
     domain=None,
-    range=Optional[Union[Union[dict, Association], List[Union[dict, Association]]]],
+    range=Optional[str],
 )
 
-slots.original_subject = Slot(
-    uri=BIOLINK.original_subject,
-    name="original_subject",
-    curie=BIOLINK.curie("original_subject"),
-    model_uri=ONTOASSOC.original_subject,
+slots.score = Slot(
+    uri=SIM.score,
+    name="score",
+    curie=SIM.curie("score"),
+    model_uri=SIM.score,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[str],
 )
 
-slots.original_predicate = Slot(
-    uri=BIOLINK.original_predicate,
-    name="original_predicate",
-    curie=BIOLINK.curie("original_predicate"),
-    model_uri=ONTOASSOC.original_predicate,
+slots.information_content = Slot(
+    uri=SIM.information_content,
+    name="information_content",
+    curie=SIM.curie("information_content"),
+    model_uri=SIM.information_content,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[float, NegativeLogValue]],
 )
 
-slots.original_object = Slot(
-    uri=BIOLINK.original_object,
-    name="original_object",
-    curie=BIOLINK.curie("original_object"),
-    model_uri=ONTOASSOC.original_object,
+slots.subject_information_content = Slot(
+    uri=SIM.subject_information_content,
+    name="subject_information_content",
+    curie=SIM.curie("subject_information_content"),
+    model_uri=SIM.subject_information_content,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[float, NegativeLogValue]],
 )
 
-slots.publications = Slot(
-    uri=BIOLINK.publications,
-    name="publications",
-    curie=BIOLINK.curie("publications"),
-    model_uri=ONTOASSOC.publications,
-    domain=None,
-    range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]],
+slots.object_information_content = Slot(
+    uri=SIM.object_information_content,
+    name="object_information_content",
+    curie=SIM.curie("object_information_content"),
+    model_uri=SIM.object_information_content,
+    domain=None,
+    range=Optional[Union[float, NegativeLogValue]],
 )
 
-slots.primary_knowledge_source = Slot(
-    uri=BIOLINK.primary_knowledge_source,
-    name="primary_knowledge_source",
-    curie=BIOLINK.curie("primary_knowledge_source"),
-    model_uri=ONTOASSOC.primary_knowledge_source,
+slots.ancestor_information_content = Slot(
+    uri=SIM.ancestor_information_content,
+    name="ancestor_information_content",
+    curie=SIM.curie("ancestor_information_content"),
+    model_uri=SIM.ancestor_information_content,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[float, NegativeLogValue]],
 )
 
-slots.aggregator_knowledge_source = Slot(
-    uri=BIOLINK.aggregator_knowledge_source,
-    name="aggregator_knowledge_source",
-    curie=BIOLINK.curie("aggregator_knowledge_source"),
-    model_uri=ONTOASSOC.aggregator_knowledge_source,
+slots.jaccard_similarity = Slot(
+    uri=SIM.jaccard_similarity,
+    name="jaccard_similarity",
+    curie=SIM.curie("jaccard_similarity"),
+    model_uri=SIM.jaccard_similarity,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[float, ZeroToOne]],
 )
 
-slots.denormalized_slot = Slot(
-    uri=ONTOASSOC.denormalized_slot,
-    name="denormalized_slot",
-    curie=ONTOASSOC.curie("denormalized_slot"),
-    model_uri=ONTOASSOC.denormalized_slot,
+slots.dice_similarity = Slot(
+    uri=SIM.dice_similarity,
+    name="dice_similarity",
+    curie=SIM.curie("dice_similarity"),
+    model_uri=SIM.dice_similarity,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[float, ZeroToOne]],
 )
 
-slots.summary_group = Slot(
-    uri=ONTOASSOC.summary_group,
-    name="summary_group",
-    curie=ONTOASSOC.curie("summary_group"),
-    model_uri=ONTOASSOC.summary_group,
+slots.phenodigm_score = Slot(
+    uri=SIM.phenodigm_score,
+    name="phenodigm_score",
+    curie=SIM.curie("phenodigm_score"),
+    model_uri=SIM.phenodigm_score,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[float, NonNegativeFloat]],
 )
 
-slots.publication_is_added = Slot(
-    uri=ONTOASSOC.publication_is_added,
-    name="publication_is_added",
-    curie=ONTOASSOC.curie("publication_is_added"),
-    model_uri=ONTOASSOC.publication_is_added,
+slots.overlap_coefficient = Slot(
+    uri=SIM.overlap_coefficient,
+    name="overlap_coefficient",
+    curie=SIM.curie("overlap_coefficient"),
+    model_uri=SIM.overlap_coefficient,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[Union[float, ZeroToOne]],
 )
 
-slots.publication_is_deleted = Slot(
-    uri=ONTOASSOC.publication_is_deleted,
-    name="publication_is_deleted",
-    curie=ONTOASSOC.curie("publication_is_deleted"),
-    model_uri=ONTOASSOC.publication_is_deleted,
+slots.subsumes_score = Slot(
+    uri=SIM.subsumes_score,
+    name="subsumes_score",
+    curie=SIM.curie("subsumes_score"),
+    model_uri=SIM.subsumes_score,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[Union[float, ZeroToOne]],
 )
 
-slots.old_predicate = Slot(
-    uri=ONTOASSOC.old_predicate,
-    name="old_predicate",
-    curie=ONTOASSOC.curie("old_predicate"),
-    model_uri=ONTOASSOC.old_predicate,
+slots.subsumed_by_score = Slot(
+    uri=SIM.subsumed_by_score,
+    name="subsumed_by_score",
+    curie=SIM.curie("subsumed_by_score"),
+    model_uri=SIM.subsumed_by_score,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[float, ZeroToOne]],
 )
 
-slots.new_predicate = Slot(
-    uri=ONTOASSOC.new_predicate,
-    name="new_predicate",
-    curie=ONTOASSOC.curie("new_predicate"),
-    model_uri=ONTOASSOC.new_predicate,
+slots.intersection_count = Slot(
+    uri=SIM.intersection_count,
+    name="intersection_count",
+    curie=SIM.curie("intersection_count"),
+    model_uri=SIM.intersection_count,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[int, ItemCount]],
 )
 
-slots.old_object = Slot(
-    uri=ONTOASSOC.old_object,
-    name="old_object",
-    curie=ONTOASSOC.curie("old_object"),
-    model_uri=ONTOASSOC.old_object,
+slots.union_count = Slot(
+    uri=SIM.union_count,
+    name="union_count",
+    curie=SIM.curie("union_count"),
+    model_uri=SIM.union_count,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[int, ItemCount]],
 )
 
-slots.new_object = Slot(
-    uri=ONTOASSOC.new_object,
-    name="new_object",
-    curie=ONTOASSOC.curie("new_object"),
-    model_uri=ONTOASSOC.new_object,
+slots.subject_termset = Slot(
+    uri=SIM.subject_termset,
+    name="subject_termset",
+    curie=SIM.curie("subject_termset"),
+    model_uri=SIM.subject_termset,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[
+        Union[Dict[Union[str, TermInfoId], Union[dict, TermInfo]], List[Union[dict, TermInfo]]]
+    ],
 )
 
-slots.old_object_obsolete = Slot(
-    uri=ONTOASSOC.old_object_obsolete,
-    name="old_object_obsolete",
-    curie=ONTOASSOC.curie("old_object_obsolete"),
-    model_uri=ONTOASSOC.old_object_obsolete,
+slots.object_termset = Slot(
+    uri=SIM.object_termset,
+    name="object_termset",
+    curie=SIM.curie("object_termset"),
+    model_uri=SIM.object_termset,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[
+        Union[Dict[Union[str, TermInfoId], Union[dict, TermInfo]], List[Union[dict, TermInfo]]]
+    ],
 )
 
-slots.is_migration = Slot(
-    uri=ONTOASSOC.is_migration,
-    name="is_migration",
-    curie=ONTOASSOC.curie("is_migration"),
-    model_uri=ONTOASSOC.is_migration,
+slots.subject_best_matches = Slot(
+    uri=SIM.subject_best_matches,
+    name="subject_best_matches",
+    curie=SIM.curie("subject_best_matches"),
+    model_uri=SIM.subject_best_matches,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[
+        Union[
+            Dict[Union[str, BestMatchMatchSource], Union[dict, BestMatch]],
+            List[Union[dict, BestMatch]],
+        ]
+    ],
+)
+
+slots.object_best_matches = Slot(
+    uri=SIM.object_best_matches,
+    name="object_best_matches",
+    curie=SIM.curie("object_best_matches"),
+    model_uri=SIM.object_best_matches,
+    domain=None,
+    range=Optional[
+        Union[
+            Dict[Union[str, BestMatchMatchSource], Union[dict, BestMatch]],
+            List[Union[dict, BestMatch]],
+        ]
+    ],
 )
 
-slots.is_generalization = Slot(
-    uri=ONTOASSOC.is_generalization,
-    name="is_generalization",
-    curie=ONTOASSOC.curie("is_generalization"),
-    model_uri=ONTOASSOC.is_generalization,
+slots.metric = Slot(
+    uri=SIM.metric,
+    name="metric",
+    curie=SIM.curie("metric"),
+    model_uri=SIM.metric,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[Union[str, URIorCURIE]],
 )
 
-slots.is_specialization = Slot(
-    uri=ONTOASSOC.is_specialization,
-    name="is_specialization",
-    curie=ONTOASSOC.curie("is_specialization"),
-    model_uri=ONTOASSOC.is_specialization,
+slots.average_score = Slot(
+    uri=SIM.average_score,
+    name="average_score",
+    curie=SIM.curie("average_score"),
+    model_uri=SIM.average_score,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[float],
 )
 
-slots.is_creation = Slot(
-    uri=ONTOASSOC.is_creation,
-    name="is_creation",
-    curie=ONTOASSOC.curie("is_creation"),
-    model_uri=ONTOASSOC.is_creation,
+slots.best_score = Slot(
+    uri=SIM.best_score,
+    name="best_score",
+    curie=SIM.curie("best_score"),
+    model_uri=SIM.best_score,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[float],
 )
 
-slots.is_deletion = Slot(
-    uri=ONTOASSOC.is_deletion,
-    name="is_deletion",
-    curie=ONTOASSOC.curie("is_deletion"),
-    model_uri=ONTOASSOC.is_deletion,
+slots.termInfo__id = Slot(
+    uri=SIM.id,
+    name="termInfo__id",
+    curie=SIM.curie("id"),
+    model_uri=SIM.termInfo__id,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=URIRef,
 )
 
-slots.closure_predicates = Slot(
-    uri=ONTOASSOC.closure_predicates,
-    name="closure_predicates",
-    curie=ONTOASSOC.curie("closure_predicates"),
-    model_uri=ONTOASSOC.closure_predicates,
+slots.termInfo__label = Slot(
+    uri=RDFS.label,
+    name="termInfo__label",
+    curie=RDFS.curie("label"),
+    model_uri=SIM.termInfo__label,
     domain=None,
-    range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]],
+    range=Optional[str],
 )
 
-slots.parserConfiguration__preserve_negated_associations = Slot(
-    uri=ONTOASSOC.preserve_negated_associations,
-    name="parserConfiguration__preserve_negated_associations",
-    curie=ONTOASSOC.curie("preserve_negated_associations"),
-    model_uri=ONTOASSOC.parserConfiguration__preserve_negated_associations,
+slots.bestMatch__match_source = Slot(
+    uri=SIM.match_source,
+    name="bestMatch__match_source",
+    curie=SIM.curie("match_source"),
+    model_uri=SIM.bestMatch__match_source,
+    domain=None,
+    range=URIRef,
+)
+
+slots.bestMatch__match_source_label = Slot(
+    uri=SIM.match_source_label,
+    name="bestMatch__match_source_label",
+    curie=SIM.curie("match_source_label"),
+    model_uri=SIM.bestMatch__match_source_label,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[str],
 )
 
-slots.parserConfiguration__include_association_attributes = Slot(
-    uri=ONTOASSOC.include_association_attributes,
-    name="parserConfiguration__include_association_attributes",
-    curie=ONTOASSOC.curie("include_association_attributes"),
-    model_uri=ONTOASSOC.parserConfiguration__include_association_attributes,
+slots.bestMatch__match_target = Slot(
+    uri=SIM.match_target,
+    name="bestMatch__match_target",
+    curie=SIM.curie("match_target"),
+    model_uri=SIM.bestMatch__match_target,
     domain=None,
-    range=Optional[Union[bool, Bool]],
+    range=Optional[str],
 )
 
-slots.parserConfiguration__primary_knowledge_source = Slot(
-    uri=BIOLINK.primary_knowledge_source,
-    name="parserConfiguration__primary_knowledge_source",
-    curie=BIOLINK.curie("primary_knowledge_source"),
-    model_uri=ONTOASSOC.parserConfiguration__primary_knowledge_source,
+slots.bestMatch__match_target_label = Slot(
+    uri=SIM.match_target_label,
+    name="bestMatch__match_target_label",
+    curie=SIM.curie("match_target_label"),
+    model_uri=SIM.bestMatch__match_target_label,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[str],
+)
+
+slots.bestMatch__score = Slot(
+    uri=SIM.score,
+    name="bestMatch__score",
+    curie=SIM.curie("score"),
+    model_uri=SIM.bestMatch__score,
+    domain=None,
+    range=float,
 )
 
-slots.parserConfiguration__aggregator_knowledge_source = Slot(
-    uri=BIOLINK.aggregator_knowledge_source,
-    name="parserConfiguration__aggregator_knowledge_source",
-    curie=BIOLINK.curie("aggregator_knowledge_source"),
-    model_uri=ONTOASSOC.parserConfiguration__aggregator_knowledge_source,
+slots.bestMatch__match_subsumer = Slot(
+    uri=SIM.match_subsumer,
+    name="bestMatch__match_subsumer",
+    curie=SIM.curie("match_subsumer"),
+    model_uri=SIM.bestMatch__match_subsumer,
     domain=None,
     range=Optional[Union[str, URIorCURIE]],
 )
+
+slots.bestMatch__match_subsumer_label = Slot(
+    uri=SIM.match_subsumer_label,
+    name="bestMatch__match_subsumer_label",
+    curie=SIM.curie("match_subsumer_label"),
+    model_uri=SIM.bestMatch__match_subsumer_label,
+    domain=None,
+    range=Optional[str],
+)
+
+slots.bestMatch__similarity = Slot(
+    uri=SIM.similarity,
+    name="bestMatch__similarity",
+    curie=SIM.curie("similarity"),
+    model_uri=SIM.bestMatch__similarity,
+    domain=None,
+    range=Union[dict, TermPairwiseSimilarity],
+)
```

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,182 @@
-id: https://w3id.org/oak/association
-title: OAK Association Data Model
-name: association
-description: |-
-  A datamodel for representing generic associations.
-  
-  The core datamodel is broad, encompassing the W3 Open Annotation data model as well
-  as common ontology annotation data models using in the biosciences.
-
+id: https://w3id.org/oak/taxon_constraints
+title: Taxon Constraints Reporting Datamodel
+name: taxon-constraints
+description: >-
+  A datamodel for representing inferred and asserted taxon constraints.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
   linkml: https://w3id.org/linkml/
-  ontoassoc: https://w3id.org/oak/association/
-  oa: http://www.w3.org/ns/oa#
-  biolink: https://w3id.org/biolink/vocab/
-  sssom: https://w3id.org/sssom/
+  tc: https://w3id.org/linkml/taxon_constraints/
+  skos: http://www.w3.org/2004/02/skos/core#
+  pav: http://purl.org/pav/
+  schema: http://schema.org/
+  sh: https://w3id.org/shacl/
+  prov: http://www.w3.org/ns/prov#
+  RO: http://purl.obolibrary.org/obo/RO_
+
+default_prefix: tc
+default_range: string
+
+default_curi_maps:
+  - semweb_context
+
+emit_prefixes:
+  - linkml
+  - rdf
+  - rdfs
+  - xsd
+  - owl
+
 imports:
   - linkml:types
-default_prefix: ontoassoc
 
+#==================================
+# Classes                         #
+#==================================
 classes:
-
-  Association:
-    class_uri: oa:Annotation
-    description: A generic association between a thing (subject) and another thing (object).
-    slots:
-      - subject
-      - predicate
-      - object
-      - property_values
-      - subject_label
-      - predicate_label
-      - object_label
-      - publications
-      - primary_knowledge_source
-      - aggregator_knowledge_source
-
-  NegatedAssociation:
-    description: A negated association between a thing (subject) and another thing (object).
-    slots:
-      - subject
-      - predicate
-      - object
-      - property_values
-      - subject_label
-      - predicate_label
-      - object_label
-      - publications
-      - primary_knowledge_source
-      - aggregator_knowledge_source
-
-  PropertyValue:
-    description: A generic tag-value that can be associated with an association.
-    slots:
-      - predicate
-      - object
-
-  RollupGroup:
-    slots:
-      - group_object
-      - sub_groups
-      - associations
-
-  ParserConfiguration:
+  Term:
+    description: An ontology term. In this model this is either the SubjectTerm of a taxon constraint, or an actual taxon
+    abstract: true
+    class_uri: owl:Class
     attributes:
-      preserve_negated_associations:
-        range: boolean
-        description: |-
-          If true, then the parser will keep negated associations in the output.
-          If false, then the parser will remove negated associations from the output.
-      include_association_attributes:
-        range: boolean
-        description: |-
-          If true, then the parser will include non S/P/O properties as additional attributes.
-          This may result in slower parsing
-      primary_knowledge_source:
-        range: uriorcurie
-        slot_uri: biolink:primary_knowledge_source
-        description: |-
-          The default primary knowledge source for all associations in this resource.
-      aggregator_knowledge_source:
+      id:
         range: uriorcurie
-        slot_uri: biolink:aggregator_knowledge_source
-        description: |-
-          The default aggregator knowledge source for all associations in this resource.
-
-  AssociationChange:
-    slots:
-      - summary_group
-      - publications
-      - publication_is_added
-      - publication_is_deleted
-      - subject
-      - old_predicate
-      - new_predicate
-      - old_object
-      - new_object
-      - old_object_obsolete
-      - is_migration
-      - is_generalization
-      - is_specialization
-      - is_creation
-      - is_deletion
-      - closure_predicates
-      
-
-slots:
-  subject:
-    description: The thing which the association is about.
-    comments:
-      - it is conventional for the subject to be the "entity" and the object to be the ontological descriptor
-    slot_uri: rdf:subject
-    range: uriorcurie
-    exact_mappings:
-      - oa:hasBody
-  subject_label:
-    description: The label of the thing which the association is about.
-    slot_uri: sssom:subject_label
-    range: string
-    mixins:
-      - denormalized_slot
-  predicate:
-    description: The type of relationship between the subject and object.
-    slot_uri: rdf:predicate
-    range: uriorcurie
-  predicate_label:
-    description: The label of the type of relationship between the subject and object.
-    slot_uri: sssom:predicate_label
-    range: string
-    mixins:
-      - denormalized_slot
-  object:
-    description: An ontology entity that is associated with the subject.
-    comments:
-      - it is conventional for the subject to be the "entity" and the object to be the ontological descriptor
-    slot_uri: rdf:object
-    range: uriorcurie
-    exact_mappings:
-      - oa:hasTarget
-  object_label:
-    description: The label of the ontology entity that is associated with the subject.
-    slot_uri: sssom:object_label
-    range: string
-    mixins:
-      - denormalized_slot
-  property_values:
-    multivalued: true
-    range: PropertyValue
-    inlined: true
-  group_object:
-    description: |-
-      An ontology entity that is the ancestor of the objects in the group's 
-      associations and sub-group associations.
-    slot_uri: rdf:object
-    range: uriorcurie
-  sub_groups:
-    description: Container for groups within a rollup group.
-    range: RollupGroup
-    multivalued: true
-    inlined_as_list: true
-  associations:
-    range: Association
-    multivalued: true
-    inlined_as_list: true
-  original_subject:
-    description: The original subject of the association prior to normalization
-    slot_uri: biolink:original_subject
-    range: uriorcurie
-    exact_mappings:
-      - biolink:original_subject
-  original_predicate:
-    description: The original subject of the association prior to normalization
-    slot_uri: biolink:original_predicate
-    range: uriorcurie
-    exact_mappings:
-      - biolink:original_predicate
-  original_object:
-    description: The original object of the association prior to normalization
-    slot_uri: biolink:original_object
-    range: uriorcurie
+        identifier: true
+        description: the OBO CURIE for the term
+      label:
+        slot_uri: rdfs:label
+        range: string
+        description: the human readable name or label of the term
+  SubjectTerm:
+    description: >-
+      A term that is the subject of a taxon constraint. Typically comes from ontologies like GO, UBERON, CL, ...
+    is_a: Term
+    attributes:
+      description:
+        description: A description of the term
+      unsatisfiable:
+        range: boolean
+        description: If true then some combination of taxon constraints plus ontology lead to contradictions
+      only_in:
+        description: >
+          Points to a taxon constraint that states the SubjectTerm is ONLY found in a taxon or descendant.
+          Formally, the term AND its descendants MUST be in the specified taxon, or a descendant of that taxon
+        comments:
+          - Note that we conflate between the RO "only in taxon" and "in taxon" relations here
+        range: TaxonConstraint
+        multivalued: true
+        slot_uri: RO:0002160
+      never_in:
+        description: >
+          Points to a taxon constraint that states the SubjectTerm is NEVER found in a taxon or descendant.
+          Formally, the term AND its descendants MUST NOT be in the specified taxon, or a descendant of that taxon
+        range: TaxonConstraint
+        multivalued: true
+        slot_uri: RO:0002161
+      present_in:
+        range: TaxonConstraint
+        description: >
+          The term MAY be in the specified taxon, or a descendant of that taxon
+        multivalued: true
+        slot_uri: RO:0002175
+      present_in_ancestor_of:
+        range: TaxonConstraint
+        multivalued: true
+        #slot_uri:
+  Taxon:
+    description: A term that represents a taxonomic group, may be at species level of a higher level
+    is_a: Term
     exact_mappings:
-      - biolink:original_object
-  publications:
-    description: The publications that support the association
-    slot_uri: biolink:publications
-    range: uriorcurie
-    multivalued: true
-  primary_knowledge_source:
-    description: The primary knowledge source for the association
-    slot_uri: biolink:primary_knowledge_source
-    range: uriorcurie
-  aggregator_knowledge_source:
-    description: The knowledge source that aggregated the association
-    slot_uri: biolink:aggregator_knowledge_source
-    range: uriorcurie
-  denormalized_slot:
-    mixin: true
-    description: |-
-      denormalized slots are for models that follow a denormalized data model
-  summary_group:
-    range: string
-  publication_is_added:
-    range: boolean
-  publication_is_deleted:
-    range: boolean
-  old_predicate:
-    is_a: predicate
-  new_predicate:
-    is_a: predicate
-  old_object:
-    is_a: object
-  new_object:
-    is_a: object
-  old_object_obsolete:
-    range: boolean
-  is_migration:
-    range: boolean
-  is_generalization:
-    range: boolean
-  is_specialization:
-    range: boolean
-  is_creation:
-    range: boolean
-  is_deletion:
-    range: boolean
-  closure_predicates:
-    range: uriorcurie
-    multivalued: true
+      - NCBITaxon:1
+    id_prefixes:
+      - NCBITaxon
+      - NCBITaxon_Union
+  PredicateTerm:
+    description: >-
+      A term that represents a relationship type
+    is_a: Term
+    id_prefixes:
+      - RO
+
+  TaxonConstraint:
+    description: >-
+      An individual taxon constraint
+    class_uri: rdf:Statement
+    attributes:
+      subject:
+        slot_uri: rdf:subject
+        range: SubjectTerm
+        description: The term to which the constraint applies
+        comments:
+          - this is a reciprocal slot and will be the same as the containing SubjectTerm
+      predicate:
+        slot_uri: rdf:predicate
+        range: PredicateTerm
+        description: The relationship type for the contraint (e.g. in_taxon, never_in taxon)
+        todos:
+          - define a value set of this
+      asserted:
+        range: boolean
+        description: >-
+          holds if the constraint is asserted in the source ontology, rather than inferred by rules or reasoning
+      evolutionary:
+        range: boolean
+        description: >-
+          holds if the constraint is an evolutionary statement
+      redundant:
+        range: boolean
+        description: >-
+          True if this is redundant within the set of constraints of the same type (never vs only)
+      redundant_with_only_in:
+        range: boolean
+        description: >-
+          True for never in constraints that are subsumed by an only in
+      taxon:
+        slot_uri: rdf:object
+        description: >-
+          The taxon which this constraint is about. May be species or a more general class.
+        range: Taxon
+        inlined: true
+      redundant_with:
+        range: TaxonConstraint
+        multivalued: true
+        description: >-
+          If the taxon constraint is redundant, then this is the set of taxon constraints that it is redundant with
+      contradicted_by:
+        range: TaxonConstraint
+        multivalued: true
+        description: >-
+          If the taxon constraint conflicts with another, 
+          then this is the set of taxon constraints that it is redundant with
+      via_terms:
+        description: >-
+          For inferred taxon constraints, this is the term or terms that have the taxon constraint asserted
+        range: SubjectTerm
+        multivalued: true
+        inlined: true
+        inlined_as_list: true
+      predicates:
+        description: >-
+          The predicates that connect the subject term to the via_terms.
+        range: PredicateTerm
+        multivalued: true
+      sources:
+        range: uriorcurie
+        multivalued: true
+      comments:
+        range: string
+        multivalued: true
+      candidate:
+        range: boolean
+        description: >-
+          true if this is a proposed candidate constraint
+
+enums:
+
+  ConfigurationOption:
+    permissible_values:
+      ExcludeRedundant:
+      IncludeRedundant:
+      IncludeNeverInIfRedundantWithOnlyIn:
+      ExcludeNeverInIfRedundantWithOnlyIn:
```

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.4/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.4/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/cx.py` & `oaklib-0.5.4/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.4/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/input_specification.py` & `oaklib-0.5.4/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.4/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.4/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.4/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.4/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.4/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/search.py` & `oaklib-0.5.4/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.4/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.4/src/oaklib/datamodels/text_annotator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-# Auto generated from similarity.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-10T09:38:53
-# Schema: similarity
+# Auto generated from text_annotator.yaml by pythongen.py version: 0.9.0
+# Generation date: 2023-04-09T15:53:59
+# Schema: text-annotator
 #
-# id: https://w3id.org/oak/similarity
-# description: A datamodel for representing semantic similarity between terms or lists of terms.
+# id: https://w3id.org/oak/text_annotator
+# description: A datamodel for representing the results of textual named entity recognition annotation results.
+#              This draws upon both SSSOM and https://www.w3.org/TR/annotation-model/
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
 import sys
 from dataclasses import dataclass
 from typing import Any, ClassVar, Dict, List, Optional, Union
 
 from jsonasobj2 import JsonObj, as_dict
 from linkml_runtime.linkml_model.meta import (
     EnumDefinition,
     PermissibleValue,
     PvFormulaOptions,
 )
-from linkml_runtime.linkml_model.types import Float, Integer, String, Uriorcurie
+from linkml_runtime.linkml_model.types import (
+    Boolean,
+    Float,
+    Integer,
+    String,
+    Uriorcurie,
+)
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.utils.dataclass_extensions_376 import (
     dataclasses_init_fn_with_kwargs,
 )
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
-from linkml_runtime.utils.metamodelcore import URIorCURIE, bnode, empty_dict, empty_list
+from linkml_runtime.utils.metamodelcore import (
+    Bool,
+    URIorCURIE,
+    bnode,
+    empty_dict,
+    empty_list,
+)
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.yamlutils import (
     YAMLRoot,
     extended_float,
     extended_int,
     extended_str,
 )
@@ -38,681 +51,553 @@
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
+ANN = CurieNamespace("ann", "https://w3id.org/linkml/text_annotator/")
+BPA = CurieNamespace("bpa", "https://bioportal.bioontology.org/annotator/")
 LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
+OA = CurieNamespace("oa", "http://www.w3.org/ns/oa#")
 OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
 PAV = CurieNamespace("pav", "http://purl.org/pav/")
 PROV = CurieNamespace("prov", "http://www.w3.org/ns/prov#")
 RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
 RDFS = CurieNamespace("rdfs", "http://www.w3.org/2000/01/rdf-schema#")
 SCHEMA = CurieNamespace("schema", "http://schema.org/")
 SH = CurieNamespace("sh", "https://w3id.org/shacl/")
-SIM = CurieNamespace("sim", "https://w3id.org/linkml/similarity/")
 SKOS = CurieNamespace("skos", "http://www.w3.org/2004/02/skos/core#")
 SSSOM = CurieNamespace("sssom", "http://w3id.org/sssom/")
 XSD = CurieNamespace("xsd", "http://www.w3.org/2001/XMLSchema#")
-DEFAULT_ = SIM
+DEFAULT_ = ANN
 
 
 # Types
-class ZeroToOne(Float):
-    type_class_uri = XSD.float
-    type_class_curie = "xsd:float"
-    type_name = "ZeroToOne"
-    type_model_uri = SIM.ZeroToOne
-
-
-class NonNegativeFloat(Float):
-    type_class_uri = XSD.float
-    type_class_curie = "xsd:float"
-    type_name = "NonNegativeFloat"
-    type_model_uri = SIM.NonNegativeFloat
-
-
-class NegativeLogValue(Float):
-    type_class_uri = XSD.float
-    type_class_curie = "xsd:float"
-    type_name = "NegativeLogValue"
-    type_model_uri = SIM.NegativeLogValue
-
-
-class ItemCount(Integer):
+class Position(Integer):
     type_class_uri = XSD.integer
     type_class_curie = "xsd:integer"
-    type_name = "ItemCount"
-    type_model_uri = SIM.ItemCount
+    type_name = "Position"
+    type_model_uri = ANN.Position
 
 
 # Class references
-class TermInfoId(extended_str):
-    pass
-
-
-class BestMatchMatchSource(extended_str):
+class TextualElementId(URIorCURIE):
     pass
 
 
-class PairwiseSimilarity(YAMLRoot):
+@dataclass
+class TextAnnotationConfiguration(YAMLRoot):
     """
-    Abstract grouping for representing individual pairwise similarities
+    configuration for search
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = SIM.PairwiseSimilarity
-    class_class_curie: ClassVar[str] = "sim:PairwiseSimilarity"
-    class_name: ClassVar[str] = "PairwiseSimilarity"
-    class_model_uri: ClassVar[URIRef] = SIM.PairwiseSimilarity
+    class_class_uri: ClassVar[URIRef] = ANN.TextAnnotationConfiguration
+    class_class_curie: ClassVar[str] = "ann:TextAnnotationConfiguration"
+    class_name: ClassVar[str] = "TextAnnotationConfiguration"
+    class_model_uri: ClassVar[URIRef] = ANN.TextAnnotationConfiguration
+
+    matches_whole_text: Optional[Union[bool, Bool]] = None
+    sources: Optional[Union[str, List[str]]] = empty_list()
+    limit: Optional[int] = None
+    token_exclusion_list: Optional[Union[str, List[str]]] = empty_list()
+    model: Optional[str] = None
+    include_aliases: Optional[Union[bool, Bool]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.matches_whole_text is not None and not isinstance(self.matches_whole_text, Bool):
+            self.matches_whole_text = Bool(self.matches_whole_text)
+
+        if not isinstance(self.sources, list):
+            self.sources = [self.sources] if self.sources is not None else []
+        self.sources = [v if isinstance(v, str) else str(v) for v in self.sources]
+
+        if self.limit is not None and not isinstance(self.limit, int):
+            self.limit = int(self.limit)
+
+        if not isinstance(self.token_exclusion_list, list):
+            self.token_exclusion_list = (
+                [self.token_exclusion_list] if self.token_exclusion_list is not None else []
+            )
+        self.token_exclusion_list = [
+            v if isinstance(v, str) else str(v) for v in self.token_exclusion_list
+        ]
+
+        if self.model is not None and not isinstance(self.model, str):
+            self.model = str(self.model)
+
+        if self.include_aliases is not None and not isinstance(self.include_aliases, Bool):
+            self.include_aliases = Bool(self.include_aliases)
+
+        super().__post_init__(**kwargs)
 
 
 @dataclass
-class TermPairwiseSimilarity(PairwiseSimilarity):
+class TextAnnotationResultSet(YAMLRoot):
     """
-    A simple pairwise similarity between two atomic concepts/terms
+    A collection of annotation results
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = SIM.TermPairwiseSimilarity
-    class_class_curie: ClassVar[str] = "sim:TermPairwiseSimilarity"
-    class_name: ClassVar[str] = "TermPairwiseSimilarity"
-    class_model_uri: ClassVar[URIRef] = SIM.TermPairwiseSimilarity
-
-    subject_id: Union[str, URIorCURIE] = None
-    subject_label: Optional[str] = None
-    subject_source: Optional[str] = None
-    object_id: Optional[Union[str, URIorCURIE]] = None
-    object_label: Optional[str] = None
-    object_source: Optional[str] = None
-    ancestor_id: Optional[Union[str, URIorCURIE]] = None
-    ancestor_label: Optional[str] = None
-    ancestor_source: Optional[str] = None
-    object_information_content: Optional[Union[float, NegativeLogValue]] = None
-    subject_information_content: Optional[Union[float, NegativeLogValue]] = None
-    ancestor_information_content: Optional[Union[float, NegativeLogValue]] = None
-    jaccard_similarity: Optional[Union[float, ZeroToOne]] = None
-    dice_similarity: Optional[Union[float, ZeroToOne]] = None
-    phenodigm_score: Optional[Union[float, NonNegativeFloat]] = None
+    class_class_uri: ClassVar[URIRef] = ANN.TextAnnotationResultSet
+    class_class_curie: ClassVar[str] = "ann:TextAnnotationResultSet"
+    class_name: ClassVar[str] = "TextAnnotationResultSet"
+    class_model_uri: ClassVar[URIRef] = ANN.TextAnnotationResultSet
+
+    annotations: Optional[
+        Union[Union[dict, "TextAnnotation"], List[Union[dict, "TextAnnotation"]]]
+    ] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self._is_empty(self.subject_id):
-            self.MissingRequiredField("subject_id")
-        if not isinstance(self.subject_id, URIorCURIE):
-            self.subject_id = URIorCURIE(self.subject_id)
+        if not isinstance(self.annotations, list):
+            self.annotations = [self.annotations] if self.annotations is not None else []
+        self.annotations = [
+            v if isinstance(v, TextAnnotation) else TextAnnotation(**as_dict(v))
+            for v in self.annotations
+        ]
 
-        if self.subject_label is not None and not isinstance(self.subject_label, str):
-            self.subject_label = str(self.subject_label)
+        super().__post_init__(**kwargs)
 
-        if self.subject_source is not None and not isinstance(self.subject_source, str):
-            self.subject_source = str(self.subject_source)
 
-        if self.object_id is not None and not isinstance(self.object_id, URIorCURIE):
-            self.object_id = URIorCURIE(self.object_id)
+@dataclass
+class TextualElement(YAMLRoot):
+    _inherited_slots: ClassVar[List[str]] = []
 
-        if self.object_label is not None and not isinstance(self.object_label, str):
-            self.object_label = str(self.object_label)
+    class_class_uri: ClassVar[URIRef] = ANN.TextualElement
+    class_class_curie: ClassVar[str] = "ann:TextualElement"
+    class_name: ClassVar[str] = "TextualElement"
+    class_model_uri: ClassVar[URIRef] = ANN.TextualElement
+
+    id: Union[str, TextualElementId] = None
+    text: Optional[str] = None
+    source_text: Optional[str] = None
+    parent_document: Optional[Union[str, URIorCURIE]] = None
 
-        if self.object_source is not None and not isinstance(self.object_source, str):
-            self.object_source = str(self.object_source)
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, TextualElementId):
+            self.id = TextualElementId(self.id)
 
-        if self.ancestor_id is not None and not isinstance(self.ancestor_id, URIorCURIE):
-            self.ancestor_id = URIorCURIE(self.ancestor_id)
+        if self.text is not None and not isinstance(self.text, str):
+            self.text = str(self.text)
 
-        if self.ancestor_label is not None and not isinstance(self.ancestor_label, str):
-            self.ancestor_label = str(self.ancestor_label)
+        if self.source_text is not None and not isinstance(self.source_text, str):
+            self.source_text = str(self.source_text)
 
-        if self.ancestor_source is not None and not isinstance(self.ancestor_source, str):
-            self.ancestor_source = str(self.ancestor_source)
+        if self.parent_document is not None and not isinstance(self.parent_document, URIorCURIE):
+            self.parent_document = URIorCURIE(self.parent_document)
 
-        if self.object_information_content is not None and not isinstance(
-            self.object_information_content, NegativeLogValue
-        ):
-            self.object_information_content = NegativeLogValue(self.object_information_content)
+        super().__post_init__(**kwargs)
 
-        if self.subject_information_content is not None and not isinstance(
-            self.subject_information_content, NegativeLogValue
-        ):
-            self.subject_information_content = NegativeLogValue(self.subject_information_content)
 
-        if self.ancestor_information_content is not None and not isinstance(
-            self.ancestor_information_content, NegativeLogValue
-        ):
-            self.ancestor_information_content = NegativeLogValue(self.ancestor_information_content)
+@dataclass
+class HasSpan(YAMLRoot):
+    _inherited_slots: ClassVar[List[str]] = []
 
-        if self.jaccard_similarity is not None and not isinstance(
-            self.jaccard_similarity, ZeroToOne
-        ):
-            self.jaccard_similarity = ZeroToOne(self.jaccard_similarity)
+    class_class_uri: ClassVar[URIRef] = ANN.HasSpan
+    class_class_curie: ClassVar[str] = "ann:HasSpan"
+    class_name: ClassVar[str] = "HasSpan"
+    class_model_uri: ClassVar[URIRef] = ANN.HasSpan
+
+    subject_start: Optional[Union[int, Position]] = None
+    subject_end: Optional[Union[int, Position]] = None
+    subject_label: Optional[str] = None
+    subject_source: Optional[str] = None
+    subject_text_id: Optional[Union[str, TextualElementId]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.subject_start is not None and not isinstance(self.subject_start, Position):
+            self.subject_start = Position(self.subject_start)
 
-        if self.dice_similarity is not None and not isinstance(self.dice_similarity, ZeroToOne):
-            self.dice_similarity = ZeroToOne(self.dice_similarity)
+        if self.subject_end is not None and not isinstance(self.subject_end, Position):
+            self.subject_end = Position(self.subject_end)
 
-        if self.phenodigm_score is not None and not isinstance(
-            self.phenodigm_score, NonNegativeFloat
+        if self.subject_label is not None and not isinstance(self.subject_label, str):
+            self.subject_label = str(self.subject_label)
+
+        if self.subject_source is not None and not isinstance(self.subject_source, str):
+            self.subject_source = str(self.subject_source)
+
+        if self.subject_text_id is not None and not isinstance(
+            self.subject_text_id, TextualElementId
         ):
-            self.phenodigm_score = NonNegativeFloat(self.phenodigm_score)
+            self.subject_text_id = TextualElementId(self.subject_text_id)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class TermSetPairwiseSimilarity(PairwiseSimilarity):
+class TextAnnotation(YAMLRoot):
     """
-    A simple pairwise similarity between two sets of concepts/terms
+    An individual text annotation
     """
 
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = SIM.TermSetPairwiseSimilarity
-    class_class_curie: ClassVar[str] = "sim:TermSetPairwiseSimilarity"
-    class_name: ClassVar[str] = "TermSetPairwiseSimilarity"
-    class_model_uri: ClassVar[URIRef] = SIM.TermSetPairwiseSimilarity
-
-    subject_termset: Optional[
-        Union[Dict[Union[str, TermInfoId], Union[dict, "TermInfo"]], List[Union[dict, "TermInfo"]]]
-    ] = empty_dict()
-    object_termset: Optional[
-        Union[Dict[Union[str, TermInfoId], Union[dict, "TermInfo"]], List[Union[dict, "TermInfo"]]]
-    ] = empty_dict()
-    subject_best_matches: Optional[
-        Union[
-            Dict[Union[str, BestMatchMatchSource], Union[dict, "BestMatch"]],
-            List[Union[dict, "BestMatch"]],
-        ]
-    ] = empty_dict()
-    object_best_matches: Optional[
-        Union[
-            Dict[Union[str, BestMatchMatchSource], Union[dict, "BestMatch"]],
-            List[Union[dict, "BestMatch"]],
-        ]
-    ] = empty_dict()
-    average_score: Optional[float] = None
-    best_score: Optional[float] = None
-    metric: Optional[Union[str, URIorCURIE]] = None
-
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        self._normalize_inlined_as_dict(
-            slot_name="subject_termset", slot_type=TermInfo, key_name="id", keyed=True
-        )
-
-        self._normalize_inlined_as_dict(
-            slot_name="object_termset", slot_type=TermInfo, key_name="id", keyed=True
-        )
-
-        self._normalize_inlined_as_dict(
-            slot_name="subject_best_matches",
-            slot_type=BestMatch,
-            key_name="match_source",
-            keyed=True,
-        )
-
-        self._normalize_inlined_as_dict(
-            slot_name="object_best_matches",
-            slot_type=BestMatch,
-            key_name="match_source",
-            keyed=True,
-        )
+    class_class_uri: ClassVar[URIRef] = OA.Annotation
+    class_class_curie: ClassVar[str] = "oa:Annotation"
+    class_name: ClassVar[str] = "TextAnnotation"
+    class_model_uri: ClassVar[URIRef] = ANN.TextAnnotation
 
-        if self.average_score is not None and not isinstance(self.average_score, float):
-            self.average_score = float(self.average_score)
-
-        if self.best_score is not None and not isinstance(self.best_score, float):
-            self.best_score = float(self.best_score)
+    predicate_id: Optional[str] = None
+    object_id: Optional[str] = None
+    object_label: Optional[str] = None
+    object_source: Optional[str] = None
+    confidence: Optional[float] = None
+    match_string: Optional[str] = None
+    is_longest_match: Optional[Union[bool, Bool]] = None
+    matches_whole_text: Optional[Union[bool, Bool]] = None
+    match_type: Optional[str] = None
+    info: Optional[str] = None
+    object_aliases: Optional[Union[str, List[str]]] = empty_list()
+    subject_start: Optional[Union[int, Position]] = None
+    subject_end: Optional[Union[int, Position]] = None
+    subject_label: Optional[str] = None
+    subject_source: Optional[str] = None
+    subject_text_id: Optional[Union[str, TextualElementId]] = None
 
-        if self.metric is not None and not isinstance(self.metric, URIorCURIE):
-            self.metric = URIorCURIE(self.metric)
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.predicate_id is not None and not isinstance(self.predicate_id, str):
+            self.predicate_id = str(self.predicate_id)
 
-        super().__post_init__(**kwargs)
+        if self.object_id is not None and not isinstance(self.object_id, str):
+            self.object_id = str(self.object_id)
 
+        if self.object_label is not None and not isinstance(self.object_label, str):
+            self.object_label = str(self.object_label)
 
-@dataclass
-class TermInfo(YAMLRoot):
-    _inherited_slots: ClassVar[List[str]] = []
+        if self.object_source is not None and not isinstance(self.object_source, str):
+            self.object_source = str(self.object_source)
 
-    class_class_uri: ClassVar[URIRef] = SIM.TermInfo
-    class_class_curie: ClassVar[str] = "sim:TermInfo"
-    class_name: ClassVar[str] = "TermInfo"
-    class_model_uri: ClassVar[URIRef] = SIM.TermInfo
+        if self.confidence is not None and not isinstance(self.confidence, float):
+            self.confidence = float(self.confidence)
 
-    id: Union[str, TermInfoId] = None
-    label: Optional[str] = None
+        if self.match_string is not None and not isinstance(self.match_string, str):
+            self.match_string = str(self.match_string)
 
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self._is_empty(self.id):
-            self.MissingRequiredField("id")
-        if not isinstance(self.id, TermInfoId):
-            self.id = TermInfoId(self.id)
+        if self.is_longest_match is not None and not isinstance(self.is_longest_match, Bool):
+            self.is_longest_match = Bool(self.is_longest_match)
 
-        if self.label is not None and not isinstance(self.label, str):
-            self.label = str(self.label)
+        if self.matches_whole_text is not None and not isinstance(self.matches_whole_text, Bool):
+            self.matches_whole_text = Bool(self.matches_whole_text)
 
-        super().__post_init__(**kwargs)
+        if self.match_type is not None and not isinstance(self.match_type, str):
+            self.match_type = str(self.match_type)
 
+        if self.info is not None and not isinstance(self.info, str):
+            self.info = str(self.info)
 
-@dataclass
-class BestMatch(YAMLRoot):
-    _inherited_slots: ClassVar[List[str]] = []
+        if not isinstance(self.object_aliases, list):
+            self.object_aliases = [self.object_aliases] if self.object_aliases is not None else []
+        self.object_aliases = [v if isinstance(v, str) else str(v) for v in self.object_aliases]
 
-    class_class_uri: ClassVar[URIRef] = SIM.BestMatch
-    class_class_curie: ClassVar[str] = "sim:BestMatch"
-    class_name: ClassVar[str] = "BestMatch"
-    class_model_uri: ClassVar[URIRef] = SIM.BestMatch
-
-    match_source: Union[str, BestMatchMatchSource] = None
-    score: float = None
-    similarity: Union[dict, TermPairwiseSimilarity] = None
-    match_source_label: Optional[str] = None
-    match_target: Optional[str] = None
-    match_target_label: Optional[str] = None
-    match_subsumer: Optional[Union[str, URIorCURIE]] = None
-    match_subsumer_label: Optional[str] = None
+        if self.subject_start is not None and not isinstance(self.subject_start, Position):
+            self.subject_start = Position(self.subject_start)
 
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self._is_empty(self.match_source):
-            self.MissingRequiredField("match_source")
-        if not isinstance(self.match_source, BestMatchMatchSource):
-            self.match_source = BestMatchMatchSource(self.match_source)
-
-        if self._is_empty(self.score):
-            self.MissingRequiredField("score")
-        if not isinstance(self.score, float):
-            self.score = float(self.score)
-
-        if self._is_empty(self.similarity):
-            self.MissingRequiredField("similarity")
-        if not isinstance(self.similarity, TermPairwiseSimilarity):
-            self.similarity = TermPairwiseSimilarity(**as_dict(self.similarity))
-
-        if self.match_source_label is not None and not isinstance(self.match_source_label, str):
-            self.match_source_label = str(self.match_source_label)
-
-        if self.match_target is not None and not isinstance(self.match_target, str):
-            self.match_target = str(self.match_target)
+        if self.subject_end is not None and not isinstance(self.subject_end, Position):
+            self.subject_end = Position(self.subject_end)
 
-        if self.match_target_label is not None and not isinstance(self.match_target_label, str):
-            self.match_target_label = str(self.match_target_label)
+        if self.subject_label is not None and not isinstance(self.subject_label, str):
+            self.subject_label = str(self.subject_label)
 
-        if self.match_subsumer is not None and not isinstance(self.match_subsumer, URIorCURIE):
-            self.match_subsumer = URIorCURIE(self.match_subsumer)
+        if self.subject_source is not None and not isinstance(self.subject_source, str):
+            self.subject_source = str(self.subject_source)
 
-        if self.match_subsumer_label is not None and not isinstance(self.match_subsumer_label, str):
-            self.match_subsumer_label = str(self.match_subsumer_label)
+        if self.subject_text_id is not None and not isinstance(
+            self.subject_text_id, TextualElementId
+        ):
+            self.subject_text_id = TextualElementId(self.subject_text_id)
 
         super().__post_init__(**kwargs)
 
 
 # Enumerations
+class TransformationType(EnumDefinitionImpl):
+    """
+    A controlled datamodels of the types of transformation that can be applied to
+    """
+
+    Stemming = PermissibleValue(
+        text="Stemming",
+        description="Removal of the last few characters of a word to yield a stem term for each word in the term",
+    )
+    Lemmatization = PermissibleValue(
+        text="Lemmatization",
+        description="Contextual reduction of a word to its base form for each word in the term",
+    )
+    WordOrderNormalization = PermissibleValue(
+        text="WordOrderNormalization",
+        description="reorder words in the term to a standard order such that comparisons are order-independent",
+    )
+    Depluralization = PermissibleValue(
+        text="Depluralization",
+        description="Transform plural form to singular form for each word in a term",
+    )
+    CaseNormalization = PermissibleValue(
+        text="CaseNormalization",
+        description="Transform term to a standard case, typically lowercase",
+    )
+    WhitespaceNormalization = PermissibleValue(
+        text="WhitespaceNormalization",
+        description="Trim whitespace, condense whitespace runs, and transform all non-space whitespace to spaces",
+    )
+    TermExpanson = PermissibleValue(
+        text="TermExpanson", description="Expand terms using a dictionary"
+    )
+
+    _defn = EnumDefinition(
+        name="TransformationType",
+        description="A controlled datamodels of the types of transformation that can be applied to",
+    )
 
 
 # Slots
 class slots:
     pass
 
 
-slots.subject_id = Slot(
-    uri=SSSOM.subject_id,
-    name="subject_id",
-    curie=SSSOM.curie("subject_id"),
-    model_uri=SIM.subject_id,
+slots.textAnnotationConfiguration__matches_whole_text = Slot(
+    uri=ANN.matches_whole_text,
+    name="textAnnotationConfiguration__matches_whole_text",
+    curie=ANN.curie("matches_whole_text"),
+    model_uri=ANN.textAnnotationConfiguration__matches_whole_text,
     domain=None,
-    range=Union[str, URIorCURIE],
+    range=Optional[Union[bool, Bool]],
 )
 
-slots.subject_label = Slot(
-    uri=SSSOM.subject_label,
-    name="subject_label",
-    curie=SSSOM.curie("subject_label"),
-    model_uri=SIM.subject_label,
+slots.textAnnotationConfiguration__sources = Slot(
+    uri=ANN.sources,
+    name="textAnnotationConfiguration__sources",
+    curie=ANN.curie("sources"),
+    model_uri=ANN.textAnnotationConfiguration__sources,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[str, List[str]]],
 )
 
-slots.subject_source = Slot(
-    uri=SSSOM.subject_source,
-    name="subject_source",
-    curie=SSSOM.curie("subject_source"),
-    model_uri=SIM.subject_source,
+slots.textAnnotationConfiguration__limit = Slot(
+    uri=ANN.limit,
+    name="textAnnotationConfiguration__limit",
+    curie=ANN.curie("limit"),
+    model_uri=ANN.textAnnotationConfiguration__limit,
     domain=None,
-    range=Optional[str],
+    range=Optional[int],
 )
 
-slots.object_id = Slot(
-    uri=SSSOM.object_id,
-    name="object_id",
-    curie=SSSOM.curie("object_id"),
-    model_uri=SIM.object_id,
+slots.textAnnotationConfiguration__token_exclusion_list = Slot(
+    uri=ANN.token_exclusion_list,
+    name="textAnnotationConfiguration__token_exclusion_list",
+    curie=ANN.curie("token_exclusion_list"),
+    model_uri=ANN.textAnnotationConfiguration__token_exclusion_list,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[str, List[str]]],
 )
 
-slots.object_label = Slot(
-    uri=SSSOM.object_label,
-    name="object_label",
-    curie=SSSOM.curie("object_label"),
-    model_uri=SIM.object_label,
+slots.textAnnotationConfiguration__model = Slot(
+    uri=ANN.model,
+    name="textAnnotationConfiguration__model",
+    curie=ANN.curie("model"),
+    model_uri=ANN.textAnnotationConfiguration__model,
     domain=None,
     range=Optional[str],
 )
 
-slots.object_source = Slot(
-    uri=SSSOM.object_source,
-    name="object_source",
-    curie=SSSOM.curie("object_source"),
-    model_uri=SIM.object_source,
+slots.textAnnotationConfiguration__include_aliases = Slot(
+    uri=ANN.include_aliases,
+    name="textAnnotationConfiguration__include_aliases",
+    curie=ANN.curie("include_aliases"),
+    model_uri=ANN.textAnnotationConfiguration__include_aliases,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[bool, Bool]],
 )
 
-slots.ancestor_id = Slot(
-    uri=SIM.ancestor_id,
-    name="ancestor_id",
-    curie=SIM.curie("ancestor_id"),
-    model_uri=SIM.ancestor_id,
+slots.textAnnotationResultSet__annotations = Slot(
+    uri=ANN.annotations,
+    name="textAnnotationResultSet__annotations",
+    curie=ANN.curie("annotations"),
+    model_uri=ANN.textAnnotationResultSet__annotations,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[Union[Union[dict, TextAnnotation], List[Union[dict, TextAnnotation]]]],
 )
 
-slots.ancestor_label = Slot(
-    uri=SIM.ancestor_label,
-    name="ancestor_label",
-    curie=SIM.curie("ancestor_label"),
-    model_uri=SIM.ancestor_label,
+slots.textualElement__id = Slot(
+    uri=ANN.id,
+    name="textualElement__id",
+    curie=ANN.curie("id"),
+    model_uri=ANN.textualElement__id,
     domain=None,
-    range=Optional[str],
+    range=URIRef,
 )
 
-slots.ancestor_source = Slot(
-    uri=SIM.ancestor_source,
-    name="ancestor_source",
-    curie=SIM.curie("ancestor_source"),
-    model_uri=SIM.ancestor_source,
+slots.textualElement__text = Slot(
+    uri=ANN.text,
+    name="textualElement__text",
+    curie=ANN.curie("text"),
+    model_uri=ANN.textualElement__text,
     domain=None,
     range=Optional[str],
 )
 
-slots.score = Slot(
-    uri=SIM.score,
-    name="score",
-    curie=SIM.curie("score"),
-    model_uri=SIM.score,
+slots.textualElement__source_text = Slot(
+    uri=ANN.source_text,
+    name="textualElement__source_text",
+    curie=ANN.curie("source_text"),
+    model_uri=ANN.textualElement__source_text,
     domain=None,
     range=Optional[str],
 )
 
-slots.information_content = Slot(
-    uri=SIM.information_content,
-    name="information_content",
-    curie=SIM.curie("information_content"),
-    model_uri=SIM.information_content,
-    domain=None,
-    range=Optional[Union[float, NegativeLogValue]],
-)
-
-slots.subject_information_content = Slot(
-    uri=SIM.subject_information_content,
-    name="subject_information_content",
-    curie=SIM.curie("subject_information_content"),
-    model_uri=SIM.subject_information_content,
-    domain=None,
-    range=Optional[Union[float, NegativeLogValue]],
-)
-
-slots.object_information_content = Slot(
-    uri=SIM.object_information_content,
-    name="object_information_content",
-    curie=SIM.curie("object_information_content"),
-    model_uri=SIM.object_information_content,
-    domain=None,
-    range=Optional[Union[float, NegativeLogValue]],
-)
-
-slots.ancestor_information_content = Slot(
-    uri=SIM.ancestor_information_content,
-    name="ancestor_information_content",
-    curie=SIM.curie("ancestor_information_content"),
-    model_uri=SIM.ancestor_information_content,
-    domain=None,
-    range=Optional[Union[float, NegativeLogValue]],
-)
-
-slots.jaccard_similarity = Slot(
-    uri=SIM.jaccard_similarity,
-    name="jaccard_similarity",
-    curie=SIM.curie("jaccard_similarity"),
-    model_uri=SIM.jaccard_similarity,
-    domain=None,
-    range=Optional[Union[float, ZeroToOne]],
-)
-
-slots.dice_similarity = Slot(
-    uri=SIM.dice_similarity,
-    name="dice_similarity",
-    curie=SIM.curie("dice_similarity"),
-    model_uri=SIM.dice_similarity,
-    domain=None,
-    range=Optional[Union[float, ZeroToOne]],
-)
-
-slots.phenodigm_score = Slot(
-    uri=SIM.phenodigm_score,
-    name="phenodigm_score",
-    curie=SIM.curie("phenodigm_score"),
-    model_uri=SIM.phenodigm_score,
+slots.textualElement__parent_document = Slot(
+    uri=ANN.parent_document,
+    name="textualElement__parent_document",
+    curie=ANN.curie("parent_document"),
+    model_uri=ANN.textualElement__parent_document,
     domain=None,
-    range=Optional[Union[float, NonNegativeFloat]],
-)
-
-slots.overlap_coefficient = Slot(
-    uri=SIM.overlap_coefficient,
-    name="overlap_coefficient",
-    curie=SIM.curie("overlap_coefficient"),
-    model_uri=SIM.overlap_coefficient,
-    domain=None,
-    range=Optional[Union[float, ZeroToOne]],
+    range=Optional[Union[str, URIorCURIE]],
 )
 
-slots.subsumes_score = Slot(
-    uri=SIM.subsumes_score,
-    name="subsumes_score",
-    curie=SIM.curie("subsumes_score"),
-    model_uri=SIM.subsumes_score,
+slots.hasSpan__subject_start = Slot(
+    uri=ANN.subject_start,
+    name="hasSpan__subject_start",
+    curie=ANN.curie("subject_start"),
+    model_uri=ANN.hasSpan__subject_start,
     domain=None,
-    range=Optional[Union[float, ZeroToOne]],
+    range=Optional[Union[int, Position]],
 )
 
-slots.subsumed_by_score = Slot(
-    uri=SIM.subsumed_by_score,
-    name="subsumed_by_score",
-    curie=SIM.curie("subsumed_by_score"),
-    model_uri=SIM.subsumed_by_score,
+slots.hasSpan__subject_end = Slot(
+    uri=ANN.subject_end,
+    name="hasSpan__subject_end",
+    curie=ANN.curie("subject_end"),
+    model_uri=ANN.hasSpan__subject_end,
     domain=None,
-    range=Optional[Union[float, ZeroToOne]],
+    range=Optional[Union[int, Position]],
 )
 
-slots.intersection_count = Slot(
-    uri=SIM.intersection_count,
-    name="intersection_count",
-    curie=SIM.curie("intersection_count"),
-    model_uri=SIM.intersection_count,
+slots.hasSpan__subject_label = Slot(
+    uri=ANN.subject_label,
+    name="hasSpan__subject_label",
+    curie=ANN.curie("subject_label"),
+    model_uri=ANN.hasSpan__subject_label,
     domain=None,
-    range=Optional[Union[int, ItemCount]],
+    range=Optional[str],
 )
 
-slots.union_count = Slot(
-    uri=SIM.union_count,
-    name="union_count",
-    curie=SIM.curie("union_count"),
-    model_uri=SIM.union_count,
+slots.hasSpan__subject_source = Slot(
+    uri=SSSOM.subject_source,
+    name="hasSpan__subject_source",
+    curie=SSSOM.curie("subject_source"),
+    model_uri=ANN.hasSpan__subject_source,
     domain=None,
-    range=Optional[Union[int, ItemCount]],
+    range=Optional[str],
 )
 
-slots.subject_termset = Slot(
-    uri=SIM.subject_termset,
-    name="subject_termset",
-    curie=SIM.curie("subject_termset"),
-    model_uri=SIM.subject_termset,
+slots.hasSpan__subject_text_id = Slot(
+    uri=ANN.subject_text_id,
+    name="hasSpan__subject_text_id",
+    curie=ANN.curie("subject_text_id"),
+    model_uri=ANN.hasSpan__subject_text_id,
     domain=None,
-    range=Optional[
-        Union[Dict[Union[str, TermInfoId], Union[dict, TermInfo]], List[Union[dict, TermInfo]]]
-    ],
+    range=Optional[Union[str, TextualElementId]],
 )
 
-slots.object_termset = Slot(
-    uri=SIM.object_termset,
-    name="object_termset",
-    curie=SIM.curie("object_termset"),
-    model_uri=SIM.object_termset,
+slots.textAnnotation__predicate_id = Slot(
+    uri=SSSOM.predicate_id,
+    name="textAnnotation__predicate_id",
+    curie=SSSOM.curie("predicate_id"),
+    model_uri=ANN.textAnnotation__predicate_id,
     domain=None,
-    range=Optional[
-        Union[Dict[Union[str, TermInfoId], Union[dict, TermInfo]], List[Union[dict, TermInfo]]]
-    ],
+    range=Optional[str],
 )
 
-slots.subject_best_matches = Slot(
-    uri=SIM.subject_best_matches,
-    name="subject_best_matches",
-    curie=SIM.curie("subject_best_matches"),
-    model_uri=SIM.subject_best_matches,
+slots.textAnnotation__object_id = Slot(
+    uri=SSSOM.object_id,
+    name="textAnnotation__object_id",
+    curie=SSSOM.curie("object_id"),
+    model_uri=ANN.textAnnotation__object_id,
     domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, BestMatchMatchSource], Union[dict, BestMatch]],
-            List[Union[dict, BestMatch]],
-        ]
-    ],
-)
-
-slots.object_best_matches = Slot(
-    uri=SIM.object_best_matches,
-    name="object_best_matches",
-    curie=SIM.curie("object_best_matches"),
-    model_uri=SIM.object_best_matches,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, BestMatchMatchSource], Union[dict, BestMatch]],
-            List[Union[dict, BestMatch]],
-        ]
-    ],
+    range=Optional[str],
 )
 
-slots.metric = Slot(
-    uri=SIM.metric,
-    name="metric",
-    curie=SIM.curie("metric"),
-    model_uri=SIM.metric,
+slots.textAnnotation__object_label = Slot(
+    uri=SSSOM.object_label,
+    name="textAnnotation__object_label",
+    curie=SSSOM.curie("object_label"),
+    model_uri=ANN.textAnnotation__object_label,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=Optional[str],
 )
 
-slots.average_score = Slot(
-    uri=SIM.average_score,
-    name="average_score",
-    curie=SIM.curie("average_score"),
-    model_uri=SIM.average_score,
+slots.textAnnotation__object_source = Slot(
+    uri=SSSOM.object_source,
+    name="textAnnotation__object_source",
+    curie=SSSOM.curie("object_source"),
+    model_uri=ANN.textAnnotation__object_source,
     domain=None,
-    range=Optional[float],
+    range=Optional[str],
 )
 
-slots.best_score = Slot(
-    uri=SIM.best_score,
-    name="best_score",
-    curie=SIM.curie("best_score"),
-    model_uri=SIM.best_score,
+slots.textAnnotation__confidence = Slot(
+    uri=SSSOM.confidence,
+    name="textAnnotation__confidence",
+    curie=SSSOM.curie("confidence"),
+    model_uri=ANN.textAnnotation__confidence,
     domain=None,
     range=Optional[float],
 )
 
-slots.termInfo__id = Slot(
-    uri=SIM.id,
-    name="termInfo__id",
-    curie=SIM.curie("id"),
-    model_uri=SIM.termInfo__id,
-    domain=None,
-    range=URIRef,
-)
-
-slots.termInfo__label = Slot(
-    uri=RDFS.label,
-    name="termInfo__label",
-    curie=RDFS.curie("label"),
-    model_uri=SIM.termInfo__label,
+slots.textAnnotation__match_string = Slot(
+    uri=SSSOM.match_string,
+    name="textAnnotation__match_string",
+    curie=SSSOM.curie("match_string"),
+    model_uri=ANN.textAnnotation__match_string,
     domain=None,
     range=Optional[str],
 )
 
-slots.bestMatch__match_source = Slot(
-    uri=SIM.match_source,
-    name="bestMatch__match_source",
-    curie=SIM.curie("match_source"),
-    model_uri=SIM.bestMatch__match_source,
-    domain=None,
-    range=URIRef,
-)
-
-slots.bestMatch__match_source_label = Slot(
-    uri=SIM.match_source_label,
-    name="bestMatch__match_source_label",
-    curie=SIM.curie("match_source_label"),
-    model_uri=SIM.bestMatch__match_source_label,
+slots.textAnnotation__is_longest_match = Slot(
+    uri=ANN.is_longest_match,
+    name="textAnnotation__is_longest_match",
+    curie=ANN.curie("is_longest_match"),
+    model_uri=ANN.textAnnotation__is_longest_match,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[bool, Bool]],
 )
 
-slots.bestMatch__match_target = Slot(
-    uri=SIM.match_target,
-    name="bestMatch__match_target",
-    curie=SIM.curie("match_target"),
-    model_uri=SIM.bestMatch__match_target,
+slots.textAnnotation__matches_whole_text = Slot(
+    uri=ANN.matches_whole_text,
+    name="textAnnotation__matches_whole_text",
+    curie=ANN.curie("matches_whole_text"),
+    model_uri=ANN.textAnnotation__matches_whole_text,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[bool, Bool]],
 )
 
-slots.bestMatch__match_target_label = Slot(
-    uri=SIM.match_target_label,
-    name="bestMatch__match_target_label",
-    curie=SIM.curie("match_target_label"),
-    model_uri=SIM.bestMatch__match_target_label,
+slots.textAnnotation__match_type = Slot(
+    uri=ANN.match_type,
+    name="textAnnotation__match_type",
+    curie=ANN.curie("match_type"),
+    model_uri=ANN.textAnnotation__match_type,
     domain=None,
     range=Optional[str],
 )
 
-slots.bestMatch__score = Slot(
-    uri=SIM.score,
-    name="bestMatch__score",
-    curie=SIM.curie("score"),
-    model_uri=SIM.bestMatch__score,
-    domain=None,
-    range=float,
-)
-
-slots.bestMatch__match_subsumer = Slot(
-    uri=SIM.match_subsumer,
-    name="bestMatch__match_subsumer",
-    curie=SIM.curie("match_subsumer"),
-    model_uri=SIM.bestMatch__match_subsumer,
-    domain=None,
-    range=Optional[Union[str, URIorCURIE]],
-)
-
-slots.bestMatch__match_subsumer_label = Slot(
-    uri=SIM.match_subsumer_label,
-    name="bestMatch__match_subsumer_label",
-    curie=SIM.curie("match_subsumer_label"),
-    model_uri=SIM.bestMatch__match_subsumer_label,
+slots.textAnnotation__info = Slot(
+    uri=ANN.info,
+    name="textAnnotation__info",
+    curie=ANN.curie("info"),
+    model_uri=ANN.textAnnotation__info,
     domain=None,
     range=Optional[str],
 )
 
-slots.bestMatch__similarity = Slot(
-    uri=SIM.similarity,
-    name="bestMatch__similarity",
-    curie=SIM.curie("similarity"),
-    model_uri=SIM.bestMatch__similarity,
+slots.textAnnotation__object_aliases = Slot(
+    uri=ANN.object_aliases,
+    name="textAnnotation__object_aliases",
+    curie=ANN.curie("object_aliases"),
+    model_uri=ANN.textAnnotation__object_aliases,
     domain=None,
-    range=Union[dict, TermPairwiseSimilarity],
+    range=Optional[Union[str, List[str]]],
 )
```

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.4/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.4/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.4/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.4/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.4/src/oaklib/datamodels/vocabulary.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 IS_A = omd.slots.subClassOf.curie
 DISJOINT_WITH = "owl:disjointWith"
 SUBPROPERTY_OF = "rdfs:subPropertyOf"
 RDFS_DOMAIN = "rdfs:domain"
 RDFS_RANGE = "rdfs:range"
 INVERSE_OF = "owl:inverseOf"
 RDF_TYPE = "rdf:type"
+RDFS_LABEL = "rdfs:label"
 EQUIVALENT_CLASS = "owl:equivalentClass"
 OWL_SAME_AS = "owl:sameAs"
 RDF_SEE_ALSO = "rdfs:seeAlso"
 
 OWL_META_CLASSES = [
     OWL_CLASS,
     OWL_OBJECT_PROPERTY,
```

### Comparing `oaklib-0.5.3/src/oaklib/implementations/__init__.py` & `oaklib-0.5.4/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/gilda.py` & `oaklib-0.5.4/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.4/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.4/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/rustsim/rustsim_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/rustsim/rustsim_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.4/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.4/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     OWL_NOTHING,
     OWL_THING,
     OWL_VERSION_IRI,
     PREFIX_PREDICATE,
     RDF_TYPE,
     RDFS_COMMENT,
     RDFS_DOMAIN,
+    RDFS_LABEL,
     RDFS_RANGE,
     SEMAPV,
     STANDARD_ANNOTATION_PROPERTIES,
     SUBPROPERTY_OF,
     SYNONYM_PREDICATES,
     TERM_REPLACED_BY,
     TERMS_MERGED,
@@ -1132,21 +1133,31 @@
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: AssocationProviderInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def associations(self, *args, **kwargs) -> Iterator[Association]:
         if not self.can_store_associations:
+            logging.info("Using base method")
             yield from super().associations(*args, **kwargs)
             return
         q = self._associations_query(*args, **kwargs)
-        for row in q:
-            yield Association(
-                row.subject, row.predicate, row.object, primary_knowledge_source=row.source
-            )
+        for row_it in chunk(q):
+            assocs = []
+            for row in row_it:
+                association = Association(
+                    row.subject, row.predicate, row.object, primary_knowledge_source=row.source
+                )
+                assocs.append(association)
+            subjects = {a.subject for a in assocs}
+            label_map = {s: l for s, l in self.labels(subjects)}
+            for association in assocs:
+                if association.subject in label_map:
+                    association.subject_label = label_map[association.subject]
+            yield from assocs
 
     def _associations_query(
         self,
         subjects: Iterable[CURIE] = None,
         predicates: Iterable[PRED_CURIE] = None,
         objects: Iterable[CURIE] = None,
         property_filter: Dict[PRED_CURIE, Any] = None,
@@ -1187,15 +1198,18 @@
                 q = q.filter(TermAssociation.object.in_(subquery))
             else:
                 q = q.filter(TermAssociation.object.in_(tuple(objects)))
         logging.info(f"Association query: {q}")
         return q
 
     def add_associations(
-        self, associations: Iterable[Association], normalizers: List[EntityNormalizer] = None
+        self,
+        associations: Iterable[Association],
+        normalizers: List[EntityNormalizer] = None,
+        **kwargs,
     ) -> bool:
         if not self.can_store_associations:
             return super().add_associations(associations, normalizers=normalizers)
         for a in associations:
             if normalizers:
                 a = a.normalize(normalizers)
             if a.property_values:
@@ -1203,14 +1217,21 @@
             stmt = insert(TermAssociation).values(
                 subject=a.subject,
                 predicate=a.predicate,
                 object=a.object,
                 source=a.primary_knowledge_source,
             )
             self._execute(stmt)
+            if a.subject_label:
+                stmt = insert(Statements).values(
+                    subject=a.subject,
+                    predicate=RDFS_LABEL,
+                    value=a.subject_label,
+                )
+                self._execute(stmt)
         self.session.flush()
         return True
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: OboGraphInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
```

### Comparing `oaklib-0.5.3/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.4/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.4/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.4/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/association_provider_interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import logging
 from abc import ABC
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple
 
-from oaklib.datamodels.association import Association
+from oaklib.datamodels.association import Association, PairwiseCoAssociation
 from oaklib.interfaces import MappingProviderInterface
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE, PRED_CURIE, SUBSET_CURIE
 from oaklib.utilities.associations.association_index import AssociationIndex
+from oaklib.utilities.iterator_utils import chunk
+
+ASSOCIATION_CORRELATION = Tuple[
+    CURIE, CURIE, int, Optional[List[CURIE]], Optional[List[Association]]
+]
 
 
 def associations_subjects(associations: Iterable[Association]) -> Iterator[CURIE]:
     """
     Yields distinct subjects for all associations.
 
     :param associations:
@@ -61,14 +66,65 @@
     slots: List[str] = field(default_factory=list)
 
 
 @dataclass
 class AssociationProviderInterface(BasicOntologyInterface, ABC):
     """
     An ontology provider that provides associations.
+
+    Associations (also known as annotations) connect data elements or entities to
+    an ontology class. Examples of associations include:
+
+    - Gene associations to terms in ontologies like GO, Mondo, Uberon, HPO, MPO, CL
+    - Associations between spans of text and ontology entities
+
+    Data models and file formats include:
+
+    - The GO GAF and GPAD formats.
+    - The HPOA association file format.
+    - KGX (Knowledge Graph Exchange).
+    - The W3 `Open Annotation <https://www.w3.org/TR/annotation-model/>`_ (OA) data model
+
+    The OA datamodel considers an annotation to be between a *body* and a *target*:
+
+    .. image:: https://www.w3.org/TR/annotation-vocab/images/examples/annotation.png
+
+    .. warning::
+
+        the signature of some methods are subject to change while we
+        decide on the best patterns to define here.
+
+    Note that most ontology sources are not themselves providers of associations; there is no agreed upon
+    way to represent associations in OWL, and associations are typically distributed separately from
+    ontologies. See the section :ref:`associations` in the OAK guide for more details.
+
+    OAK provides a number of ways to augment an ontology adapter with associations.
+
+    The most expressive way is to provide an :ref:`InputSpecification`:
+
+    >>> from oaklib import get_adapter
+    >>> adapter = get_adapter("src/oaklib/conf/go-pombase-input-spec.yaml")
+
+    This combines an ontology source with one or more association sources.
+
+    Another approach is to use an adapter that directly supports associations. An example of this
+    is the :ref:`amigo_implementation`:
+
+    >>> from oaklib import get_adapter
+    >>> amigo = get_adapter("amigo:NCBITaxon:10090") # mouse
+
+
+
+
+    Command Line Use
+    ----------------
+
+    .. code::
+
+       runoak -i foo.db associations UBERON:0002101
     """
 
     _association_index: AssociationIndex = None
     """In-memory index of associations"""
 
     normalizers: List[EntityNormalizer] = field(default_factory=list)
 
@@ -82,24 +138,42 @@
         predicate_closure_predicates: Optional[List[PRED_CURIE]] = None,
         object_closure_predicates: Optional[List[PRED_CURIE]] = None,
         include_modified: bool = False,
     ) -> Iterator[Association]:
         """
         Yield all matching associations.
 
+        To query by subject (e.g. genes):
+
         >>> from oaklib import get_adapter
         >>> adapter = get_adapter("src/oaklib/conf/go-pombase-input-spec.yaml")
         >>> genes = ["PomBase:SPAC1142.02c", "PomBase:SPAC3H1.05", "PomBase:SPAC1142.06", "PomBase:SPAC4G8.02c"]
         >>> for assoc in adapter.associations(genes):
         ...    print(f"{assoc.object} {adapter.label(assoc.object)}")
         <BLANKLINE>
         ...
         GO:0006620 post-translational protein targeting to endoplasmic reticulum membrane
         ...
 
+        To query by object (e.g. descriptor terms):
+
+        >>> from oaklib import get_adapter
+        >>> from oaklib.datamodels.vocabulary import IS_A, PART_OF
+        >>> adapter = get_adapter("src/oaklib/conf/go-pombase-input-spec.yaml")
+        >>> for assoc in adapter.associations(objects=["GO:0006620"], object_closure_predicates=[IS_A, PART_OF]):
+        ...    print(f"{assoc.subject} {assoc.subject_label}")
+        <BLANKLINE>
+        ...
+        PomBase:SPAC1142.02c sgt2
+        ...
+
+        When determinining a match on `objects`, the predicates in ``object_closure_predicates`` is used.
+        We recommend you always explicitly provide this. A good choice is typically IS_A and PART_OF for
+        ontologies like GO, Uberon, CL, ENVO.
+
         :param subjects: constrain to these subjects (e.g. genes in a gene association)
         :param predicates: constrain to these predicates (e.g. involved-in for a gene to pathway association)
         :param objects: constrain to these objects (e.g. terms)
         :param property_filter: generic query filter
         :param subject_closure_predicates: subjects is treated as descendant via these predicates
         :param predicate_closure_predicates: predicates is treated as descendant via these predicates
         :param object_closure_predicates: object is treated as descendant via these predicates
@@ -115,16 +189,116 @@
                 )
             else:
                 raise NotImplementedError
         ix = self._association_index
         if ix is None:
             logging.warning("No association index")
             return
-        for a in ix.lookup(subjects, predicates, objects):
-            yield a
+        yield from ix.lookup(subjects, predicates, objects)
+
+    def _inject_subject_labels(self, association_iterator: Iterable[Association]):
+        for assoc_it in chunk(association_iterator):
+            associations = list(assoc_it)
+            subjects = {a.subject for a in associations}
+            label_map = {s: l for s, l in self.labels(subjects)}
+            logging.info(f"LABEL MAP: {label_map} for {subjects}")
+            for association in associations:
+                if association.subject in label_map:
+                    association.subject_label = label_map[association.subject]
+            yield from associations
+
+    def associations_subjects(self, **kwargs) -> Iterator[CURIE]:
+        """
+        Yields all distinct subjects.
+
+        >>> from oaklib import get_adapter
+        >>> from oaklib.datamodels.vocabulary import IS_A, PART_OF
+        >>> adapter = get_adapter("src/oaklib/conf/go-pombase-input-spec.yaml")
+        >>> genes = ["PomBase:SPAC1142.02c", "PomBase:SPAC3H1.05", "PomBase:SPAC1142.06", "PomBase:SPAC4G8.02c"]
+        >>> for assoc in adapter.associations(genes, object_closure_predicates=[IS_A, PART_OF]):
+        ...    print(f"{assoc.object} {adapter.label(assoc.object)}")
+        <BLANKLINE>
+        ...
+        GO:0006620 post-translational protein targeting to endoplasmic reticulum membrane
+        ...
+
+        :param kwargs: same arguments as for :ref:`associations`
+        :return:
+        """
+        # individual implementations should override this to be more efficient
+        yielded = set()
+        for a in self.associations(**kwargs):
+            s = a.subject
+            if s in yielded:
+                continue
+            yield s
+            yielded.add(s)
+
+    def association_pairwise_coassociations(
+        self,
+        curies1: Iterable[CURIE],
+        curies2: Iterable[CURIE],
+        inputs_are_subjects=False,
+        include_reciprocals=False,
+        include_diagonal=True,
+        include_entities=True,
+        **kwargs,
+    ) -> Iterator[PairwiseCoAssociation]:
+        """
+        Find co-associations.
+
+        >>> from oaklib import get_adapter
+        >>> from oaklib.datamodels.vocabulary import IS_A, PART_OF
+        >>> adapter = get_adapter("src/oaklib/conf/go-pombase-input-spec.yaml")
+        >>> terms = ["GO:0000910", "GO:0006281", "GO:0006412"]
+        >>> preds = [IS_A, PART_OF]
+        >>> for coassoc in adapter.association_pairwise_coassociations(curies1=terms,
+        ...                                              curies2=terms,
+        ...                                              object_closure_predicates=preds):
+        ...    print(coassoc.object1, coassoc.object2, coassoc.number_subjects_in_common)
+        <BLANKLINE>
+        ...
+        GO:0006281 GO:0000910 0
+        ...
+
+        :param curies1:
+        :param curies2:
+        :param inputs_are_subjects:
+        :param kwargs:
+        :return:
+        """
+        if inputs_are_subjects:
+            raise NotImplementedError
+        curies1 = list(curies1)
+        curies2 = list(curies2)
+        assocmap1 = {c: list(self.associations(objects=[c], **kwargs)) for c in curies1}
+        assocmap2 = {c: list(self.associations(objects=[c], **kwargs)) for c in curies2}
+        for c1 in curies1:
+            for c2 in curies2:
+                if c2 > c1 and not include_reciprocals:
+                    continue
+                if c1 == c2 and not include_diagonal:
+                    continue
+                assocs1 = assocmap1[c1]
+                assocs2 = assocmap2[c2]
+                elements1 = {a.subject for a in assocs1}
+                elements2 = {a.subject for a in assocs2}
+                common = elements1.intersection(elements2)
+                assocs_to_common = [a for a in assocs1 + assocs2 if a.subject in common]
+                coassoc = PairwiseCoAssociation(
+                    object1=c1,
+                    object2=c2,
+                    number_subjects_in_common=len(common),
+                    number_subject_unique_to_entity1=len(elements1.difference(elements2)),
+                    number_subject_unique_to_entity2=len(elements2.difference(elements1)),
+                )
+                if include_entities:
+                    coassoc.subjects_in_common = list(common)
+                    coassoc.associations_for_subjects_in_common = assocs_to_common
+                yield coassoc
 
     def add_associations(
         self,
         associations: Iterable[Association],
         normalizers: List[EntityNormalizer] = None,
         **kwargs,
     ) -> bool:
```

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         GO:0006620 post-translational protein targeting to endoplasmic reticulum membrane
         ...
 
         :param subjects: The set of entities to test for over-representation of classes
         :param item_list: An item list objects as an alternate way to specify subjects
         :param background: The set of entities to use as a background for the test (recommended)
         :param hypotheses: The set of classes to test for over-representation (default is all)
-        :param cutoff: The threshold to use for p-value
+        :param cutoff: The threshold to use for the adjusted p-value
         :param labels: Whether to include labels (names) for the classes
         :param direction: The direction of the test. One of 'greater', 'less', 'two-sided'
         :param filter_redundant: Whether to filter out redundant hypotheses
         :param sort_by: The field to sort by. One of 'p_value', 'sample_count', 'background_count', 'odds_ratio'
         :param direction: The direction of the test. One of 'greater', 'less', 'two-sided'
         :return: An iterator over ClassEnrichmentResult objects
         """
```

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,31 @@
     .. note ::
 
         most ontologies only include minimal metadata about mappings at this time, so many fields
         in the sssom mapping datamodel are not populated.
 
     The core method in this interface is :py:meth:`sssom_mappings`.
 
+    .. note ::
+
+        This interface is for serving pre-calculated mappings.
+        See :ref:`sssom_utils` for on-the-fly mapping creation
+
+
+    Data Model
+    -----------
+
+    The central datamodel used here is `SSSOM <http://w3id.org/sssom>`_
+
+    Command Line Use
+    ----------------
+
+    .. code::
+
+       runoak -i bioportal: term-mappings UBERON:0002101  -O sssom -o limb-mappings.sssom.tsv
     """
 
     def sssom_mappings(
         self, curies: Optional[Union[CURIE, Iterable[CURIE]]] = None, source: Optional[str] = None
     ) -> Iterable[Mapping]:
         """
         returns all sssom mappings matching filter conditions.
```

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.4/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.4/src/oaklib/io/heatmap_writer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Dict, List, Union
 
 from linkml_runtime.utils.yamlutils import YAMLRoot
 
+from oaklib.datamodels.association import PairwiseCoAssociation
 from oaklib.datamodels.similarity import TermPairwiseSimilarity
 from oaklib.io.streaming_writer import StreamingWriter
 
 
 @dataclass
 class HeatmapWriter(StreamingWriter):
     """
@@ -30,18 +31,27 @@
 
     def emit(self, obj: Union[YAMLRoot, dict], label_fields=None):
         if isinstance(obj, TermPairwiseSimilarity):
             t1 = obj.subject_id + f" {obj.subject_label}" if obj.subject_label else ""
             t2 = obj.object_id + f" {obj.object_label}" if obj.object_label else ""
             v = getattr(obj, self.value_field)
             self.items.append({"term1": t1, "term2": t2, "score": v})
+        if isinstance(obj, PairwiseCoAssociation):
+            if label_fields and self.autolabel:
+                t1 = f"{obj.object1} {self.ontology_interface.label(obj.object1)}"
+                t2 = f"{obj.object2} {self.ontology_interface.label(obj.object2)}"
+            else:
+                t1 = obj.object1
+                t2 = obj.object2
+            v = obj.number_subjects_in_common
+            self.items.append({"term1": t1, "term2": t2, "score": v})
         else:
             raise ValueError(f"Cannot handle: {obj}")
 
     def finish(self):
         import pandas
         import seaborn
 
         df = pandas.DataFrame(self.items)
-        df = df.pivot(*list(self.items[0].keys()))
+        df = df.pivot(index="term1", columns="term2", values="score")
         ax = seaborn.heatmap(df, annot=True, fmt=".2f")
         ax.get_figure().savefig(self.output, bbox_inches="tight")
```

### Comparing `oaklib-0.5.3/src/oaklib/io/html_writer.py` & `oaklib-0.5.4/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.4/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.4/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_csv_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 NULL_VALUE = "None"
 
 
 def _keyval(x: Any) -> str:
     if isinstance(x, CurieNamespace):
         return str(x.curie())
+    if isinstance(x, list):
+        return "|".join([str(v) for v in x])
     # if isinstance(x, EnumDefinitionImpl):
     #    if x.curie:
     #        return str(x.curie)
     return str(x)
 
 
 @dataclass(eq=False)
```

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.4/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.4/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.4/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/__init__.py` & `oaklib-0.5.4/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.4/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/phaf_association_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-"""Parser for GAF association formats"""
+"""Parser for PomBase PHAF association formats"""
 from dataclasses import dataclass, field
 
 from oaklib.parsers.parser_base import ColumnReference
 from oaklib.parsers.xaf_association_parser import XafAssociationParser
 
 
 @dataclass
-class HpoaAssociationParser(XafAssociationParser):
-    """Parsers for Hpoa format."""
+class PhafAssociationParser(XafAssociationParser):
+    """Parsers for PHAF format."""
 
     comment_character: str = "#"
 
-    subject_column: ColumnReference = field(default_factory=lambda: ColumnReference(0))
+    subject_prefix_column: ColumnReference = field(default_factory=lambda: ColumnReference(0))
+    subject_column: ColumnReference = field(default_factory=lambda: ColumnReference(1))
     predicate_column: ColumnReference = None
-    object_column: ColumnReference = field(default_factory=lambda: ColumnReference(3))
+    object_column: ColumnReference = field(default_factory=lambda: ColumnReference(2))
+    expected_object_prefixes = ["FYPO"]
```

### Comparing `oaklib-0.5.3/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.4/src/oaklib/parsers/parser_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 
         :param file: file-like object to parse
         :param kwargs: additional arguments
         :return:
         """
         raise NotImplementedError
 
-    def index_lookup_function(self, column_reference: Optional[ColumnReference]) -> Callable:
+    def index_lookup_function(
+        self, column_reference: Optional[ColumnReference]
+    ) -> Optional[Callable]:
         """
         Returns a function that can be used to lookup a row by reference.
 
         :param column_reference:
         :return:
         """
         if column_reference is None:
```

### Comparing `oaklib-0.5.3/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.4/src/oaklib/parsers/xaf_association_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass, field
 from typing import Dict, Iterator, List, Optional, TextIO, Union
 
 from oaklib.datamodels.association import (
     Association,
     NegatedAssociation,
     ParserConfiguration,
+    PropertyValue,
 )
 from oaklib.parsers.association_parser import AssociationParser
 from oaklib.parsers.parser_base import ColumnReference
 
 
 def _check_identifier(s: str, expected_prefixes: List[str], must_be_curie: bool):
     if ":" not in s:
@@ -58,24 +59,34 @@
     """
 
     subject_column: Optional[ColumnReference] = None
     """
     Column that contains the subject (e.g. gene ID).
     """
 
+    subject_label_column: Optional[ColumnReference] = None
+    """
+    Column that contains the subject label (e.g. gene symbol)
+    """
+
     predicate_column: Optional[ColumnReference] = None
     """
     Column that contains the predicate (e.g. RO:0002200)
     """
 
     object_column: Optional[ColumnReference] = None
     """
     Column that contains the object (e.g. GO or Phenotype term ID)
     """
 
+    object_label_column: Optional[ColumnReference] = None
+    """
+    Column that contains the object label (e.g. term name)
+    """
+
     subject_must_be_curie = False
     """
     If True, then the subject column is validated to ensure it is a CURIE
     """
 
     object_must_be_curie = False
     """
@@ -136,26 +147,21 @@
         :param file: File to parse
         :param configuration: Configuration for the parser
         :param kwargs: Additional arguments
         :return:
         """
         lookup_subject_prefix = self.index_lookup_function(self.subject_prefix_column)
         lookup_subject = self.index_lookup_function(self.subject_column)
+        lookup_subject_label = self.index_lookup_function(self.subject_label_column)
         lookup_predicate = self.index_lookup_function(self.predicate_column)
         lookup_object = self.index_lookup_function(self.object_column)
-        if self.publications_column:
-            lookup_publications = self.index_lookup_function(self.publications_column)
-        else:
-            lookup_publications = None
-        if self.primary_knowledge_source_column:
-            lookup_primary_knowledge_source = self.index_lookup_function(
-                self.primary_knowledge_source_column
-            )
-        else:
-            lookup_primary_knowledge_source = None
+        lookup_publications = self.index_lookup_function(self.publications_column)
+        lookup_primary_knowledge_source = self.index_lookup_function(
+            self.primary_knowledge_source_column
+        )
         if (
             self.subject_prefix_column
             and self.expected_subject_prefixes
             and self.subject_prefix not in self.expected_subject_prefixes
         ):
             raise ValueError(f"Unexpected subject prefix {self.subject_prefix} in file")
         if (
@@ -181,25 +187,34 @@
             elif self.subject_prefix:
                 s = f"{self.subject_prefix}:{s}"
             else:
                 _check_identifier(s, self.expected_subject_prefixes, self.subject_must_be_curie)
             _check_identifier(o, self.expected_object_prefixes, self.object_must_be_curie)
             if self.expected_predicates and p not in self.expected_predicates:
                 raise ValueError(f"Unexpected predicate {p} in line: {line}")
+            if s.startswith("MGI:MGI:"):
+                # TODO: make this more configurable
+                s = s.replace("MGI:MGI:", "MGI:")
             association = Association(s, p, o)
             if lookup_publications:
                 pub = lookup_publications(vals)
                 if pub:
                     association.publications = pub.split("|")
             if lookup_primary_knowledge_source:
                 src = lookup_primary_knowledge_source(vals)
                 if src:
+                    if ":" not in src:
+                        src = f"infores:{src}"
                     association.primary_knowledge_source = src
+            if lookup_subject_label:
+                sl = lookup_subject_label(vals)
+                if sl:
+                    association.subject_label = sl
             if self.other_column_mappings:
                 for i, attr in self.other_column_mappings.items():
-                    setattr(association, attr, vals[i])
+                    association.property_values[attr] = PropertyValue(attr, vals[i])
             for processed_association in self.post_process(association):
                 if isinstance(processed_association, NegatedAssociation):
                     if configuration and configuration.preserve_negated_associations:
                         yield processed_association
                 else:
                     yield processed_association
```

### Comparing `oaklib-0.5.3/src/oaklib/resource.py` & `oaklib-0.5.4/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/selector.py` & `oaklib-0.5.4/src/oaklib/selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,24 +165,26 @@
             logging.info(f"Normalizers: {normalizers}")
             add_associations(
                 adapter,
                 r.selector,
                 r.format,
                 normalizers,
                 primary_knowledge_source=r.primary_knowledge_source,
+                aggregator_knowledge_source=r.aggregator_knowledge_source,
             )
     return adapter
 
 
 def add_associations(
     adapter: AssociationProviderInterface,
     descriptor: str,
     format: str = None,
     normalizers: Optional[List[Normalizer]] = None,
     primary_knowledge_source: Optional[str] = None,
+    aggregator_knowledge_source: Optional[str] = None,
 ) -> None:
     """
     Adds associations to an adapter.
 
     :param adapter:
     :param descriptor:
     :param format:
@@ -209,16 +211,22 @@
             file = file_from_gzip_url(url)
         else:
             file = file_from_url(url)
         association_parser = get_association_parser(format)
         logging.info(f"Adding associations from {url}")
         if primary_knowledge_source is None:
             primary_knowledge_source = f"infores:{scheme}"
+        if aggregator_knowledge_source is None:
+            aggregator_knowledge_source = f"infores:{scheme}"
         assocs = list(association_parser.parse(file))
-        association_parser.add_metadata(assocs, primary_knowledge_source=primary_knowledge_source)
+        association_parser.add_metadata(
+            assocs,
+            primary_knowledge_source=primary_knowledge_source,
+            aggregator_knowledge_source=aggregator_knowledge_source,
+        )
         adapter.add_associations(assocs, normalizers=normalizers)
         return
     if not format:
         toks = descriptor.split(".")
         while toks:
             format = toks[-1]
             if format not in ("csv", "tsv", "txt"):
```

### Comparing `oaklib-0.5.3/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.4/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.4/src/oaklib/utilities/associations/association_differ.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from collections import defaultdict
 from copy import copy
 from dataclasses import dataclass, field
-from typing import Iterator, List, Mapping, Set, Tuple
+from typing import Collection, Iterator, List, Mapping, Set, Tuple
 
 from oaklib.datamodels.association import Association, AssociationChange
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE, PRED_CURIE
 from oaklib.utilities.basic_utils import pairs_as_dict
 from oaklib.utilities.subsets.slimmer_utils import filter_redundant
 
@@ -59,86 +59,119 @@
 
     def calculate_change_objects(
         self,
         assocs1: List[Association],
         assocs2: List[Association],
         predicates: List[PRED_CURIE],
     ) -> Iterator[AssociationChange]:
+        """
+        Calculates diff between two association sets.
+
+        :param assocs1: the old association set
+        :param assocs2: the new association set
+        :param predicates: closure predicates
+        :return:
+        """
         obsoletion_map = self.obsoletion_map
         subject_map1 = pairs_as_dict([(a.subject, a) for a in assocs1])
         subject_map2 = pairs_as_dict([(a.subject, a) for a in assocs2])
-        entities = set(subject_map1.keys()).union(set(subject_map2.keys()))
-        for entity in entities:
-            if entity not in subject_map1:
-                for a in subject_map2[entity]:
-                    yield AssociationChange(
-                        subject=a.subject,
-                        new_object=a.object,
-                        is_creation=True,
-                    )
-                continue
-            if entity not in subject_map2:
-                for a in subject_map1[entity]:
-                    yield AssociationChange(
-                        subject=a.subject,
-                        old_object=a.object,
-                        is_deletion=True,
-                    )
-                continue
+        entities1 = set(subject_map1.keys())
+        entities2 = set(subject_map2.keys())
+
+        def _count_closure(o: CURIE, bg: Collection[CURIE]) -> int:
+            if o in bg:
+                return 0
+            bg_closure = self.adapter.ancestors(list(bg), predicates)
+            diff = set(self.adapter.ancestors([o], predicates)).difference(bg_closure)
+            return len(diff)
+
+        for entity in entities2.difference(entities1):
+            objects1 = set([a.object for a in subject_map1[entity]])
+            for a in subject_map2[entity]:
+                yield AssociationChange(
+                    subject=a.subject,
+                    new_object=a.object,
+                    is_creation=True,
+                    closure_delta=_count_closure(a.object, objects1),
+                )
+        for entity in entities1.difference(entities2):
+            objects2 = set([a.object for a in subject_map2[entity]])
+            for a in subject_map1[entity]:
+                yield AssociationChange(
+                    subject=a.subject,
+                    old_object=a.object,
+                    is_deletion=True,
+                    closure_delta=-_count_closure(a.object, objects2),
+                )
+        for entity in entities1.intersection(entities2):
             objects1 = set([a.object for a in subject_map1[entity]])
             objects2 = set([a.object for a in subject_map2[entity]])
+            common = objects1.intersection(objects2)
             accounted_for_in_objects2 = set()
             for o in objects1.difference(objects2):
+                logging.debug(f"Trying to account for {o} (unique to old) in {entity}")
                 old_object_obsolete = False
                 if o in obsoletion_map:
                     old_object_obsolete = True
                     ixn = objects2.intersection(obsoletion_map[o])
                     if ixn:
                         for o2 in ixn:
                             yield AssociationChange(
                                 subject=entity,
                                 old_object=o,
                                 new_object=o2,
                                 is_migration=True,
                                 old_object_obsolete=old_object_obsolete,
+                                closure_predicates=predicates,
+                                closure_delta=0,
                             )
                     continue
                 if not predicates:
                     yield AssociationChange(
                         subject=entity,
                         old_object=o,
                         is_deletion=True,
                         old_object_obsolete=old_object_obsolete,
                         closure_predicates=[],
+                        closure_delta=-1,
                     )
                     continue
                 o_ancestors = list(
                     self.adapter.ancestors([o], predicates=predicates, reflexive=True)
                 )
-                ixn = objects2.intersection(o_ancestors)
+                # candidate generalizations: any ancestor of o that is
+                # not accounted for in the common set
+                ixn = objects2.intersection(o_ancestors).difference(common)
                 if ixn:
                     o2 = ixn.pop()
                     accounted_for_in_objects2.add(o2)
+                    all_o2_ancestors = list(self.adapter.ancestors(list(objects2), predicates))
                     yield AssociationChange(
                         subject=entity,
                         old_object=o,
                         new_object=o2,
                         is_generalization=True,
                         old_object_obsolete=old_object_obsolete,
                         closure_predicates=predicates,
+                        closure_delta=-_count_closure(o, all_o2_ancestors),
                     )
                     continue
-                o2_ancestors = list(
-                    self.adapter.ancestors(list(objects2), predicates=predicates, reflexive=True)
+                # detect specializations, where o becomes a descendant of o
+                # ancestors of all in new
+                o2_ancestors_of_unique = list(
+                    self.adapter.ancestors(
+                        list(objects2.difference(objects1)), predicates=predicates, reflexive=True
+                    )
                 )
                 # o_descendants = list(
                 #    self.adapter.descendants([o], predicates=predicates, reflexive=True)
                 # )
                 # ixn = objects2.intersection(o_descendants)
-                if o in o2_ancestors:
+                if o in o2_ancestors_of_unique:
+                    all_o1_ancestors = list(self.adapter.ancestors(list(objects1), predicates))
                     new_object = None
                     for o2 in objects2:
                         if o in list(
                             self.adapter.ancestors([o2], predicates=predicates, reflexive=True)
                         ):
                             new_object = o2
                             break
@@ -147,32 +180,35 @@
                     yield AssociationChange(
                         subject=entity,
                         old_object=o,
                         new_object=new_object,
                         is_specialization=True,
                         old_object_obsolete=old_object_obsolete,
                         closure_predicates=predicates,
+                        closure_delta=_count_closure(new_object, all_o1_ancestors),
                     )
                     continue
                 # neither specialization nor generalization
                 yield AssociationChange(
                     subject=entity,
                     old_object=o,
                     is_deletion=True,
                     old_object_obsolete=old_object_obsolete,
                     closure_predicates=predicates,
+                    closure_delta=-_count_closure(o, objects2),
                 )
             for o in objects2.difference(objects1):
                 if o in accounted_for_in_objects2:
                     continue
                 yield AssociationChange(
                     subject=entity,
                     new_object=o,
                     is_creation=True,
                     closure_predicates=predicates,
+                    closure_delta=_count_closure(o, objects1),
                 )
 
     def compare(
         self,
         assocs1: List[Association],
         assocs2: List[Association],
         predicates: List[PRED_CURIE],
@@ -238,19 +274,30 @@
         pubs_in_common = set(pubmap1.keys()).intersection(set(pubmap2.keys()))
         for pub in pubs_in_common:
             for change in self.calculate_change_objects(pubmap1[pub], pubmap2[pub], predicates):
                 change.publications = [pub]
                 change.summary_group = pub
                 yield change
         for pub in set(pubmap1.keys()).difference(set(pubmap2.keys())):
-            yield AssociationChange(
-                publications=[pub],
-                publication_is_deleted=True,
-            )
+            for assoc in pubmap1[pub]:
+                yield AssociationChange(
+                    publications=[pub],
+                    publication_is_deleted=True,
+                    subject=assoc.subject,
+                    old_object=assoc.object,
+                    old_object_obsolete=assoc.object in self.obsoletion_map,
+                )
         for pub in set(pubmap2.keys()).difference(set(pubmap1.keys())):
+            for assoc in pubmap1[pub]:
+                yield AssociationChange(
+                    publications=[pub],
+                    publication_is_added=True,
+                    subject=assoc.subject,
+                    new_object=assoc.object,
+                )
             yield AssociationChange(
                 publications=[pub],
                 publication_is_added=True,
             )
 
     def changes_by_primary_knowledge_source(
         self,
```

### Comparing `oaklib-0.5.3/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.4/src/oaklib/utilities/associations/association_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """An in-memory sqlite index for simple associations."""
 import logging
 import sqlite3
-from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Iterator
+from collections import defaultdict
+from dataclasses import dataclass, field
+from typing import Any, Dict, Iterable, Iterator, List, Tuple
 
 from semsql.sqla.semsql import TermAssociation
 from sqlalchemy import Column, String, create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session, sessionmaker
 
 from oaklib.datamodels.association import Association
@@ -30,38 +31,49 @@
     subject_property_values_json = Column(String)
     object_property_values_json = Column(String)
     association_property_values_json = Column(String)
 
 
 @dataclass
 class AssociationIndex:
+    """
+    A sqlite in-memory index for a collection of associations.
+    """
+
     _connection: sqlite3.Connection = None
     _session: Session = None
     _engine: Engine = None
+    _associations_by_spo: Dict[Tuple[CURIE, PRED_CURIE, CURIE], List[Association]] = field(
+        default_factory=lambda: defaultdict(list)
+    )
 
     def create(self):
         connection_string: str = "sqlite:///:memory:"
         engine = create_engine(connection_string)
         con = engine.raw_connection()
         # con = sqlite3.connect(":memory:")
         con.execute(f"create table term_association({','.join(COLS)})")
         self._connection = con
         session_cls = sessionmaker(engine)
         self._session = session_cls()
         self._engine = engine
 
     def populate(self, associations: Iterable[Association]):
+        associations = list(associations)
         tups = [
             (a.subject, a.predicate, a.object, a.primary_knowledge_source) for a in associations
         ]
         logging.info(f"Bulk loading {len(tups)} associations")
         self._connection.executemany(
             "insert into term_association(subject, predicate, object, source) values (?,?,?,?)",
             tups,
         )
+        for a in associations:
+            tup = (a.subject, a.predicate, a.object)
+            self._associations_by_spo[tup].append(a)
 
     def lookup(
         self,
         subjects: Iterable[CURIE] = None,
         predicates: Iterable[PRED_CURIE] = None,
         objects: Iterable[CURIE] = None,
         property_filter: Dict[PRED_CURIE, Any] = None,
@@ -74,13 +86,9 @@
             q = q.filter(TermAssociation.subject.in_(tuple(subjects)))
         if predicates:
             q = q.filter(TermAssociation.predicate.in_(tuple(predicates)))
         if objects:
             q = q.filter(TermAssociation.object.in_(tuple(objects)))
         logging.info(f"Association query: {q}")
         for row in q:
-            yield Association(
-                subject=row.subject,
-                predicate=row.predicate,
-                object=row.object,
-                primary_knowledge_source=row.source,
-            )
+            tup = (row.subject, row.predicate, row.object)
+            yield from self._associations_by_spo[tup]
```

### Comparing `oaklib-0.5.3/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.4/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.4/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.4/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.4/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.4/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.4/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.4/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.4/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.4/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.4/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.4/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.4/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.4/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE, PRED_CURIE
 
 
 def filter_redundant(
     oi: OboGraphInterface, curies: Collection[CURIE], predicates: List[PRED_CURIE] = None
 ) -> List[CURIE]:
+    """
+    Filters a set of nodes to the non-redundant subset.
+
+    :param oi:
+    :param curies:
+    :param predicates:
+    :return:
+    """
     return [curie for curie in curies if not is_redundant(oi, curie, curies, predicates)]
 
 
 def is_redundant(
     oi: OboGraphInterface,
     curie: CURIE,
     curies: Collection[CURIE],
```

### Comparing `oaklib-0.5.3/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.4/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.4/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.4/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.4/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.4/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.4/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.4/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.4/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.3/PKG-INFO` & `oaklib-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.3
+Version: 0.5.4
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Provides-Extra: gilda
 Provides-Extra: seaborn
 Requires-Dist: SPARQLWrapper
-Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0)
-Requires-Dist: airium (>=0.2.5,<0.3.0)
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: bioregistry (>=0.6.35,<0.7.0)
+Requires-Dist: SQLAlchemy (>=1.4.32)
+Requires-Dist: airium (>=0.2.5)
+Requires-Dist: appdirs (>=1.4.4)
+Requires-Dist: bioregistry (>=0.6.35)
 Requires-Dist: class-resolver (>=0.4.2)
-Requires-Dist: curies (>=0.4.0,<0.5.0)
-Requires-Dist: eutils (>=0.6.0,<0.7.0)
-Requires-Dist: funowl (>=0.1.12,<0.2.0)
+Requires-Dist: click
+Requires-Dist: curies (>=0.4.0)
+Requires-Dist: eutils (>=0.6.0)
+Requires-Dist: funowl (>=0.1.12)
 Requires-Dist: gilda (>=0.10.1,<0.11.0) ; extra == "gilda"
 Requires-Dist: kgcl-rdflib (>=0.3.0,<0.4.0)
-Requires-Dist: kgcl-schema (>=0.3.5,<0.4.0)
-Requires-Dist: lark (>=1.1.2,<2.0.0)
-Requires-Dist: linkml-renderer (>=0.1.2,<0.2.0)
-Requires-Dist: linkml-runtime (>=1.2.15,<2.0.0)
+Requires-Dist: kgcl-schema (>=0.3.5)
+Requires-Dist: lark (>=1.1.2)
+Requires-Dist: linkml-renderer (>=0.1.2)
+Requires-Dist: linkml-runtime (>=1.2.15)
 Requires-Dist: ndex2 (>=3.5.0,<4.0.0)
-Requires-Dist: networkx (>=2.7.1,<3.0.0)
-Requires-Dist: nxontology (>=0.4.0,<0.5.0)
-Requires-Dist: ols-client (>=0.1.1,<0.2.0)
-Requires-Dist: ontoportal-client (==0.0.3)
-Requires-Dist: pandas (>=1.5.1,<2.0.0)
-Requires-Dist: prefixmaps (>=0.1.2,<0.2.0)
-Requires-Dist: pronto (>=2.5.0,<3.0.0)
+Requires-Dist: networkx (>=2.7.1)
+Requires-Dist: ols-client (>=0.1.1)
+Requires-Dist: ontoportal-client (>=0.0.3)
+Requires-Dist: prefixmaps (>=0.1.2)
+Requires-Dist: pronto (>=2.5.0)
 Requires-Dist: pysolr (>=3.9.0,<4.0.0)
-Requires-Dist: pystow (>=0.5.0,<0.6.0)
-Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
+Requires-Dist: pystow (>=0.5.0)
+Requires-Dist: ratelimit (>=2.2.1)
+Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
 Requires-Dist: rustsim (>=0.1.6)
-Requires-Dist: semsql (>=0.3.1,<0.4.0)
-Requires-Dist: sssom (>=0.3.26,<0.4.0)
-Requires-Dist: sssom-schema (>=0.11.0,<0.12.0)
-Requires-Dist: upsetplot (>=0.8.0,<0.9.0)
+Requires-Dist: semsql (>=0.3.1)
+Requires-Dist: sssom (>=0.3.26)
+Requires-Dist: sssom-schema (>=0.11.0)
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
 
 Python lib for common ontology operations over a variety of backends.
 
 <img src="docs/logos/oak-logo_black-icon.png" width="20%">
```

