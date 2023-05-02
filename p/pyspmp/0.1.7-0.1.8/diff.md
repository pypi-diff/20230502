# Comparing `tmp/pyspmp-0.1.7.tar.gz` & `tmp/pyspmp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspmp-0.1.7.tar", max compression
+gzip compressed data, was "pyspmp-0.1.8.tar", max compression
```

## Comparing `pyspmp-0.1.7.tar` & `pyspmp-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      738 2023-05-02 18:18:41.102825 pyspmp-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      411 2023-05-02 18:45:21.475668 pyspmp-0.1.7/pyspmp/__init__.py
--rw-r--r--   0        0        0     5026 2023-05-02 18:46:04.126645 pyspmp-0.1.7/pyspmp/buscar_dados_pi.py
--rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/carregar_csv.py
--rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/dataset/dataset.csv
--rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/dataset.py
--rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/parametros/parametros.csv
--rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/parametros/parametros_pi.csv
--rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/periodos.py
--rw-r--r--   0        0        0    11306 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/resultado_busca/df_sp_TGA_P62.csv
--rw-r--r--   0        0        0   659569 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv
--rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/variaveis_out.py
--rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.7/README.md
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 pyspmp-0.1.7/setup.py
--rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 pyspmp-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      718 2023-05-02 19:02:49.849564 pyspmp-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      411 2023-05-02 18:57:32.822820 pyspmp-0.1.8/pyspmp/__init__.py
+-rw-r--r--   0        0        0     5014 2023-05-02 19:04:56.771655 pyspmp-0.1.8/pyspmp/buscar_dados_pi.py
+-rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/carregar_csv.py
+-rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/dataset/dataset.csv
+-rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/dataset.py
+-rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/parametros/parametros.csv
+-rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/parametros/parametros_pi.csv
+-rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/periodos.py
+-rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.8/pyspmp/variaveis_out.py
+-rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.8/README.md
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 pyspmp-0.1.8/setup.py
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 pyspmp-0.1.8/PKG-INFO
```

### Comparing `pyspmp-0.1.7/pyproject.toml` & `pyspmp-0.1.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [tool.poetry]
 name = "pyspmp"
-version = "0.1.7"
+version = "0.1.8"
 description = "Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos"
 authors = ["Leandro Ribeiro de Castro <lr.castro@yahoo.com.br>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pandas = "^1.4.3"
+clr = { version = "^1.0.3", optional = true }
 
-[tool.poetry.group.buscapi]
-optional = true
-
-[tool.poetry.group.buscapi.dependencies]
-clr = "^1.0.3"
+[tool.poetry.extras]
+clr = ["clr"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.0.3"
 
 [build-system]
```

### Comparing `pyspmp-0.1.7/pyspmp/buscar_dados_pi.py` & `pyspmp-0.1.8/pyspmp/buscar_dados_pi.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,9 +104,9 @@
         df_tags_out.to_csv(os.path.join(path,r'df_tagsout_' + equipamento + '_' + unidade + '.csv'),',')
 
         duration = fim_time - inicio_time
 
         return duration
 except:
     def buscar_dados(unidade, equipamento, server_name, inicio, final, time_span, df_parametros, path):
-        msg = 'Para usar essa função, instale-a usando pip install pyspmp[buscapi]'
+        msg = 'Para usar essa função, instale-a usando pip install clr'
         return msg
```

### Comparing `pyspmp-0.1.7/pyspmp/carregar_csv.py` & `pyspmp-0.1.8/pyspmp/carregar_csv.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/pyspmp/dataset/dataset.csv` & `pyspmp-0.1.8/pyspmp/dataset/dataset.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/pyspmp/dataset.py` & `pyspmp-0.1.8/pyspmp/dataset.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/pyspmp/parametros/parametros.csv` & `pyspmp-0.1.8/pyspmp/parametros/parametros.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/pyspmp/parametros/parametros_pi.csv` & `pyspmp-0.1.8/pyspmp/parametros/parametros_pi.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/pyspmp/periodos.py` & `pyspmp-0.1.8/pyspmp/periodos.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/pyspmp/variaveis_out.py` & `pyspmp-0.1.8/pyspmp/variaveis_out.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/README.md` & `pyspmp-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.7/setup.py` & `pyspmp-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pyspmp']
 
 package_data = \
-{'': ['*'], 'pyspmp': ['dataset/*', 'parametros/*', 'resultado_busca/*']}
+{'': ['*'], 'pyspmp': ['dataset/*', 'parametros/*']}
 
 install_requires = \
 ['pandas>=1.4.3,<2.0.0']
 
+extras_require = \
+{'clr': ['clr>=1.0.3,<2.0.0']}
+
 setup_kwargs = {
     'name': 'pyspmp',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos',
     'long_description': '# PySPMP GitLab\n\n## Descrição\n\nEste projeto tem como objetivo realizar buscas e pré seleção de períodos dentro dos parâmentros definidos pelo usuário para modelos de monitoramento e predição de máquinas e equipamentos, visando mitigar e reduzir o esforço de trabalho do usuário na busca de períodos adequados para um bom modelo de monitoramento e predição.\n\n## Fonte\n\nA fonte do PySPMP é [hospedado em\nGitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).\n\n## Requisitos\n\npython = "^3.8.1"\npandas = "^1.4.3"\nclr = "^1.0.3"\n\n',
     'author': 'Leandro Ribeiro de Castro',
     'author_email': 'lr.castro@yahoo.com.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyspmp-0.1.7/PKG-INFO` & `pyspmp-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pyspmp
-Version: 0.1.7
+Version: 0.1.8
 Summary: Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos
 Author: Leandro Ribeiro de Castro
 Author-email: lr.castro@yahoo.com.br
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: clr
+Requires-Dist: clr (>=1.0.3,<2.0.0) ; extra == "clr"
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PySPMP GitLab
 
 ## Descrição
```

