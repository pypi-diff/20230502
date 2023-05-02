# Comparing `tmp/ptal_api-0.11.4.2.tar.gz` & `tmp/ptal_api-0.11.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.4.2.tar", max compression
+gzip compressed data, was "ptal_api-0.11.5.tar", max compression
```

## Comparing `ptal_api-0.11.4.2.tar` & `ptal_api-0.11.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/README.md
--rw-r--r--   0        0        0        0 2023-04-24 15:02:15.010257 ptal_api-0.11.4.2/ptal_api/__init__.py
--rw-r--r--   0        0        0    98013 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/adapter.py
--rw-r--r--   0        0        0      127 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      752 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    12105 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      905 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3240 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2107 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1399 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4565 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    22266 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1828 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3364 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-04-24 15:02:15.014257 ptal_api-0.11.4.2/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4803 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1211 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-04-24 15:02:15.014257 ptal_api-0.11.4.2/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   288848 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    92810 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   136157 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3641 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-04-24 15:02:15.014257 ptal_api-0.11.4.2/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1047 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 ptal_api-0.11.4.2/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-04-24 11:37:57.778944 ptal_api-0.11.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 11:50:59.012123 ptal_api-0.11.5/ptal_api/__init__.py
+-rw-r--r--   0        0        0    99057 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/adapter.py
+-rw-r--r--   0        0        0      127 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    12302 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-04-24 11:37:57.778944 ptal_api-0.11.5/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-04-24 11:37:57.782944 ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-04-24 11:37:57.782944 ptal_api-0.11.5/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3279 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:50:59.016123 ptal_api-0.11.5/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4668 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1186 2023-05-02 11:50:58.952123 ptal_api-0.11.5/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 11:50:59.016123 ptal_api-0.11.5/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   288920 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    92810 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   136157 2023-05-02 11:50:58.956123 ptal_api-0.11.5/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-05-02 11:50:58.960123 ptal_api-0.11.5/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:50:59.016123 ptal_api-0.11.5/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-02 11:50:58.960123 ptal_api-0.11.5/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1871 2023-05-02 11:50:58.960123 ptal_api-0.11.5/pyproject.toml
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 ptal_api-0.11.5/PKG-INFO
```

### Comparing `ptal_api-0.11.4.2/README.md` & `ptal_api-0.11.5/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.2/ptal_api/adapter.py` & `ptal_api-0.11.5/ptal_api/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,122 +1,213 @@
+import logging
 from copy import copy
 from functools import wraps
 from time import time
-from typing import Optional, List, Any, Iterable, Dict, Sequence, Union
-import logging
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
-from .core.values.value_mapping import get_map_helper
+from sgqlc.operation import Fragment, Operation
+
+from .core.kb_sync.kb_iterator_config import KBIteratorConfig
+from .core.kb_sync.object_time_interval import ObjectTimeInterval
 from .core.type_mapper.data_model.base_data_model import TypeMapping
 from .core.type_mapper.modules.type_mapping_loader.type_mapping_loader import TypeMappingLoader
 from .core.type_mapper.modules.type_mapping_loader.type_mapping_loader_interface import TypeMappingLoaderInterface
-from .core.kb_sync.kb_iterator_config import KBIteratorConfig
-from .core.kb_sync.object_time_interval import ObjectTimeInterval
-from .tdm_builder.tdm_builder import AbstractTdmBuilder
+from .core.values.value_mapping import get_map_helper
 from .providers.gql_providers import AbstractGQLClient
-from .schema.api_schema import ConceptCandidateFact, Query, Mutation, StoryPagination, ConceptLinkPagination, \
-    ConceptFactPagination, ConceptPropertyPagination, SortDirection, ConceptSorting, DocumentSorting, \
-    DocumentGrouping, TimestampInterval, PerformSynchronously, ConceptPropertyTypeSorting, ConceptTypeSorting, \
-    ConceptLinkTypeSorting, ConceptPropertyValueTypeSorting, CompositePropertyTypeSorting
-from .schema.api_schema import \
-    ValueInput, IntValueInput, StringValueInput, DateTimeValue, StringLocaleValue, StringValue, LinkValue, \
-    DoubleValue, IntValue, ConceptPropertyFilterSettings, ConceptLinkFilterSettings, ExtraSettings, Story, Document,\
-    DocumentFilterSettings, Concept, ConceptLink, ConceptPagination, ConceptFilterSettings, PropertyFilterSettings, \
-    StringFilter, ConceptType, ConceptTypeFilterSettings, ConceptTypePagination, ConceptPropertyType, \
-    ConceptPropertyTypePagination, ConceptPropertyTypeFilterSettings, ConceptLinkType, ConceptLinkTypePagination, \
-    ConceptLinkTypeFilterSettings, ConceptPropertyValueType, ConceptPropertyValueTypePagination, \
-    ConceptPropertyValueTypeFilterSettings, ConceptPropertyValueTypeUpdateInput, ConceptProperty, \
-    ConceptMutationInput, ConceptUpdateInput, ConceptPropertyUpdateInput, ConceptPropertyCreateInput, \
-    ConceptLinkPropertyInput, ConceptLinkCreationMutationInput, ComponentValueInput, CompositeConcept, \
-    CompositeConceptWidgetRowPagination, DocumentLinkFilterSetting, ConceptFact, \
-    ConceptLinkPropertyTypeCreationInput, ConceptPropertyTypeCreationInput, State, \
-    CompositePropertyValueTemplate, CompositePropertyValueType, CompositeValue, DateTimeValueInput, \
-    LinkValueInput, DoubleValueInput, StringLocaleValueInput, CompositePropertyTypeFilterSettings, \
-    ConceptLinkPropertyTypeUpdateInput, FactInput
-from .schema.crawlers_api_schema import Query as CrQuery
-from .schema.crawlers_api_schema import Crawler, CrawlerPagination
-from .schema import utils_api_schema as uas
 from .schema import tcontroller_api_schema as tc
-from sgqlc.operation import Operation, Fragment
-
+from .schema import utils_api_schema as uas
+from .schema.api_schema import (
+    ComponentValueInput,
+    CompositeConcept,
+    CompositeConceptWidgetRowPagination,
+    CompositePropertyTypeFilterSettings,
+    CompositePropertyTypeSorting,
+    CompositePropertyValueTemplate,
+    CompositePropertyValueType,
+    CompositeValue,
+    Concept,
+    ConceptCandidateFact,
+    ConceptFact,
+    ConceptFactPagination,
+    ConceptFilterSettings,
+    ConceptLink,
+    ConceptLinkCreationMutationInput,
+    ConceptLinkFilterSettings,
+    ConceptLinkPagination,
+    ConceptLinkPropertyInput,
+    ConceptLinkPropertyTypeCreationInput,
+    ConceptLinkPropertyTypeUpdateInput,
+    ConceptLinkType,
+    ConceptLinkTypeFilterSettings,
+    ConceptLinkTypePagination,
+    ConceptLinkTypeSorting,
+    ConceptMergeInput,
+    ConceptMutationInput,
+    ConceptPagination,
+    ConceptProperty,
+    ConceptPropertyCreateInput,
+    ConceptPropertyFilterSettings,
+    ConceptPropertyPagination,
+    ConceptPropertyType,
+    ConceptPropertyTypeCreationInput,
+    ConceptPropertyTypeFilterSettings,
+    ConceptPropertyTypePagination,
+    ConceptPropertyTypeSorting,
+    ConceptPropertyUpdateInput,
+    ConceptPropertyValueType,
+    ConceptPropertyValueTypeFilterSettings,
+    ConceptPropertyValueTypePagination,
+    ConceptPropertyValueTypeSorting,
+    ConceptPropertyValueTypeUpdateInput,
+    ConceptSorting,
+    ConceptType,
+    ConceptTypeFilterSettings,
+    ConceptTypePagination,
+    ConceptTypeSorting,
+    ConceptUnmergeInput,
+    ConceptUpdateInput,
+    DateTimeValue,
+    DateTimeValueInput,
+    Document,
+    DocumentFilterSettings,
+    DocumentGrouping,
+    DocumentLinkFilterSetting,
+    DocumentSorting,
+    DoubleValue,
+    DoubleValueInput,
+    ExtraSettings,
+    FactInput,
+    IntValue,
+    IntValueInput,
+    LinkValue,
+    LinkValueInput,
+    Mutation,
+    PerformSynchronously,
+    PropertyFilterSettings,
+    Query,
+    SortDirection,
+    State,
+    Story,
+    StoryPagination,
+    StringFilter,
+    StringLocaleValue,
+    StringLocaleValueInput,
+    StringValue,
+    StringValueInput,
+    TimestampInterval,
+    ValueInput,
+)
+from .schema.crawlers_api_schema import Crawler, CrawlerPagination
+from .schema.crawlers_api_schema import Query as CrQuery
+from .tdm_builder.tdm_builder import AbstractTdmBuilder
 
 logger = logging.getLogger(__name__)
 
 
 def check_utils_gql_client(f):
     @wraps(f)
-    def wrapper(self: 'TalismanAPIAdapter', *args, **kwargs):
+    def wrapper(self: "TalismanAPIAdapter", *args, **kwargs):
         if self._utils_gql_client is None:
-            raise Exception('Utils methods cannot be used because the corresponding gql_client is not specified.')
+            raise Exception("Utils methods cannot be used because the corresponding gql_client is not specified.")
         return f(self, *args, **kwargs)
 
     return wrapper
 
 
 class TalismanAPIAdapter:
     def __init__(
-        self, gql_client: Optional[AbstractGQLClient], type_mapping: Optional[Union[str, dict, TypeMapping]] = None,
-        type_mapping_loader: Optional[TypeMappingLoaderInterface] = None, tdm_builder: AbstractTdmBuilder = None,
-        utils_gql_client: Optional[AbstractGQLClient] = None, kb_iterator_config: KBIteratorConfig = None,
-        limit: int = 100, perform_synchronously: bool = True
+        self,
+        gql_client: Optional[AbstractGQLClient],
+        type_mapping: Optional[Union[str, dict, TypeMapping]] = None,
+        type_mapping_loader: Optional[TypeMappingLoaderInterface] = None,
+        tdm_builder: AbstractTdmBuilder = None,
+        utils_gql_client: Optional[AbstractGQLClient] = None,
+        kb_iterator_config: KBIteratorConfig = None,
+        limit: int = 100,
+        perform_synchronously: bool = True,
     ) -> None:
         self._gql_client = gql_client
         self._utils_gql_client = utils_gql_client
         self._type_mapping_loader = type_mapping_loader if type_mapping_loader else TypeMappingLoader(logger)
         self._type_mapping = self._type_mapping_loader.load_type_mapping(type_mapping)
         self._limit = limit
         self._perform_synchronously = perform_synchronously
 
-        self.document_fields_truncated = ('id', 'external_url')
+        self.document_fields_truncated = ("id", "external_url")
         self.document_fields = (
-            'id', 'title', 'external_url', 'publication_author', 'publication_date', 'internal_url', 'markers',
-            'system_registration_date', 'system_update_date', 'notes', 'access_level', 'trust_level', 'uuid'
+            "id",
+            "title",
+            "external_url",
+            "publication_author",
+            "publication_date",
+            "internal_url",
+            "markers",
+            "system_registration_date",
+            "system_update_date",
+            "notes",
+            "access_level",
+            "trust_level",
+            "uuid",
         )
         self.document_fields_extended = (
-            'id', 'title', 'publication_author', 'publication_date', 'external_url',
-            'markers', 'notes', 'access_level', 'trust_level'
-        )
+            "id",
+            "title",
+            "publication_author",
+            "publication_date",
+            "external_url",
+            "markers",
+            "notes",
+            "access_level",
+            "trust_level",
+        )
+
+        self.document_text_fields_truncated = ("text",)
+        self.document_text_fields = ("node_id", "text")
+        self.document_text_metadata_fields = ("paragraph_type",)
 
-        self.document_text_fields_truncated = ('text',)
-        self.document_text_fields = ('node_id', 'text')
-        self.document_text_metadata_fields = ('paragraph_type',)
+        self.document_platform_fields = ("id", "name")
+        self.document_account_fields = ("id", "name")
 
-        self.document_platform_fields = ('id', 'name')
-        self.document_account_fields = ('id', 'name')
-
-        self.user_fields = ('id',)
+        self.user_fields = ("id",)
 
         self.concept_fields = (
-            'id', 'name', 'notes', 'metric', 'markers', 'system_registration_date', 'system_update_date'
-        )
-        self.concept_type_fields = ('id', 'name')
-
-        self.concept_property_fields = ('is_main', 'id', 'system_registration_date')
-        self.concept_property_type_fields_truncated = ('id',)
-        self.concept_property_type_fields = ('id', 'name')
-        self.cpvt_fields_truncated = ('id', 'name', 'value_type')
-        self.cpvt_fields = ('id', 'name', 'value_type', 'value_restriction', 'pretrained_nercmodels')
+            "id",
+            "name",
+            "notes",
+            "metric",
+            "markers",
+            "system_registration_date",
+            "system_update_date",
+        )
+        self.concept_type_fields = ("id", "name")
+
+        self.concept_property_fields = ("is_main", "id", "system_registration_date")
+        self.concept_property_type_fields_truncated = ("id",)
+        self.concept_property_type_fields = ("id", "name")
+        self.cpvt_fields_truncated = ("id", "name", "value_type")
+        self.cpvt_fields = ("id", "name", "value_type", "value_restriction", "pretrained_nercmodels")
+
+        self.concept_link_fields = ("id", "notes")
+        self.concept_link_concept_from_fields = ("id",)
+        self.concept_link_concept_to_fields = ("id",)
+        self.concept_link_type_fields = ("id", "name", "is_directed", "is_hierarchical")
+        self.concept_link_type_fields_truncated = ("id", "name", "is_directed")
+
+        self.concept_fact_fields = ("id",)
+
+        self.composite_concept_widget_type = ("id", "name")
+        self.composite_concept_widget_type_columns_info = ("name",)
 
-        self.concept_link_fields = ('id', 'notes')
-        self.concept_link_concept_from_fields = ('id',)
-        self.concept_link_concept_to_fields = ('id',)
-        self.concept_link_type_fields = ('id', 'name', 'is_directed', 'is_hierarchical')
-        self.concept_link_type_fields_truncated = ('id', 'name', 'is_directed')
+        self.date_time_value_date_fields = ("year", "month", "day")
+        self.date_time_value_time_fields = ("hour", "minute", "second")
 
-        self.concept_fact_fields = ('id',)
+        self.pipeline_config_fields = ("id", "description")
 
-        self.composite_concept_widget_type = ('id', 'name')
-        self.composite_concept_widget_type_columns_info = ('name',)
-
-        self.date_time_value_date_fields = ('year', 'month', 'day')
-        self.date_time_value_time_fields = ('hour', 'minute', 'second')
-
-        self.pipeline_config_fields = ('id', 'description')
-
-        self.pipeline_topic_fields = ('topic', 'description', 'stopped', 'metrics', 'pipeline')
-        self.pipeline_metrics_fields = ('duplicate', 'failed', 'messages', 'ok')
+        self.pipeline_topic_fields = ("topic", "description", "stopped", "metrics", "pipeline")
+        self.pipeline_metrics_fields = ("duplicate", "failed", "messages", "ok")
 
         self.tdm_builder = tdm_builder
 
         if kb_iterator_config:
             self.kb_iterator_config = kb_iterator_config
         else:
             self.kb_iterator_config = KBIteratorConfig(1000, 1609448400)  # Fri Jan 01 2021 00:00:00 GMT+0300
@@ -151,51 +242,47 @@
     def get_take_value(self, take: Optional[int]) -> int:
         return self.limit if take is None else take
 
     def get_perform_synchronously_value(self, perform_synchronously: Optional[bool]) -> bool:
         return self.perform_synchronously if perform_synchronously is None else perform_synchronously
 
     def _configure_property_value_type_fields(self, graphql_value, truncated: bool = True):
-        conpvt_frag: Fragment = Fragment(ConceptPropertyValueType, 'ConceptPropertyValueType')
+        conpvt_frag: Fragment = Fragment(ConceptPropertyValueType, "ConceptPropertyValueType")
         for f in self.cpvt_fields_truncated if truncated else self.cpvt_fields:
             conpvt_frag.__getattr__(f)()
 
-        compvt_frag = Fragment(CompositePropertyValueTemplate, 'CompositePropertyValueTemplate')
-        compvt_frag.__fields__('id', 'name')
+        compvt_frag = Fragment(CompositePropertyValueTemplate, "CompositePropertyValueTemplate")
+        compvt_frag.__fields__("id", "name")
         compvt_frag.component_value_types()
 
         graphql_value.__fragment__(conpvt_frag)
         graphql_value.__fragment__(compvt_frag)
 
     def _configure_output_value_fields(self, graphql_value):
-        dtv_frag = Fragment(DateTimeValue, 'DateTimeFull')
+        dtv_frag = Fragment(DateTimeValue, "DateTimeFull")
         dtv_frag.date().__fields__(*self.date_time_value_date_fields)
         dtv_frag.time().__fields__(*self.date_time_value_time_fields)
 
-        # dtiv_frag = Fragment(DateTimeIntervalValue, 'DateTimeIntervalFull')
-        # dtiv_frag.start.__fragment__(dtv_frag)
-        # dtiv_frag.end.__fragment__(dtv_frag)
-
-        slv_frag = Fragment(StringLocaleValue, 'StringLocaleFull')
+        slv_frag = Fragment(StringLocaleValue, "StringLocaleFull")
         slv_frag.value()
         slv_frag.locale()
 
-        sv_frag = Fragment(StringValue, 'StringFull')
+        sv_frag = Fragment(StringValue, "StringFull")
         sv_frag.value()
 
-        lv_frag = Fragment(LinkValue, 'LinkFull')
+        lv_frag = Fragment(LinkValue, "LinkFull")
         lv_frag.link()
 
-        dv_frag = Fragment(DoubleValue, 'DoubleFull')
-        dv_frag.value(__alias__='double')
+        dv_frag = Fragment(DoubleValue, "DoubleFull")
+        dv_frag.value(__alias__="double")
 
-        iv_frag = Fragment(IntValue, 'IntFull')
-        iv_frag.value(__alias__='number')
+        iv_frag = Fragment(IntValue, "IntFull")
+        iv_frag.value(__alias__="number")
 
-        cv_frag = Fragment(CompositeValue, 'CompFull')
+        cv_frag = Fragment(CompositeValue, "CompFull")
         cv_frag.list_value().id()
         cv_frag.list_value().property_value_type()
         cv_frag.list_value().value().__fragment__(slv_frag)
         cv_frag.list_value().value().__fragment__(sv_frag)
         cv_frag.list_value().value().__fragment__(lv_frag)
         cv_frag.list_value().value().__fragment__(dv_frag)
         cv_frag.list_value().value().__fragment__(iv_frag)
@@ -204,48 +291,47 @@
         graphql_value.__fragment__(slv_frag)
         graphql_value.__fragment__(sv_frag)
         graphql_value.__fragment__(lv_frag)
         graphql_value.__fragment__(dv_frag)
         graphql_value.__fragment__(iv_frag)
         graphql_value.__fragment__(dtv_frag)
         graphql_value.__fragment__(cv_frag)
-        # graphql_value.__fragment__(dtiv_frag)
 
     def _configure_output_concept_fields(
-        self, concept_object, with_aliases=False, with_properties=False, with_links=False,
-        with_link_properties=False, with_facts=False, with_potential_facts=False
+        self,
+        concept_object,
+        with_aliases=False,
+        with_properties=False,
+        with_links=False,
+        with_link_properties=False,
+        with_facts=False,
+        with_potential_facts=False,
     ):
         concept_object.__fields__(*self.concept_fields)
         concept_object.concept_type.__fields__(*self.concept_type_fields)
         if with_aliases:
-            sv_frag = Fragment(StringValue, 'StringFull')
+            sv_frag = Fragment(StringValue, "StringFull")
             sv_frag.value()
             concept_object.list_alias.value.__fragment__(sv_frag)
         if with_properties:
             pcp: ConceptPropertyPagination = concept_object.pagination_concept_property(
-                offset=0,
-                limit=10000,
-                filter_settings=ConceptPropertyFilterSettings()
+                offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
             )
             lcp = pcp.list_concept_property()
             lcp.__fields__(*self.concept_property_fields)
             lcp.property_type().__fields__(*self.concept_property_type_fields)
             self._configure_output_value_fields(lcp.value)
         if with_links:
             pcl: ConceptLinkPagination = concept_object.pagination_concept_link(
-                offset=0,
-                limit=10000,
-                filter_settings=ConceptLinkFilterSettings()
+                offset=0, limit=10000, filter_settings=ConceptLinkFilterSettings()
             )
             self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         if with_facts:
             pcf: ConceptFactPagination = concept_object.pagination_concept_fact(
-                offset=0,
-                limit=10000,
-                filter_settings=DocumentLinkFilterSetting()
+                offset=0, limit=10000, filter_settings=DocumentLinkFilterSetting()
             )
             lcf = pcf.list_concept_fact()
             lcf.__fields__(*self.concept_fact_fields)
             d = lcf.document()
             d.__fields__(*self.document_fields_extended)
             dm = d.metadata()
             dm.platform().__fields__(*self.document_platform_fields)
@@ -255,59 +341,54 @@
             lccf.__fields__(*self.concept_fact_fields)
             d = lccf.document()
             d.__fields__(*self.document_fields_extended)
             dm = d.metadata()
             dm.platform().__fields__(*self.document_platform_fields)
             dm.account().__fields__(*self.document_account_fields)
 
-    def _configure_output_link_fields(
-        self, link_object, with_link_properties=False
-    ):
+    def _configure_output_link_fields(self, link_object, with_link_properties=False):
         link_object.__fields__(*self.concept_link_fields)
         link_object.concept_from().__fields__(*self.concept_link_concept_from_fields)
         link_object.concept_to().__fields__(*self.concept_link_concept_to_fields)
         link_object.concept_link_type().__fields__(*self.concept_link_type_fields_truncated)
         if with_link_properties:
             pcp: ConceptPropertyPagination = link_object.pagination_concept_link_property(
-                offset=0,
-                limit=10000,
-                filter_settings=ConceptPropertyFilterSettings()
+                offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
             )
             lcp = pcp.list_concept_property()
             lcp.__fields__(*self.concept_property_fields)
             lcp.property_type().__fields__(*self.concept_property_type_fields)
             self._configure_output_value_fields(lcp.value)
 
     def _create_concept_with_input(
-        self, input: ConceptMutationInput, with_properties=False, with_links=False, with_link_properties=False,
-        perform_synchronously: Optional[bool] = None
+        self,
+        form: ConceptMutationInput,
+        with_properties=False,
+        with_links=False,
+        with_link_properties=False,
+        perform_synchronously: Optional[bool] = None,
     ) -> Concept:
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
         op = Operation(Mutation)
         ac = op.add_concept(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
-            form=input
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously), form=form
         )
         self._configure_output_concept_fields(
-            ac, with_properties=with_properties, with_links=with_links,
-            with_link_properties=with_link_properties
+            ac, with_properties=with_properties, with_links=with_links, with_link_properties=with_link_properties
         )
         res = self._gql_client.execute(op)
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.add_concept)
 
         return res.add_concept
 
     def _get_components_mapping(
-        self, component_values: Dict[str, str],
-        component_value_types: List[CompositePropertyValueType]
+        self, component_values: Dict[str, str], component_value_types: List[CompositePropertyValueType]
     ) -> Dict[str, CompositePropertyValueType]:
         components_type_mapping = {}
         for component_value in component_values:
             for component_value_type in component_value_types:
                 if component_value_type.name != component_values[component_value]:
                     continue
                 components_type_mapping[component_value] = component_value_type
@@ -317,98 +398,119 @@
         self, values: dict, components_type_mapping: Dict[str, CompositePropertyValueType]
     ) -> List[ComponentValueInput]:
         value_input = []
         for field in values:
             if field not in components_type_mapping:
                 continue
             value_id = components_type_mapping[field].id
-            value_input.append(ComponentValueInput(
-                id=value_id,
-                value=get_map_helper(
-                    components_type_mapping[field].value_type.value_type).get_value_input(values[field])
-            ))
+            value_input.append(
+                ComponentValueInput(
+                    id=value_id,
+                    value=get_map_helper(components_type_mapping[field].value_type.value_type).get_value_input(
+                        values[field]
+                    ),
+                )
+            )
         return value_input
 
     def _configure_pipeline_topic_fields(self, kafka_topic: tc.KafkaTopic):
         kafka_topic.__fields__(*self.pipeline_topic_fields)
         kafka_topic.metrics().__fields__(*self.pipeline_metrics_fields)
         kafka_topic.pipeline().pipeline_config().__fields__(*self.pipeline_config_fields)
 
     def get_all_documents(
-        self, grouping: DocumentGrouping = 'none', filter_settings: DocumentFilterSettings = None,
-        direction: SortDirection = 'descending', sort_field: DocumentSorting = 'score',
-        extra_settings: ExtraSettings = None, with_extended_information: bool = False
+        self,
+        grouping: DocumentGrouping = "none",
+        filter_settings: DocumentFilterSettings = None,
+        direction: SortDirection = "descending",
+        sort_field: DocumentSorting = "score",
+        extra_settings: ExtraSettings = None,
+        with_extended_information: bool = False,
     ) -> Iterable[Story]:
         if filter_settings is None:
             filter_settings = DocumentFilterSettings()
         if extra_settings is None:
             extra_settings = ExtraSettings()
 
         total = self.get_documents_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
-            had_creation_date = hasattr(filter_settings, 'registration_date')
+            had_creation_date = hasattr(filter_settings, "registration_date")
             old_timestamp_interval = None
             if had_creation_date:
                 old_timestamp_interval = copy(filter_settings.registration_date)
-            start: int = getattr(old_timestamp_interval, 'start', self.kb_iterator_config.earliest_created_time)
-            end: int = getattr(old_timestamp_interval, 'end', int(time()))
+            start: int = getattr(old_timestamp_interval, "start", self.kb_iterator_config.earliest_created_time)
+            end: int = getattr(old_timestamp_interval, "end", int(time()))
             middle: int = (end + start) // 2
 
-            for start, end in (start, middle), (middle, end):
-                filter_settings.registration_date = TimestampInterval(start=start, end=end)
-                for c in self.get_all_documents(
-                    grouping=grouping, filter_settings=filter_settings, direction=direction, sort_field=sort_field,
-                    extra_settings=extra_settings, with_extended_information=with_extended_information
-                ):
-                    yield c
+            for next_start, next_end in (start, middle), (middle, end):
+                if next_start == start and next_end == end:
+                    logger.info(f"Processed only {self._limit} documents, {total - self._limit} ignored")
+                    continue
+                filter_settings.registration_date = TimestampInterval(start=next_start, end=next_end)
+                yield from self.get_all_documents(
+                    grouping=grouping,
+                    filter_settings=filter_settings,
+                    direction=direction,
+                    sort_field=sort_field,
+                    extra_settings=extra_settings,
+                    with_extended_information=with_extended_information,
+                )
 
             if had_creation_date:
                 filter_settings.registration_date = old_timestamp_interval
             else:
-                delattr(filter_settings, 'registration_date')
+                delattr(filter_settings, "registration_date")
             return
         elif not total:
             return
 
         documents: Iterable = [None]
         i: int = 0
         while documents:
-            documents = self.get_documents(
-                skip=i * self._limit, take=self._limit, grouping=grouping, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field, extra_settings=extra_settings,
-                with_extended_information=with_extended_information
+            yield from self.get_documents(
+                skip=i * self._limit,
+                take=self._limit,
+                grouping=grouping,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
+                extra_settings=extra_settings,
+                with_extended_information=with_extended_information,
             )
-            for d in documents:
-                yield d
             i += 1
 
     def get_documents(
-        self, skip: int = 0, take: Optional[int] = None, grouping: DocumentGrouping = 'none',
-        filter_settings: DocumentFilterSettings = None, direction: SortDirection = 'descending',
-        sort_field: DocumentSorting = 'score', extra_settings: ExtraSettings = None,
-        with_extended_information: bool = False
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        grouping: DocumentGrouping = "none",
+        filter_settings: DocumentFilterSettings = None,
+        direction: SortDirection = "descending",
+        sort_field: DocumentSorting = "score",
+        extra_settings: ExtraSettings = None,
+        with_extended_information: bool = False,
     ) -> Sequence[Story]:
         take = self.get_take_value(take)
-        pagination_story_kwargs = dict()
+        pagination_story_kwargs = {}
         if filter_settings is None:
             filter_settings = DocumentFilterSettings()
         if extra_settings is None:
             extra_settings = ExtraSettings()
 
         op = Operation(Query)
         ps: StoryPagination = op.pagination_story(
             offset=skip,
             limit=take,
             grouping=grouping,
             filter_settings=filter_settings,
             direction=direction,
             sort_field=sort_field,
             extra_settings=extra_settings,
-            **pagination_story_kwargs
+            **pagination_story_kwargs,
         )
         ps.list_story().list_document().__fields__(*self.document_fields_truncated)
         m = ps.list_story().main()
         if with_extended_information:
             m.__fields__(*self.document_fields_extended)
             mdm = m.metadata()
             mdm.platform().__fields__(*self.document_platform_fields)
@@ -423,49 +525,48 @@
 
     def get_documents_count(self, filter_settings: DocumentFilterSettings = None) -> int:
         if filter_settings is None:
             filter_settings = DocumentFilterSettings()
 
         op = Operation(Query)
         ps: StoryPagination = op.pagination_story(
-            limit=1,
-            filter_settings=filter_settings,
-            extra_settings=ExtraSettings()
+            limit=1, filter_settings=filter_settings, extra_settings=ExtraSettings()
         )
         ps.show_total()
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_story.show_total
 
     def get_documents_by_limit_offset_filter_extra_settings(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: Optional[DocumentFilterSettings] = None,
-        extra_settings: Optional[ExtraSettings] = None
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: Optional[DocumentFilterSettings] = None,
+        extra_settings: Optional[ExtraSettings] = None,
     ) -> Sequence[Story]:
         take = self.get_take_value(take)
         op = Operation(Query)
         ps: StoryPagination = op.pagination_story(
             offset=skip,
             limit=take,
             extra_settings=extra_settings if extra_settings else ExtraSettings(),
-            filter_settings=filter_settings if filter_settings else DocumentFilterSettings()
+            filter_settings=filter_settings if filter_settings else DocumentFilterSettings(),
         )
         ps.list_story().list_document().__fields__(*self.document_fields_truncated)
         m = ps.list_story().main()
         m.__fields__(*self.document_fields_truncated)
         m.text().__fields__(*self.document_text_fields_truncated)
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_story.list_story
 
     def get_document(self, document_id: str) -> Document:
         op = Operation(Query)
-        d: Document = op.document(
-            id=document_id
-        )
+        d: Document = op.document(id=document_id)
         d.__fields__(*self.document_fields)
         d.last_updater().__fields__(*self.user_fields)
         d.metadata().platform().__fields__(*self.document_platform_fields)
         d.metadata().account().__fields__(*self.document_account_fields)
         d.creator().__fields__(*self.user_fields)
         dt = d.text(show_hidden=True)
         dt.__fields__(*self.document_text_fields)
@@ -503,44 +604,47 @@
         )
         pcl.total()
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link.total
 
     def get_concept(
-        self, concept_id: str, with_aliases: bool = False,
-        with_properties: bool = True, with_links: bool = True,
-        with_link_properties: bool = True, with_facts: bool = False,
-        with_potential_facts: bool = False
+        self,
+        concept_id: str,
+        with_aliases: bool = False,
+        with_properties: bool = True,
+        with_links: bool = True,
+        with_link_properties: bool = True,
+        with_facts: bool = False,
+        with_potential_facts: bool = False,
     ) -> Concept:
         op = Operation(Query)
-        c: Concept = op.concept(
-            id=concept_id
-        )
+        c: Concept = op.concept(id=concept_id)
         self._configure_output_concept_fields(
-            c, with_aliases=with_aliases, with_properties=with_properties,
-            with_links=with_links, with_link_properties=with_link_properties,
-            with_facts=with_facts, with_potential_facts=with_potential_facts
+            c,
+            with_aliases=with_aliases,
+            with_properties=with_properties,
+            with_links=with_links,
+            with_link_properties=with_link_properties,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.concept)
 
         return res.concept
 
     def get_concept_facts(
         self, concept_id: str, filter_settings: DocumentLinkFilterSetting = None
     ) -> Sequence[ConceptFact]:
-
         op = Operation(Query)
-        c: Concept = op.concept(
-            id=concept_id
-        )
+        c: Concept = op.concept(id=concept_id)
         pcf: ConceptFactPagination = c.pagination_concept_fact(
             filter_settings=filter_settings if filter_settings else DocumentLinkFilterSetting()
         )
         lcf = pcf.list_concept_fact()
         lcf.__fields__(*self.concept_fact_fields)
         d = lcf.document()
         d.__fields__(*self.document_fields_extended)
@@ -551,483 +655,529 @@
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.concept.pagination_concept_fact.list_concept_fact
 
     def get_concept_link(self, link_id: str, with_facts: bool = False) -> ConceptLink:
         op = Operation(Query)
-        cl: ConceptLink = op.concept_link(
-            id=link_id
-        )
+        cl: ConceptLink = op.concept_link(id=link_id)
         cl.__fields__(*self.concept_link_fields)
         self._configure_output_concept_fields(cl.concept_from)
         self._configure_output_concept_fields(cl.concept_to)
         cl.concept_link_type.__fields__(*self.concept_link_type_fields_truncated)
         if with_facts:
-            cl.__fields__('list_concept_link_fact')
+            cl.__fields__("list_concept_link_fact")
         res = self._gql_client.execute(op)
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_fact(res.concept_link)
 
         return res.concept_link
 
     def get_all_concepts(
-        self, filter_settings: ConceptFilterSettings = None,
-        direction: SortDirection = 'descending', sort_field: ConceptSorting = 'score',
-        with_aliases: bool = False, with_properties: bool = False, with_links: bool = False,
-        with_link_properties: bool = False, with_facts: bool = False, with_potential_facts: bool = False
+        self,
+        filter_settings: ConceptFilterSettings = None,
+        direction: SortDirection = "descending",
+        sort_field: ConceptSorting = "score",
+        with_aliases: bool = False,
+        with_properties: bool = False,
+        with_links: bool = False,
+        with_link_properties: bool = False,
+        with_facts: bool = False,
+        with_potential_facts: bool = False,
     ) -> Iterable[Concept]:
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
         total = self.get_concept_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
-            had_creation_date = hasattr(filter_settings, 'creation_date')
+            had_creation_date = hasattr(filter_settings, "creation_date")
             old_timestamp_interval = None
             if had_creation_date:
                 old_timestamp_interval = copy(filter_settings.creation_date)
-            start: int = getattr(old_timestamp_interval, 'start', self.kb_iterator_config.earliest_created_time)
-            end: int = getattr(old_timestamp_interval, 'end', int(time()))
+            start: int = getattr(old_timestamp_interval, "start", self.kb_iterator_config.earliest_created_time)
+            end: int = getattr(old_timestamp_interval, "end", int(time()))
             middle: int = (end + start) // 2
 
-            for start, end in (start, middle), (middle, end):
-                filter_settings.creation_date = TimestampInterval(start=start, end=end)
+            for next_start, next_end in (start, middle), (middle, end):
+                if next_start == start and next_end == end:
+                    logger.info(f"Processed only {self._limit} concepts, {total - self._limit} ignored")
+                    continue
+                filter_settings.creation_date = TimestampInterval(start=next_start, end=next_end)
                 yield from self.get_all_concepts(
-                    filter_settings=filter_settings, direction=direction, sort_field=sort_field,
-                    with_aliases=with_aliases, with_properties=with_properties, with_links=with_links,
-                    with_link_properties=with_link_properties, with_facts=with_facts,
-                    with_potential_facts=with_potential_facts
+                    filter_settings=filter_settings,
+                    direction=direction,
+                    sort_field=sort_field,
+                    with_aliases=with_aliases,
+                    with_properties=with_properties,
+                    with_links=with_links,
+                    with_link_properties=with_link_properties,
+                    with_facts=with_facts,
+                    with_potential_facts=with_potential_facts,
                 )
 
             if had_creation_date:
                 filter_settings.creation_date = old_timestamp_interval
             else:
-                delattr(filter_settings, 'creation_date')
+                delattr(filter_settings, "creation_date")
             return
         elif not total:
             return
 
         concepts: Iterable = [None]
         i: int = 0
         while concepts:
             concepts = self.get_concepts(
-                skip=i * self._limit, take=self._limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field, with_aliases=with_aliases,
-                with_properties=with_properties, with_links=with_links,
-                with_link_properties=with_link_properties, with_facts=with_facts,
-                with_potential_facts=with_potential_facts
+                skip=i * self._limit,
+                take=self._limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
+                with_aliases=with_aliases,
+                with_properties=with_properties,
+                with_links=with_links,
+                with_link_properties=with_link_properties,
+                with_facts=with_facts,
+                with_potential_facts=with_potential_facts,
             )
-            for c in concepts:
-                yield c
+            yield from concepts
             i += 1
 
     def get_concepts(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptFilterSettings = None,
-        direction: SortDirection = 'descending', sort_field: ConceptSorting = 'score',
-        with_aliases: bool = False, with_properties: bool = False, with_links: bool = False,
-        with_link_properties: bool = False, with_facts: bool = False, with_potential_facts=False
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptFilterSettings = None,
+        direction: SortDirection = "descending",
+        sort_field: ConceptSorting = "score",
+        with_aliases: bool = False,
+        with_properties: bool = False,
+        with_links: bool = False,
+        with_link_properties: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> Sequence[Concept]:
         take = self.get_take_value(take)
-        pagination_concept_kwargs = dict()
+        pagination_concept_kwargs = {}
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
 
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             limit=take,
             offset=skip,
             filter_settings=filter_settings,
             direction=direction,
             sort_field=sort_field,
-            **pagination_concept_kwargs
+            **pagination_concept_kwargs,
         )
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_properties=with_properties,
-            with_links=with_links, with_link_properties=with_link_properties,
-            with_facts=with_facts, with_potential_facts=with_potential_facts
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_properties=with_properties,
+            with_links=with_links,
+            with_link_properties=with_link_properties,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concepts_by_limit_offset_filter_settings(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: Optional[ConceptFilterSettings] = None,
-        with_aliases: bool = False, with_facts: bool = False, with_potential_facts=False
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: Optional[ConceptFilterSettings] = None,
+        with_aliases: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> Sequence[Concept]:
         take = self.get_take_value(take)
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
-            filter_settings=filter_settings if filter_settings else ConceptFilterSettings(),
-            offset=skip,
-            limit=take
+            filter_settings=filter_settings if filter_settings else ConceptFilterSettings(), offset=skip, limit=take
         )
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
-            with_potential_facts=with_potential_facts
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_all_concept_links(
         self, filter_settings: ConceptLinkFilterSettings = None, with_link_properties: bool = False
     ) -> Iterable[ConceptLink]:
         if not filter_settings:
             filter_settings = ConceptLinkFilterSettings()
 
         total = self.get_concept_link_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
-            had_creation_date = hasattr(filter_settings, 'creation_date')
+            had_creation_date = hasattr(filter_settings, "creation_date")
             old_timestamp_interval = None
             if had_creation_date:
                 old_timestamp_interval = copy(filter_settings.creation_date)
-            start: int = getattr(old_timestamp_interval, 'start', self.kb_iterator_config.earliest_created_time)
-            end: int = getattr(old_timestamp_interval, 'end', int(time()))
+            start: int = getattr(old_timestamp_interval, "start", self.kb_iterator_config.earliest_created_time)
+            end: int = getattr(old_timestamp_interval, "end", int(time()))
             middle: int = (end + start) // 2
 
-            for start, end in (start, middle), (middle, end):
-                filter_settings.creation_date = TimestampInterval(start=start, end=end)
-                for c in self.get_all_concept_links(filter_settings=filter_settings,
-                                                    with_link_properties=with_link_properties):
+            for next_start, next_end in (start, middle), (middle, end):
+                if next_start == start and next_end == end:
+                    logger.info(f"Processed only {self._limit} links, {total - self._limit} ignored")
+                    continue
+                filter_settings.creation_date = TimestampInterval(start=next_start, end=next_end)
+                for c in self.get_all_concept_links(
+                    filter_settings=filter_settings, with_link_properties=with_link_properties
+                ):
                     yield c
 
             if had_creation_date:
                 filter_settings.creation_date = old_timestamp_interval
             else:
-                delattr(filter_settings, 'creation_date')
+                delattr(filter_settings, "creation_date")
             return
         elif not total:
             return
 
         links: Iterable = [None]
         i: int = 0
         while links:
             links = self.get_concept_links_by_limit_offset_filter_settings(
-                skip=i * self._limit, take=self._limit,
-                filter_settings=filter_settings, with_link_properties=with_link_properties
+                skip=i * self._limit,
+                take=self._limit,
+                filter_settings=filter_settings,
+                with_link_properties=with_link_properties,
             )
-            for link in links:
-                yield link
+            yield from links
             i += 1
 
     def get_concept_links_by_limit_offset_filter_settings(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptLinkFilterSettings = None,
-        with_link_properties: bool = False
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptLinkFilterSettings = None,
+        with_link_properties: bool = False,
     ) -> Sequence[ConceptLink]:
         take = self.get_take_value(take)
         op = Operation(Query)
         pcl: ConceptLinkPagination = op.pagination_concept_link(
-            filter_settings=filter_settings if filter_settings else ConceptLinkFilterSettings(),
-            offset=skip,
-            limit=take
+            filter_settings=filter_settings if filter_settings else ConceptLinkFilterSettings(), offset=skip, limit=take
         )
         self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link.list_concept_link
 
     def get_concepts_by_type_id_with_offset(
-        self, type_id: str, skip: int, take: Optional[int] = None, direction='descending',
-        sort_field='systemRegistrationDate', with_aliases: bool = False, with_properties: bool = False,
-        with_links: bool = False, with_link_properties: bool = False, with_facts: bool = False,
-        with_potential_facts=False
+        self,
+        type_id: str,
+        skip: int,
+        take: Optional[int] = None,
+        direction="descending",
+        sort_field="systemRegistrationDate",
+        with_aliases: bool = False,
+        with_properties: bool = False,
+        with_links: bool = False,
+        with_link_properties: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> ConceptPagination:
         take = self.get_take_value(take)
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
-            filter_settings=ConceptFilterSettings(
-                concept_type_ids=[type_id]
-            ),
+            filter_settings=ConceptFilterSettings(concept_type_ids=[type_id]),
             limit=take,
             offset=skip,
             direction=direction,
-            sort_field=sort_field
+            sort_field=sort_field,
         )
         cp.total()
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_properties=with_properties, with_links=with_links,
-            with_link_properties=with_link_properties, with_facts=with_facts, with_potential_facts=with_potential_facts
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_properties=with_properties,
+            with_links=with_links,
+            with_link_properties=with_link_properties,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept
 
     def get_concepts_by_type_id_with_offset_with_markers(
-        self, type_id: str, skip: int = 0, take: Optional[int] = None, markers: Optional[List[str]] = None,
-        direction='descending', sort_field='systemRegistrationDate', with_aliases: bool = False,
-        with_facts: bool = False, with_potential_facts=False
+        self,
+        type_id: str,
+        skip: int = 0,
+        take: Optional[int] = None,
+        markers: Optional[List[str]] = None,
+        direction="descending",
+        sort_field="systemRegistrationDate",
+        with_aliases: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> ConceptPagination:
         take = self.get_take_value(take)
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=ConceptFilterSettings(
                 concept_type_ids=[type_id],
                 markers=markers,
             ),
             limit=take,
             offset=skip,
             direction=direction,
-            sort_field=sort_field
+            sort_field=sort_field,
         )
         cp.total()
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
-            with_potential_facts=with_potential_facts)
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
+        )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept
 
     def get_concepts_by_name(
-        self, name: str, type_id: Optional[str] = None, with_aliases: bool = False,
-        with_facts: bool = False, with_potential_facts=False
+        self,
+        name: str,
+        type_id: Optional[str] = None,
+        with_aliases: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> Sequence[Concept]:
-
         op = Operation(Query)
         if type_id:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
-                exact_name=name,
-                concept_type_ids=[type_id]
+                exact_name=name, concept_type_ids=[type_id]
             )
         else:
-            concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
-                exact_name=name
-            )
-        cp: ConceptPagination = op.pagination_concept(
-            filter_settings=concept_filter_settings
-        )
+            concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(exact_name=name)
+        cp: ConceptPagination = op.pagination_concept(filter_settings=concept_filter_settings)
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
-            with_potential_facts=with_potential_facts
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concepts_by_near_name(
-        self, name: str, type_id: Optional[str] = None, with_aliases: bool = False,
-        with_facts: bool = False, with_potential_facts=False
+        self,
+        name: str,
+        type_id: Optional[str] = None,
+        with_aliases: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> Sequence[Concept]:
-
         op = Operation(Query)
         if type_id:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
-                name=name,
-                concept_type_ids=[type_id]
+                name=name, concept_type_ids=[type_id]
             )
         else:
-            concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
-                name=name
-            )
-        cp: ConceptPagination = op.pagination_concept(
-            filter_settings=concept_filter_settings
-        )
+            concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(name=name)
+        cp: ConceptPagination = op.pagination_concept(filter_settings=concept_filter_settings)
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
-            with_potential_facts=with_potential_facts
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concepts_by_property_name(
-        self, property_type_id: str, string_filter: str, property_type: str = 'concept', with_aliases: bool = False,
-        with_facts: bool = False, with_potential_facts=False
+        self,
+        property_type_id: str,
+        string_filter: str,
+        property_type: str = "concept",
+        with_aliases: bool = False,
+        with_facts: bool = False,
+        with_potential_facts=False,
     ) -> Sequence[Concept]:
-
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=ConceptFilterSettings(
-                property_filter_settings=[PropertyFilterSettings(
-                    property_type=property_type,
-                    property_type_id=property_type_id,
-                    string_filter=StringFilter(
-                        str=string_filter
+                property_filter_settings=[
+                    PropertyFilterSettings(
+                        property_type=property_type,
+                        property_type_id=property_type_id,
+                        string_filter=StringFilter(str=string_filter),
                     )
-                )]
+                ]
             )
         )
         self._configure_output_concept_fields(
-            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
-            with_potential_facts=with_potential_facts
+            cp.list_concept(),
+            with_aliases=with_aliases,
+            with_facts=with_facts,
+            with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concept_properties(self, concept_id: str, with_facts: bool = False) -> Sequence[ConceptProperty]:
         op = Operation(Query)
-        concept: Concept = op.concept(
-            id=concept_id
-        )
+        concept: Concept = op.concept(id=concept_id)
         pcp: ConceptPropertyPagination = concept.pagination_concept_property(
-            offset=0,
-            limit=10000,
-            filter_settings=ConceptPropertyFilterSettings()
+            offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
         )
         lcp = pcp.list_concept_property()
         lcp.__fields__(*self.concept_property_fields)
         lcp.property_type().__fields__(*self.concept_property_type_fields)
         self._configure_output_value_fields(lcp.value)
         if with_facts:
-            lcp.__fields__('list_concept_property_fact')
+            lcp.__fields__("list_concept_property_fact")
 
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept.pagination_concept_property.list_concept_property
 
     def get_concept_links(self, concept_id: str, with_link_properties: bool = False) -> Sequence[ConceptLink]:
         op = Operation(Query)
 
-        concept: Concept = op.concept(
-            id=concept_id
-        )
+        concept: Concept = op.concept(id=concept_id)
         pcl: ConceptLinkPagination = concept.pagination_concept_link(
-            offset=0,
-            limit=10000,
-            filter_settings=ConceptLinkFilterSettings()
+            offset=0, limit=10000, filter_settings=ConceptLinkFilterSettings()
         )
         self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept.pagination_concept_link.list_concept_link
 
     def get_concept_links_concept(
-            self, concept_id: str, link_type_id: str, with_link_properties: bool = False
+        self, concept_id: str, link_type_id: str, with_link_properties: bool = False
     ) -> Sequence[ConceptLink]:
         op = Operation(Query)
 
-        concept = op.concept(
-            id=concept_id
-        )
+        concept = op.concept(id=concept_id)
         pcl = concept.pagination_concept_link(
-            offset=0,
-            limit=10000,
-            filter_settings=ConceptLinkFilterSettings(
-                concept_link_type=[link_type_id]
-            )
+            offset=0, limit=10000, filter_settings=ConceptLinkFilterSettings(concept_link_type=[link_type_id])
         )
         self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept.pagination_concept_link.list_concept_link
 
     def get_link_properties(self, link_id: str, with_facts: bool = False) -> Sequence[ConceptProperty]:
         op = Operation(Query)
-        concept_link: ConceptLink = op.concept_link(
-            id=link_id
-        )
+        concept_link: ConceptLink = op.concept_link(id=link_id)
         pcp: ConceptPropertyPagination = concept_link.pagination_concept_link_property(
-            offset=0,
-            limit=10000,
-            filter_settings=ConceptPropertyFilterSettings()
+            offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
         )
         lcp = pcp.list_concept_property()
         lcp.__fields__(*self.concept_property_fields)
         lcp.property_type().__fields__(*self.concept_property_type_fields)
         self._configure_output_value_fields(lcp.value)
         if with_facts:
-            lcp.__fields__('list_concept_property_fact')
+            lcp.__fields__("list_concept_property_fact")
 
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept_link.pagination_concept_link_property.list_concept_property
 
     def get_concept_time_intervals(
         self, filter_settings: ConceptFilterSettings = None, max_interval_size: Optional[int] = None
     ) -> Iterable[ObjectTimeInterval]:
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
-        for time_interval in self._get_object_time_intervals(filter_settings, max_interval_size):
-            yield time_interval
+        yield from self._get_object_time_intervals(filter_settings, max_interval_size)
 
     def get_concept_link_time_intervals(
         self, filter_settings: ConceptLinkFilterSettings = None, max_interval_size: Optional[int] = None
     ) -> Iterable[ObjectTimeInterval]:
         if not filter_settings:
             filter_settings = ConceptLinkFilterSettings()
-        for time_interval in self._get_object_time_intervals(filter_settings, max_interval_size):
-            yield time_interval
+        yield from self._get_object_time_intervals(filter_settings, max_interval_size)
 
     def get_document_time_intervals(
         self, filter_settings: DocumentFilterSettings = None, max_interval_size: Optional[int] = None
     ) -> Iterable[ObjectTimeInterval]:
         if not filter_settings:
             filter_settings = DocumentFilterSettings()
-        for time_interval in self._get_object_time_intervals(filter_settings, max_interval_size):
-            yield time_interval
+        yield from self._get_object_time_intervals(filter_settings, max_interval_size)
 
     def _get_object_time_intervals(
-        self, filter_settings: Union[ConceptFilterSettings, ConceptLinkFilterSettings, DocumentFilterSettings],
-        max_interval_size: Optional[int] = None
+        self,
+        filter_settings: Union[ConceptFilterSettings, ConceptLinkFilterSettings, DocumentFilterSettings],
+        max_interval_size: Optional[int] = None,
     ) -> Iterable[ObjectTimeInterval]:
         max_interval_size = max_interval_size if max_interval_size else self.kb_iterator_config.max_total_count
 
-        creation_date_field_name = 'creation_date'
+        creation_date_field_name = "creation_date"
         if isinstance(filter_settings, ConceptFilterSettings):
             object_count = self.get_concept_count(filter_settings)
         elif isinstance(filter_settings, ConceptLinkFilterSettings):
             object_count = self.get_concept_link_count(filter_settings)
         elif isinstance(filter_settings, DocumentFilterSettings):
             object_count = self.get_documents_count(filter_settings)
-            creation_date_field_name = 'registration_date'
+            creation_date_field_name = "registration_date"
         else:
-            raise Exception('Time division is only available for concepts, links and documents')
+            raise Exception("Time division is only available for concepts, links and documents")
         creation_date = getattr(filter_settings, creation_date_field_name, None)
-        start: int = getattr(creation_date, 'start', self.kb_iterator_config.earliest_created_time)
-        end: int = getattr(creation_date, 'end', int(time()))
+        start: int = getattr(creation_date, "start", self.kb_iterator_config.earliest_created_time)
+        end: int = getattr(creation_date, "end", int(time()))
 
         if (object_count > max_interval_size) and (start < end):
             middle = (end + start) // 2
 
-            for start, end in (start, middle), (middle + 1, end):
-                setattr(filter_settings, creation_date_field_name, TimestampInterval(start=start, end=end))
+            for mod_start, mod_end in (start, middle), (middle + 1, end):
+                setattr(filter_settings, creation_date_field_name, TimestampInterval(start=mod_start, end=mod_end))
                 for time_interval in self._get_object_time_intervals(filter_settings, max_interval_size):
                     yield time_interval
         elif object_count > 0:
             yield ObjectTimeInterval(
-                start_time=start,
-                end_time=end,
-                object_count=object_count,
-                max_interval_size=max_interval_size
+                start_time=start, end_time=end, object_count=object_count, max_interval_size=max_interval_size
             )
 
     def create_concept(
-        self, name: str, type_id: str, notes: str = None, with_properties=False, with_links=False,
-        with_link_properties=False, perform_synchronously: Optional[bool] = None
+        self,
+        name: str,
+        type_id: str,
+        notes: str = None,
+        with_properties=False,
+        with_links=False,
+        with_link_properties=False,
+        perform_synchronously: Optional[bool] = None,
     ) -> Concept:
-
-        cmi: ConceptMutationInput = ConceptMutationInput(
-            name=name,
-            concept_type_id=type_id,
-            notes=notes
-        )
+        cmi: ConceptMutationInput = ConceptMutationInput(name=name, concept_type_id=type_id, notes=notes)
         return self._create_concept_with_input(
-            cmi, with_properties=with_properties, with_links=with_links,
-            with_link_properties=with_link_properties, perform_synchronously=perform_synchronously
+            cmi,
+            with_properties=with_properties,
+            with_links=with_links,
+            with_link_properties=with_link_properties,
+            perform_synchronously=perform_synchronously,
         )
 
     def update_concept(
         self, c: Concept, markers: List[str] = None, notes: str = None, perform_synchronously: Optional[bool] = None
     ) -> Concept:
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
         op = Operation(Mutation)
         uc: Concept = op.update_concept(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptUpdateInput(
                 concept_id=c.id,
                 name=c.name,
                 concept_type_id=c.concept_type.id,
                 markers=markers if markers is not None else c.markers,
-                notes=notes if notes is not None else c.notes
-            )
+                notes=notes if notes is not None else c.notes,
+            ),
         )
         self._configure_output_concept_fields(uc)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept
 
@@ -1035,196 +1185,175 @@
         op = Operation(Mutation)
         ucpvt = op.update_concept_property_value_type(
             form=ConceptPropertyValueTypeUpdateInput(
                 id=cpvt.id,
                 name=cpvt.name,
                 value_type=cpvt.value_type,
                 pretrained_nercmodels=cpvt.pretrained_nercmodels,
-                value_restriction=cpvt.value_restriction
+                value_restriction=cpvt.value_restriction,
             )
         )
-        ucpvt.__fields__('id')
+        ucpvt.__fields__("id")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property_value_type
 
     def update_concept_string_property(self, cp: ConceptProperty) -> ConceptProperty:
         op = Operation(Mutation)
         ucp: ConceptProperty = op.update_concept_property(
             form=ConceptPropertyUpdateInput(
                 property_id=cp.id,
                 is_main=cp.is_main,
                 value_input=[
-                    ComponentValueInput(
-                        value=ValueInput(
-                            string_value_input=StringValueInput(
-                                value=cp.value.value
-                            )
-                        )
-                    )
-                ]
+                    ComponentValueInput(value=ValueInput(string_value_input=StringValueInput(value=cp.value.value)))
+                ],
             )
         )
-        ucp.__fields__('id')
+        ucp.__fields__("id")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property
 
     def update_concept_int_property(self, cp: ConceptProperty) -> ConceptProperty:
         op = Operation(Mutation)
         ucp: ConceptProperty = op.update_concept_property(
             form=ConceptPropertyUpdateInput(
                 property_id=cp.id,
                 is_main=cp.is_main,
                 value_input=[
-                    ComponentValueInput(
-                        value=ValueInput(
-                            int_value_input=IntValueInput(
-                                value=cp.value.number
-                            )
-                        )
-                    )
-                ]
+                    ComponentValueInput(value=ValueInput(int_value_input=IntValueInput(value=cp.value.number)))
+                ],
             )
         )
-        ucp.__fields__('id')
+        ucp.__fields__("id")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property
 
     def update_concept_composite_property(self, cp: ConceptProperty) -> ConceptProperty:
         value_input = []
         for value in cp.value.list_value:
             if type(value.value) is StringValue:
-                value_input.append(ComponentValueInput(
-                    id=value.id,
-                    value=ValueInput(
-                        string_value_input=StringValueInput(value=value.value.value)
-                    ))
+                value_input.append(
+                    ComponentValueInput(
+                        id=value.id, value=ValueInput(string_value_input=StringValueInput(value=value.value.value))
+                    )
                 )
             elif type(value.value) is IntValue:
-                value_input.append(ComponentValueInput(
-                    id=value.id,
-                    value=ValueInput(
-                        int_value_input=IntValueInput(value=value.value.number)
-                    ))
+                value_input.append(
+                    ComponentValueInput(
+                        id=value.id, value=ValueInput(int_value_input=IntValueInput(value=value.value.number))
+                    )
                 )
             elif type(value.value) is DateTimeValue:
-                value_input.append(ComponentValueInput(
-                    id=value.id,
-                    value=ValueInput(
-                        date_time_value_input=DateTimeValueInput(date=value.value.date, time=value.value.time)
-                    ))
+                value_input.append(
+                    ComponentValueInput(
+                        id=value.id,
+                        value=ValueInput(
+                            date_time_value_input=DateTimeValueInput(date=value.value.date, time=value.value.time)
+                        ),
+                    )
                 )
             elif type(value.value) is StringLocaleValue:
-                value_input.append(ComponentValueInput(
-                    id=value.id,
-                    value=ValueInput(
-                        string_locale_value_input=StringLocaleValueInput(
-                            value=value.value.value,
-                            locale=value.value.locale
-                        )
-                    ))
+                value_input.append(
+                    ComponentValueInput(
+                        id=value.id,
+                        value=ValueInput(
+                            string_locale_value_input=StringLocaleValueInput(
+                                value=value.value.value, locale=value.value.locale
+                            )
+                        ),
+                    )
                 )
             elif type(value.value) is LinkValue:
-                value_input.append(ComponentValueInput(
-                    id=value.id,
-                    value=ValueInput(
-                        link_value_input=LinkValueInput(link=value.value.link)
-                    ))
+                value_input.append(
+                    ComponentValueInput(
+                        id=value.id, value=ValueInput(link_value_input=LinkValueInput(link=value.value.link))
+                    )
                 )
             elif type(value.value) is DoubleValue:
-                value_input.append(ComponentValueInput(
-                    id=value.id,
-                    value=ValueInput(
-                        double_value_input=DoubleValueInput(double=value.value.double)
-                    ))
+                value_input.append(
+                    ComponentValueInput(
+                        id=value.id, value=ValueInput(double_value_input=DoubleValueInput(double=value.value.double))
+                    )
                 )
         op = Operation(Mutation)
         ucp: ConceptProperty = op.update_concept_property(
-            form=ConceptPropertyUpdateInput(
-                property_id=cp.id,
-                is_main=cp.is_main,
-                value_input=value_input
-            )
+            form=ConceptPropertyUpdateInput(property_id=cp.id, is_main=cp.is_main, value_input=value_input)
         )
-        ucp.__fields__('id')
+        ucp.__fields__("id")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property
 
     def delete_concept_property(self, cp_id: str) -> bool:
         op = Operation(Mutation)
-        dcp = op.delete_concept_property(
-            id=cp_id
-        )
-        dcp.__fields__('is_success')
+        dcp = op.delete_concept_property(id=cp_id)
+        dcp.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_property.is_success
 
     def get_all_concept_types(
-        self, filter_settings: ConceptTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: ConceptTypeSorting = 'id'
+        self,
+        filter_settings: ConceptTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptTypeSorting = "id",
     ) -> Iterable[ConceptType]:
         current_step = 0
         while True:
             concept_types = self.get_concept_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_types) < 1:
                 break
             current_step += self.limit
-            for concept_type in concept_types:
-                yield concept_type
+            yield from concept_types
 
     def get_concept_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: ConceptTypeSorting = 'id'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptTypeSorting = "id",
     ) -> Sequence[ConceptType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptTypeFilterSettings()
 
         op = Operation(Query)
         pct: ConceptTypePagination = op.pagination_concept_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         pct.list_concept_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_type.list_concept_type
 
     def get_concept_types_by_name(self, name: str) -> Sequence[ConceptType]:
         op = Operation(Query)
-        ctp: ConceptTypePagination = op.pagination_concept_type(
-            filter_settings=ConceptTypeFilterSettings(
-                name=name
-            )
-        )
+        ctp: ConceptTypePagination = op.pagination_concept_type(filter_settings=ConceptTypeFilterSettings(name=name))
         ctp.list_concept_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_type.list_concept_type
 
     def get_concept_type_info(self, concept_type_id: str) -> ConceptType:
         op = Operation(Query)
-        ct = op.concept_type(
-            id=concept_type_id
-        )
+        ct = op.concept_type(id=concept_type_id)
         ct.__fields__(*self.concept_type_fields)
         lcpt = ct.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         lclt = ct.list_concept_link_type()
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.list_concept_link_property_type().__fields__(*self.concept_property_type_fields)
 
@@ -1239,103 +1368,108 @@
 
         concept_type_name = self._type_mapping.get_concept_type_name(concept_type_code)
         concept_types = self.get_concept_types_by_name(concept_type_name)
         for concept_type in concept_types:
             if concept_type.name == concept_type_name:
                 self._type_mapping.add_concept_type(concept_type_code, concept_type)
                 return concept_type
+        return None
 
     def get_all_concept_property_types(
-        self, filter_settings: ConceptPropertyTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: ConceptPropertyTypeSorting = 'name'
+        self,
+        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_property_types = self.get_concept_property_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_property_types) < 1:
                 break
             current_step += self.limit
-            for concept_property_type in concept_property_types:
-                yield concept_property_type
+            yield from concept_property_types
 
     def get_concept_property_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptPropertyTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: ConceptPropertyTypeSorting = 'name'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyTypeFilterSettings()
 
         op = Operation(Query)
         pcpt: ConceptPropertyTypePagination = op.pagination_concept_property_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pcpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_type.list_concept_property_type
 
     def get_concept_properties_types_by_name(
-            self, concept_type_id: str, prop_name: str
+        self, concept_type_id: str, prop_name: str
     ) -> Sequence[ConceptPropertyType]:
-
         op = Operation(Query)
         cptp: ConceptPropertyTypePagination = op.pagination_concept_property_type(
-            filter_settings=ConceptPropertyTypeFilterSettings(
-                name=prop_name,
-                concept_type_id=concept_type_id
-            )
+            filter_settings=ConceptPropertyTypeFilterSettings(name=prop_name, concept_type_id=concept_type_id)
         )
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_type.list_concept_property_type
 
     def get_all_concept_composite_property_types(
-        self, filter_settings: CompositePropertyTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: CompositePropertyTypeSorting = 'name'
+        self,
+        filter_settings: CompositePropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: CompositePropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_composite_property_types = self.get_concept_composite_property_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_composite_property_types) < 1:
                 break
             current_step += self.limit
-            for concept_composite_property_type in concept_composite_property_types:
-                yield concept_composite_property_type
+            yield from concept_composite_property_types
 
     def get_concept_composite_property_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: CompositePropertyTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: CompositePropertyTypeSorting = 'name'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: CompositePropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: CompositePropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = CompositePropertyTypeFilterSettings()
 
         op = Operation(Query)
         pccpt: ConceptPropertyTypePagination = op.pagination_composite_concept_property_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pccpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_concept_property_type.list_concept_property_type
@@ -1345,70 +1479,73 @@
     ) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_property_type(concept_type_code, property_type_code)
         if property_type:
             return property_type
 
         concept_type = self.get_concept_type(concept_type_code)
         if not concept_type:
-            raise Exception('Cannot get concept property type: no concept type id')
+            raise Exception("Cannot get concept property type: no concept type id")
 
         property_type_name = self._type_mapping.get_concept_property_type_name(concept_type_code, property_type_code)
         property_types = self.get_concept_properties_types_by_name(concept_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_property_type(concept_type_code, property_type_code, property_type)
                 return property_type
+        return None
 
     def get_all_concept_property_value_types(
-        self, filter_settings: ConceptPropertyValueTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: ConceptPropertyValueTypeSorting = 'id'
+        self,
+        filter_settings: ConceptPropertyValueTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptPropertyValueTypeSorting = "id",
     ) -> Iterable[ConceptPropertyValueType]:
         current_step = 0
         while True:
             concept_property_value_types = self.get_concept_property_value_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_property_value_types) < 1:
                 break
             current_step += self.limit
-            for concept_property_value_type in concept_property_value_types:
-                yield concept_property_value_type
+            yield from concept_property_value_types
 
     def get_concept_property_value_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptPropertyValueTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: ConceptPropertyValueTypeSorting = 'id'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptPropertyValueTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptPropertyValueTypeSorting = "id",
     ) -> Sequence[ConceptPropertyValueType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyValueTypeFilterSettings()
 
         op = Operation(Query)
         pcpvt: ConceptPropertyValueTypePagination = op.pagination_concept_property_value_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         pcpvt.list_concept_property_value_type().__fields__(*self.cpvt_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_value_type.list_concept_property_value_type
 
     def get_concept_property_value_types_by_name(
         self, prop_value_type_name: str, limit: int = 20, offset: int = 0
     ) -> Sequence[ConceptPropertyValueType]:
         op = Operation(Query)
         cpvtp: ConceptPropertyValueTypePagination = op.pagination_concept_property_value_type(
-            filter_settings=ConceptPropertyValueTypeFilterSettings(
-                name=prop_value_type_name
-            ),
+            filter_settings=ConceptPropertyValueTypeFilterSettings(name=prop_value_type_name),
             limit=limit,
-            offset=offset
+            offset=offset,
         )
         cpvtp.list_concept_property_value_type().__fields__(*self.cpvt_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_value_type.list_concept_property_value_type
 
     def get_concept_property_value_type(
@@ -1420,117 +1557,120 @@
 
         value_type_name = self._type_mapping.get_concept_property_value_type_name(concept_property_value_type_code)
         value_types = self.get_concept_property_value_types_by_name(value_type_name)
         for value_type in value_types:
             if value_type.name == value_type_name:
                 self._type_mapping.add_concept_property_value_type(concept_property_value_type_code, value_type)
                 return value_type
+        return None
 
     def get_all_concept_link_property_types(
-        self, filter_settings: ConceptPropertyTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: ConceptPropertyTypeSorting = 'name'
+        self,
+        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_link_property_types = self.get_link_property_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_link_property_types) < 1:
                 break
             current_step += self.limit
-            for concept_link_property_type in concept_link_property_types:
-                yield concept_link_property_type
+            yield from concept_link_property_types
 
     def get_link_property_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptPropertyTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: ConceptPropertyTypeSorting = 'name'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyTypeFilterSettings()
 
         op = Operation(Query)
         pclpt: ConceptPropertyTypePagination = op.pagination_concept_link_property_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pclpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_property_type.list_concept_property_type
 
     def get_link_properties_types_by_name(self, link_type_id: str, prop_name: str) -> Sequence[ConceptPropertyType]:
         op = Operation(Query)
         cptp: ConceptPropertyTypePagination = op.pagination_concept_link_property_type(
-            filter_settings=ConceptPropertyTypeFilterSettings(
-                name=prop_name,
-                concept_link_type_id=link_type_id
-            )
+            filter_settings=ConceptPropertyTypeFilterSettings(name=prop_name, concept_link_type_id=link_type_id)
         )
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_property_type.list_concept_property_type
 
     def get_all_concept_link_composite_property_types(
-        self, filter_settings: CompositePropertyTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: CompositePropertyTypeSorting = 'name'
+        self,
+        filter_settings: CompositePropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: CompositePropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_link_composite_property_types = self.get_link_composite_property_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_link_composite_property_types) < 1:
                 break
             current_step += self.limit
-            for concept_link_composite_property_type in concept_link_composite_property_types:
-                yield concept_link_composite_property_type
+            yield from concept_link_composite_property_types
 
     def get_link_composite_property_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: CompositePropertyTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: CompositePropertyTypeSorting = 'name'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: CompositePropertyTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: CompositePropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = CompositePropertyTypeFilterSettings()
 
         op = Operation(Query)
         pclpt: ConceptPropertyTypePagination = op.pagination_composite_link_property_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pclpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_link_property_type.list_concept_property_type
 
     def get_composite_link_properties_types_by_name(
         self, link_type_id: str, prop_name: str
     ) -> Sequence[ConceptPropertyType]:
         op = Operation(Query)
         cptp: ConceptPropertyTypePagination = op.pagination_composite_link_property_type(
-            filter_settings=CompositePropertyTypeFilterSettings(
-                name=prop_name,
-                link_type_id=link_type_id
-            )
+            filter_settings=CompositePropertyTypeFilterSettings(name=prop_name, link_type_id=link_type_id)
         )
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_link_property_type.list_concept_property_type
@@ -1544,14 +1684,15 @@
 
         property_type_name = self._type_mapping.get_concept_link_property_type_name(link_type_code, property_type_code)
         property_types = self.get_link_properties_types_by_name(link_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_link_property_type(link_type_code, property_type_code, property_type)
                 return property_type
+        return None
 
     def get_link_composite_property_type(
         self, link_type_code: str, link_type: ConceptLinkType, property_type_code: str
     ) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_link_composite_property_type(link_type_code, property_type_code)
         if property_type:
             return property_type
@@ -1562,98 +1703,104 @@
         property_types = self.get_composite_link_properties_types_by_name(link_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_link_composite_property_type(
                     link_type_code, property_type_code, property_type
                 )
                 return property_type
+        return None
 
     def add_property_by_id(
-        self, id: str, type_id: str, value: Any, is_main: bool, value_type: str,
-        perform_synchronously: Optional[bool] = None
+        self,
+        id: str,
+        type_id: str,
+        value: Any,
+        is_main: bool,
+        value_type: str,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
         op = Operation(Mutation)
         acp = op.add_concept_property(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptPropertyCreateInput(
                 concept_id=id,
                 property_type_id=type_id,
                 is_main=is_main,
-                value_input=[
-                    ComponentValueInput(
-                        value=get_map_helper(value_type).get_value_input(value)
-                    )
-                ]
-            )
+                value_input=[ComponentValueInput(value=get_map_helper(value_type).get_value_input(value))],
+            ),
         )
-        acp.__fields__('id')
+        acp.__fields__("id")
         acp.property_type().__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_property
 
     def add_property(
-        self, concept_id: str, concept_type_code: str, property_type_code: str, value: Any, is_main: bool = False,
-        perform_synchronously: Optional[bool] = None
+        self,
+        concept_id: str,
+        concept_type_code: str,
+        property_type_code: str,
+        value: Any,
+        is_main: bool = False,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
-
         property_type: ConceptPropertyType = self.get_concept_property_type(concept_type_code, property_type_code)
         if not property_type:
-            raise Exception('Cannot add property: no property type id')
+            raise Exception("Cannot add property: no property type id")
         if type(property_type.value_type) is CompositePropertyValueTemplate:
             prop = self.add_composite_property_by_id(
-                concept_id, property_type.id, value, is_main, property_type.value_type.component_value_types,
-                concept_type_code, property_type_code, perform_synchronously
+                concept_id,
+                property_type.id,
+                value,
+                is_main,
+                property_type.value_type.component_value_types,
+                concept_type_code,
+                property_type_code,
+                perform_synchronously,
             )
         else:
             prop = self.add_property_by_id(
                 concept_id, property_type.id, value, is_main, property_type.value_type.value_type, perform_synchronously
             )
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_property_fact(prop, self.get_concept(concept_id), value, property_type)
 
         return prop
 
     def add_link_property_by_id(
-        self, link_id: str, type_id: str, value: str, is_main: bool, value_type: str,
-        perform_synchronously: Optional[bool] = None
+        self,
+        link_id: str,
+        type_id: str,
+        value: str,
+        is_main: bool,
+        value_type: str,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
         op = Operation(Mutation)
 
         aclp = op.add_concept_link_property(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptLinkPropertyInput(
                 property_type_id=type_id,
                 link_id=link_id,
                 is_main=is_main,
-                value_input=[
-                    ComponentValueInput(
-                        value=get_map_helper(value_type).get_value_input(value)
-                    )
-                ]
-            )
+                value_input=[ComponentValueInput(value=get_map_helper(value_type).get_value_input(value))],
+            ),
         )
-        aclp.__fields__('id')
+        aclp.__fields__("id")
         aclp.property_type().__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link_property
 
-    def add_concept_link_property_type(
-        self, link_type_id: str, name: str, value_type_id: str
-    ) -> ConceptPropertyType:
-
+    def add_concept_link_property_type(self, link_type_id: str, name: str, value_type_id: str) -> ConceptPropertyType:
         op = Operation(Mutation)
 
         aclpt = op.add_concept_link_property_type(
             form=ConceptLinkPropertyTypeCreationInput(
                 link_type_id=link_type_id,
                 name=name,
                 value_type_id=value_type_id,
@@ -1664,15 +1811,14 @@
         res = op + res
 
         return res.add_concept_link_property_type
 
     def update_concept_link_property_type(
         self, link_property_type_id: str, name: str, value_type_id: str
     ) -> ConceptPropertyType:
-
         op = Operation(Mutation)
 
         acpt = op.update_concept_link_property_type(
             form=ConceptLinkPropertyTypeUpdateInput(
                 id=link_property_type_id,
                 name=name,
                 value_type_id=value_type_id,
@@ -1680,32 +1826,24 @@
         )
         acpt.__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_link_property_type
 
-    def delete_concept_link_property_type(
-        self, property_type_id: str
-    ) -> State:
-
+    def delete_concept_link_property_type(self, property_type_id: str) -> State:
         op = Operation(Mutation)
 
-        op.delete_concept_link_property_type(
-            id=property_type_id
-        )
+        op.delete_concept_link_property_type(id=property_type_id)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_link_property_type
 
-    def add_concept_property_type(
-        self, concept_type_id: str, name: str, value_type_id: str
-    ) -> ConceptPropertyType:
-
+    def add_concept_property_type(self, concept_type_id: str, name: str, value_type_id: str) -> ConceptPropertyType:
         op = Operation(Mutation)
 
         acpt = op.add_concept_property_type(
             form=ConceptPropertyTypeCreationInput(
                 concept_type_id=concept_type_id,
                 name=name,
                 value_type_id=value_type_id,
@@ -1713,168 +1851,185 @@
         )
         acpt.__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_property_type
 
-    def delete_concept_property_type(
-        self, property_type_id: str
-    ) -> State:
-
+    def delete_concept_property_type(self, property_type_id: str) -> State:
         op = Operation(Mutation)
 
-        op.delete_concept_property_type(
-            id=property_type_id
-        )
+        op.delete_concept_property_type(id=property_type_id)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_property_type
 
     def add_link_composite_property_by_id(
-        self, link_id: str, property_type_id: str, values: dict,
+        self,
+        link_id: str,
+        property_type_id: str,
+        values: dict,
         component_value_types: List[CompositePropertyValueType],
-        link_composite_property_code: str, link_code: str, is_main: bool, perform_synchronously: Optional[bool] = None
+        link_composite_property_code: str,
+        link_code: str,
+        is_main: bool,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         components_type_mapping: Dict[str, CompositePropertyValueType] = {}
         for relation in self._type_mapping.relations_types_mapping:
             if relation.old_relation_type == link_code:
                 component_values = relation.composite_properties[link_composite_property_code].component_values
                 components_type_mapping = self._get_components_mapping(component_values, component_value_types)
         value_input = self._get_value_input(values, components_type_mapping)
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
 
         op = Operation(Mutation)
         aclp = op.add_concept_link_property(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptLinkPropertyInput(
-                property_type_id=property_type_id,
-                link_id=link_id,
-                is_main=is_main,
-                value_input=value_input
-            )
+                property_type_id=property_type_id, link_id=link_id, is_main=is_main, value_input=value_input
+            ),
         )
-        aclp.__fields__('id')
+        aclp.__fields__("id")
         aclp.property_type().__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link_property
 
     def add_composite_property_by_id(
-        self, id: str, type_id: str, values: dict, is_main: bool,
-        component_value_types: List[CompositePropertyValueType], concept_type_code: str, property_type_code: str,
-        perform_synchronously: Optional[bool] = None
+        self,
+        id: str,
+        type_id: str,
+        values: dict,
+        is_main: bool,
+        component_value_types: List[CompositePropertyValueType],
+        concept_type_code: str,
+        property_type_code: str,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         concept_composite_properties = self._type_mapping.concepts_types_mapping[concept_type_code].composite_properties
         concept_component_values = concept_composite_properties[property_type_code].component_values
         components_type_mapping = self._get_components_mapping(concept_component_values, component_value_types)
         value_input = self._get_value_input(values, components_type_mapping)
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
 
         op = Operation(Mutation)
         acp = op.add_concept_property(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptPropertyCreateInput(
-                concept_id=id,
-                property_type_id=type_id,
-                is_main=is_main,
-                value_input=value_input
-            )
+                concept_id=id, property_type_id=type_id, is_main=is_main, value_input=value_input
+            ),
         )
-        acp.__fields__('id')
+        acp.__fields__("id")
         acp.property_type().__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_property
 
     def add_link_property(
-        self, link_id: str, link_type_code: str, link_type: ConceptLinkType, property_type_code: str, value: Any,
-        is_composite: Optional[bool] = False, is_main: bool = False, perform_synchronously: Optional[bool] = None
+        self,
+        link_id: str,
+        link_type_code: str,
+        link_type: ConceptLinkType,
+        property_type_code: str,
+        value: Any,
+        is_composite: Optional[bool] = False,
+        is_main: bool = False,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
-        property_type = self.get_link_composite_property_type(
-            link_type_code, link_type, property_type_code
-        ) if is_composite else self.get_link_property_type(link_type_code, link_type, property_type_code)
+        property_type = (
+            self.get_link_composite_property_type(link_type_code, link_type, property_type_code)
+            if is_composite
+            else self.get_link_property_type(link_type_code, link_type, property_type_code)
+        )
         if not property_type:
-            raise Exception('Cannot add property: no property type id')
+            raise Exception("Cannot add property: no property type id")
 
         if is_composite:
             link_property = self.add_link_composite_property_by_id(
-                link_id, property_type.id, value, property_type.value_type.component_value_types,
-                property_type_code, link_type_code, is_main, perform_synchronously
+                link_id,
+                property_type.id,
+                value,
+                property_type.value_type.component_value_types,
+                property_type_code,
+                link_type_code,
+                is_main,
+                perform_synchronously,
             )
         else:
             link_property = self.add_link_property_by_id(
-                link_id, property_type.id, value, is_main,
-                property_type.value_type.value_type, perform_synchronously=perform_synchronously
+                link_id,
+                property_type.id,
+                value,
+                is_main,
+                property_type.value_type.value_type,
+                perform_synchronously=perform_synchronously,
             )
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_property_fact(link_property, self.get_concept_link(link_id), value, property_type)
 
         return link_property
 
     def get_all_concept_link_types(
-        self, filter_settings: ConceptLinkTypeFilterSettings = None, direction: SortDirection = 'ascending',
-        sort_field: ConceptLinkTypeSorting = 'id'
+        self,
+        filter_settings: ConceptLinkTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptLinkTypeSorting = "id",
     ) -> Iterable[ConceptLinkType]:
         current_step = 0
         while True:
             concept_link_types = self.get_concept_link_types(
-                skip=current_step, take=self.limit, filter_settings=filter_settings,
-                direction=direction, sort_field=sort_field
+                skip=current_step,
+                take=self.limit,
+                filter_settings=filter_settings,
+                direction=direction,
+                sort_field=sort_field,
             )
             if len(concept_link_types) < 1:
                 break
             current_step += self.limit
-            for concept_link_type in concept_link_types:
-                yield concept_link_type
+            yield from concept_link_types
 
     def get_concept_link_types(
-        self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptLinkTypeFilterSettings = None,
-        direction: SortDirection = 'ascending', sort_field: ConceptLinkTypeSorting = 'id'
+        self,
+        skip: int = 0,
+        take: Optional[int] = None,
+        filter_settings: ConceptLinkTypeFilterSettings = None,
+        direction: SortDirection = "ascending",
+        sort_field: ConceptLinkTypeSorting = "id",
     ) -> Sequence[ConceptLinkType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptLinkTypeFilterSettings()
 
         op = Operation(Query)
         pclt: ConceptLinkTypePagination = op.pagination_concept_link_type(
-            direction=direction,
-            filter_settings=filter_settings,
-            limit=take,
-            offset=skip,
-            sort_field=sort_field
+            direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lclt = pclt.list_concept_link_type()
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.concept_from_type().__fields__(*self.concept_type_fields)
         lclt.concept_to_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_type.list_concept_link_type
 
     def get_concept_link_type_by_name(
         self, link_name: str, from_type_id: str, to_type_id: str, limit: int = 20
     ) -> Sequence[ConceptLinkType]:
-
         op = Operation(Query)
         pclt: ConceptLinkTypePagination = op.pagination_concept_link_type(
             filter_settings=ConceptLinkTypeFilterSettings(
-                name=link_name,
-                concept_from_type_id=from_type_id,
-                concept_to_type_id=to_type_id
+                name=link_name, concept_from_type_id=from_type_id, concept_to_type_id=to_type_id
             ),
-            limit=limit
+            limit=limit,
         )
         lclt = pclt.list_concept_link_type()
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.concept_from_type().__fields__(*self.concept_type_fields)
         lclt.concept_to_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
@@ -1891,89 +2046,81 @@
         concept_to_type = self.get_concept_type(concept_to_type_code)
         link_type_name = self._type_mapping.get_concept_link_type_name(link_type_code)
         link_types = self.get_concept_link_type_by_name(link_type_name, concept_from_type.id, concept_to_type.id)
         for link_type in link_types:
             if link_type.name == link_type_name:
                 self._type_mapping.add_concept_link_type(link_type_code, link_type)
                 return link_type
+        return None
 
     def add_relation_by_id(
         self, from_id: str, to_id: str, link_type_id: str, perform_synchronously: Optional[bool] = None
     ) -> ConceptLink:
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
         op = Operation(Mutation)
         acl = op.add_concept_link(
-            performance_control=PerformSynchronously(
-                perform_synchronously=perform_synchronously
-            ),
+            performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptLinkCreationMutationInput(
-                concept_from_id=from_id,
-                concept_to_id=to_id,
-                link_type_id=link_type_id
-            )
+                concept_from_id=from_id, concept_to_id=to_id, link_type_id=link_type_id
+            ),
         )
         acl.__fields__(*self.concept_link_fields)
         acl.concept_link_type.__fields__(*self.concept_property_type_fields)
         acl.concept_link_type.__fields__(*self.concept_link_type_fields_truncated)
         self._configure_output_concept_fields(acl.concept_from)
         self._configure_output_concept_fields(acl.concept_to)
 
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link
 
     def add_relation(
-        self, concept_from_id: str, concept_to_id: str, concept_from_type_code: str, concept_to_type_code: str,
-        type_code: str, perform_synchronously: Optional[bool] = None
+        self,
+        concept_from_id: str,
+        concept_to_id: str,
+        concept_from_type_code: str,
+        concept_to_type_code: str,
+        type_code: str,
+        perform_synchronously: Optional[bool] = None,
     ) -> ConceptLink:
-
         link_type = self.get_link_type(concept_from_type_code, concept_to_type_code, type_code)
         if not link_type:
-            raise Exception('Cannot add relation: no link type')
+            raise Exception("Cannot add relation: no link type")
         relation = self.add_relation_by_id(
             concept_from_id, concept_to_id, link_type.id, perform_synchronously=perform_synchronously
         )
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_fact(relation)
 
         return relation
 
     def delete_concept(self, concept_id: str) -> bool:
-
         op = Operation(Mutation)
-        dc: Concept = op.delete_concept(
-            id=concept_id
-        )
-        dc.__fields__('is_success')
+        dc: Concept = op.delete_concept(id=concept_id)
+        dc.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept.is_success
 
     def delete_concept_link(self, link_id: str) -> bool:
-
         op = Operation(Mutation)
-        dcl: ConceptLink = op.delete_concept_link(
-            id=link_id
-        )
-        dcl.__fields__('is_success')
+        dcl: ConceptLink = op.delete_concept_link(id=link_id)
+        dcl.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_link.is_success
 
     def delete_concept_link_property(self, link_property_id: str) -> bool:
-
         op = Operation(Mutation)
-        clp: ConceptProperty = op.delete_concept_link_property(
-            id=link_property_id
-        )
-        clp.__fields__('is_success')
+        clp: ConceptProperty = op.delete_concept_link_property(id=link_property_id)
+        clp.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_link_property.is_success
 
     def add_concept_markers(
         self, concept_id: str, markers: List[str], perform_synchronously: Optional[bool] = None
@@ -1988,59 +2135,52 @@
     ) -> Concept:
         c = self.get_concept(concept_id)
         return self.update_concept(c, markers=markers, perform_synchronously=perform_synchronously)
 
     def get_composite_concept(self, root_concept_id: str, composite_concept_type_id: str) -> CompositeConcept:
         op = Operation(Query)
         cc: CompositeConcept = op.composite_concept(
-            root_concept_id=root_concept_id,
-            composite_concept_type_id=composite_concept_type_id
+            root_concept_id=root_concept_id, composite_concept_type_id=composite_concept_type_id
         )
         self._configure_output_concept_fields(
-            cc.root_concept, with_aliases=False, with_link_properties=False,
-            with_links=False, with_properties=False
+            cc.root_concept, with_aliases=False, with_link_properties=False, with_links=False, with_properties=False
         )
         lwt = cc.composite_concept_type().list_widget_type()
         lwt.__fields__(*self.composite_concept_widget_type)
         lwt.columns_info.__fields__(*self.composite_concept_widget_type_columns_info)
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.composite_concept
 
     def get_single_widget(
-        self, root_concept_id: str, composite_concept_type_id: str, widget_type_id: str,
-        limit: int = 20, offset: int = 0
+        self,
+        root_concept_id: str,
+        composite_concept_type_id: str,
+        widget_type_id: str,
+        limit: int = 20,
+        offset: int = 0,
     ) -> CompositeConceptWidgetRowPagination:
-
         op = Operation(Query)
         cc: CompositeConcept = op.composite_concept(
-            root_concept_id=root_concept_id,
-            composite_concept_type_id=composite_concept_type_id
+            root_concept_id=root_concept_id, composite_concept_type_id=composite_concept_type_id
         )
         psw: CompositeConceptWidgetRowPagination = cc.paginate_single_widget(
-            widget_type_id=widget_type_id,
-            limit=limit,
-            offset=offset
+            widget_type_id=widget_type_id, limit=limit, offset=offset
         )
-        psw.__fields__('total')
+        psw.__fields__("total")
         self._configure_output_value_fields(psw.rows)
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.composite_concept.paginate_single_widget
 
     def add_concept_fact(self, concept_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        op.add_concept_fact(
-            id=concept_id,
-            fact=FactInput(
-                document_id=document_id
-            )
-        )
+        op.add_concept_fact(id=concept_id, fact=FactInput(document_id=document_id))
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_fact
 
     def delete_concept_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
         op.delete_concept_fact(
@@ -2048,20 +2188,15 @@
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_fact
 
     def add_concept_property_fact(self, property_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        op.add_concept_property_fact(
-            id=property_id,
-            fact=FactInput(
-                document_id=document_id
-            )
-        )
+        op.add_concept_property_fact(id=property_id, fact=FactInput(document_id=document_id))
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_property_fact
 
     def delete_concept_property_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
         op.delete_concept_property_fact(
@@ -2069,20 +2204,15 @@
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_property_fact
 
     def add_concept_link_fact(self, link_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        op.add_concept_link_fact(
-            id=link_id,
-            fact=FactInput(
-                document_id=document_id
-            )
-        )
+        op.add_concept_link_fact(id=link_id, fact=FactInput(document_id=document_id))
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_link_fact
 
     def delete_concept_link_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
         op.delete_concept_link_fact(
@@ -2090,223 +2220,238 @@
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_link_fact
 
     def add_concept_link_property_fact(self, link_property_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        op.add_concept_link_property_fact(
-            id=link_property_id,
-            fact=FactInput(
-                document_id=document_id
-            )
-        )
+        op.add_concept_link_property_fact(id=link_property_id, fact=FactInput(document_id=document_id))
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_link_property_fact
 
     def delete_concept_link_property_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
         op.delete_concept_link_property_fact(
             id=fact_id,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_link_property_fact
 
+    def merge_concepts(self, c_main_id: str, c_merged_id: str) -> Concept:
+        op = Operation(Mutation)
+        mc: Concept = op.merge_concepts(
+            form=ConceptMergeInput(main_concept_id=c_main_id, merged_concept_id=c_merged_id)
+        )
+        self._configure_output_concept_fields(mc)
+        res = self._gql_client.execute(op)
+        res = op + res
+
+        return res.merge_concepts
+
+    def unmerge_concepts(self, c_main_id: str, c_merged_id: List[str]) -> Concept:
+        op = Operation(Mutation)
+        umc: Concept = op.unmerge_concepts(
+            form=ConceptUnmergeInput(main_concept_id=c_main_id, merged_concept_id=c_merged_id)
+        )
+        self._configure_output_concept_fields(umc)
+        res = self._gql_client.execute(op)
+        res = op + res
+
+        return res.unmerge_concepts
+
     # region Crawlers methods
 
     def get_crawler_start_urls(self, take: Optional[int] = None) -> Sequence[Crawler]:
         take = self.get_take_value(take)
         op = Operation(CrQuery)
-        pc: CrawlerPagination = op.pagination_crawler(
-            limit=take
-        )
+        pc: CrawlerPagination = op.pagination_crawler(limit=take)
         lc = pc.list_crawler()
-        lc.__fields__('start_urls')
+        lc.__fields__("start_urls")
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_crawler.list_crawler
 
     # endregion
 
     # region Utils methods
 
     @check_utils_gql_client
     def create_or_get_concept_by_name(
-        self, name: str, type_id: str, notes: str = None, take_first_result: bool = False,
-        with_properties=False, with_links=False, with_link_properties=False
+        self,
+        name: str,
+        type_id: str,
+        notes: str = None,
+        take_first_result: bool = False,
+        with_properties=False,
+        with_links=False,
+        with_link_properties=False,
     ) -> Concept:
-
         if type_id:
             concept_filter_settings: ConceptFilterSettings = uas.ConceptFilterSettings(
-                exact_name=name,
-                concept_type_ids=[type_id]
+                exact_name=name, concept_type_ids=[type_id]
             )
         else:
-            concept_filter_settings: ConceptFilterSettings = uas.ConceptFilterSettings(
-                exact_name=name
-            )
+            concept_filter_settings: ConceptFilterSettings = uas.ConceptFilterSettings(exact_name=name)
 
         op = Operation(uas.Mutation)
         goac = op.get_or_add_concept(
             filter_settings=concept_filter_settings,
-            form=uas.ConceptMutationInput(
-                name=name,
-                concept_type_id=type_id,
-                notes=notes
-            ),
-            take_first_result=take_first_result
+            form=uas.ConceptMutationInput(name=name, concept_type_id=type_id, notes=notes),
+            take_first_result=take_first_result,
         )
         self._configure_output_concept_fields(
-            goac, with_properties=with_properties, with_links=with_links,
-            with_link_properties=with_link_properties
+            goac, with_properties=with_properties, with_links=with_links, with_link_properties=with_link_properties
         )
 
         res = self._utils_gql_client.execute(op)
         res = op + res  # type: uas.Mutation
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.get_or_add_concept)
 
         return res.get_or_add_concept
 
     @check_utils_gql_client
     def get_tdm(self, doc_id: str):
         op = Operation(uas.Query)
-        op.tdm(
-            id=doc_id
-        )
+        op.tdm(id=doc_id)
         res = self._utils_gql_client.execute(op)
         res = op + res
         return res
 
     # endregion
 
     # region tcontroller methods
 
     def get_pipeline_configs(
-        self, with_transforms: bool = True, filter_settings: tc.PipelineConfigFilter = None,
-        limit: Optional[int] = None, offset: Optional[int] = None, sort_by: tc.PipelineConfigSort = 'id',
-        sort_direction: tc.SortDirection = 'ascending'
+        self,
+        with_transforms: bool = True,
+        filter_settings: tc.PipelineConfigFilter = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        sort_by: tc.PipelineConfigSort = "id",
+        sort_direction: tc.SortDirection = "ascending",
     ) -> tc.PipelineConfigList:
         op = Operation(tc.Query)
         pcl: tc.PipelineConfigList = op.pipeline_configs(
-            filter=filter_settings,
-            limit=limit,
-            offset=offset,
-            sort_by=sort_by,
-            sort_direction=sort_direction
+            filter=filter_settings, limit=limit, offset=offset, sort_by=sort_by, sort_direction=sort_direction
         )
         pc = pcl.pipeline_configs()
         pc.__fields__(*self.pipeline_config_fields)
         if with_transforms:
-            pc.transforms().__fields__('id')
-            pc.transforms().__fields__('params')
+            pc.transforms().__fields__("id")
+            pc.transforms().__fields__("params")
         res = self._gql_client.execute(op)
         res = op + res
         return res.pipeline_configs
 
     def get_pipeline_topics(
-        self, filter_settings: tc.KafkaTopicFilter = None,
-        limit: Optional[int] = None, offset: Optional[int] = None, sort_by: tc.KafkaTopicSort = 'topic',
-        sort_direction: tc.SortDirection = 'ascending'
+        self,
+        filter_settings: tc.KafkaTopicFilter = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        sort_by: tc.KafkaTopicSort = "topic",
+        sort_direction: tc.SortDirection = "ascending",
     ) -> tc.KafkaTopicList:
         op = Operation(tc.Query)
         ktl: tc.KafkaTopicList = op.kafka_topics(
-            filter=filter_settings,
-            limit=limit,
-            offset=offset,
-            sort_by=sort_by,
-            sort_direction=sort_direction
+            filter=filter_settings, limit=limit, offset=offset, sort_by=sort_by, sort_direction=sort_direction
         )
         self._configure_pipeline_topic_fields(ktl.topics())
         res = self._gql_client.execute(op)
         res = op + res
         return res.kafka_topics
 
     def upsert_pipeline_topic(self, topic_id: str, config_id: str, stopped: bool) -> tc.KafkaTopic:
         op = Operation(tc.Mutation)
         kt: tc.KafkaTopic = op.put_kafka_topic(
-            topic=topic_id,
-            pipeline=tc.PipelineSetupInput(
-                pipeline_config=config_id
-            ),
-            stopped=stopped
+            topic=topic_id, pipeline=tc.PipelineSetupInput(pipeline_config=config_id), stopped=stopped
         )
         self._configure_pipeline_topic_fields(kt)
         res = self._gql_client.execute(op)
         res = op + res
         return res.put_kafka_topic
 
     def get_failed_messages_from_topic(
-        self, topic_id: str, filter_settings: tc.MessageFilter = None, offset: Optional[int] = None,
-        limit: Optional[int] = None, sort_by: tc.MessageSort = 'timestamp',
-        sort_direction: tc.SortDirection = 'descending'
+        self,
+        topic_id: str,
+        filter_settings: tc.MessageFilter = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+        sort_by: tc.MessageSort = "timestamp",
+        sort_direction: tc.SortDirection = "descending",
     ) -> tc.FailedMessageList:
         op = Operation(tc.Query)
         fm: tc.FailedMessageList = op.failed_messages(
             topic=topic_id,
             filter=filter_settings,
             offset=offset,
             limit=limit,
             sort_by=sort_by,
-            sort_direction=sort_direction
+            sort_direction=sort_direction,
         )
         fm.messages().id()
         fm.messages().info().error().description()
         fm.messages().info().message()
         res = self._gql_client.execute(op)
         res = op + res
         return res.failed_messages
 
     def get_ok_messages_from_topic(
-        self, topic_id: str, filter_settings: tc.MessageFilter = None, offset: Optional[int] = None,
-        limit: Optional[int] = None, sort_by: tc.MessageSort = 'timestamp',
-        sort_direction: tc.SortDirection = 'descending'
+        self,
+        topic_id: str,
+        filter_settings: tc.MessageFilter = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+        sort_by: tc.MessageSort = "timestamp",
+        sort_direction: tc.SortDirection = "descending",
     ) -> tc.CompletedOkMessageList:
         op = Operation(tc.Query)
         om: tc.CompletedOkMessageList = op.completed_ok_messages(
             topic=topic_id,
             filter=filter_settings,
             offset=offset,
             limit=limit,
             sort_by=sort_by,
-            sort_direction=sort_direction
+            sort_direction=sort_direction,
         )
         om.messages().id()
         om.messages().info().message()
         res = self._gql_client.execute(op)
         res = op + res
         return res.completed_ok_messages
 
     def get_active_messages_from_topic(
-        self, topic_id: str, filter_settings: tc.MessageFilter = None, offset: Optional[int] = None,
-        limit: Optional[int] = None, sort_by: tc.MessageSort = 'timestamp',
-        sort_direction: tc.SortDirection = 'descending'
+        self,
+        topic_id: str,
+        filter_settings: tc.MessageFilter = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+        sort_by: tc.MessageSort = "timestamp",
+        sort_direction: tc.SortDirection = "descending",
     ) -> tc.CompletedOkMessageList:
         op = Operation(tc.Query)
         am: tc.CompletedOkMessageList = op.active_messages(
             topic=topic_id,
             filter=filter_settings,
             offset=offset,
             limit=limit,
             sort_by=sort_by,
-            sort_direction=sort_direction
+            sort_direction=sort_direction,
         )
         am.messages().id()
         am.messages().info().message()
         res = self._gql_client.execute(op)
         res = op + res
         return res.active_messages
 
     def retry_failed_in_topic(self, topic_id: str) -> int:
         op = Operation(tc.Mutation)
-        op.retry_failed_in_topic(
-            topic=topic_id
-        )
+        op.retry_failed_in_topic(topic=topic_id)
         res = self._gql_client.execute(op)
         res = op + res
         return res.retry_failed_in_topic
 
     # endregion
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/common/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import re
 import os
+import re
 
 from transliterate import translit
 
-
 valid_character_pattern = re.compile("[^a-zA-Z 0-9]+")
 space_pattern = re.compile("[ ]+")
 
 
-def perform_transliteration(text_string: str, language_code: str = 'ru', _reversed: bool = True) -> str:
+def perform_transliteration(text_string: str, language_code: str = "ru", _reversed: bool = True) -> str:
     transliterated_text = translit(text_string, language_code=language_code, reversed=_reversed)
-    return space_pattern.sub(
-        '_', valid_character_pattern.sub('', transliterated_text).strip()
-    ).lower()
+    return space_pattern.sub("_", valid_character_pattern.sub("", transliterated_text).strip()).lower()
 
 
 def generate_file(input_data: bytes, file_path: str) -> None:
     directory_path = os.path.dirname(file_path)
     if directory_path and not os.path.exists(directory_path):
         os.makedirs(directory_path)
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
-
 from dataclasses import dataclass, field
+
 from marshmallow import EXCLUDE
 
-from ptal_api.schema.api_schema import ConceptType, ConceptLinkType, ConceptPropertyType, ConceptPropertyValueType
+from ptal_api.schema.api_schema import ConceptLinkType, ConceptPropertyType, ConceptPropertyValueType, ConceptType
 
 
 @dataclass
 class MappedCompositePropertyType:
     name: str
     component_values: typing.Dict[str, str] = field(
         default_factory=dict
@@ -50,43 +50,43 @@
     old_relation_type: typing.Optional[str] = field(default=None)
     new_relation_type: typing.Optional[str] = field(default=None)
 
 
 @dataclass
 class CacheKeeper:
     concept_type_cache: typing.Dict[str, ConceptType] = field(
-        metadata=dict(marshmallow_field=ConceptType), default_factory=dict
+        metadata={"marshmallow_field": ConceptType}, default_factory=dict
     )  # Dict[concept_type_code, concept_type]
     concept_link_type_cache: typing.Dict[str, ConceptLinkType] = field(
-        metadata=dict(marshmallow_field=ConceptLinkType), default_factory=dict
+        metadata={"marshmallow_field": ConceptLinkType}, default_factory=dict
     )  # Dict[concept_link_type_code, concept_link_type]
     concept_property_value_type_cache: typing.Dict[str, ConceptPropertyValueType] = field(
-        metadata=dict(marshmallow_field=ConceptPropertyValueType), default_factory=dict
+        metadata={"marshmallow_field": ConceptPropertyValueType}, default_factory=dict
     )  # Dict[concept_property_value_type_code, concept_property_value_type]
     concept_property_type_cache: typing.Dict[typing.Tuple[str, str], ConceptPropertyType] = field(
-        metadata=dict(marshmallow_field=ConceptPropertyType), default_factory=dict
+        metadata={"marshmallow_field": ConceptPropertyType}, default_factory=dict
     )  # Dict[(concept_type_code, concept_property_type_code), concept_property_type]
     concept_composite_property_type_cache: typing.Dict[typing.Tuple[str, str], ConceptPropertyType] = field(
-        metadata=dict(marshmallow_field=ConceptPropertyType), default_factory=dict
+        metadata={"marshmallow_field": ConceptPropertyType}, default_factory=dict
     )  # Dict[(concept_type_code, concept_composite_property_type_code), concept_property_type]
     concept_link_property_type_cache: typing.Dict[typing.Tuple[str, str], ConceptPropertyType] = field(
-        metadata=dict(marshmallow_field=ConceptPropertyType), default_factory=dict
+        metadata={"marshmallow_field": ConceptPropertyType}, default_factory=dict
     )  # Dict[(concept_link_type_code, concept_link_property_type_code), concept_property_type]
     concept_link_composite_property_type_cache: typing.Dict[typing.Tuple[str, str], ConceptPropertyType] = field(
-        metadata=dict(marshmallow_field=ConceptPropertyType), default_factory=dict
+        metadata={"marshmallow_field": ConceptPropertyType}, default_factory=dict
     )  # Dict[(concept_link_type_code, concept_link_composite_property_type_code), concept_property_type]
 
     def get_concept_type(self, concept_type_code: str) -> typing.Optional[ConceptType]:
         return self.concept_type_cache.get(concept_type_code, None)
 
     def get_concept_link_type(self, concept_link_type_code: str) -> typing.Optional[ConceptLinkType]:
         return self.concept_link_type_cache.get(concept_link_type_code, None)
 
     def get_concept_property_value_type(
-            self, concept_property_value_type_code: str
+        self, concept_property_value_type_code: str
     ) -> typing.Optional[ConceptPropertyValueType]:
         return self.concept_property_value_type_cache.get(concept_property_value_type_code, None)
 
     def get_concept_property_type(
         self, concept_type_code: str, property_type_code: str
     ) -> typing.Optional[ConceptPropertyType]:
         type_code_key = (concept_type_code, property_type_code)
@@ -151,72 +151,82 @@
     concepts_types_mapping: typing.Dict[str, MappedConceptType] = field(default_factory=dict)
     relations_types_mapping: typing.List[MappedConceptLinkType] = field(default_factory=list)
     value_types_mapping: typing.Dict[str, str] = field(default_factory=dict)
 
     def get_concept_type_name(self, concept_type_code: str) -> typing.Optional[str]:
         if concept_type_code in self.concepts_types_mapping:
             return self.concepts_types_mapping.get(concept_type_code).name
+        return None
 
     def get_concept_property_type_name(self, concept_type_code: str, property_type_code: str) -> typing.Optional[str]:
         if concept_type_code in self.concepts_types_mapping:
             mapped_concept_type = self.concepts_types_mapping.get(concept_type_code)
             return mapped_concept_type.properties.get(property_type_code, None)
+        return None
 
     def get_concept_property_value_type_name(self, concept_property_value_type_code: str) -> typing.Optional[str]:
         return self.value_types_mapping.get(concept_property_value_type_code, None)
 
     def get_concept_link_type_name(self, concept_link_type_code: str) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 return relation_type_mapping.new_relation_type
+        return None
 
     def get_concept_link_property_type_name(
         self, concept_link_type_code: str, property_type_code: str
     ) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 return relation_type_mapping.properties.get(property_type_code, None)
+        return None
 
     def get_concept_composite_property_type_name(
         self, concept_type_code: str, composite_property_type_code: str
     ) -> typing.Optional[str]:
         if concept_type_code in self.concepts_types_mapping:
             mapped_concept_type = self.concepts_types_mapping.get(concept_type_code)
             if composite_property_type_code in mapped_concept_type.composite_properties:
                 return mapped_concept_type.composite_properties.get(composite_property_type_code).name
+            return None
+        return None
 
     def get_concept_composite_property_component_value_type_name(
         self, concept_type_code: str, composite_property_type_code: str, component_value_type_code: str
     ) -> typing.Optional[str]:
         if concept_type_code in self.concepts_types_mapping:
             mapped_concept_type = self.concepts_types_mapping.get(concept_type_code)
             if composite_property_type_code in mapped_concept_type.composite_properties:
                 mapped_composite_property = mapped_concept_type.composite_properties.get(composite_property_type_code)
                 return mapped_composite_property.component_values.get(component_value_type_code, None)
+            return None
+        return None
 
     def get_concept_link_composite_property_type_name(
         self, concept_link_type_code: str, composite_property_type_code: str
     ) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 if composite_property_type_code in relation_type_mapping.composite_properties:
                     return relation_type_mapping.composite_properties.get(composite_property_type_code).name
                 return None
+        return None
 
     def get_concept_link_composite_property_component_value_type_name(
         self, concept_link_type_code: str, composite_property_type_code: str, component_value_type_code: str
     ) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 if composite_property_type_code in relation_type_mapping.composite_properties:
                     mapped_composite_property = relation_type_mapping.composite_properties.get(
                         composite_property_type_code
                     )
                     return mapped_composite_property.component_values.get(component_value_type_code, None)
                 return None
+        return None
 
     def add_mapped_concept_type(self, concept_type_code: str, mapped_concept_type: MappedConceptType) -> None:
         self.concepts_types_mapping[concept_type_code] = mapped_concept_type
 
     def add_mapped_concept_link_type(self, mapped_concept_link_type: MappedConceptLinkType) -> None:
         self.relations_types_mapping.append(mapped_concept_link_type)
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import typing
-
 from dataclasses import dataclass, field
 
 
 @dataclass
 class DefaultTypeCodeStorage:
-    concept_type_code: str = field(default='concept_code')
-    concept_link_type_code: str = field(default='concept_link_code')
-    property_type_code: str = field(default='property_code')
-    composite_property_type_code: str = field(default='composite_property_code')
-    composite_property_component_value_type_code: str = field(default='component_value_code')
-    concept_property_value_type_code: str = field(default='property_value_code')
+    concept_type_code: str = field(default="concept_code")
+    concept_link_type_code: str = field(default="concept_link_code")
+    property_type_code: str = field(default="property_code")
+    composite_property_type_code: str = field(default="composite_property_code")
+    composite_property_component_value_type_code: str = field(default="component_value_code")
+    concept_property_value_type_code: str = field(default="property_value_code")
 
 
 @dataclass
 class FileGenerationSettings:
-    default_file_path: str = field(default='./type_mapping/type_mapping.json')
+    default_file_path: str = field(default="./type_mapping/type_mapping.json")
     indent: int = field(default=4)
     sort_keys: bool = field(default=True)
     generated_fields: typing.Set[str] = field(
-        default_factory=lambda: {'concepts_types_mapping', 'relations_types_mapping', 'value_types_mapping'}
+        default_factory=lambda: {"concepts_types_mapping", "relations_types_mapping", "value_types_mapping"}
     )
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
-
 from dataclasses import dataclass, field
+
 from marshmallow import EXCLUDE, pre_load
 
 
 @dataclass
 class CustomTypeCodeStorage:
     concept_type_codes: typing.Dict[str, str] = field(
         default_factory=dict
@@ -49,15 +49,16 @@
     def get_concept_link_type_code(
         self, concept_from_type_name: str, concept_to_type_name: str, concept_link_type_name: str
     ) -> typing.Optional[str]:
         if concept_link_type_name in self.concept_link_type_codes:
             for item in self.concept_link_type_codes[concept_link_type_name]:
                 if item[0] == concept_from_type_name and item[1] == concept_to_type_name:
                     return item[2]
+        return None
 
     @pre_load
-    def exclude_null_value_items(self, input_data: dict, **kwargs) -> dict:
+    def exclude_null_value_items(self, input_data: dict, **_) -> dict:
         return {key: value for key, value in input_data.items() if value is not None}
 
     class Meta:
         ordered = True
         unknown = EXCLUDE
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.11.5/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from collections import Counter
 from typing import Dict, List, Optional, Tuple, Union
 
 import marshmallow_dataclass
-import ruamel.yaml as yaml
+from ruamel import yaml
 
 from ptal_api.core.type_mapper.data_model.custom_data_model import CustomTypeCodeStorage
 
 
 class CustomDataHandler:
     def __init__(self, logger: logging.Logger):
         self._logger = logger
@@ -17,30 +17,34 @@
         custom_concept_link_type_codes: Dict[str, List[Tuple[str, str, str]]]
     ) -> Dict[Tuple[str, str, str], str]:
         return {
             (key, item[0], item[1]): item[2] for key, value in custom_concept_link_type_codes.items() for item in value
         }
 
     def get_custom_name_code_mapping(self, file_path: str) -> CustomTypeCodeStorage:
-        with open(file_path, "r", encoding="utf-8") as file:
+        with open(file_path, encoding="utf-8") as file:
             name_code_mapping = yaml.safe_load(file)
             if name_code_mapping:
                 self._verify_custom_name_code_mapping(name_code_mapping)
                 return marshmallow_dataclass.class_schema(CustomTypeCodeStorage)().load(name_code_mapping)
             return CustomTypeCodeStorage()
 
     def _verify_custom_name_code_mapping(
         self, name_code_mapping: Dict[str, Optional[Dict[str, Union[str, List[Tuple[str, str, str]]]]]]
     ) -> None:
         has_duplicate_codes = False
         for object_type, object_mapping in name_code_mapping.items():
             if not object_mapping:
                 continue
-            elif object_type == 'concept_link_type_codes':
-                object_mapping = self.unite_all_concept_link_mapping(object_mapping)
-            most_common_code, most_common_count = Counter(object_mapping.values()).most_common(n=1)[0]
+            if object_type == "concept_link_type_codes":
+                mod_object_mapping = self.unite_all_concept_link_mapping(object_mapping)
+            else:
+                mod_object_mapping = object_mapping
+            most_common_code, most_common_count = Counter(mod_object_mapping.values()).most_common(n=1)[0]
             if most_common_count > 1:
-                self._logger.error(f"The key \"{object_type}\" in custom name-code mapping has {most_common_count}"
-                                   f" type codes named \"{most_common_code}\". Use unique type codes")
+                self._logger.error(
+                    f'The key "{object_type}" in custom name-code mapping has {most_common_count}'
+                    f' type codes named "{most_common_code}". Use unique type codes'
+                )
                 has_duplicate_codes = True
         if has_duplicate_codes:
-            raise Exception('Invalid custom name-code mapping')
+            raise Exception("Invalid custom name-code mapping")
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 from ptal_api.core.type_mapper.data_model.base_data_model import TypeMapping
 from ptal_api.core.type_mapper.data_model.config_data_model import FileGenerationSettings
 
 
 class FileGenerator:
     def __init__(self, file_generation_settings: Optional[FileGenerationSettings], logger: logging.Logger):
         self._logger = logger
-        self._file_generation_settings = file_generation_settings if file_generation_settings \
-            else FileGenerationSettings()
+        self._file_generation_settings = (
+            file_generation_settings if file_generation_settings else FileGenerationSettings()
+        )
 
     def generate_file(self, type_mapping: TypeMapping, file_path: str) -> None:
         try:
-            json_string = marshmallow_dataclass.class_schema(TypeMapping)(
-                only=self._file_generation_settings.generated_fields
-            ).dumps(
-                obj=type_mapping,
-                indent=self._file_generation_settings.indent,
-                sort_keys=self._file_generation_settings.sort_keys,
-                ensure_ascii=False
-            ).encode("utf-8")
+            json_string = (
+                marshmallow_dataclass.class_schema(TypeMapping)(only=self._file_generation_settings.generated_fields)
+                .dumps(
+                    obj=type_mapping,
+                    indent=self._file_generation_settings.indent,
+                    sort_keys=self._file_generation_settings.sort_keys,
+                    ensure_ascii=False,
+                )
+                .encode("utf-8")
+            )
 
             generate_file(json_string, file_path)
             self._logger.debug(f"Generated file based on type mapping: {file_path}")
         except Exception as ex:
-            self._logger.info(f"Failed to generate a file \"{file_path}\" based on type mapping")
+            self._logger.info(f'Failed to generate a file "{file_path}" based on type mapping')
             self._logger.exception(ex)
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,71 +9,79 @@
     @staticmethod
     def _generate_concept_link_name(
         concept_from_type_name: str, concept_link_type_name: str, concept_to_type_name: str
     ) -> str:
         return f"{concept_from_type_name} {concept_link_type_name} {concept_to_type_name}"
 
     def create_transformed_object_type_name(
-        self, object_name: str, default_name: str, cache_names: Dict[str, str],
-        *custom_object_type_code_dicts: Dict[str, str]
+        self,
+        object_name: str,
+        default_name: str,
+        cache_names: Dict[str, str],
+        *custom_object_type_code_dicts: Dict[str, str],
     ) -> Tuple[str, Dict[str, str]]:
         for custom_object_type_code_dict in custom_object_type_code_dicts:
             if object_name in custom_object_type_code_dict:
                 return custom_object_type_code_dict[object_name], cache_names
         return self._transform_object_type_name(
-            object_name=object_name,
-            default_name=default_name,
-            cache_names=cache_names
+            object_name=object_name, default_name=default_name, cache_names=cache_names
         )
 
     def create_transformed_concept_link_type_name(
-        self, concept_link_type_name: str, default_concept_link_type_name: str, concept_from_type_name: str,
-        concept_to_type_name: str, transformed_concept_from_type_name: str, transformed_concept_to_type_name: str,
-        link_cache_names: Dict[str, str], custom_type_code_storage: CustomTypeCodeStorage
+        self,
+        concept_link_type_name: str,
+        default_concept_link_type_name: str,
+        concept_from_type_name: str,
+        concept_to_type_name: str,
+        transformed_concept_from_type_name: str,
+        transformed_concept_to_type_name: str,
+        link_cache_names: Dict[str, str],
+        custom_type_code_storage: CustomTypeCodeStorage,
     ) -> Tuple[str, Dict[str, str]]:
         transformed_concept_link_type_name = custom_type_code_storage.get_concept_link_type_code(
             concept_from_type_name, concept_to_type_name, concept_link_type_name
         )
         if transformed_concept_link_type_name:
             return transformed_concept_link_type_name, link_cache_names
         return self._transform_object_type_name(
             object_name=self._generate_concept_link_name(
-                transformed_concept_from_type_name, concept_link_type_name,
-                transformed_concept_to_type_name
+                transformed_concept_from_type_name, concept_link_type_name, transformed_concept_to_type_name
             ),
             cache_names=link_cache_names,
-            default_name=default_concept_link_type_name
+            default_name=default_concept_link_type_name,
         )
 
     def get_transformed_concept_type_name(
-        self, concept_type_name: str, default_concept_name: str, concept_type_id: str, type_mapping: TypeMapping,
-        custom_type_code_storage: CustomTypeCodeStorage, index_suffix: int = 1
+        self,
+        concept_type_name: str,
+        default_concept_name: str,
+        concept_type_id: str,
+        type_mapping: TypeMapping,
+        custom_type_code_storage: CustomTypeCodeStorage,
+        index_suffix: int = 1,
     ) -> Optional[str]:
         custom_concept_type_codes = custom_type_code_storage.concept_type_codes
         if concept_type_name in custom_concept_type_codes:
             return custom_concept_type_codes[concept_type_name]
 
         transformed_concept_name, _concept_cache_names = self._transform_object_type_name(
-            object_name=concept_type_name,
-            cache_names={},
-            default_name=default_concept_name,
-            index_suffix=index_suffix
+            object_name=concept_type_name, cache_names={}, default_name=default_concept_name, index_suffix=index_suffix
         )
 
         if transformed_concept_name not in type_mapping.concepts_types_mapping:
             return None
-        elif concept_type_id != type_mapping.concepts_types_mapping[transformed_concept_name].id:
+        if concept_type_id != type_mapping.concepts_types_mapping[transformed_concept_name].id:
             index_suffix += 1
             return self.get_transformed_concept_type_name(
                 concept_type_name=concept_type_name,
                 default_concept_name=default_concept_name,
                 concept_type_id=concept_type_id,
                 type_mapping=type_mapping,
                 custom_type_code_storage=custom_type_code_storage,
-                index_suffix=index_suffix
+                index_suffix=index_suffix,
             )
         return transformed_concept_name
 
     def _transform_object_type_name(
         self, object_name: str, default_name: str, cache_names: Dict[str, str], index_suffix: int = 1
     ) -> Tuple[str, Dict[str, str]]:
         _cache_names = cache_names.copy()
@@ -86,14 +94,11 @@
             transliterated_name += f"_{index_suffix}"
 
         if transliterated_name not in _cache_names:
             _cache_names[transliterated_name] = object_name
         elif object_name != _cache_names[transliterated_name]:
             index_suffix += 1
             return self._transform_object_type_name(
-                object_name=object_name,
-                cache_names=_cache_names,
-                default_name=default_name,
-                index_suffix=index_suffix
+                object_name=object_name, cache_names=_cache_names, default_name=default_name, index_suffix=index_suffix
             )
 
         return transliterated_name, _cache_names
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 import logging
 from typing import Any, Dict, Optional, Tuple
 
+from ptal_api.adapter import TalismanAPIAdapter
+from ptal_api.core.type_mapper.data_model.base_data_model import (
+    MappedCompositePropertyType,
+    MappedConceptLinkType,
+    MappedConceptType,
+    TypeMapping,
+)
+from ptal_api.core.type_mapper.data_model.config_data_model import DefaultTypeCodeStorage
+from ptal_api.core.type_mapper.data_model.custom_data_model import CustomTypeCodeStorage
 from ptal_api.core.type_mapper.modules.custom_data_handler import CustomDataHandler
 from ptal_api.core.type_mapper.modules.object_name_transformer import ObjectTypeNameTransformer
-from ptal_api.core.type_mapper.data_model.custom_data_model import CustomTypeCodeStorage
-from ptal_api.core.type_mapper.data_model.config_data_model import DefaultTypeCodeStorage
-from ptal_api.core.type_mapper.data_model.base_data_model import MappedConceptType, MappedConceptLinkType, \
-    TypeMapping, MappedCompositePropertyType
-
-from ptal_api.adapter import TalismanAPIAdapter
-from ptal_api.schema.api_schema import ConceptPropertyTypeFilterSettings, CompositePropertyTypeFilterSettings, \
-    ConceptPropertyType, CompositePropertyValueTemplate
+from ptal_api.schema.api_schema import (
+    CompositePropertyTypeFilterSettings,
+    CompositePropertyValueTemplate,
+    ConceptPropertyType,
+    ConceptPropertyTypeFilterSettings,
+)
 
 
 class TypeMappingGenerator:
     def __init__(
-        self, api_adapter: TalismanAPIAdapter, logger: logging.Logger,
+        self,
+        api_adapter: TalismanAPIAdapter,
+        logger: logging.Logger,
         default_type_code_storage: Optional[DefaultTypeCodeStorage] = None,
-        custom_type_code_storage: Optional[CustomTypeCodeStorage] = None
+        custom_type_code_storage: Optional[CustomTypeCodeStorage] = None,
     ):
         self._api_adapter = api_adapter
         self._logger = logger
-        self._default_type_code_storage = default_type_code_storage if default_type_code_storage \
-            else DefaultTypeCodeStorage()
-        self._custom_type_code_storage = custom_type_code_storage if custom_type_code_storage \
-            else CustomTypeCodeStorage()
+        self._default_type_code_storage = (
+            default_type_code_storage if default_type_code_storage else DefaultTypeCodeStorage()
+        )
+        self._custom_type_code_storage = (
+            custom_type_code_storage if custom_type_code_storage else CustomTypeCodeStorage()
+        )
         self._type_mapping: Optional[TypeMapping] = None
         self._name_transformer = ObjectTypeNameTransformer()
 
     @staticmethod
     def _initialize_object_type_cache_names(custom_object_type_codes: Dict[Any, Any]) -> Dict[Any, Any]:
         return {value: key for key, value in custom_object_type_codes.items()}
 
@@ -40,25 +51,26 @@
         custom_concept_type_codes = self._custom_type_code_storage.concept_type_codes
         _concept_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(custom_concept_type_codes)
 
         for concept_type in self._api_adapter.get_all_concept_types():
             try:
                 concept_type_name = concept_type.name
 
-                transformed_concept_name, _concept_cache_names = self._name_transformer\
-                    .create_transformed_object_type_name(
-                        concept_type_name, self._default_type_code_storage.concept_type_code, _concept_cache_names,
-                        custom_concept_type_codes
-                    )
+                (
+                    transformed_concept_name,
+                    _concept_cache_names,
+                ) = self._name_transformer.create_transformed_object_type_name(
+                    concept_type_name,
+                    self._default_type_code_storage.concept_type_code,
+                    _concept_cache_names,
+                    custom_concept_type_codes,
+                )
 
                 self._type_mapping.add_mapped_concept_type(
-                    transformed_concept_name, MappedConceptType(
-                        id=concept_type.id,
-                        name=concept_type_name
-                    )
+                    transformed_concept_name, MappedConceptType(id=concept_type.id, name=concept_type_name)
                 )
                 self._type_mapping.add_concept_type(transformed_concept_name, concept_type)
                 self._logger.debug(f"Processed a concept type with id equal to {concept_type.id}")
             except Exception as ex:
                 self._logger.info(f"Failed to process a concept type with id equal to {concept_type.id}")
                 self._logger.exception(ex)
 
@@ -68,86 +80,101 @@
         custom_concept_property_type_codes = self._custom_type_code_storage.concept_property_type_codes
         _property_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(
             {**custom_any_property_type_codes, **custom_property_type_codes, **custom_concept_property_type_codes}
         )
 
         for transformed_concept_name, mapped_concept_type in self._type_mapping.concepts_types_mapping.items():
             for property_type in self._api_adapter.get_all_concept_property_types(
-                filter_settings=ConceptPropertyTypeFilterSettings(
-                    concept_type_id=mapped_concept_type.id
-                )
+                filter_settings=ConceptPropertyTypeFilterSettings(concept_type_id=mapped_concept_type.id)
             ):
                 try:
                     if self._is_property_type_composite(property_type):
                         continue
 
                     property_type_name = property_type.name
 
-                    transformed_property_name, _property_cache_names = self._name_transformer\
-                        .create_transformed_object_type_name(
-                            property_type_name, self._default_type_code_storage.property_type_code,
-                            _property_cache_names, custom_concept_property_type_codes, custom_property_type_codes,
-                            custom_any_property_type_codes
-                        )
+                    (
+                        transformed_property_name,
+                        _property_cache_names,
+                    ) = self._name_transformer.create_transformed_object_type_name(
+                        property_type_name,
+                        self._default_type_code_storage.property_type_code,
+                        _property_cache_names,
+                        custom_concept_property_type_codes,
+                        custom_property_type_codes,
+                        custom_any_property_type_codes,
+                    )
 
                     mapped_concept_type.add_mapped_property_type(transformed_property_name, property_type_name)
                     self._type_mapping.add_concept_property_type(
                         transformed_concept_name, transformed_property_name, property_type
                     )
-                    self._logger.debug(f"Processed a property type with id equal to {property_type.id}"
-                                       f" for a concept type with id equal to {mapped_concept_type.id}")
+                    self._logger.debug(
+                        f"Processed a property type with id equal to {property_type.id}"
+                        f" for a concept type with id equal to {mapped_concept_type.id}"
+                    )
                 except Exception as ex:
-                    self._logger.info(f"Failed to process a property type with id equal to {property_type.id}"
-                                      f" for a concept type with id equal to {mapped_concept_type.id}")
+                    self._logger.info(
+                        f"Failed to process a property type with id equal to {property_type.id}"
+                        f" for a concept type with id equal to {mapped_concept_type.id}"
+                    )
                     self._logger.exception(ex)
 
     def _process_concept_composite_property_type_mapping(self) -> None:
         custom_any_property_type_codes = self._custom_type_code_storage.any_property_type_codes
         custom_composite_property_type_codes = self._custom_type_code_storage.composite_property_type_codes
-        custom_concept_composite_property_type_codes = self._custom_type_code_storage\
-            .concept_composite_property_type_codes
+        custom_concept_composite_property_type_codes = (
+            self._custom_type_code_storage.concept_composite_property_type_codes
+        )
         custom_component_value_type_codes = self._custom_type_code_storage.composite_property_component_value_type_codes
-        custom_concept_component_value_type_codes = self._custom_type_code_storage\
-            .concept_composite_property_component_value_type_codes
+        custom_concept_component_value_type_codes = (
+            self._custom_type_code_storage.concept_composite_property_component_value_type_codes
+        )
         _composite_property_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(
             {
-                **custom_any_property_type_codes, **custom_composite_property_type_codes,
-                **custom_concept_composite_property_type_codes
+                **custom_any_property_type_codes,
+                **custom_composite_property_type_codes,
+                **custom_concept_composite_property_type_codes,
             }
         )
         _component_value_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(
             {**custom_component_value_type_codes, **custom_concept_component_value_type_codes}
         )
 
         for transformed_concept_name, mapped_concept_type in self._type_mapping.concepts_types_mapping.items():
             for composite_property_type in self._api_adapter.get_all_concept_composite_property_types(
-                filter_settings=CompositePropertyTypeFilterSettings(
-                    concept_type_id=mapped_concept_type.id
-                )
+                filter_settings=CompositePropertyTypeFilterSettings(concept_type_id=mapped_concept_type.id)
             ):
                 try:
                     composite_property_type_name = composite_property_type.name
 
-                    transformed_composite_property_name, _composite_property_cache_names = self._name_transformer\
-                        .create_transformed_object_type_name(
-                            composite_property_type_name, self._default_type_code_storage.composite_property_type_code,
-                            _composite_property_cache_names, custom_concept_composite_property_type_codes,
-                            custom_composite_property_type_codes, custom_any_property_type_codes
-                        )
+                    (
+                        transformed_composite_property_name,
+                        _composite_property_cache_names,
+                    ) = self._name_transformer.create_transformed_object_type_name(
+                        composite_property_type_name,
+                        self._default_type_code_storage.composite_property_type_code,
+                        _composite_property_cache_names,
+                        custom_concept_composite_property_type_codes,
+                        custom_composite_property_type_codes,
+                        custom_any_property_type_codes,
+                    )
 
                     component_values, _component_value_cache_names = self._process_composite_component_value_types(
-                        composite_property_type, _component_value_cache_names,
-                        custom_concept_component_value_type_codes, custom_component_value_type_codes
+                        composite_property_type,
+                        _component_value_cache_names,
+                        custom_concept_component_value_type_codes,
+                        custom_component_value_type_codes,
                     )
 
                     mapped_concept_type.add_mapped_composite_property_type(
-                        transformed_composite_property_name, MappedCompositePropertyType(
-                            name=composite_property_type_name,
-                            component_values=component_values
-                        )
+                        transformed_composite_property_name,
+                        MappedCompositePropertyType(
+                            name=composite_property_type_name, component_values=component_values
+                        ),
                     )
                     self._type_mapping.add_concept_composite_property_type(
                         transformed_concept_name, transformed_composite_property_name, composite_property_type
                     )
                     self._logger.debug(
                         f"Processed a composite property type with id equal to {composite_property_type.id}"
                         f" for a concept type with id equal to {mapped_concept_type.id}"
@@ -167,36 +194,49 @@
 
         for concept_link_type in self._api_adapter.get_all_concept_link_types():
             try:
                 concept_link_type_name = concept_link_type.name
                 concept_from_type_name = concept_link_type.concept_from_type.name
                 concept_to_type_name = concept_link_type.concept_to_type.name
                 transformed_concept_from_type_name = self._name_transformer.get_transformed_concept_type_name(
-                    concept_from_type_name, self._default_type_code_storage.concept_type_code,
-                    concept_link_type.concept_from_type.id, self._type_mapping, self._custom_type_code_storage
+                    concept_from_type_name,
+                    self._default_type_code_storage.concept_type_code,
+                    concept_link_type.concept_from_type.id,
+                    self._type_mapping,
+                    self._custom_type_code_storage,
                 )
                 transformed_concept_to_type_name = self._name_transformer.get_transformed_concept_type_name(
-                    concept_to_type_name, self._default_type_code_storage.concept_type_code,
-                    concept_link_type.concept_to_type.id, self._type_mapping, self._custom_type_code_storage
+                    concept_to_type_name,
+                    self._default_type_code_storage.concept_type_code,
+                    concept_link_type.concept_to_type.id,
+                    self._type_mapping,
+                    self._custom_type_code_storage,
+                )
+
+                (
+                    transformed_concept_link_name,
+                    _link_cache_names,
+                ) = self._name_transformer.create_transformed_concept_link_type_name(
+                    concept_link_type_name,
+                    self._default_type_code_storage.concept_link_type_code,
+                    concept_from_type_name,
+                    concept_to_type_name,
+                    transformed_concept_from_type_name,
+                    transformed_concept_to_type_name,
+                    _link_cache_names,
+                    self._custom_type_code_storage,
                 )
 
-                transformed_concept_link_name, _link_cache_names = self._name_transformer\
-                    .create_transformed_concept_link_type_name(
-                        concept_link_type_name, self._default_type_code_storage.concept_link_type_code,
-                        concept_from_type_name, concept_to_type_name, transformed_concept_from_type_name,
-                        transformed_concept_to_type_name, _link_cache_names, self._custom_type_code_storage
-                    )
-
                 self._type_mapping.add_mapped_concept_link_type(
                     MappedConceptLinkType(
                         id=concept_link_type.id,
                         source_type=transformed_concept_from_type_name,
                         target_type=transformed_concept_to_type_name,
                         old_relation_type=transformed_concept_link_name,
-                        new_relation_type=concept_link_type_name
+                        new_relation_type=concept_link_type_name,
                     )
                 )
                 self._type_mapping.add_concept_link_type(transformed_concept_link_name, concept_link_type)
                 self._logger.debug(f"Processed a concept link type with id equal to {concept_link_type.id}")
             except Exception as ex:
                 self._logger.info(f"Failed to process a concept link type with id equal to {concept_link_type.id}")
                 self._logger.exception(ex)
@@ -207,90 +247,106 @@
         custom_concept_link_property_type_codes = self._custom_type_code_storage.concept_link_property_type_codes
         _property_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(
             {**custom_any_property_type_codes, **custom_property_type_codes, **custom_concept_link_property_type_codes}
         )
 
         for mapped_concept_link_type in self._type_mapping.relations_types_mapping:
             for property_type in self._api_adapter.get_all_concept_link_property_types(
-                filter_settings=ConceptPropertyTypeFilterSettings(
-                    concept_link_type_id=mapped_concept_link_type.id
-                )
+                filter_settings=ConceptPropertyTypeFilterSettings(concept_link_type_id=mapped_concept_link_type.id)
             ):
                 try:
                     if self._is_property_type_composite(property_type):
                         continue
 
                     property_type_name = property_type.name
 
-                    transformed_property_name, _property_cache_names = self._name_transformer\
-                        .create_transformed_object_type_name(
-                            property_type_name, self._default_type_code_storage.property_type_code,
-                            _property_cache_names, custom_concept_link_property_type_codes, custom_property_type_codes,
-                            custom_any_property_type_codes
-                        )
+                    (
+                        transformed_property_name,
+                        _property_cache_names,
+                    ) = self._name_transformer.create_transformed_object_type_name(
+                        property_type_name,
+                        self._default_type_code_storage.property_type_code,
+                        _property_cache_names,
+                        custom_concept_link_property_type_codes,
+                        custom_property_type_codes,
+                        custom_any_property_type_codes,
+                    )
 
                     mapped_concept_link_type.add_mapped_property_type(transformed_property_name, property_type_name)
                     self._type_mapping.add_concept_link_property_type(
                         mapped_concept_link_type.old_relation_type, transformed_property_name, property_type
                     )
-                    self._logger.debug(f"Processed a property type with id equal to {property_type.id}"
-                                       f" for a concept link type with id equal to {mapped_concept_link_type.id}")
+                    self._logger.debug(
+                        f"Processed a property type with id equal to {property_type.id}"
+                        f" for a concept link type with id equal to {mapped_concept_link_type.id}"
+                    )
                 except Exception as ex:
-                    self._logger.info(f"Failed to process a property type with id equal to {property_type.id}"
-                                      f" for a concept link type with id equal to {mapped_concept_link_type.id}")
+                    self._logger.info(
+                        f"Failed to process a property type with id equal to {property_type.id}"
+                        f" for a concept link type with id equal to {mapped_concept_link_type.id}"
+                    )
                     self._logger.exception(ex)
 
     def _process_relation_composite_property_type_mapping(self) -> None:
         custom_any_property_type_codes = self._custom_type_code_storage.any_property_type_codes
         custom_composite_property_type_codes = self._custom_type_code_storage.composite_property_type_codes
-        custom_concept_link_composite_property_type_codes = self._custom_type_code_storage\
-            .concept_link_composite_property_type_codes
+        custom_concept_link_composite_property_type_codes = (
+            self._custom_type_code_storage.concept_link_composite_property_type_codes
+        )
         custom_component_value_type_codes = self._custom_type_code_storage.composite_property_component_value_type_codes
-        custom_concept_link_component_value_type_codes = self._custom_type_code_storage\
-            .concept_link_composite_property_component_value_type_codes
+        custom_concept_link_component_value_type_codes = (
+            self._custom_type_code_storage.concept_link_composite_property_component_value_type_codes
+        )
         _composite_property_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(
             {
-                **custom_any_property_type_codes, **custom_composite_property_type_codes,
-                **custom_concept_link_composite_property_type_codes
+                **custom_any_property_type_codes,
+                **custom_composite_property_type_codes,
+                **custom_concept_link_composite_property_type_codes,
             }
         )
         _component_value_cache_names: Dict[str, str] = self._initialize_object_type_cache_names(
             {**custom_component_value_type_codes, **custom_concept_link_component_value_type_codes}
         )
 
         for mapped_concept_link_type in self._type_mapping.relations_types_mapping:
             for composite_property_type in self._api_adapter.get_all_concept_link_composite_property_types(
-                filter_settings=CompositePropertyTypeFilterSettings(
-                    link_type_id=mapped_concept_link_type.id
-                )
+                filter_settings=CompositePropertyTypeFilterSettings(link_type_id=mapped_concept_link_type.id)
             ):
                 try:
                     composite_property_type_name = composite_property_type.name
 
-                    transformed_composite_property_name, _composite_property_cache_names = self._name_transformer\
-                        .create_transformed_object_type_name(
-                            composite_property_type_name, self._default_type_code_storage.composite_property_type_code,
-                            _composite_property_cache_names, custom_concept_link_composite_property_type_codes,
-                            custom_composite_property_type_codes, custom_any_property_type_codes
-                        )
+                    (
+                        transformed_composite_property_name,
+                        _composite_property_cache_names,
+                    ) = self._name_transformer.create_transformed_object_type_name(
+                        composite_property_type_name,
+                        self._default_type_code_storage.composite_property_type_code,
+                        _composite_property_cache_names,
+                        custom_concept_link_composite_property_type_codes,
+                        custom_composite_property_type_codes,
+                        custom_any_property_type_codes,
+                    )
 
                     component_values, _component_value_cache_names = self._process_composite_component_value_types(
-                        composite_property_type, _component_value_cache_names,
-                        custom_concept_link_component_value_type_codes, custom_component_value_type_codes
+                        composite_property_type,
+                        _component_value_cache_names,
+                        custom_concept_link_component_value_type_codes,
+                        custom_component_value_type_codes,
                     )
 
                     mapped_concept_link_type.add_mapped_composite_property_type(
-                        transformed_composite_property_name, MappedCompositePropertyType(
-                            name=composite_property_type_name,
-                            component_values=component_values
-                        )
+                        transformed_composite_property_name,
+                        MappedCompositePropertyType(
+                            name=composite_property_type_name, component_values=component_values
+                        ),
                     )
                     self._type_mapping.add_concept_link_composite_property_type(
-                        mapped_concept_link_type.old_relation_type, transformed_composite_property_name,
-                        composite_property_type
+                        mapped_concept_link_type.old_relation_type,
+                        transformed_composite_property_name,
+                        composite_property_type,
                     )
                     self._logger.debug(
                         f"Processed a composite property type with id equal to {composite_property_type.id}"
                         f" for a concept link type with id equal to {mapped_concept_link_type.id}"
                     )
                 except Exception as ex:
                     self._logger.info(
@@ -305,53 +361,65 @@
             custom_concept_property_value_type_codes
         )
 
         for property_value_type in self._api_adapter.get_all_concept_property_value_types():
             try:
                 property_value_type_name = property_value_type.name
 
-                transformed_property_value_name, _property_value_cache_names = self._name_transformer\
-                    .create_transformed_object_type_name(
-                        property_value_type_name, self._default_type_code_storage.concept_property_value_type_code,
-                        _property_value_cache_names, custom_concept_property_value_type_codes
-                    )
+                (
+                    transformed_property_value_name,
+                    _property_value_cache_names,
+                ) = self._name_transformer.create_transformed_object_type_name(
+                    property_value_type_name,
+                    self._default_type_code_storage.concept_property_value_type_code,
+                    _property_value_cache_names,
+                    custom_concept_property_value_type_codes,
+                )
 
                 self._type_mapping.add_mapped_concept_property_value_type(
                     transformed_property_value_name, property_value_type_name
                 )
                 self._type_mapping.add_concept_property_value_type(transformed_property_value_name, property_value_type)
                 self._logger.debug(f"Processed a concept property value type with id equal to {property_value_type.id}")
             except Exception as ex:
                 self._logger.info(
                     f"Failed to process a concept property value type with id equal to {property_value_type.id}"
                 )
                 self._logger.exception(ex)
 
     def _process_composite_component_value_types(
-        self, composite_property_type: ConceptPropertyType, component_value_type_cache_names: Dict[str, str],
-        custom_object_component_value_type_codes: Dict[str, str], custom_component_value_type_codes: Dict[str, str]
+        self,
+        composite_property_type: ConceptPropertyType,
+        component_value_type_cache_names: Dict[str, str],
+        custom_object_component_value_type_codes: Dict[str, str],
+        custom_component_value_type_codes: Dict[str, str],
     ) -> Tuple[Dict[str, str], Dict[str, str]]:
         component_value_types: Dict[str, str] = {}  # Dict[component_value_type_code, component_value_type_name]
         _component_value_type_cache_names = component_value_type_cache_names.copy()
 
         for component_value_type in composite_property_type.value_type.component_value_types:
             try:
                 component_value_type_name = component_value_type.name
 
-                transformed_component_value_name, _component_value_type_cache_names = self._name_transformer\
-                    .create_transformed_object_type_name(
-                        component_value_type_name,
-                        self._default_type_code_storage.composite_property_component_value_type_code,
-                        _component_value_type_cache_names, custom_object_component_value_type_codes,
-                        custom_component_value_type_codes
-                    )
+                (
+                    transformed_component_value_name,
+                    _component_value_type_cache_names,
+                ) = self._name_transformer.create_transformed_object_type_name(
+                    component_value_type_name,
+                    self._default_type_code_storage.composite_property_component_value_type_code,
+                    _component_value_type_cache_names,
+                    custom_object_component_value_type_codes,
+                    custom_component_value_type_codes,
+                )
 
                 component_value_types[transformed_component_value_name] = component_value_type_name
-                self._logger.debug(f"Processed a component value type with id equal to {component_value_type.id}"
-                                   f" for a composite property type with id equal to {composite_property_type.id}")
+                self._logger.debug(
+                    f"Processed a component value type with id equal to {component_value_type.id}"
+                    f" for a composite property type with id equal to {composite_property_type.id}"
+                )
             except Exception as ex:
                 self._logger.debug(
                     f"Failed to process a component value type with id equal to {component_value_type.id}"
                     f" for a composite property type with id equal to {composite_property_type.id}"
                 )
                 self._logger.exception(ex)
         return component_value_types, _component_value_type_cache_names
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.11.5/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 from typing import Optional, Union
 
 import marshmallow_dataclass
 
 from ptal_api.core.type_mapper.data_model.base_data_model import TypeMapping
-from ptal_api.core.type_mapper.modules.type_mapping_loader.type_mapping_loader_interface import \
-    TypeMappingLoaderInterface
+from ptal_api.core.type_mapper.modules.type_mapping_loader.type_mapping_loader_interface import (
+    TypeMappingLoaderInterface,
+)
 
 
 class TypeMappingLoader(TypeMappingLoaderInterface):
     def __init__(self, logger: logging.Logger):
         super().__init__(logger)
 
     def _load_type_mapping_from_file(self, file_path: str) -> Optional[TypeMapping]:
         try:
-            with open(file_path, "r", encoding="utf-8") as file:
+            with open(file_path, encoding="utf-8") as file:
                 type_mapping = marshmallow_dataclass.class_schema(TypeMapping)().loads(file.read())
-                self._logger.info(f"Loaded type mapping from file \"{file_path}\"")
+                self._logger.info(f'Loaded type mapping from file "{file_path}"')
                 return type_mapping
         except Exception as ex:
-            self._logger.info(f"Failed to load type mapping from file \"{file_path}\"")
+            self._logger.info(f'Failed to load type mapping from file "{file_path}"')
             raise ex
 
     def _load_type_mapping_from_dict(self, input_dict: dict) -> Optional[TypeMapping]:
         try:
             type_mapping = marshmallow_dataclass.class_schema(TypeMapping)().load(input_dict)
             self._logger.info("Loaded type mapping from input dictionary")
             return type_mapping
         except Exception as ex:
             self._logger.info("Failed to load type mapping from input dictionary")
             raise ex
 
     def load_type_mapping(self, input_data: Optional[Union[str, dict, TypeMapping]]) -> TypeMapping:
         if isinstance(input_data, TypeMapping):
             return input_data
-        elif isinstance(input_data, str):
+        if isinstance(input_data, str):
             return self._load_type_mapping_from_file(input_data)
-        elif isinstance(input_data, dict):
+        if isinstance(input_data, dict):
             return self._load_type_mapping_from_dict(input_data)
-        else:
-            return TypeMapping()
+        return TypeMapping()
```

### Comparing `ptal_api-0.11.4.2/ptal_api/core/values/value_mapping.py` & `ptal_api-0.11.5/ptal_api/core/values/value_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from abc import ABCMeta, abstractmethod
 from datetime import date
 from typing import Any, Dict, Type, Union
 
 from sgqlc.types import Input
 
 from ptal_api.schema.api_schema import (
-    ValueInput, DateTimeValueInput, DateInput, StringValueInput, IntValueInput,
-    DoubleValueInput, LinkValueInput
+    DateInput,
+    DateTimeValueInput,
+    DoubleValueInput,
+    IntValueInput,
+    LinkValueInput,
+    StringValueInput,
+    ValueInput,
 )
 from .date_dataclass import PartialDateValue
 
 
 class AbstractValueMapper(metaclass=ABCMeta):
     @staticmethod
     @abstractmethod
@@ -31,45 +36,45 @@
 
         value_input = ValueInput()
         value_input.string_value_input = string_input
         return value_input
 
     @staticmethod
     def get_tdm_value_format(value: str) -> Dict:
-        return {'value': value}
+        return {"value": value}
 
 
 class IntValueMapper(AbstractValueMapper):
     @staticmethod
     def get_value_input(value: int) -> Input:
         int_input = IntValueInput()
         int_input.value = value
 
         value_input = ValueInput()
         value_input.int_value_input = int_input
         return value_input
 
     @staticmethod
     def get_tdm_value_format(value: int) -> Dict:
-        return {'value': value}
+        return {"value": value}
 
 
 class DoubleValueMapper(AbstractValueMapper):
     @staticmethod
     def get_value_input(value: float) -> Input:
         double_input = DoubleValueInput()
         double_input.value = value
 
         value_input = ValueInput()
         value_input.double_value_input = double_input
         return value_input
 
     @staticmethod
     def get_tdm_value_format(value: float) -> Dict:
-        return {'value': value}
+        return {"value": value}
 
 
 class DateValueMapper(AbstractValueMapper):
     @staticmethod
     def get_value_input(value: Union[date, PartialDateValue]) -> Input:
         date_obj = DateInput()
         date_obj.day = value.day
@@ -81,44 +86,37 @@
 
         value_input = ValueInput()
         value_input.date_time_value_input = date_input
         return value_input
 
     @staticmethod
     def get_tdm_value_format(value: date) -> Dict:
-        return {
-            'date': {
-                'day': value.day,
-                'month': value.month,
-                'year': value.year
-            }
-        }
+        return {"date": {"day": value.day, "month": value.month, "year": value.year}}
 
 
 class LinkValueMapper(AbstractValueMapper):
     @staticmethod
     def get_value_input(value: str) -> Input:
         link_input = LinkValueInput()
         link_input.link = value
 
         value_input = ValueInput()
         value_input.link_value_input = link_input
         return value_input
 
     @staticmethod
     def get_tdm_value_format(value: str) -> Dict:
-        return {'link': value}
+        return {"link": value}
 
 
 def get_map_helper(value_type: str) -> Type[AbstractValueMapper]:
-    if value_type == 'String':
+    if value_type == "String":
         return StringValueMapper
-    elif value_type == 'Int':
+    if value_type == "Int":
         return IntValueMapper
-    elif value_type == 'Double':
+    if value_type == "Double":
         return DoubleValueMapper
-    elif value_type == 'Date':
+    if value_type == "Date":
         return DateValueMapper
-    elif value_type == 'Link':
+    if value_type == "Link":
         return LinkValueMapper
-    else:
-        raise NotImplementedError(f'{value_type} type not implemented')
+    raise NotImplementedError(f"{value_type} type not implemented")
```

### Comparing `ptal_api-0.11.4.2/ptal_api/providers/gql_providers.py` & `ptal_api-0.11.5/ptal_api/providers/gql_providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,48 @@
-from contextlib import AbstractContextManager
 import logging
 import time
+from contextlib import AbstractContextManager
 from typing import Optional
 
-from sgqlc.endpoint.http import HTTPEndpoint, BaseEndpoint
 from keycloak import KeycloakOpenID
-
+from sgqlc.endpoint.http import BaseEndpoint, HTTPEndpoint
 
 logger = logging.getLogger(__name__)
 
 
 def _configure_gql_client(
-    uri: str, timeout: float = None, retries: int = 0, auth_token: Optional[str] = None
+    uri: str, timeout: float = None, _retries: int = 0, auth_token: Optional[str] = None
 ) -> HTTPEndpoint:
-    headers = {
-        "X-Auth-Token": auth_token,
-        "Authorization": f"Bearer {auth_token}"
-    } if auth_token is not None else None
-    transport = HTTPEndpoint(uri, headers, timeout=timeout)
-    return transport
+    headers = {"X-Auth-Token": auth_token, "Authorization": f"Bearer {auth_token}"} if auth_token is not None else None
+    return HTTPEndpoint(uri, headers, timeout=timeout)
 
 
 class AbstractGQLClient(AbstractContextManager):
     def __init__(self, gql_uri: str, timeout: float, retries: int, retry_timeout: float) -> None:
         super().__init__()
         self._gql_uri = gql_uri
         self._timeout = timeout
         self._retries = retries
         self._retry_timeout = retry_timeout
         self._gql_client: Optional[BaseEndpoint] = None
 
         if self._retries < 0:
-            raise ValueError('Retries count cannot be negative')
+            raise ValueError("Retries count cannot be negative")
 
     def execute(self, query, *args, **kwargs):
         for i in range(self._retries + 1):
             try:
                 return self._gql_client.__call__(query, *args, **kwargs)
             except Exception as e:
                 logger.exception(e)
-                logger.error(f'Exception during executing {query}, retry...')
+                logger.error(f"Exception during executing {query}, retry...")
                 if i == self._retries - 1:
                     raise e
                 time.sleep(self._retry_timeout)
+        return None
 
 
 class NoAuthGQLClient(AbstractGQLClient):
     def __init__(self, gql_uri: str, timeout: float, retries: int, retry_timeout: float = 1) -> None:
         super().__init__(gql_uri, timeout, retries, retry_timeout)
 
     def __enter__(self):
@@ -57,31 +53,39 @@
         self._gql_client = None
 
 
 class KeycloakAwareGQLClient(AbstractGQLClient):
     _TIME_OFFSET = 10  # in seconds
 
     def __init__(
-        self, gql_uri: str, timeout: float, retries: int,
-        auth_url: str, realm: str, client_id: str, client_secret: str, user: str, pwd: str,
-        retry_timeout: float = 1
+        self,
+        gql_uri: str,
+        timeout: float,
+        retries: int,
+        auth_url: str,
+        realm: str,
+        client_id: str,
+        client_secret: str,
+        user: str,
+        pwd: str,
+        retry_timeout: float = 1,
     ) -> None:
         super().__init__(gql_uri, timeout, retries, retry_timeout)
 
         self._auth_url = auth_url
         self._realm = realm
         self._client_id = client_id
         self._client_secret = client_secret
         self._user = user
         self._pwd = pwd
 
-        if any(env is None for env in [
-            self._auth_url, self._realm, self._client_id,
-            self._client_secret, self._user, self._pwd
-        ]):
+        if any(
+            env is None
+            for env in [self._auth_url, self._realm, self._client_id, self._client_secret, self._user, self._pwd]
+        ):
             raise ValueError("Authorization variables values are not set")
 
         self._keycloak_openid: Optional[KeycloakOpenID] = None
         self._access_token: Optional[str] = None
         self._refresh_token: Optional[str] = None
         self._access_expiration_timestamp: Optional[float] = None
         self._refresh_expiration_timestamp: Optional[float] = None
@@ -89,24 +93,21 @@
     def _ensure_session_liveness(self):
         offsetted_time = time.time() + self._TIME_OFFSET
         if self._access_expiration_timestamp is not None and offsetted_time < self._access_expiration_timestamp:
             return
 
         time_before_req = time.time()
         # if self._refresh_expiration_timestamp is not None and offsetted_time < self._refresh_expiration_timestamp:
-        #     logger.info("refreshing access token with refresh token")
-        #     token_info = self._keycloak_openid.refresh_token(self._refresh_token)
-        # else:
         logger.info("refreshing access token with credentials")
         token_info = self._keycloak_openid.token(self._user, self._pwd)
 
-        self._access_token = token_info['access_token']
-        self._access_expiration_timestamp = time_before_req + token_info['expires_in']
-        self._refresh_token = token_info['refresh_token']
-        self._refresh_expiration_timestamp = time_before_req + token_info['refresh_expires_in']
+        self._access_token = token_info["access_token"]
+        self._access_expiration_timestamp = time_before_req + token_info["expires_in"]
+        self._refresh_token = token_info["refresh_token"]
+        self._refresh_expiration_timestamp = time_before_req + token_info["refresh_expires_in"]
 
         self._gql_client = _configure_gql_client(self._gql_uri, self._timeout, self._retries, self._access_token)
 
     def __enter__(self):
         self._keycloak_openid = KeycloakOpenID(self._auth_url, self._realm, self._client_id, self._client_secret)
         return self
```

### Comparing `ptal_api-0.11.4.2/ptal_api/schema/README.md` & `ptal_api-0.11.5/ptal_api/schema/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 sgqlc-codegen schema introspection.json utils_api_schema.py
 ```
 2.4. Generate code for tcontroller_api_schema
 ```bash
 sgqlc-codegen schema introspection.json tcontroller_api_schema.py
 ```
 3. do not forget to comment/remove `import sgqlc.types.datetime` in `api_schema.py` and `utils_api_schema.py`.
-4. add both `introspection.json` and `api_schema.py` files to commit
+4. add all `*api_schema.py` files to commit
```

### Comparing `ptal_api-0.11.4.2/ptal_api/schema/api_schema.py` & `ptal_api-0.11.5/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,17 +490,18 @@
     has_supporting_documents = sgqlc.types.Field(Boolean, graphql_name='hasSupportingDocuments')
     has_header_information = sgqlc.types.Field(Boolean, graphql_name='hasHeaderInformation')
     show_in_menu = sgqlc.types.Field(Boolean, graphql_name='showInMenu')
 
 
 class CompositeConceptTypeUpdateTemplateFilenameInput(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('id', 'filename')
+    __field_names__ = ('id', 'filename', 'bucket')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     filename = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='filename')
+    bucket = sgqlc.types.Field(String, graphql_name='bucket')
 
 
 class CompositeConceptTypeViewInput(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('concept_type_id', 'composite_concept_type_id')
     concept_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptTypeId')
     composite_concept_type_id = sgqlc.types.Field(ID, graphql_name='compositeConceptTypeId')
@@ -1764,14 +1765,33 @@
     is_event = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isEvent')
 
 
 
 ########################################################################
 # Output Objects and Interfaces
 ########################################################################
+class FactInterface(sgqlc.types.Interface):
+    __schema__ = api_schema
+    __field_names__ = ('id', 'mention', 'system_registration_date', 'system_update_date', 'document')
+    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
+    mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('TextBounding'))), graphql_name='mention')
+    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
+    document = sgqlc.types.Field(sgqlc.types.non_null('Document'), graphql_name='document')
+
+
+class RecordInterface(sgqlc.types.Interface):
+    __schema__ = api_schema
+    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
+    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
+    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
+    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
+
+
 class AccessLevel(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('id', 'name', 'order')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     order = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='order')
 
@@ -2386,24 +2406,14 @@
 class Facet(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('value', 'count')
     value = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='value')
     count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='count')
 
 
-class FactInterface(sgqlc.types.Interface):
-    __schema__ = api_schema
-    __field_names__ = ('id', 'mention', 'system_registration_date', 'system_update_date', 'document')
-    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
-    mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('TextBounding'))), graphql_name='mention')
-    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
-    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
-    document = sgqlc.types.Field(sgqlc.types.non_null('Document'), graphql_name='document')
-
-
 class FlatDocumentStructure(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('text', 'annotations', 'metadata', 'document_id', 'node_id', 'hierarchy_level', 'translated_text', 'id', 'language')
     text = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='text')
     annotations = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Annotation))), graphql_name='annotations')
     metadata = sgqlc.types.Field(sgqlc.types.non_null('ParagraphMetadata'), graphql_name='metadata')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
@@ -3607,23 +3617,14 @@
     )
     preview_chart = sgqlc.types.Field(sgqlc.types.non_null(Chart), graphql_name='previewChart', args=sgqlc.types.ArgDict((
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(ChartDescriptionInput), graphql_name='form', default=None)),
 ))
     )
 
 
-class RecordInterface(sgqlc.types.Interface):
-    __schema__ = api_schema
-    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
-    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
-    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
-    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
-    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
-
-
 class RedmineIssue(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('id', 'subject', 'tracker', 'status', 'priority', 'author', 'assignee', 'creation_date')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     subject = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='subject')
     tracker = sgqlc.types.Field(sgqlc.types.non_null('RedmineTracker'), graphql_name='tracker')
     status = sgqlc.types.Field(sgqlc.types.non_null('RedmineStatus'), graphql_name='status')
```

### Comparing `ptal_api-0.11.4.2/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.11.5/ptal_api/schema/crawlers_api_schema.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -501,14 +501,23 @@
     with_removed_versions = sgqlc.types.Field(Boolean, graphql_name='withRemovedVersions')
 
 
 
 ########################################################################
 # Output Objects and Interfaces
 ########################################################################
+class RecordInterface(sgqlc.types.Interface):
+    __schema__ = crawlers_api_schema
+    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
+    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
+    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
+    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
+
+
 class ArgsAndSettingsDescription(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('args', 'settings')
     args = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SettingDescription')), graphql_name='args')
     settings = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SettingDescription')), graphql_name='settings')
 
 
@@ -1160,23 +1169,14 @@
     )
     web_scraper_version_is_compatible = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='webScraperVersionIsCompatible', args=sgqlc.types.ArgDict((
         ('web_scraper_version', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='webScraperVersion', default=None)),
 ))
     )
 
 
-class RecordInterface(sgqlc.types.Interface):
-    __schema__ = crawlers_api_schema
-    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
-    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
-    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
-    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
-    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
-
-
 class RecoveryJob(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'crawler_data', 'source_version_data', 'result_version_data', 'status', 'start_time', 'end_time', 'progress', 'progress_message', 'creator', 'system_registration_date', 'last_updater', 'system_update_date')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     crawler_data = sgqlc.types.Field(sgqlc.types.non_null(CrawlerData), graphql_name='crawlerData')
     source_version_data = sgqlc.types.Field(sgqlc.types.non_null('VersionData'), graphql_name='sourceVersionData')
     result_version_data = sgqlc.types.Field('VersionData', graphql_name='resultVersionData')
```

### Comparing `ptal_api-0.11.4.2/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.11.5/ptal_api/schema/tcontroller_api_schema.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -330,14 +330,23 @@
     environment = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(UserServiceEnvironmentVariableInput)), graphql_name='environment')
 
 
 
 ########################################################################
 # Output Objects and Interfaces
 ########################################################################
+class RecordInterface(sgqlc.types.Interface):
+    __schema__ = tcontroller_api_schema
+    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
+    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
+    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
+    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
+
+
 class ActiveMessageList(sgqlc.types.Type):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('messages', 'total')
     messages = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ActiveMessageStatus'))), graphql_name='messages')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
 
 
@@ -1034,23 +1043,14 @@
     user_pipeline_transform = sgqlc.types.Field(sgqlc.types.non_null('UserPipelineTransform'), graphql_name='userPipelineTransform', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     debug_dump_extensions = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='debugDumpExtensions')
 
 
-class RecordInterface(sgqlc.types.Interface):
-    __schema__ = tcontroller_api_schema
-    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
-    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
-    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
-    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
-    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
-
-
 class ServiceStats(sgqlc.types.Type):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('name', 'duration', 'load', 'ok_requests', 'failed_requests', 'ok_request_max_duration')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     duration = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='duration')
     load = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='load')
     ok_requests = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='okRequests')
```

### Comparing `ptal_api-0.11.4.2/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.11.5/ptal_api/schema/utils_api_schema.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -636,14 +636,33 @@
     is_event = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isEvent')
 
 
 
 ########################################################################
 # Output Objects and Interfaces
 ########################################################################
+class FactInterface(sgqlc.types.Interface):
+    __schema__ = utils_api_schema
+    __field_names__ = ('id', 'mention', 'system_registration_date', 'system_update_date', 'document')
+    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
+    mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('TextBounding'))), graphql_name='mention')
+    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
+    document = sgqlc.types.Field(sgqlc.types.non_null('Document'), graphql_name='document')
+
+
+class RecordInterface(sgqlc.types.Interface):
+    __schema__ = utils_api_schema
+    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
+    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
+    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
+    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
+
+
 class AccessLevel(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('id', 'name', 'order')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     order = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='order')
 
@@ -1006,24 +1025,14 @@
 class Facet(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('value', 'count')
     value = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='value')
     count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='count')
 
 
-class FactInterface(sgqlc.types.Interface):
-    __schema__ = utils_api_schema
-    __field_names__ = ('id', 'mention', 'system_registration_date', 'system_update_date', 'document')
-    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
-    mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('TextBounding'))), graphql_name='mention')
-    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
-    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
-    document = sgqlc.types.Field(sgqlc.types.non_null('Document'), graphql_name='document')
-
-
 class FlatDocumentStructure(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('text', 'annotations', 'metadata', 'document_id', 'node_id', 'hierarchy_level', 'translated_text', 'id', 'language')
     text = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='text')
     annotations = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Annotation))), graphql_name='annotations')
     metadata = sgqlc.types.Field(sgqlc.types.non_null('ParagraphMetadata'), graphql_name='metadata')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
@@ -1338,23 +1347,14 @@
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptPropertyTypeFilterSettings), graphql_name='filterSettings', default=None)),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
         ('sort_field', sgqlc.types.Arg(ConceptPropertyTypeSorting, graphql_name='sortField', default='name')),
 ))
     )
 
 
-class RecordInterface(sgqlc.types.Interface):
-    __schema__ = utils_api_schema
-    __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
-    system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
-    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
-    creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
-    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
-
-
 class RedmineIssue(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('id', 'subject', 'tracker', 'status', 'priority', 'author', 'assignee', 'creation_date')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     subject = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='subject')
     tracker = sgqlc.types.Field(sgqlc.types.non_null('RedmineTracker'), graphql_name='tracker')
     status = sgqlc.types.Field(sgqlc.types.non_null('RedmineStatus'), graphql_name='status')
```

### Comparing `ptal_api-0.11.4.2/ptal_api/scripts/type_mapper.py` & `ptal_api-0.11.5/ptal_api/scripts/type_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,82 +2,96 @@
 import os
 from typing import Optional
 
 import click
 
 from ptal_api.core.type_mapper.data_model.base_data_model import TypeMapping
 
-
 current_directory_name = os.path.dirname(__file__)
 logging.config.fileConfig(
     f"{current_directory_name if current_directory_name else '.'}/../core/type_mapper/app_settings/logging.conf",
-    disable_existing_loggers=False
+    disable_existing_loggers=False,
 )
-logger = logging.getLogger('type_mapper')
+logger = logging.getLogger("type_mapper")
 
-graphql_uri = os.environ.get('GRAPHQL_URI', None)
-keykloak_auth_url = os.environ.get('KEYCLOAK_AUTH_URL', None)
-realm = os.environ.get('KEYCLOAK_REALM', None)
-cliend_id = os.environ.get('KEYCLOAK_CLIENT_ID', None)
-client_key = os.environ.get('KEYCLOAK_CLIENT_KEY', None)
-user = os.environ.get('KEYCLOAK_USER', None)
-pwd = os.environ.get('KEYCLOAK_PWD', None)
+graphql_uri = os.environ.get("GRAPHQL_URI", None)
+keykloak_auth_url = os.environ.get("KEYCLOAK_AUTH_URL", None)
+realm = os.environ.get("KEYCLOAK_REALM", None)
+cliend_id = os.environ.get("KEYCLOAK_CLIENT_ID", None)
+client_key = os.environ.get("KEYCLOAK_CLIENT_KEY", None)
+user = os.environ.get("KEYCLOAK_USER", None)
+pwd = os.environ.get("KEYCLOAK_PWD", None)
 
 
 @click.command()
-@click.option('--file_path', required=False, type=str, default=None,
-              help='The path to the file to be generated.'
-                   '\n\nExample: "./files/file_name.json". The default value is "./type_mapping/type_mapping.json".')
-@click.option('--custom_name_code_mapping_file_path', required=False, type=str, default=None,
-              help='The path to the custom name-code mapping file.'
-                   '\n\nExample: "./model_parameters/name_code_mapping.yml".')
+@click.option(
+    "--file_path",
+    required=False,
+    type=str,
+    default=None,
+    help="The path to the file to be generated."
+    '\n\nExample: "./files/file_name.json". The default value is "./type_mapping/type_mapping.json".',
+)
+@click.option(
+    "--custom_name_code_mapping_file_path",
+    required=False,
+    type=str,
+    default=None,
+    help="The path to the custom name-code mapping file." '\n\nExample: "./model_parameters/name_code_mapping.yml".',
+)
 def generate_type_mapping_file(
     file_path: Optional[str], custom_name_code_mapping_file_path: Optional[str]
 ) -> TypeMapping:
     from ptal_api.core.type_mapper.data_model.config_data_model import DefaultTypeCodeStorage, FileGenerationSettings
-    from ptal_api.core.type_mapper.modules.file_generator import FileGenerator
     from ptal_api.core.type_mapper.modules.custom_data_handler import CustomDataHandler
+    from ptal_api.core.type_mapper.modules.file_generator import FileGenerator
     from ptal_api.core.type_mapper.modules.type_mapping_generator import TypeMappingGenerator
 
     api_adapter = _generate_api_adapter()
     file_generation_settings = FileGenerationSettings()
     file_path = file_path if file_path else file_generation_settings.default_file_path
 
     default_type_code_storage = DefaultTypeCodeStorage()
 
     custom_type_code_storage = None
     if custom_name_code_mapping_file_path:
         custom_data_handler = CustomDataHandler(logger)
         custom_type_code_storage = custom_data_handler.get_custom_name_code_mapping(custom_name_code_mapping_file_path)
-        logger.info(f"The custom name-code mapping file \"{custom_name_code_mapping_file_path}\""
-                    f" has been successfully processed")
+        logger.info(
+            f'The custom name-code mapping file "{custom_name_code_mapping_file_path}"'
+            f" has been successfully processed"
+        )
 
     logger.info("The type name-code mapping process has started")
     type_mapping_generator = TypeMappingGenerator(
         api_adapter, logger, default_type_code_storage, custom_type_code_storage
     )
     type_mapping = type_mapping_generator.process_type_mapping()
     logger.info("The type name-code mapping process has completed successfully")
 
     logger.info("The output file generating process has begun")
     file_generator = FileGenerator(file_generation_settings, logger)
     file_generator.generate_file(type_mapping, file_path)
-    logger.info(f"The output file generating process has completed successfully"
-                f"\nThe output file: {file_path}")
+    logger.info(f"The output file generating process has completed successfully" f"\nThe output file: {file_path}")
     return type_mapping
 
 
 def _generate_api_adapter():
     from ptal_api.adapter import TalismanAPIAdapter
     from ptal_api.providers.gql_providers import KeycloakAwareGQLClient
 
     gql_client = KeycloakAwareGQLClient(
-        graphql_uri, 10000, 5,
+        graphql_uri,
+        10000,
+        5,
         auth_url=keykloak_auth_url,
-        realm=realm, client_id=cliend_id, user=user, pwd=pwd,
-        client_secret=client_key
+        realm=realm,
+        client_id=cliend_id,
+        user=user,
+        pwd=pwd,
+        client_secret=client_key,
     ).__enter__()
     return TalismanAPIAdapter(gql_client, None)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     generate_type_mapping_file()
```

### Comparing `ptal_api-0.11.4.2/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.11.5/ptal_api/tdm_builder/tdm_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Union
 
-from ..schema.api_schema import (
-    Concept, ConceptLink, ConceptProperty, ConceptPropertyType
-)
+from ..schema.api_schema import Concept, ConceptLink, ConceptProperty, ConceptPropertyType
 
 
 class AbstractTdmBuilder(ABC):
     def __init__(self, logger: logging.Logger) -> None:
         self.logger = logger
 
     @abstractmethod
     def reset_adding_restrictions(
-        self, add_concepts: bool = True, add_links: bool = True,
-        add_concept_properties: bool = True, add_link_properties: bool = True
+        self,
+        add_concepts: bool = True,
+        add_links: bool = True,
+        add_concept_properties: bool = True,
+        add_link_properties: bool = True,
     ):
         pass
 
     @abstractmethod
-    def build_tdm(
-        self, message: Union[str, dict], title: str, _uuid: str, url: str = None
-    ):
+    def build_tdm(self, message: Union[str, dict], title: str, _uuid: str, url: str = None):
         pass
 
     @abstractmethod
     def add_concept_fact(self, concept: Concept):
         pass
 
     @abstractmethod
     def add_link_fact(self, link: ConceptLink):
         pass
 
     @abstractmethod
     def add_concept_property_fact(
-        self, concept_property: ConceptProperty, concept: Concept,
-        value: Any, property_type: ConceptPropertyType
+        self, concept_property: ConceptProperty, concept: Concept, value: Any, property_type: ConceptPropertyType
     ):
         pass
 
     @abstractmethod
     def add_link_property_fact(
-        self, concept_property: ConceptProperty, link: ConceptLink,
-        value: Any, link_property_type: ConceptPropertyType
+        self, concept_property: ConceptProperty, link: ConceptLink, value: Any, link_property_type: ConceptPropertyType
     ):
         pass
```

### Comparing `ptal_api-0.11.4.2/PKG-INFO` & `ptal_api-0.11.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.4.2
+Version: 0.11.5
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

