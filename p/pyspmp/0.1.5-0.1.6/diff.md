# Comparing `tmp/pyspmp-0.1.5.tar.gz` & `tmp/pyspmp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspmp-0.1.5.tar", max compression
+gzip compressed data, was "pyspmp-0.1.6.tar", max compression
```

## Comparing `pyspmp-0.1.5.tar` & `pyspmp-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      636 2023-04-10 17:08:35.824633 pyspmp-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      412 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/__init__.py
--rw-r--r--   0        0        0     4436 2023-04-10 17:07:38.706368 pyspmp-0.1.5/pyspmp/buscar_dados_pi.py
--rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/carregar_csv.py
--rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/dataset/dataset.csv
--rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/dataset.py
--rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/parametros/parametros.csv
--rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/parametros/parametros_pi.csv
--rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/periodos.py
--rw-r--r--   0        0        0    11306 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/resultado_busca/df_sp_TGA_P62.csv
--rw-r--r--   0        0        0   659569 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv
--rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.5/pyspmp/variaveis_out.py
--rw-r--r--   0        0        0      556 2023-03-17 13:58:59.000000 pyspmp-0.1.5/README.md
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pyspmp-0.1.5/setup.py
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 pyspmp-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      651 2023-05-02 14:07:48.990567 pyspmp-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      412 2023-05-02 14:07:55.149888 pyspmp-0.1.6/pyspmp/__init__.py
+-rw-r--r--   0        0        0     4436 2023-04-10 17:07:38.706368 pyspmp-0.1.6/pyspmp/buscar_dados_pi.py
+-rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/carregar_csv.py
+-rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/dataset/dataset.csv
+-rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/dataset.py
+-rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/parametros/parametros.csv
+-rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/parametros/parametros_pi.csv
+-rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/periodos.py
+-rw-r--r--   0        0        0    11306 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/resultado_busca/df_sp_TGA_P62.csv
+-rw-r--r--   0        0        0   659569 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv
+-rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/variaveis_out.py
+-rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.6/README.md
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 pyspmp-0.1.6/setup.py
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 pyspmp-0.1.6/PKG-INFO
```

### Comparing `pyspmp-0.1.5/pyspmp/buscar_dados_pi.py` & `pyspmp-0.1.6/pyspmp/buscar_dados_pi.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/carregar_csv.py` & `pyspmp-0.1.6/pyspmp/carregar_csv.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/dataset/dataset.csv` & `pyspmp-0.1.6/pyspmp/dataset/dataset.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/dataset.py` & `pyspmp-0.1.6/pyspmp/dataset.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/parametros/parametros.csv` & `pyspmp-0.1.6/pyspmp/parametros/parametros.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/parametros/parametros_pi.csv` & `pyspmp-0.1.6/pyspmp/parametros/parametros_pi.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/periodos.py` & `pyspmp-0.1.6/pyspmp/periodos.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/resultado_busca/df_sp_TGA_P62.csv` & `pyspmp-0.1.6/pyspmp/resultado_busca/df_sp_TGA_P62.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv` & `pyspmp-0.1.6/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/pyspmp/variaveis_out.py` & `pyspmp-0.1.6/pyspmp/variaveis_out.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.5/README.md` & `pyspmp-0.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,10 +7,11 @@
 ## Fonte
 
 A fonte do PySPMP é [hospedado em
 GitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).
 
 ## Requisitos
 
-python = "^3.9"
+python = "^3.8.1"
 pandas = "^1.4.3"
+clr = "^1.0.3"
```

### Comparing `pyspmp-0.1.5/setup.py` & `pyspmp-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['pyspmp']
 
 package_data = \
 {'': ['*'], 'pyspmp': ['dataset/*', 'parametros/*', 'resultado_busca/*']}
 
 install_requires = \
-['pandas>=1.4.3,<2.0.0']
+['clr>=1.0.3,<2.0.0', 'pandas>=1.4.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyspmp',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos',
-    'long_description': '# PySPMP GitLab\n\n## Descrição\n\nEste projeto tem como objetivo realizar buscas e pré seleção de períodos dentro dos parâmentros definidos pelo usuário para modelos de monitoramento e predição de máquinas e equipamentos, visando mitigar e reduzir o esforço de trabalho do usuário na busca de períodos adequados para um bom modelo de monitoramento e predição.\n\n## Fonte\n\nA fonte do PySPMP é [hospedado em\nGitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).\n\n## Requisitos\n\npython = "^3.9"\npandas = "^1.4.3"\n\n',
+    'long_description': '# PySPMP GitLab\n\n## Descrição\n\nEste projeto tem como objetivo realizar buscas e pré seleção de períodos dentro dos parâmentros definidos pelo usuário para modelos de monitoramento e predição de máquinas e equipamentos, visando mitigar e reduzir o esforço de trabalho do usuário na busca de períodos adequados para um bom modelo de monitoramento e predição.\n\n## Fonte\n\nA fonte do PySPMP é [hospedado em\nGitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).\n\n## Requisitos\n\npython = "^3.8.1"\npandas = "^1.4.3"\nclr = "^1.0.3"\n\n',
     'author': 'Leandro Ribeiro de Castro',
     'author_email': 'lr.castro@yahoo.com.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyspmp-0.1.5/PKG-INFO` & `pyspmp-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyspmp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos
 Author: Leandro Ribeiro de Castro
 Author-email: lr.castro@yahoo.com.br
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: clr (>=1.0.3,<2.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PySPMP GitLab
 
 ## Descrição
 
@@ -21,11 +22,12 @@
 ## Fonte
 
 A fonte do PySPMP é [hospedado em
 GitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).
 
 ## Requisitos
 
-python = "^3.9"
+python = "^3.8.1"
 pandas = "^1.4.3"
+clr = "^1.0.3"
```

