# Comparing `tmp/fairscape_cli-0.1.4.tar.gz` & `tmp/fairscape_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.4.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.5.tar", max compression
```

## Comparing `fairscape_cli-0.1.4.tar` & `fairscape_cli-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0        0 2023-03-27 17:10:03.768235 fairscape_cli-0.1.4/fairscape_cli/cli.py
--rw-r--r--   0        0        0      397 2023-03-27 17:19:39.488146 fairscape_cli-0.1.4/fairscape_cli/main.py
--rw-r--r--   0        0        0      221 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0      291 2023-04-05 21:07:55.345808 fairscape_cli-0.1.4/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/models/models.py
--rw-r--r--   0        0        0      924 2023-04-06 16:03:52.996807 fairscape_cli-0.1.4/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0      128 2023-04-05 21:07:30.355812 fairscape_cli-0.1.4/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    14576 2023-04-07 17:58:08.150148 fairscape_cli-0.1.4/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-04-07 16:01:30.543608 fairscape_cli-0.1.4/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1476 2023-04-07 18:56:09.799649 fairscape_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 fairscape_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0      397 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/main.py
+-rw-r--r--   0        0        0      221 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0      924 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0    12386 2023-05-02 17:00:11.896184 fairscape_cli-0.1.5/fairscape_cli/models/schema.py
+-rw-r--r--   0        0        0      128 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    14880 2023-05-02 17:50:35.055165 fairscape_cli-0.1.5/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-04-17 19:02:18.839104 fairscape_cli-0.1.5/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1534 2023-05-02 17:11:26.855959 fairscape_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5/PKG-INFO
```

### Comparing `fairscape_cli-0.1.4/LICENSE` & `fairscape_cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/README.md` & `fairscape_cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.5/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/models/rocrate.py` & `fairscape_cli-0.1.5/fairscape_cli/models/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/rocrate/rocrate.py` & `fairscape_cli-0.1.5/fairscape_cli/rocrate/rocrate.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,27 +37,30 @@
 def validate():
     pass
 
 @rocrate.command('zip')
 def zip():
     pass
 
+
 @rocrate.command('create')
 @click.option('--guid', required=False, type=str, default="", show_default=False)
-@click.option('--name', required=True, type=str)
-@click.option('--organization-name', required=True, type=str)
-@click.option('--project-name', required=True, type=str)
+@click.option('--name', required=True, type=str, prompt = "ROCrate Name (e.g. B2AI_ROCRATE)")
+@click.option('--organization-name', required=True, type=str, prompt = "Organization Name")
+@click.option('--project-name', required=True, type=str, prompt = "Project Name")
 @click.argument('crate-path', type=click.Path(exists=False, path_type=pathlib.Path))
 def create(
     guid: str,
     name: str,
     organization_name: str,
     project_name: str,
     crate_path: pathlib.Path, 
 ): 
+    '''
+    '''
 
 
     organization_guid = f"ark:/{organization_name.replace(' ', '_')}"
     project_guid = organization_guid + f"/{project_name.replace(' ', '_')}"
 
     if guid == "":
         guid = project_guid + f"/{name.replace(' ', '_')}"
@@ -117,32 +120,32 @@
 
 
 
 ##########################
 # RO Crate add subcommands
 ##########################
 
-def add_element_ro_crate():
+def add_element_ro_crate(element: Union[Dataset,Computation,Software], ro_crate: pathlib.Path):
     pass
 
 # RO Crate add subcommands
 @rocrate.group('add')
 def add():
     pass
 
 
 @add.command('software')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, type=str, default="", show_default=False)
-@click.option('--name', required=True)
-@click.option('--author', required=True)
-@click.option('--version', required=True)
-@click.option('--description', required=True)
-@click.option('--file-format', required=True)
-@click.option('--url', required=False)
+@click.option('--name',    required=True, prompt = "Software Name")
+@click.option('--author',  required=True, prompt = "Author Name")
+@click.option('--version', required=True, prompt = "Software Version")
+@click.option('--description', required = True, prompt = "Software Description")
+@click.option('--file-format', required = True, prompt = "File Format of Software")
+@click.option('--url',     required = False)
 @click.option('--source-filepath', required=False)
 @click.option('--destination-filepath', required=False)
 @click.option('--date-modified', required=False)
 @click.option('--used-by-computation', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def software(
@@ -150,16 +153,16 @@
     guid: str,
     name: str,
     author: str,
     version: str,
     description: str, 
     file_format: str,
     url: str,
-    source_path: str,
-    destination_path: str,
+    source_filepath: str,
+    destination_filepath: str,
     date_modified: str,
     used_by_computation: Optional[List[str]],
     associated_publication: Optional[str],
     additional_documentation: Optional[str]
 ):
 
 
@@ -256,23 +259,23 @@
 
     # TODO add to cache
 
 
 @add.command('dataset')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, default="", type=str)
-@click.option('--name', required=True)
+@click.option('--name', required=True, prompt="Dataset Name")
 @click.option('--url', required=False)
-@click.option('--author', required=True)
-@click.option('--version', required=True)
-@click.option('--date-published', required=True)
-@click.option('--description', required=True)
-@click.option('--data-format', required=True)
-@click.option('--source-filepath', required=True)
-@click.option('--destination-filepath', required=True)
+@click.option('--author', required=True, prompt="Dataset Author")
+@click.option('--version', required=True, prompt="Dataset Version")
+@click.option('--date-published', required=True, prompt="Date Published")
+@click.option('--description', required=True, prompt="Dataset Description")
+@click.option('--data-format', required=True, prompt="Data Format i.e. (csv, tsv)")
+@click.option('--source-filepath', required=False)
+@click.option('--destination-filepath', required=False)
 @click.option('--used-by', required=False, multiple=True)
 @click.option('--derived-from', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def dataset(
     rocrate_path: pathlib.Path,
     guid: str,
@@ -386,19 +389,19 @@
     # TODO add to cache
     
 
 
 @add.command('computation')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, default="", type=str, show_default=False)
-@click.option('--name', required=True)
-@click.option('--run-by', required=True)
-@click.option('--command', required=False)
-@click.option('--date-created', required=True)
-@click.option('--description', required=True)
+@click.option('--name', required=True, prompt="Computation Name")
+@click.option('--run-by', required=True, prompt="Computation Run By")
+@click.option('--command', required=False, prompt="Command")
+@click.option('--date-created', required=True, prompt="Date Created")
+@click.option('--description', required=True, prompt="Computation Description")
 @click.option('--used-software', required=False, multiple=True)
 @click.option('--used-dataset', required=False, multiple=True)
 @click.option('--generated', required=False, multiple=True)
 def computation(
     rocrate_path: pathlib.Path,
     guid: str,
     name: str,
@@ -461,18 +464,7 @@
 
 
     except ValidationError as e:
         click.echo("Computation Validation Error")
         click.echo(e)
         click.Abort()
 
-###############################################
-# Interactive propmpt for missing metadata
-###############################################
-
-@rocrate.group('add-prompt')
-def add_prompt():
-    """
-    Add an element with interactive prompts for input from the user.
-    Temporary as individual command will be merged as a seperate flag
-    """
-    pass
```

### Comparing `fairscape_cli-0.1.4/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.5/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.5/fairscape_cli/validate/validate_json.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.4/pyproject.toml` & `fairscape_cli-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,43 +17,46 @@
 dependencies = [
         "pydantic",
         "fairscape-models",
         "typer[all]",
         "pydantic",
         "pyld"
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
 authors = ["mlev71 <max.adam.levinson@gmail.com>"]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "fairscape_cli"}]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 pydantic = "^1.10.7"
 pyld = "^2.0.3"
 click = "^8.1.3"
 fairscape-models = "^0.1.2"
+imageio = "^2.27.0"
+pandas = "^2.0.0"
 
 
 [tool.poetry.scripts]
-fairscape-cli = "fairscape_cli.main:app"
+fairscape-cli = "fairscape_cli.main:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.test]
 
 [tool.poetry.group.test.dependencies]
 pytest= "^7.2.2"
+autopep8 = "^2.0.2"
```

### Comparing `fairscape_cli-0.1.4/PKG-INFO` & `fairscape_cli-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
 Author: mlev71
 Author-email: max.adam.levinson@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fairscape-models (>=0.1.2,<0.2.0)
+Requires-Dist: imageio (>=2.27.0,<3.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyld (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # fairscape-cli
 Data Validation and Packaging utility for sending evidence graphs to FAIRSCAPE
```

