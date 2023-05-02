# Comparing `tmp/linkml_runtime-1.5.1.tar.gz` & `tmp/linkml_runtime-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_runtime-1.5.1.tar", max compression
+gzip compressed data, was "linkml_runtime-1.5.2.tar", max compression
```

## Comparing `linkml_runtime-1.5.1.tar` & `linkml_runtime-1.5.2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     7048 2023-04-14 20:04:34.213671 linkml_runtime-1.5.1/LICENSE
--rw-r--r--   0        0        0     1990 2023-04-14 20:04:34.213671 linkml_runtime-1.5.1/README.md
--rw-r--r--   0        0        0     1179 2023-04-14 20:04:34.213671 linkml_runtime-1.5.1/linkml_runtime/__init__.py
--rw-r--r--   0        0        0      426 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/csv_dumper.py
--rw-r--r--   0        0        0      863 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/dumper_root.py
--rw-r--r--   0        0        0     3950 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/json_dumper.py
--rw-r--r--   0        0        0     3771 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/rdf_dumper.py
--rw-r--r--   0        0        0     7077 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/rdflib_dumper.py
--rw-r--r--   0        0        0      751 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/dumpers/yaml_dumper.py
--rw-r--r--   0        0        0        0 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/index/__init__.py
--rw-r--r--   0        0        0     8875 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/index/object_index.py
--rw-r--r--   0        0        0      119 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/README.md
--rw-r--r--   0        0        0      738 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/__init__.py
--rw-r--r--   0        0        0     3240 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/annotations.py
--rw-r--r--   0        0        0     3333 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/extensions.py
--rw-r--r--   0        0        0      114 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/graphql/README.md
--rw-r--r--   0        0        0    30306 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/graphql/meta.graphql
--rw-r--r--   0        0        0      111 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/README.md
--rw-r--r--   0        0        0    11169 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/annotations.json
--rw-r--r--   0        0        0     9306 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/extensions.json
--rw-r--r--   0        0        0    12109 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/mappings.json
--rw-r--r--   0        0        0   222072 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/meta.json
--rw-r--r--   0        0        0     6442 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/types.json
--rw-r--r--   0        0        0    22401 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/units.json
--rw-r--r--   0        0        0    14834 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/validation.json
--rw-r--r--   0        0        0      113 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/README.md
--rw-r--r--   0        0        0      648 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
--rw-r--r--   0        0        0      648 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
--rw-r--r--   0        0        0     7019 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/context.jsonld
--rw-r--r--   0        0        0      587 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
--rw-r--r--   0        0        0      587 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
--rw-r--r--   0        0        0     1615 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
--rw-r--r--   0        0        0     1615 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
--rw-r--r--   0        0        0    13814 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
--rw-r--r--   0        0        0    14266 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
--rw-r--r--   0        0        0      610 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.context.jsonld
--rw-r--r--   0        0        0      610 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
--rw-r--r--   0        0        0     2065 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.context.jsonld
--rw-r--r--   0        0        0     2065 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
--rw-r--r--   0        0        0     1910 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
--rw-r--r--   0        0        0     1910 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
--rw-r--r--   0        0        0      117 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/README.md
--rw-r--r--   0        0        0     4196 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
--rw-r--r--   0        0        0     1984 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
--rw-r--r--   0        0        0      297 2023-04-14 20:04:34.217671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
--rw-r--r--   0        0        0   353208 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/meta.schema.json
--rw-r--r--   0        0        0      291 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/types.schema.json
--rw-r--r--   0        0        0     5621 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/units.schema.json
--rw-r--r--   0        0        0     2291 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/validation.schema.json
--rw-r--r--   0        0        0     7126 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/linkml_files.py
--rw-r--r--   0        0        0     1821 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/mappings.py
--rw-r--r--   0        0        0   249036 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/meta.py
--rw-r--r--   0        0        0      112 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/README.md
--rw-r--r--   0        0        0      118 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/docs/credits.md
--rw-r--r--   0        0        0      141 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/docs/home.md
--rw-r--r--   0        0        0        5 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/import_map.json
--rw-r--r--   0        0        0      119 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/README.md
--rw-r--r--   0        0        0      833 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/annotations.yaml
--rw-r--r--   0        0        0     1057 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/extensions.yaml
--rw-r--r--   0        0        0     2755 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/mappings.yaml
--rw-r--r--   0        0        0    89120 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/meta.yaml
--rw-r--r--   0        0        0     3880 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/types.yaml
--rw-r--r--   0        0        0     2776 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/units.yaml
--rw-r--r--   0        0        0     2953 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/validation.yaml
--rw-r--r--   0        0        0      110 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/owl/README.md
--rw-r--r--   0        0        0   192274 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/owl/meta.owl.ttl
--rw-r--r--   0        0        0      110 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/README.md
--rw-r--r--   0        0        0    13054 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.model.ttl
--rw-r--r--   0        0        0    13054 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.ttl
--rw-r--r--   0        0        0    10932 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.model.ttl
--rw-r--r--   0        0        0    10932 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.ttl
--rw-r--r--   0        0        0    13825 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.model.ttl
--rw-r--r--   0        0        0    13825 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.ttl
--rw-r--r--   0        0        0   207795 2023-04-14 20:04:34.221671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.model.ttl
--rw-r--r--   0        0        0   207795 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.ttl
--rw-r--r--   0        0        0     7565 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.model.ttl
--rw-r--r--   0        0        0     7565 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.ttl
--rw-r--r--   0        0        0    25276 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.model.ttl
--rw-r--r--   0        0        0    25276 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.ttl
--rw-r--r--   0        0        0    16810 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.model.ttl
--rw-r--r--   0        0        0    16810 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.ttl
--rw-r--r--   0        0        0      113 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/README.md
--rw-r--r--   0        0        0     1261 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shex
--rw-r--r--   0        0        0     8918 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shexj
--rw-r--r--   0        0        0      821 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shex
--rw-r--r--   0        0        0     5303 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shexj
--rw-r--r--   0        0        0      424 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/mappings.shex
--rw-r--r--   0        0        0     2568 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/mappings.shexj
--rw-r--r--   0        0        0    37441 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shex
--rw-r--r--   0        0        0   254576 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shexj
--rw-r--r--   0        0        0      459 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/types.shex
--rw-r--r--   0        0        0     2568 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/types.shexj
--rw-r--r--   0        0        0     1682 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shex
--rw-r--r--   0        0        0    11643 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shexj
--rw-r--r--   0        0        0     1519 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shex
--rw-r--r--   0        0        0     7343 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shexj
--rw-r--r--   0        0        0     4599 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/types.py
--rw-r--r--   0        0        0     3332 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/units.py
--rw-r--r--   0        0        0     6897 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/linkml_model/validation.py
--rw-r--r--   0        0        0      426 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/context_flattener.py
--rw-r--r--   0        0        0     1933 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/csv_loader.py
--rw-r--r--   0        0        0     1318 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/json_loader.py
--rw-r--r--   0        0        0     5199 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/loader_root.py
--rw-r--r--   0        0        0     4735 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/rdf_loader.py
--rw-r--r--   0        0        0    14065 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/rdflib_loader.py
--rw-r--r--   0        0        0     1358 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/requests_ssl_patch.py
--rw-r--r--   0        0        0     1821 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/loaders/yaml_loader.py
--rw-r--r--   0        0        0    42218 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/processing/referencevalidator.py
--rw-r--r--   0        0        0    26951 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.py
--rw-r--r--   0        0        0    10253 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.yaml
--rw-r--r--   0        0        0        0 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/__init__.py
--rw-r--r--   0        0        0      850 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/comparefiles.py
--rw-r--r--   0        0        0     1972 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/compile_python.py
--rw-r--r--   0        0        0     4034 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/context_utils.py
--rw-r--r--   0        0        0     2389 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/csvutils.py
--rw-r--r--   0        0        0      486 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/curienamespace.py
--rw-r--r--   0        0        0     1325 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/dataclass_extensions_376.py
--rw-r--r--   0        0        0      433 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/dictutils.py
--rw-r--r--   0        0        0     2554 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/distroutils.py
--rw-r--r--   0        0        0     3683 2023-04-14 20:04:34.225671 linkml_runtime-1.5.1/linkml_runtime/utils/enumerations.py
--rw-r--r--   0        0        0     6755 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/eval_utils.py
--rw-r--r--   0        0        0     6594 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/formatutils.py
--rw-r--r--   0        0        0     5672 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/inference_utils.py
--rw-r--r--   0        0        0     1976 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/introspection.py
--rw-r--r--   0        0        0    11553 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/metamodelcore.py
--rw-r--r--   0        0        0    10580 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/namespaces.py
--rw-r--r--   0        0        0     2870 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/pattern.py
--rw-r--r--   0        0        0     6697 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/permissiblevalueimpl.py
--rw-r--r--   0        0        0     4720 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/ruleutils.py
--rw-r--r--   0        0        0     2287 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schema_as_dict.py
--rw-r--r--   0        0        0     9312 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schema_builder.py
--rw-r--r--   0        0        0     2815 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schemaops.py
--rw-r--r--   0        0        0    66900 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schemaview.py
--rw-r--r--   0        0        0     4327 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/schemaview_cli.py
--rw-r--r--   0        0        0      368 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/slot.py
--rw-r--r--   0        0        0      641 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/strictness.py
--rw-r--r--   0        0        0     1405 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/walker_utils.py
--rw-r--r--   0        0        0    19743 2023-04-14 20:04:34.229671 linkml_runtime-1.5.1/linkml_runtime/utils/yamlutils.py
--rw-r--r--   0        0        0     1826 2023-04-14 20:04:54.545859 linkml_runtime-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 linkml_runtime-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1996 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/README.md
+-rw-r--r--   0        0        0     1179 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/__init__.py
+-rw-r--r--   0        0        0     1225 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/csv_dumper.py
+-rw-r--r--   0        0        0      863 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/dumper_root.py
+-rw-r--r--   0        0        0     3950 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/json_dumper.py
+-rw-r--r--   0        0        0     3771 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/rdf_dumper.py
+-rw-r--r--   0        0        0     7077 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/rdflib_dumper.py
+-rw-r--r--   0        0        0      751 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/dumpers/yaml_dumper.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/index/__init__.py
+-rw-r--r--   0        0        0     8875 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/index/object_index.py
+-rw-r--r--   0        0        0      119 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/README.md
+-rw-r--r--   0        0        0      738 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/__init__.py
+-rw-r--r--   0        0        0     3240 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/annotations.py
+-rw-r--r--   0        0        0     3333 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/extensions.py
+-rw-r--r--   0        0        0      114 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/graphql/README.md
+-rw-r--r--   0        0        0    30306 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/graphql/meta.graphql
+-rw-r--r--   0        0        0      111 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/README.md
+-rw-r--r--   0        0        0    11169 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/annotations.json
+-rw-r--r--   0        0        0     9306 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/extensions.json
+-rw-r--r--   0        0        0    12109 2023-05-02 19:04:18.262419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/mappings.json
+-rw-r--r--   0        0        0   222072 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/meta.json
+-rw-r--r--   0        0        0     6442 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/types.json
+-rw-r--r--   0        0        0    22401 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/units.json
+-rw-r--r--   0        0        0    14834 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/validation.json
+-rw-r--r--   0        0        0      113 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/README.md
+-rw-r--r--   0        0        0      648 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
+-rw-r--r--   0        0        0      648 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
+-rw-r--r--   0        0        0     7019 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/context.jsonld
+-rw-r--r--   0        0        0      587 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
+-rw-r--r--   0        0        0      587 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
+-rw-r--r--   0        0        0    13814 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
+-rw-r--r--   0        0        0    14266 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
+-rw-r--r--   0        0        0      610 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/types.context.jsonld
+-rw-r--r--   0        0        0      610 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/units.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
+-rw-r--r--   0        0        0      117 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/README.md
+-rw-r--r--   0        0        0     4196 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
+-rw-r--r--   0        0        0     1984 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
+-rw-r--r--   0        0        0      297 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
+-rw-r--r--   0        0        0   353208 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/meta.schema.json
+-rw-r--r--   0        0        0      291 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/types.schema.json
+-rw-r--r--   0        0        0     5621 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/units.schema.json
+-rw-r--r--   0        0        0     2291 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/validation.schema.json
+-rw-r--r--   0        0        0     7126 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/linkml_files.py
+-rw-r--r--   0        0        0     1821 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/mappings.py
+-rw-r--r--   0        0        0   249036 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/meta.py
+-rw-r--r--   0        0        0      112 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/README.md
+-rw-r--r--   0        0        0      118 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/docs/credits.md
+-rw-r--r--   0        0        0      141 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/docs/home.md
+-rw-r--r--   0        0        0        5 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/import_map.json
+-rw-r--r--   0        0        0      119 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/README.md
+-rw-r--r--   0        0        0      833 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/annotations.yaml
+-rw-r--r--   0        0        0     1057 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/extensions.yaml
+-rw-r--r--   0        0        0     2755 2023-05-02 19:04:18.266419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/mappings.yaml
+-rw-r--r--   0        0        0    89120 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/meta.yaml
+-rw-r--r--   0        0        0     3880 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/types.yaml
+-rw-r--r--   0        0        0     2776 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/units.yaml
+-rw-r--r--   0        0        0     2953 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/validation.yaml
+-rw-r--r--   0        0        0      110 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/owl/README.md
+-rw-r--r--   0        0        0   192274 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/owl/meta.owl.ttl
+-rw-r--r--   0        0        0      110 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/README.md
+-rw-r--r--   0        0        0    13054 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/annotations.model.ttl
+-rw-r--r--   0        0        0    13054 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/annotations.ttl
+-rw-r--r--   0        0        0    10932 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/extensions.model.ttl
+-rw-r--r--   0        0        0    10932 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/extensions.ttl
+-rw-r--r--   0        0        0    13825 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/mappings.model.ttl
+-rw-r--r--   0        0        0    13825 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/mappings.ttl
+-rw-r--r--   0        0        0   207795 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/meta.model.ttl
+-rw-r--r--   0        0        0   207795 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/meta.ttl
+-rw-r--r--   0        0        0     7565 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/types.model.ttl
+-rw-r--r--   0        0        0     7565 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/types.ttl
+-rw-r--r--   0        0        0    25276 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/units.model.ttl
+-rw-r--r--   0        0        0    25276 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/units.ttl
+-rw-r--r--   0        0        0    16810 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/validation.model.ttl
+-rw-r--r--   0        0        0    16810 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/validation.ttl
+-rw-r--r--   0        0        0      113 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/README.md
+-rw-r--r--   0        0        0     1261 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/annotations.shex
+-rw-r--r--   0        0        0     8918 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/annotations.shexj
+-rw-r--r--   0        0        0      821 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/extensions.shex
+-rw-r--r--   0        0        0     5303 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/extensions.shexj
+-rw-r--r--   0        0        0      424 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/mappings.shex
+-rw-r--r--   0        0        0     2568 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/mappings.shexj
+-rw-r--r--   0        0        0    37441 2023-05-02 19:04:18.270419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/meta.shex
+-rw-r--r--   0        0        0   254576 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/meta.shexj
+-rw-r--r--   0        0        0      459 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/types.shex
+-rw-r--r--   0        0        0     2568 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/types.shexj
+-rw-r--r--   0        0        0     1682 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/units.shex
+-rw-r--r--   0        0        0    11643 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/units.shexj
+-rw-r--r--   0        0        0     1519 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/validation.shex
+-rw-r--r--   0        0        0     7343 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/validation.shexj
+-rw-r--r--   0        0        0     4599 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/types.py
+-rw-r--r--   0        0        0     3332 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/units.py
+-rw-r--r--   0        0        0     6897 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/linkml_model/validation.py
+-rw-r--r--   0        0        0      426 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/__init__.py
+-rw-r--r--   0        0        0     1533 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/context_flattener.py
+-rw-r--r--   0        0        0     1933 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/csv_loader.py
+-rw-r--r--   0        0        0     1318 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/json_loader.py
+-rw-r--r--   0        0        0     5199 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/loader_root.py
+-rw-r--r--   0        0        0     4735 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/rdf_loader.py
+-rw-r--r--   0        0        0    14065 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/rdflib_loader.py
+-rw-r--r--   0        0        0     1358 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/requests_ssl_patch.py
+-rw-r--r--   0        0        0     1821 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/loaders/yaml_loader.py
+-rw-r--r--   0        0        0    42276 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/processing/referencevalidator.py
+-rw-r--r--   0        0        0    26951 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/processing/validation_datamodel.py
+-rw-r--r--   0        0        0    10253 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/processing/validation_datamodel.yaml
+-rw-r--r--   0        0        0        0 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/__init__.py
+-rw-r--r--   0        0        0      850 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/comparefiles.py
+-rw-r--r--   0        0        0     1972 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/compile_python.py
+-rw-r--r--   0        0        0     4034 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/context_utils.py
+-rw-r--r--   0        0        0     2389 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/csvutils.py
+-rw-r--r--   0        0        0      486 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/curienamespace.py
+-rw-r--r--   0        0        0     1325 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/dataclass_extensions_376.py
+-rw-r--r--   0        0        0      433 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/dictutils.py
+-rw-r--r--   0        0        0     2554 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/distroutils.py
+-rw-r--r--   0        0        0     3683 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/enumerations.py
+-rw-r--r--   0        0        0     6755 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/eval_utils.py
+-rw-r--r--   0        0        0     6594 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/formatutils.py
+-rw-r--r--   0        0        0     5672 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/inference_utils.py
+-rw-r--r--   0        0        0     1976 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/introspection.py
+-rw-r--r--   0        0        0    11553 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/metamodelcore.py
+-rw-r--r--   0        0        0    10580 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/namespaces.py
+-rw-r--r--   0        0        0     2870 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/pattern.py
+-rw-r--r--   0        0        0     6697 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/permissiblevalueimpl.py
+-rw-r--r--   0        0        0     4720 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/ruleutils.py
+-rw-r--r--   0        0        0     2287 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/schema_as_dict.py
+-rw-r--r--   0        0        0     9312 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/schema_builder.py
+-rw-r--r--   0        0        0     2815 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/schemaops.py
+-rw-r--r--   0        0        0    66900 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/schemaview.py
+-rw-r--r--   0        0        0     4327 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/schemaview_cli.py
+-rw-r--r--   0        0        0      368 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/slot.py
+-rw-r--r--   0        0        0      641 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/strictness.py
+-rw-r--r--   0        0        0     1405 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/walker_utils.py
+-rw-r--r--   0        0        0    19743 2023-05-02 19:04:18.274419 linkml_runtime-1.5.2/linkml_runtime/utils/yamlutils.py
+-rw-r--r--   0        0        0     1826 2023-05-02 19:04:38.202384 linkml_runtime-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 linkml_runtime-1.5.2/PKG-INFO
```

### Comparing `linkml_runtime-1.5.1/LICENSE` & `linkml_runtime-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/README.md` & `linkml_runtime-1.5.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![](https://github.com/linkml/linkml-runtime/workflows/Build/badge.svg)
 [![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml-runtime/main?filepath=notebooks)
 [![PyPi](https://img.shields.io/pypi/v/linkml-runtime.svg)](https://pypi.python.org/pypi/linkml)
 [![PyPIDownloadsTotal](https://pepy.tech/badge/linkml-runtime)](https://pepy.tech/project/linkml-runtime)
 [![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml-runtime?logo=PyPI&color=blue)](https://pypi.org/project/linkml-runtime)
 [![codecov](https://codecov.io/gh/linkml/linkml-runtime/branch/main/graph/badge.svg?token=FOBHNSK5WG)](https://codecov.io/gh/linkml/linkml-runtime)
 
-Runtime support for linkml generated models
+Runtime support for linkml generated data classes
 
 ## About
 
 This python library provides runtime support for [LinkML](https://linkml.io/linkml/) datamodels.
 
 See the [LinkML repo](https://github.com/linkml/linkml) for the [Python Dataclass Generator](https://linkml.io/linkml/generators/python.html) which will convert a schema into a Python object model. That model will have dependencies on functionality in this library.
```

### Comparing `linkml_runtime-1.5.1/linkml_runtime/__init__.py` & `linkml_runtime-1.5.2/linkml_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/dumpers/csv_dumper.py` & `linkml_runtime-1.5.2/linkml_runtime/dumpers/csv_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/dumpers/dumper_root.py` & `linkml_runtime-1.5.2/linkml_runtime/dumpers/dumper_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/dumpers/json_dumper.py` & `linkml_runtime-1.5.2/linkml_runtime/dumpers/json_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/dumpers/rdf_dumper.py` & `linkml_runtime-1.5.2/linkml_runtime/dumpers/rdf_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/dumpers/rdflib_dumper.py` & `linkml_runtime-1.5.2/linkml_runtime/dumpers/rdflib_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/dumpers/yaml_dumper.py` & `linkml_runtime-1.5.2/linkml_runtime/dumpers/yaml_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/index/object_index.py` & `linkml_runtime-1.5.2/linkml_runtime/index/object_index.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/__init__.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/annotations.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/annotations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/extensions.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/extensions.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/graphql/meta.graphql` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/graphql/meta.graphql`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/annotations.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/annotations.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/extensions.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/extensions.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/mappings.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/mappings.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/meta.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/meta.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/types.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/types.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/units.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/units.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/json/validation.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/json/validation.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/meta.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/types.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/units.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/validation.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/annotations.schema.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/extensions.schema.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/extensions.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/meta.schema.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/meta.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/units.schema.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/units.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/jsonschema/validation.schema.json` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/jsonschema/validation.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/linkml_files.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/linkml_files.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/mappings.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/mappings.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/meta.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/meta.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/annotations.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/annotations.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/extensions.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/extensions.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/mappings.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/mappings.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/meta.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/meta.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/types.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/types.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/units.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/units.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/model/schema/validation.yaml` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/model/schema/validation.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/owl/meta.owl.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/owl/meta.owl.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/annotations.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/annotations.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/annotations.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/extensions.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/extensions.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/extensions.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/mappings.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/mappings.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/mappings.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/meta.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/meta.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/meta.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/types.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/types.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/types.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/units.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/units.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/units.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.model.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/validation.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/rdf/validation.ttl` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/rdf/validation.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shex` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/annotations.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/annotations.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/annotations.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shex` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/extensions.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/extensions.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/extensions.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/mappings.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/mappings.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shex` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/meta.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/meta.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/meta.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/types.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/types.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shex` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/units.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/units.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/units.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shex` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/validation.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/shex/validation.shexj` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/shex/validation.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/types.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/types.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/units.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/units.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/linkml_model/validation.py` & `linkml_runtime-1.5.2/linkml_runtime/linkml_model/validation.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/context_flattener.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/context_flattener.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/csv_loader.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/json_loader.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/loader_root.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/loader_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/rdf_loader.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/rdf_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/rdflib_loader.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/rdflib_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/requests_ssl_patch.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/requests_ssl_patch.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/loaders/yaml_loader.py` & `linkml_runtime-1.5.2/linkml_runtime/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/processing/referencevalidator.py` & `linkml_runtime-1.5.2/linkml_runtime/processing/referencevalidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,16 @@
         obj = copy(obj)
         del obj[pk_slot_name]
     return obj
 
 
 def _add_pk(obj: dict, pk_slot_name: str, pk_val: Any) -> dict:
     """Make a new ExpandedDict ready copy of a dict, adding the pk_slot_name"""
+    if obj is None:
+        return {pk_slot_name: pk_val}
     if pk_slot_name not in obj:
         obj = copy(obj)
         obj[pk_slot_name] = pk_val
     return obj
 
 
 def _simple_to_dict(obj: Union[dict, Any], simple_value_slot_name: str) -> dict:
```

### Comparing `linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.py` & `linkml_runtime-1.5.2/linkml_runtime/processing/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/processing/validation_datamodel.yaml` & `linkml_runtime-1.5.2/linkml_runtime/processing/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/comparefiles.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/comparefiles.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/compile_python.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/compile_python.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/context_utils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/context_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/csvutils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/csvutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/dataclass_extensions_376.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/dataclass_extensions_376.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/distroutils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/distroutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/enumerations.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/enumerations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/eval_utils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/formatutils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/formatutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/inference_utils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/introspection.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/metamodelcore.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/metamodelcore.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/namespaces.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/pattern.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/permissiblevalueimpl.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/permissiblevalueimpl.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/ruleutils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/ruleutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/schema_as_dict.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/schema_as_dict.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/schema_builder.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/schemaops.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/schemaops.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/schemaview.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/schemaview.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/schemaview_cli.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/schemaview_cli.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/strictness.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/strictness.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/walker_utils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/walker_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/linkml_runtime/utils/yamlutils.py` & `linkml_runtime-1.5.2/linkml_runtime/utils/yamlutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.1/pyproject.toml` & `linkml_runtime-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml-runtime"
-version = "v1.5.1"
+version = "v1.5.2"
 description = "Runtime environment for LinkML, the Linked open data modeling language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sierra Moxon <smoxon@lbl.gov>",
     "Bill Duncan <wdduncan@gmail.com>",
     "Harshad Hegde <hhegde@lbl.gov>"
```

### Comparing `linkml_runtime-1.5.1/PKG-INFO` & `linkml_runtime-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-runtime
-Version: 1.5.1
+Version: 1.5.2
 Summary: Runtime environment for LinkML, the Linked open data modeling language
 Home-page: https://github.com/linkml/linkml-runtime
 Keywords: linkml,metamodel,schema visualization,rdf,owl,yaml
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,15 +43,15 @@
 ![](https://github.com/linkml/linkml-runtime/workflows/Build/badge.svg)
 [![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml-runtime/main?filepath=notebooks)
 [![PyPi](https://img.shields.io/pypi/v/linkml-runtime.svg)](https://pypi.python.org/pypi/linkml)
 [![PyPIDownloadsTotal](https://pepy.tech/badge/linkml-runtime)](https://pepy.tech/project/linkml-runtime)
 [![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml-runtime?logo=PyPI&color=blue)](https://pypi.org/project/linkml-runtime)
 [![codecov](https://codecov.io/gh/linkml/linkml-runtime/branch/main/graph/badge.svg?token=FOBHNSK5WG)](https://codecov.io/gh/linkml/linkml-runtime)
 
-Runtime support for linkml generated models
+Runtime support for linkml generated data classes
 
 ## About
 
 This python library provides runtime support for [LinkML](https://linkml.io/linkml/) datamodels.
 
 See the [LinkML repo](https://github.com/linkml/linkml) for the [Python Dataclass Generator](https://linkml.io/linkml/generators/python.html) which will convert a schema into a Python object model. That model will have dependencies on functionality in this library.
```

