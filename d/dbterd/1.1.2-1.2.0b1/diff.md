# Comparing `tmp/dbterd-1.1.2.tar.gz` & `tmp/dbterd-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.1.2.tar", max compression
+gzip compressed data, was "dbterd-1.2.0b1.tar", max compression
```

## Comparing `dbterd-1.1.2.tar` & `dbterd-1.2.0b1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      203 2023-04-30 10:54:44.787016 dbterd-1.1.2/LICENSE
--rw-r--r--   0        0        0     4491 2023-04-30 10:54:44.787016 dbterd-1.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0     4465 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/base.py
--rw-r--r--   0        0        0     3157 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/filter.py
--rw-r--r--   0        0        0      545 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/meta.py
--rw-r--r--   0        0        0     2505 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     2561 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/base.py
--rw-r--r--   0        0        0      560 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      132 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      304 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0      168 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      316 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     1597 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      222 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     2026 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/cli/main.py
--rw-r--r--   0        0        0     1928 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/cli/params.py
--rw-r--r--   0        0        0      284 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4494 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-04-30 10:54:44.791016 dbterd-1.1.2/dbterd/main.py
--rw-r--r--   0        0        0     2095 2023-04-30 10:54:57.123205 dbterd-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 dbterd-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      203 2023-05-02 17:48:15.565293 dbterd-1.2.0b1/LICENSE
+-rw-r--r--   0        0        0     4473 2023-05-02 17:48:15.565293 dbterd-1.2.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     4896 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     3157 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/filter.py
+-rw-r--r--   0        0        0      571 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     2505 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     2561 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      560 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      304 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     1729 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      316 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     1597 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      222 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/cli/main.py
+-rw-r--r--   0        0        0     1928 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/cli/params.py
+-rw-r--r--   0        0        0      284 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4494 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/main.py
+-rw-r--r--   0        0        0     2097 2023-05-02 17:48:32.197444 dbterd-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 dbterd-1.2.0b1/PKG-INFO
```

### Comparing `dbterd-1.1.2/README.md` & `dbterd-1.2.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 dbterd run -ad "samples/facebookad" -o "target"
 dbterd run -ad "samples/facebookad" -o "target" -rt "model" -rt "source"
 
 dbterd run -ad "samples/shopify" -o "target"
 dbterd run -ad "samples/shopify" -o "target" -rt "model" -rt "source"
 
 # your own sample without commiting to repo
-dbterd run -mp "samples/local" -o "target" -rt "model" -rt "source"
+dbterd run -ad "samples/local" -o "target" -rt "model" -rt "source"
 ```
 
 ## Decide to exclude Relationship Tests from ERD generated
 Add `ignore_in_erd` attribute into your test's meta:
 ```yml
 version: 2
 
@@ -67,16 +67,16 @@
 ```bash
 dbt docs generate
 ```
 
 #### 2. Generate DBML
 Copy `manifest.json` into a specific folder, and run
 ```
-dbterd run -mp "/path/to/dbt/target" -o "/path/to/output"
-# dbterd run -mp "./target/v4-dbtresto" -o "./target" -s model.dbt_resto -ns model.dbt_resto.staging
+dbterd run -ad "/path/to/dbt/target" -o "/path/to/output"
+# dbterd run -ad "samples/dbtresto" -s model.dbt_resto -ns model.dbt_resto.staging
 ```
 
 File `./target/output.dbml` will be generated as the result
 
 #### 3. Build database docs site (Optional)
 Assuming you're already familiar with [dbdocs](https://dbdocs.io/docs#installation)
 ```
```

### Comparing `dbterd-1.1.2/dbterd/adapters/algos/base.py` & `dbterd-1.2.0b1/dbterd/adapters/algos/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,26 +91,37 @@
 
     if catalog_node:
         for column, metadata in catalog_node.columns.items():
             table.columns.append(
                 Column(
                     name=str(column).lower(),
                     data_type=str(metadata.type).lower(),
+                    description=metadata.comment or "",  # TODO escape quote
                 )
             )
 
     for column_name, column_metadata in manifest_node.columns.items():
         column_name = column_name.strip('"')
-        if not any(c.name.lower() == column_name.lower() for c in table.columns):
+        find_columns = [
+            c for c in table.columns if c.name.lower() == column_name.lower()
+        ]
+        if not find_columns:
             table.columns.append(
                 Column(
                     name=column_name.lower(),
                     data_type=str(column_metadata.data_type or "unknown").lower(),
+                    description=column_metadata.description or "",  # TODO escape quote
                 )
             )
+        else:
+            find_columns[0].description = (
+                find_columns[0].description
+                or column_metadata.description
+                or ""  # TODO escape quote
+            )
 
     if not table.columns:
         table.columns.append(Column())
 
     return table
```

### Comparing `dbterd-1.1.2/dbterd/adapters/algos/filter.py` & `dbterd-1.2.0b1/dbterd/adapters/algos/filter.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/adapters/algos/meta.py` & `dbterd-1.2.0b1/dbterd/adapters/algos/meta.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 @dataclass
 class Column:
     """Parsed Column object"""
 
     name: str = "unknown"
     data_type: str = "unknown"
+    description: str = ""
 
 
 @dataclass
 class Table:
     """Parsed Table object"""
 
     name: str
```

### Comparing `dbterd-1.1.2/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.2.0b1/dbterd/adapters/algos/test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/adapters/base.py` & `dbterd-1.2.0b1/dbterd/adapters/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/adapters/factory.py` & `dbterd-1.2.0b1/dbterd/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.2.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,27 @@
 
     # Build DBML content
     dbml = "//Tables (based on the selection criteria)\n"
     for table in tables:
         dbml += f"//--configured at schema: {table.database}.{table.schema}\n"
         dbml += """Table \"{table}\" {{\n{columns}\n}}\n""".format(
             table=table.name,
-            columns="\n".join([f'  "{x.name}" "{x.data_type}"' for x in table.columns]),
+            columns="\n".join(
+                [
+                    str.format(
+                        '"{0}" "{1}"{2}',
+                        x.name,
+                        x.data_type,
+                        str.format(" [note: {1}{0}{1}]", x.description, chr(34))
+                        if x.description
+                        else "",
+                    )
+                    for x in table.columns
+                ]
+            ),
         )
 
     dbml += "//Refs (based on the DBT Relationship Tests)\n"
     for rel in relationships:
         key_from = f'"{rel.table_map[1]}"."{rel.column_map[1]}"'
         key_to = f'"{rel.table_map[0]}"."{rel.column_map[0]}"'
         dbml += f"Ref: {key_from} > {key_to}\n"
```

### Comparing `dbterd-1.1.2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py` & `dbterd-1.2.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/cli/main.py` & `dbterd-1.2.0b1/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/cli/params.py` & `dbterd-1.2.0b1/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/helpers/cli_messaging.py` & `dbterd-1.2.0b1/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/helpers/dict.py` & `dbterd-1.2.0b1/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/helpers/file.py` & `dbterd-1.2.0b1/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/helpers/jsonify.py` & `dbterd-1.2.0b1/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/helpers/log.py` & `dbterd-1.2.0b1/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/dbterd/helpers/yaml.py` & `dbterd-1.2.0b1/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.2/pyproject.toml` & `dbterd-1.2.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.1.2"
+version = "1.2.0b1"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
```

### Comparing `dbterd-1.1.2/PKG-INFO` & `dbterd-1.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.1.2
+Version: 1.2.0b1
 Summary: dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -61,15 +61,15 @@
 dbterd run -ad "samples/facebookad" -o "target"
 dbterd run -ad "samples/facebookad" -o "target" -rt "model" -rt "source"
 
 dbterd run -ad "samples/shopify" -o "target"
 dbterd run -ad "samples/shopify" -o "target" -rt "model" -rt "source"
 
 # your own sample without commiting to repo
-dbterd run -mp "samples/local" -o "target" -rt "model" -rt "source"
+dbterd run -ad "samples/local" -o "target" -rt "model" -rt "source"
 ```
 
 ## Decide to exclude Relationship Tests from ERD generated
 Add `ignore_in_erd` attribute into your test's meta:
 ```yml
 version: 2
 
@@ -92,16 +92,16 @@
 ```bash
 dbt docs generate
 ```
 
 #### 2. Generate DBML
 Copy `manifest.json` into a specific folder, and run
 ```
-dbterd run -mp "/path/to/dbt/target" -o "/path/to/output"
-# dbterd run -mp "./target/v4-dbtresto" -o "./target" -s model.dbt_resto -ns model.dbt_resto.staging
+dbterd run -ad "/path/to/dbt/target" -o "/path/to/output"
+# dbterd run -ad "samples/dbtresto" -s model.dbt_resto -ns model.dbt_resto.staging
 ```
 
 File `./target/output.dbml` will be generated as the result
 
 #### 3. Build database docs site (Optional)
 Assuming you're already familiar with [dbdocs](https://dbdocs.io/docs#installation)
 ```
```

