# Comparing `tmp/ontogpt-0.2.2.tar.gz` & `tmp/ontogpt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.2.tar", max compression
+gzip compressed data, was "ontogpt-0.2.3.tar", max compression
```

## Comparing `ontogpt-0.2.2.tar` & `ontogpt-0.2.3.tar`

### file list

```diff
@@ -1,92 +1,102 @@
--rw-r--r--   0        0        0     1485 2023-04-21 22:19:33.094970 ontogpt-0.2.2/LICENSE
--rw-r--r--   0        0        0    11152 2023-04-21 22:19:33.094970 ontogpt-0.2.2/README.md
--rw-r--r--   0        0        0     2290 2023-04-21 22:20:30.911600 ontogpt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      219 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    30092 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     6962 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2921 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1122 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0       81 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5289 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0    15446 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/enrichment.py
--rw-r--r--   0        0        0    19185 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    23173 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      752 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0     3748 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/similarity_engine.py
--rw-r--r--   0        0        0    17537 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      719 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10390 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10670 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/enrichment/__init__.py
--rw-r--r--   0        0        0    12248 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/enrichment/eval_enrichment.py
--rw-r--r--   0        0        0     2950 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6164 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8973 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1191 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rw-r--r--   0        0        0     4791 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
--rwxr-xr-x   0        0        0       95 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0      586 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      386 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4329 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3255 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2350 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1440 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0      899 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0       68 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0      401 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/all.yaml
--rw-r--r--   0        0        0     5942 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     3593 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3098 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6210 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     5466 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6092 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2880 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     4709 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1613 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     8172 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6813 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     8165 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     6097 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5384 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7156 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5072 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     4887 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7501 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7222 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     7847 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2682 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    13362 1970-01-01 00:00:00.000000 ontogpt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-05-02 00:11:00.168373 ontogpt-0.2.3/LICENSE
+-rw-r--r--   0        0        0    11172 2023-05-02 00:11:00.168373 ontogpt-0.2.3/README.md
+-rw-r--r--   0        0        0     2330 2023-05-02 00:12:03.172317 ontogpt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    32137 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6962 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0    11314 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    23173 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0      752 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    17537 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    13318 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0      899 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1079 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0      993 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      560 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0       68 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/all.yaml
+-rw-r--r--   0        0        0     5942 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     2938 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     3593 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3098 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     5466 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     2880 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1614 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     4887 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     7847 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     5708 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/utils/gene_set_utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2722 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    13422 1970-01-01 00:00:00.000000 ontogpt-0.2.3/PKG-INFO
```

### Comparing `ontogpt-0.2.2/LICENSE` & `ontogpt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/README.md` & `ontogpt-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 
 Currently there are two different pipelines implemented:
 
 - SPIRES: Structured Prompt Interrogation and Recursive Extraction of Semantics
     - Zero-shot learning approach to extracting nested semantic structures from text
     - Inputs: [LinkML](https://linkml.io/) schema + text
     - Outputs: JSON, YAML, or RDF or OWL that conforms to the schema
-    - Uses text-davinci-003
+    - Uses text-davinci-003 or gpt-3.5-turbo (gtp-4 untested)
 - HALO: HAllucinating Latent Ontologies 
     - Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
     - Uses code-davinci-002
+- SPINDOCTOR: Structured Prompt Interpolation of Narrative Descriptions Or Controlled Terms for Ontological Reporting
+    - Summarize gene set descriptions (pseudo gene-set enrichment)
+    - Uses text-davinci-003 or  gpt-3.5-turbo (gtp-4 untested)
 
-SPIRES is described futher in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
+SPIRES is described further in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
 
 ## Citation
 
  - https://arxiv.org/abs/2304.02711
 
 ## SPIRES: Usage
 
@@ -330,27 +333,31 @@
 
 ## HALO: Usage
 
 TODO
 
 
 
-## Gene Enrichment
+## Gene Enrichment using SPINDOCTOR
 
 Given a set of genes, OntoGPT can find similarities among them.
 
 Example:
 ```
-ontogpt enrichment HGNC:8858 HGNC:8859 HGNC:9719
+ontogpt  enrichment -r sqlite:obo:hgnc  -U tests/input/genesets/sensory-ataxia.yaml
 ```
 
-Results:
+This gives both a narrative summary:
+
+__
+
+and structured term list:
 
 ```
-Commonality: Protein targeting to the Peroxisome. All the genes are involved in targeting proteins to the peroxisome membrane, matrix or both, and they are all located in cytoplasm; peroxisome; and/or endoplasmic reticulum. Additionally, they all enable different types of binding activity and/or hydrolysing activity which likely contribute to their roles in protein import
+
 ```
 
 ## OntoGPT Limitations
 
 ### Non-deterministic
 
 This relies on an existing LLM, and LLMs can be fickle in their responses.
```

### Comparing `ontogpt-0.2.2/pyproject.toml` & `ontogpt-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.2"
+version = "0.2.3"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 importlib = "^1.0.4"
 openai = "^0.27.4"
-oaklib = "^0.5.1"
+oaklib = "^0.5.2"
 gilda = "^0.10.3"
 jsonlines = "^3.1.0"
 python-multipart = "^0.0.5"
 linkml-owl = "^0.2.7"
 beautifulsoup4 = "^4.11.1"
 eutils = "^0.6.0"
 class-resolver = "*"
@@ -39,14 +39,15 @@
 sphinx-rtd-theme = {version = "^1.0.0", extras = ["docs"], optional = true}
 sphinx-autodoc-typehints = {version = "^1.19.4", extras = ["docs"], optional = true}
 sphinx-click = {version = "^4.3.0", extras = ["docs"], optional = true}
 myst-parser = {version = "^0.18.1", extras = ["docs"], optional = true}
 recipe-scrapers = {version = "^14.35.0", extras = ["recipes"], optional = true}
 cachier = "^2.1.0"
 wikipedia-api = "^0.5.8"
+rustsim = "^0.1.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 setuptools = ">=65.5.0"
 tox = "^3.25.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
 
@@ -70,14 +71,15 @@
 recipes = [
     "recipe-scrapers"
 ]
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 seaborn = "^0.12.2"
+papermill = "^2.4.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [tool.black]
```

### Comparing `ontogpt-0.2.2/src/ontogpt/cli.py` & `ontogpt-0.2.3/src/ontogpt/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Command line interface for oak-ai."""
 import codecs
 import logging
 import pickle
 import sys
+from copy import copy
 from dataclasses import dataclass
 from io import BytesIO, TextIOWrapper
 from pathlib import Path
 from typing import List, Optional
 
 import click
 import jsonlines
@@ -18,24 +19,25 @@
 
 from ontogpt import __version__
 from ontogpt.clients import OpenAIClient
 from ontogpt.clients.pubmed_client import PubmedClient
 from ontogpt.clients.soup_client import SoupClient
 from ontogpt.clients.wikipedia_client import WikipediaClient
 from ontogpt.engines import create_engine
-from ontogpt.engines.enrichment import EnrichmentEngine, GeneSet, parse_gene_set
+from ontogpt.engines.embedding_similarity_engine import SimilarityEngine
+from ontogpt.engines.enrichment import EnrichmentEngine
 from ontogpt.engines.halo_engine import HALOEngine
 from ontogpt.engines.knowledge_engine import KnowledgeEngine
-from ontogpt.engines.similarity_engine import SimilarityEngine
 from ontogpt.engines.spires_engine import SPIRESEngine
 from ontogpt.engines.synonym_engine import SynonymEngine
 from ontogpt.evaluation.enrichment.eval_enrichment import EvalEnrichment
 from ontogpt.evaluation.resolver import create_evaluator
 from ontogpt.io.html_exporter import HTMLExporter
 from ontogpt.io.markdown_exporter import MarkdownExporter
+from ontogpt.utils.gene_set_utils import GeneSet, parse_gene_set
 
 __all__ = [
     "main",
 ]
 
 from ontogpt.io.owl_exporter import OWLExporter
 from ontogpt.io.rdf_exporter import RDFExporter
@@ -101,14 +103,17 @@
 interactive_option = click.option(
     "--interactive/--no-interactive",
     default=False,
     show_default=True,
     help="Interactive mode - rather than call the LLM API it will prompt you do this.",
 )
 model_option = click.option("-m", "--model", help="Engine to use, e.g. text-davinci-003.")
+prompt_template_option = click.option(
+    "--prompt-template", help="Path to a file containing the prompt."
+)
 recurse_option = click.option(
     "--recurse/--no-recurse", default=True, show_default=True, help="Recursively parse structures."
 )
 output_option_wb = click.option(
     "-o", "--output", type=click.File(mode="wb"), default=sys.stdout, help="Output file."
 )
 output_option_txt = click.option(
@@ -510,14 +515,18 @@
 )
 @click.option(
     "--input-file",
     "-U",
     help="File with gene IDs to enrich (if not passed as arguments)",
 )
 @click.option(
+    "--randomize-gene-descriptions-using-file",
+    help="FOR EVALUATION ONLY. swap out gene descriptions with genes from this gene set filefile",
+)
+@click.option(
     "--ontological-synopsis/--no-ontological-synopsis",
     default=True,
     show_default=True,
     help="If set, use automated rather than manual gene descriptions",
 )
 @click.option(
     "--combined-synopsis/--no-combined-synopsis",
@@ -527,26 +536,28 @@
 )
 @click.option(
     "--annotations/--no-annotations",
     default=True,
     show_default=True,
     help="If set, include annotations in the prompt",
 )
+@prompt_template_option
 @interactive_option
 @click.argument("genes", nargs=-1)
 def enrichment(
     genes,
     context,
     input_file,
     resolver,
     output,
     model,
     show_prompt,
     interactive,
     output_format,
+    randomize_gene_descriptions_using_file,
     **kwargs,
 ):
     """Gene class enrichment.
 
     Algorithm:
 
     1. Map gene symbols to IDs using the resolver (unless IDs specified)
@@ -581,15 +592,32 @@
         ke.client.interactive = True
     if settings.cache_db:
         ke.client.cache_db_path = settings.cache_db
     if not isinstance(ke, EnrichmentEngine):
         raise ValueError(f"Expected EnrichmentEngine, got {type(ke)}")
     if resolver:
         ke.add_resolver(resolver)
-    results = ke.summarize(gene_set, normalize=resolver is not None, **kwargs)
+    if randomize_gene_descriptions_using_file:
+        print("WARNING!! Randomly spiking gene descriptions")
+        spike_gene_set = parse_gene_set(randomize_gene_descriptions_using_file)
+        aliases = {}
+        if not spike_gene_set.gene_symbols:
+            raise ValueError("No gene symbols for spike set")
+        syms = copy(gene_set.gene_symbols)
+        if len(spike_gene_set.gene_symbols) < len(gene_set.gene_symbols):
+            raise ValueError("Not enough genes in spike set")
+        for sym in spike_gene_set.gene_symbols:
+            if not syms:
+                break
+            aliases[sym] = syms.pop()
+        results = ke.summarize(
+            spike_gene_set, normalize=resolver is not None, gene_aliases=aliases, **kwargs
+        )
+    else:
+        results = ke.summarize(gene_set, normalize=resolver is not None, **kwargs)
     if results.truncation_factor is not None and results.truncation_factor < 1.0:
         logging.warning(f"Text was truncated; factor = {results.truncation_factor}")
     output = _as_text_writer(output)
     if show_prompt:
         print(results.prompt)
     output.write(dump_minimal_yaml(results))
 
@@ -778,14 +806,18 @@
 @click.option(
     "--number-to-drop",
     "-n",
     type=click.types.INT,
     default=1,
     help="Max number of genes to drop",
 )
+# @click.option(
+#    "--randomize-gene-descriptions/--no-randomize-gene-descriptions",
+#    help="DO NOT USE EXCEPT FOR EVALUATION PUPOSES."
+# )
 @click.option(
     "--annotations-path",
     "-A",
     default="tests/input/genes2go.tsv.gz",
     help="Path to annotations",
 )
 @click.argument("genes", nargs=-1)
@@ -797,23 +829,18 @@
         gene_set = GeneSet(name="TEMP", gene_symbols=genes)
     if input_file:
         if genes:
             raise ValueError("Either genes or input file must be passed")
         gene_set = parse_gene_set(input_file)
     if not gene_set:
         raise ValueError("No genes passed")
-    models = ["gpt-3.5-turbo", "text-davinci-003"]
-    all_comparisons = []
-    for model in models:
-        eval_engine = EvalEnrichment(model=model)
-        eval_engine.load_annotations(annotations_path)
-        print(f"RANDOM GENE: {eval_engine.random_gene_symbol()}")
-        comps = eval_engine.evaluate_methods_on_gene_set(gene_set, n=number_to_drop)
-        all_comparisons.extend([comp.dict() for comp in comps])
-    output.write(dump_minimal_yaml(all_comparisons))
+    eval_engine = EvalEnrichment()
+    eval_engine.load_annotations(annotations_path)
+    comps = eval_engine.evaluate_methods_on_gene_set(gene_set, n=number_to_drop, **kwargs)
+    output.write(dump_minimal_yaml(comps))
 
 
 @main.command()
 @model_option
 @recurse_option
 @output_option_txt
 @output_format_options
@@ -954,14 +981,50 @@
         context = engine.ontology.elements[0].context
     engine.fixed_slot_values = {"context": context}
     engine.hallucinate(terms, **kwargs)
     output.write(dump_minimal_yaml(engine.ontology))
 
 
 @main.command()
+@output_option_wb
+@output_format_options
+@click.option(
+    "-d",
+    "--description",
+    help="domain e.g. anatomy, industry, health-related (NOT IMPLEMENTED - currently gene only)",
+)
+@click.option(
+    "--sections", multiple=True, help="sections to include e.g. medications, vital signs, etc."
+)
+def clinical_notes(
+    description,
+    sections,
+    output,
+    output_format,
+    **kwargs,
+):
+    """Create mock clinical notes.
+
+    Example:
+
+        ontogpt clinical-notes -d "middle-aged female patient with diabetes"
+        ontogpt clinical-notes --description "middle-aged female patient with diabetes"\
+         --sections medications --sections "vital signs"
+
+    """
+    c = OpenAIClient()
+    prompt = "create mock clinical notes for a patient like this: " + description
+    if sections:
+        prompt += " including sections: " + ", ".join(sections)
+    results = c.complete(prompt)
+    print(results)
+    output.write(results)
+
+
+@main.command()
 def list_templates():
     """List the templates."""
     print("TODO")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ontogpt-0.2.2/src/ontogpt/clients/openai_client.py` & `ontogpt-0.2.3/src/ontogpt/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.3/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.3/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.2.3/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.3/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.3/src/ontogpt/engines/halo_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.3/src/ontogpt/engines/knowledge_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.3/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/engines/similarity_engine.py` & `ontogpt-0.2.3/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.3/src/ontogpt/engines/spires_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.3/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/enrichment/eval_enrichment.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/enrichment/eval_enrichment.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,47 +8,49 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, Iterator, List, Optional, Tuple
 
 import tiktoken
 import yaml
 from cachier import cachier
+from linkml_runtime.dumpers import json_dumper
 from oaklib import get_adapter, get_implementation_from_shorthand
 from oaklib.datamodels.association import Association
 from oaklib.datamodels.vocabulary import EQUIVALENT_CLASS, IS_A, PART_OF
 from oaklib.interfaces.class_enrichment_calculation_interface import (
     ClassEnrichmentCalculationInterface,
 )
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from pydantic import BaseModel
 from tiktoken import Encoding
 
 from ontogpt.engines import create_engine
-from ontogpt.engines.enrichment import (
-    ENTITY_ID,
+from ontogpt.engines.enrichment import ENTITY_ID, EnrichmentEngine
+from ontogpt.engines.knowledge_engine import MODEL_GPT_3_5_TURBO, MODEL_NAME, MODEL_TEXT_DAVINCI_003
+from ontogpt.evaluation.evaluation_engine import EvaluationEngine
+from ontogpt.templates.class_enrichment import ClassEnrichmentResult
+from ontogpt.utils.gene_set_utils import (
     SYMBOL,
-    EnrichmentEngine,
     EnrichmentPayload,
     GeneSet,
     gene_info,
     populate_ids_and_symbols,
 )
-from ontogpt.engines.knowledge_engine import MODEL_GPT_3_5_TURBO, MODEL_NAME, MODEL_TEXT_DAVINCI_003
-from ontogpt.evaluation.evaluation_engine import EvaluationEngine
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
 
 ONTOLOGICAL_SYNOPSIS = "ontological_synopsis"
 NARRATIVE_SYNOPSIS = "narrative_synopsis"
 NO_SYNOPSIS = "no_synopsis"
 STANDARD = "standard"
 STANDARD_NO_ONTOLOGY = "standard_no_ontology"
 RANDOM = "random"
 RANK_BASED = "rank_based"
+CLOSURE = "closure"
 
 ENRICHMENT_MODELS = [MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003]
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -98,25 +100,26 @@
         for model in ENRICHMENT_MODELS:
             self.engines[model] = create_engine(None, EnrichmentEngine, model=model)
             self.engines[model].add_resolver("sqlite:obo:hgnc")
         self.engine.add_resolver("sqlite:obo:hgnc")
         self.tokenizer_encoding = tiktoken.encoding_for_model(self.engine.model)
 
     def evaluate_methods_on_gene_set(
-        self, gene_set: GeneSet, max_size=999, n=4
+        self, gene_set: GeneSet, max_size=999, n=4, randomize_gene_descriptions=False, **kwargs
     ) -> List[GeneSetComparison]:
         """
         Perform evaluation of different methods on a gene set.
 
         Different permutations of the gene set are created, dropping out some members, and
         inserting random genes.
 
         :param gene_set: Gene set to evaluate
         :param max_size: Maximum size of gene set, above this the gene set will be truncated
         :param n: Number of dropouts to perform
+        :param randomize_gene_descriptions: use random gene descriptions
         """
         if n < 1:
             raise ValueError(f"n must be greater than 0: {n}")
         if n > 5:
             raise ValueError(f"n must be less than 5: {n}")
         name = gene_set.name
         hgnc = get_adapter("sqlite:obo:hgnc")
@@ -168,14 +171,15 @@
                 payload.method = method
                 model_method = f"{model}.{method}"
                 payloads[model_method] = payload
         payloads[STANDARD] = self.standard_enrichment(gene_set)
         payloads[STANDARD_NO_ONTOLOGY] = self.standard_enrichment(gene_set, use_ontology=False)
         payloads[RANDOM] = self.random_enrichment(gene_set)
         payloads[RANK_BASED] = self.null_enrichment(gene_set)
+        payloads[CLOSURE] = self.gene_term_closure(gene_set)
         for k in [STANDARD, STANDARD_NO_ONTOLOGY, RANDOM, RANK_BASED]:
             payloads[k].method = k
         comp = GeneSetComparison(
             name=name,
             gene_symbols=gene_symbols,
             payloads=payloads,
             **kwargs,
@@ -196,20 +200,34 @@
         if use_ontology:
             predicates = [IS_A, PART_OF]
         else:
             predicates = [EQUIVALENT_CLASS]  # TODO
         results = self.ontology.enriched_classes(
             gene_ids, autolabel=True, object_closure_predicates=predicates
         )
-        payload = EnrichmentPayload()
+        # awkward: convert from oaklib dataclasses to pydantic
+        results = [ClassEnrichmentResult(**json_dumper.to_dict(result)) for result in results]
+        payload = EnrichmentPayload(enrichment_results=results)
         for result in results:
+            if result.p_value_adjusted > 0.05:
+                continue
             payload.term_strings.append(result.class_label)
             payload.term_ids.append(result.class_id)
         return payload
 
+    def gene_term_closure(self, gene_set: GeneSet) -> EnrichmentPayload:
+        gene_ids = gene_set.gene_ids
+        term_ids = {a.object for a in self.ontology.associations(subjects=gene_ids)}
+        ancs = list(self.ontology.ancestors(list(term_ids), [IS_A, PART_OF]))
+        payload = EnrichmentPayload()
+        for anc in ancs:
+            payload.term_ids.append(anc)
+            payload.term_strings.append(self.ontology.label(anc))
+        return payload
+
     def random_enrichment(self, gene_set: GeneSet = None, n: int = None) -> EnrichmentPayload:
         """Randomized enrichment results."""
         if n is None:
             # by default, return a number of terms proportional to the number of genes
             if gene_set:
                 n = len(gene_set.gene_symbols)
             else:
```

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt` & `ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml` & `ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.3/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.3/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.3/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.3/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.2.3/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.2.3/src/ontogpt/io/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.3/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/core.py` & `ontogpt-0.2.3/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/core.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.3/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/drug.py` & `ontogpt-0.2.3/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -46,13 +46,13 @@
   GeneDescriptionTerm:
     tree_root: true
     is_a: NamedEntity
     attributes:
       label:
         description: the name of the GO term
     annotations:
-      annotators: sqlite:obo:go, sqlite:obo:mondo, sqlite:obo:uberon, bioportal:mesh
+      annotators: sqlite:obo:go, sqlite:obo:mondo, sqlite:obo:uberon, sqlite:obo:mesh
     id_prefixes:
       - GO
       - MONDO
       - UBERON
       - MESH
```

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.3/src/ontogpt/templates/gocam.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/halo.py` & `ontogpt-0.2.3/src/ontogpt/templates/halo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/ibd.py` & `ontogpt-0.2.3/src/ontogpt/templates/ibd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/ibd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.3/src/ontogpt/templates/ontology_class.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.3/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.3/src/ontogpt/templates/reaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.3/src/ontogpt/templates/recipe.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.3/src/ontogpt/templates/treatment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.3/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.3/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.2.3/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.2/src/ontogpt/webapp/main.py` & `ontogpt-0.2.3/src/ontogpt/webapp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 import uvicorn
 from fastapi import FastAPI, Form, Request
 from pydantic import BaseModel
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
 
-from ontogpt.engines.enrichment import EnrichmentEngine, GeneSet
+from ontogpt.engines.enrichment import EnrichmentEngine
 from ontogpt.engines.knowledge_engine import DATAMODELS, MODELS
 from ontogpt.engines.spires_engine import SPIRESEngine
 from ontogpt.io.html_exporter import HTMLExporter
+from ontogpt.utils.gene_set_utils import GeneSet
 
 this_path = Path(__file__).parent
 static_dir = this_path / "static"
 html_dir = this_path / "html"
 
 
 class Query(BaseModel):
```

### Comparing `ontogpt-0.2.2/PKG-INFO` & `ontogpt-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.2
+Version: 0.2.3
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -33,18 +33,19 @@
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: linkml (>=1.4.10,<2.0.0)
 Requires-Dist: linkml-owl (>=0.2.7,<0.3.0)
 Requires-Dist: linkml-runtime (>=1.4.9,<2.0.0)
 Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: nlpcloud (>=1.0.39,<2.0.0)
-Requires-Dist: oaklib (>=0.5.1,<0.6.0)
+Requires-Dist: oaklib (>=0.5.2,<0.6.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: recipe-scrapers[recipes] (>=14.35.0,<15.0.0) ; extra == "recipes"
+Requires-Dist: rustsim (>=0.1.8,<0.2.0)
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "web"
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
@@ -61,20 +62,23 @@
 
 Currently there are two different pipelines implemented:
 
 - SPIRES: Structured Prompt Interrogation and Recursive Extraction of Semantics
     - Zero-shot learning approach to extracting nested semantic structures from text
     - Inputs: [LinkML](https://linkml.io/) schema + text
     - Outputs: JSON, YAML, or RDF or OWL that conforms to the schema
-    - Uses text-davinci-003
+    - Uses text-davinci-003 or gpt-3.5-turbo (gtp-4 untested)
 - HALO: HAllucinating Latent Ontologies 
     - Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
     - Uses code-davinci-002
+- SPINDOCTOR: Structured Prompt Interpolation of Narrative Descriptions Or Controlled Terms for Ontological Reporting
+    - Summarize gene set descriptions (pseudo gene-set enrichment)
+    - Uses text-davinci-003 or  gpt-3.5-turbo (gtp-4 untested)
 
-SPIRES is described futher in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
+SPIRES is described further in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
 
 ## Citation
 
  - https://arxiv.org/abs/2304.02711
 
 ## SPIRES: Usage
 
@@ -383,27 +387,31 @@
 
 ## HALO: Usage
 
 TODO
 
 
 
-## Gene Enrichment
+## Gene Enrichment using SPINDOCTOR
 
 Given a set of genes, OntoGPT can find similarities among them.
 
 Example:
 ```
-ontogpt enrichment HGNC:8858 HGNC:8859 HGNC:9719
+ontogpt  enrichment -r sqlite:obo:hgnc  -U tests/input/genesets/sensory-ataxia.yaml
 ```
 
-Results:
+This gives both a narrative summary:
+
+__
+
+and structured term list:
 
 ```
-Commonality: Protein targeting to the Peroxisome. All the genes are involved in targeting proteins to the peroxisome membrane, matrix or both, and they are all located in cytoplasm; peroxisome; and/or endoplasmic reticulum. Additionally, they all enable different types of binding activity and/or hydrolysing activity which likely contribute to their roles in protein import
+
 ```
 
 ## OntoGPT Limitations
 
 ### Non-deterministic
 
 This relies on an existing LLM, and LLMs can be fickle in their responses.
```

