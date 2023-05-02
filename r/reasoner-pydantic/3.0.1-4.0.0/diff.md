# Comparing `tmp/reasoner-pydantic-3.0.1.tar.gz` & `tmp/reasoner-pydantic-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reasoner-pydantic-3.0.1.tar", last modified: Tue Aug 30 18:00:38 2022, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.0.tar", last modified: Tue May  2 17:23:33 2023, max compression
```

## Comparing `reasoner-pydantic-3.0.1.tar` & `reasoner-pydantic-4.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-30 18:00:38.000000 reasoner-pydantic-3.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-30 18:00:38.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-30 18:00:37.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-30 18:00:37.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      310 2022-08-30 18:00:37.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       18 2022-08-30 18:00:37.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-08-30 18:00:37.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)      551 2022-08-30 18:00:37.000000 reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-30 18:00:38.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (116)     2864 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (116)     1191 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1517 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (116)     3922 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (116)    12049 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/workflow.py
--rw-r--r--   0 runner    (1001) docker     (116)     4373 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (116)     3826 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (116)     1209 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (116)      956 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3554 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-30 18:00:38.000000 reasoner-pydantic-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      500 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      310 2022-08-30 18:00:38.000000 reasoner-pydantic-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2782 2022-08-30 18:00:30.000000 reasoner-pydantic-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:33.167310 reasoner-pydantic-4.0.0/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 reasoner_pydantic/__init__.py
+reasoner_pydantic/auxgraphs.py
 reasoner_pydantic/base_model.py
 reasoner_pydantic/kgraph.py
 reasoner_pydantic/message.py
 reasoner_pydantic/metakg.py
 reasoner_pydantic/qgraph.py
 reasoner_pydantic/results.py
 reasoner_pydantic/shared.py
```

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/kgraph.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .shared import (
     Attribute,
     BiolinkEntity,
     BiolinkPredicate,
     CURIE,
     EdgeIdentifier,
     Qualifier,
+    ResourceRoleEnum,
 )
 from .base_model import BaseModel
 from .utils import HashableMapping, HashableSet
 
 
 class Node(BaseModel):
     """Knowledge graph node."""
@@ -49,39 +50,76 @@
         if other.attributes:
             if self.attributes:
                 self.attributes.update(other.attributes)
             else:
                 self.attributes = other.attributes
 
 
+class RetrievalSource(BaseModel):
+    """A component of source retrieval provenance"""
+
+    resource_id: CURIE = Field(..., title="infores for source")
+
+    resource_role: ResourceRoleEnum = Field(..., title="source type")
+
+    upstream_resource_ids: Optional[HashableSet[CURIE]] = Field(None, nullable=True)
+
+    source_record_urls: Optional[HashableSet[str]] = Field(None, nullable=True)
+
+
 class Edge(BaseModel):
     """Knowledge graph edge."""
 
     subject: CURIE = Field(
         ...,
         title="subject node id",
     )
     object: CURIE = Field(
         ...,
         title="object node id",
     )
-    predicate: Optional[BiolinkPredicate] = Field(None, nullable=True)
+    predicate: BiolinkPredicate = Field(..., title="edge predicate")
+    sources: HashableSet[RetrievalSource] = Field(
+        ..., title="list of source retrievals"
+    )
     qualifiers: Optional[HashableSet[Qualifier]] = Field(None, nullable=True)
     attributes: Optional[HashableSet[Attribute]] = Field(None, nullable=True)
 
     class Config:
         title = "knowledge-graph edge"
         extra = "forbid"
 
     def update(self, other):
         if other.attributes:
             if self.attributes:
                 self.attributes.update(other.attributes)
             else:
                 self.attributes = other.attributes
+        if other.sources:
+            if self.sources:
+                self.sources.update(other.sources)
+            else:
+                self.sources = other.sources
+
+    def get_primary_knowedge_source(self):
+        for source in self.sources:
+            if source.resource_role == "biolink:primary_knowledge_source":
+                return source.resource_id
+
+    def __hash__(self) -> int:
+        primary_knowledge_source = self.get_primary_knowedge_source()
+        return hash(
+            (
+                self.subject,
+                self.object,
+                self.predicate,
+                self.qualifiers,
+                primary_knowledge_source,
+            )
+        )
 
 
 class KnowledgeGraph(BaseModel):
     """Knowledge graph."""
 
     nodes: HashableMapping[CURIE, Node] = Field(
         ...,
```

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/shared.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 
 from pydantic import Field
 from pydantic.types import ConstrainedStr
 
 from .base_model import BaseModel
 from .utils import HashableSequence
 
+
 # TODO: potential add validation for structure of CURIE
 class CURIE(str):
     """Compact URI."""
 
 
+class ResourceRoleEnum(str, Enum):
+    """Types of resources"""
+
+    aggregator_knowledge_source = "biolink:aggregator_knowledge_source"
+    primary_knowledge_source = "biolink:primary_knowledge_source"
+    supporting_data_source = "biolink:supporting_data_source"
+
+
 class KnowledgeType(str, Enum):
     "Knowledge Type."
 
     lookup = "lookup"
     inferred = "inferred"
```

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/metakg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import validator
 from reasoner_pydantic.shared import CURIE, KnowledgeType
 from typing import Optional
 
-from reasoner_pydantic import BiolinkEntity, BiolinkPredicate
+from reasoner_pydantic import BiolinkEntity, BiolinkPredicate, BiolinkQualifier
 
 from .base_model import BaseModel
 from .utils import HashableMapping, HashableSequence, nonzero_validator
 
 
 class MetaAttribute(BaseModel):
     """MetaAttribute."""
@@ -23,20 +23,27 @@
     _nonzero_id_prefixes = validator("id_prefixes", allow_reuse=True)(nonzero_validator)
     attributes: Optional[HashableSequence[MetaAttribute]]
 
     class Config:
         extra = "forbid"
 
 
+class MetaQualifier(BaseModel):
+    qualifier_type_id: CURIE
+    applicable_values: Optional[HashableSequence[str]]
+
+
 class MetaEdge(BaseModel):
     subject: BiolinkEntity
     predicate: BiolinkPredicate
     object: BiolinkEntity
+    qualifiers: Optional[HashableSequence[MetaQualifier]]
     attributes: Optional[HashableSequence[MetaAttribute]]
     knowledge_types: Optional[HashableSequence[KnowledgeType]]
+    association: Optional[BiolinkEntity]
 
     class Config:
         extra = "forbid"
 
 
 class MetaKnowledgeGraph(BaseModel):
     nodes: HashableMapping[str, MetaNode]
```

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 from .kgraph import KnowledgeGraph, Node, Edge
 from .qgraph import (
     QueryGraph,
     QNode,
     QEdge,
     AttributeConstraint,
 )
-from .results import Result, NodeBinding, EdgeBinding
+from .results import Result, NodeBinding, EdgeBinding, Results
+from .auxgraphs import AuxiliaryGraphs, AuxiliaryGraph
 from .message import (
     Message,
     Query,
     Response,
     AsyncQuery,
 )
 from .workflow import (
     Operation,
     Workflow,
 )
 from .shared import (
     Attribute,
     BiolinkEntity,
     BiolinkPredicate,
+    BiolinkQualifier,
     CURIE,
     LogEntry,
     LogLevel,
 )
 from .metakg import (
     MetaEdge,
     MetaNode,
@@ -33,14 +35,15 @@
     MetaAttribute,
 )
 
 components = [
     Attribute,
     BiolinkEntity,
     BiolinkPredicate,
+    BiolinkQualifier,
     CURIE,
     Edge,
     EdgeBinding,
     KnowledgeGraph,
     LogEntry,
     Message,
     Node,
@@ -54,8 +57,11 @@
     Response,
     LogLevel,
     AttributeConstraint,
     MetaEdge,
     MetaNode,
     MetaKnowledgeGraph,
     MetaAttribute,
+    Results,
+    AuxiliaryGraph,
+    AuxiliaryGraphs,
 ]
```

### Comparing `reasoner-pydantic-3.0.1/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.0/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-3.0.1/README.md` & `reasoner-pydantic-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     knode = Node.parse_obj({"categories": ["biolink:FooBar"]})
     knode_id = "foo:bar"
     message.knowledge_graph.nodes[knode_id] = knode
 
     # add result
     result: Result = Result.parse_obj(
         {
-            "node_bindings": {qnode_id: [{"id": knode_id}]},
-            "edge_bindings": {},
+            "node_bindings": {qnode_id: [{"id": knode_id}]}
         }
     )
 
     message.results.add(result)
 
     return message.json()
```

