# Comparing `tmp/pyspmp-0.1.8.tar.gz` & `tmp/pyspmp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspmp-0.1.8.tar", max compression
+gzip compressed data, was "pyspmp-0.1.9.tar", max compression
```

## Comparing `pyspmp-0.1.8.tar` & `pyspmp-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      718 2023-05-02 19:02:49.849564 pyspmp-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      411 2023-05-02 18:57:32.822820 pyspmp-0.1.8/pyspmp/__init__.py
--rw-r--r--   0        0        0     5014 2023-05-02 19:04:56.771655 pyspmp-0.1.8/pyspmp/buscar_dados_pi.py
--rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/carregar_csv.py
--rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/dataset/dataset.csv
--rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/dataset.py
--rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/parametros/parametros.csv
--rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/parametros/parametros_pi.csv
--rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/periodos.py
--rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/variaveis_out.py
--rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.8/README.md
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 pyspmp-0.1.8/setup.py
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 pyspmp-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      722 2023-05-02 19:19:30.261972 pyspmp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      411 2023-05-02 19:19:36.870505 pyspmp-0.1.9/pyspmp/__init__.py
+-rw-r--r--   0        0        0     5038 2023-05-02 19:20:20.974460 pyspmp-0.1.9/pyspmp/buscar_dados_pi.py
+-rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/carregar_csv.py
+-rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/dataset/dataset.csv
+-rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/dataset.py
+-rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/parametros/parametros.csv
+-rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/parametros/parametros_pi.csv
+-rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/periodos.py
+-rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.9/pyspmp/variaveis_out.py
+-rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.9/README.md
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 pyspmp-0.1.9/setup.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pyspmp-0.1.9/PKG-INFO
```

### Comparing `pyspmp-0.1.8/pyproject.toml` & `pyspmp-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pyspmp"
-version = "0.1.8"
+version = "0.1.9"
 description = "Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos"
 authors = ["Leandro Ribeiro de Castro <lr.castro@yahoo.com.br>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pandas = "^1.4.3"
 clr = { version = "^1.0.3", optional = true }
 
 [tool.poetry.extras]
-clr = ["clr"]
+buscapi = ["clr"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.0.3"
 
 [build-system]
```

### Comparing `pyspmp-0.1.8/pyspmp/buscar_dados_pi.py` & `pyspmp-0.1.9/pyspmp/buscar_dados_pi.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,11 +102,11 @@
         # Exportando df com as TAGs fora dos parâmetros
 
         df_tags_out.to_csv(os.path.join(path,r'df_tagsout_' + equipamento + '_' + unidade + '.csv'),',')
 
         duration = fim_time - inicio_time
 
         return duration
-except:
+except ImportError:
     def buscar_dados(unidade, equipamento, server_name, inicio, final, time_span, df_parametros, path):
-        msg = 'Para usar essa função, instale-a usando pip install clr'
+        msg = 'Para usar essa função, instale-a usando pip install pyspmp[buscapi]'
         return msg
```

### Comparing `pyspmp-0.1.8/pyspmp/carregar_csv.py` & `pyspmp-0.1.9/pyspmp/carregar_csv.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/pyspmp/dataset/dataset.csv` & `pyspmp-0.1.9/pyspmp/dataset/dataset.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/pyspmp/dataset.py` & `pyspmp-0.1.9/pyspmp/dataset.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/pyspmp/parametros/parametros.csv` & `pyspmp-0.1.9/pyspmp/parametros/parametros.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/pyspmp/parametros/parametros_pi.csv` & `pyspmp-0.1.9/pyspmp/parametros/parametros_pi.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/pyspmp/periodos.py` & `pyspmp-0.1.9/pyspmp/periodos.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/pyspmp/variaveis_out.py` & `pyspmp-0.1.9/pyspmp/variaveis_out.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/README.md` & `pyspmp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.8/setup.py` & `pyspmp-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 package_data = \
 {'': ['*'], 'pyspmp': ['dataset/*', 'parametros/*']}
 
 install_requires = \
 ['pandas>=1.4.3,<2.0.0']
 
 extras_require = \
-{'clr': ['clr>=1.0.3,<2.0.0']}
+{'buscapi': ['clr>=1.0.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'pyspmp',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos',
     'long_description': '# PySPMP GitLab\n\n## Descrição\n\nEste projeto tem como objetivo realizar buscas e pré seleção de períodos dentro dos parâmentros definidos pelo usuário para modelos de monitoramento e predição de máquinas e equipamentos, visando mitigar e reduzir o esforço de trabalho do usuário na busca de períodos adequados para um bom modelo de monitoramento e predição.\n\n## Fonte\n\nA fonte do PySPMP é [hospedado em\nGitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).\n\n## Requisitos\n\npython = "^3.8.1"\npandas = "^1.4.3"\nclr = "^1.0.3"\n\n',
     'author': 'Leandro Ribeiro de Castro',
     'author_email': 'lr.castro@yahoo.com.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyspmp-0.1.8/PKG-INFO` & `pyspmp-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyspmp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos
 Author: Leandro Ribeiro de Castro
 Author-email: lr.castro@yahoo.com.br
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: clr
-Requires-Dist: clr (>=1.0.3,<2.0.0) ; extra == "clr"
+Provides-Extra: buscapi
+Requires-Dist: clr (>=1.0.3,<2.0.0) ; extra == "buscapi"
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PySPMP GitLab
 
 ## Descrição
```

