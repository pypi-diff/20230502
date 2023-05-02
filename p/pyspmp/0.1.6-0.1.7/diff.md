# Comparing `tmp/pyspmp-0.1.6.tar.gz` & `tmp/pyspmp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspmp-0.1.6.tar", max compression
+gzip compressed data, was "pyspmp-0.1.7.tar", max compression
```

## Comparing `pyspmp-0.1.6.tar` & `pyspmp-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      651 2023-05-02 14:07:48.990567 pyspmp-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      412 2023-05-02 14:07:55.149888 pyspmp-0.1.6/pyspmp/__init__.py
--rw-r--r--   0        0        0     4436 2023-04-10 17:07:38.706368 pyspmp-0.1.6/pyspmp/buscar_dados_pi.py
--rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/carregar_csv.py
--rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/dataset/dataset.csv
--rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/dataset.py
--rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/parametros/parametros.csv
--rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/parametros/parametros_pi.csv
--rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/periodos.py
--rw-r--r--   0        0        0    11306 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/resultado_busca/df_sp_TGA_P62.csv
--rw-r--r--   0        0        0   659569 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv
--rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.6/pyspmp/variaveis_out.py
--rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.6/README.md
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 pyspmp-0.1.6/setup.py
--rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 pyspmp-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      738 2023-05-02 18:18:41.102825 pyspmp-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      411 2023-05-02 18:45:21.475668 pyspmp-0.1.7/pyspmp/__init__.py
+-rw-r--r--   0        0        0     5026 2023-05-02 18:46:04.126645 pyspmp-0.1.7/pyspmp/buscar_dados_pi.py
+-rw-r--r--   0        0        0      717 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/carregar_csv.py
+-rw-r--r--   0        0        0  8285393 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/dataset/dataset.csv
+-rw-r--r--   0        0        0     4001 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/dataset.py
+-rw-r--r--   0        0        0     8511 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/parametros/parametros.csv
+-rw-r--r--   0        0        0     8588 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/parametros/parametros_pi.csv
+-rw-r--r--   0        0        0     2532 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/periodos.py
+-rw-r--r--   0        0        0    11306 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/resultado_busca/df_sp_TGA_P62.csv
+-rw-r--r--   0        0        0   659569 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv
+-rw-r--r--   0        0        0     1870 2023-03-17 13:58:59.000000 pyspmp-0.1.7/pyspmp/variaveis_out.py
+-rw-r--r--   0        0        0      573 2023-05-02 14:07:07.071542 pyspmp-0.1.7/README.md
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 pyspmp-0.1.7/setup.py
+-rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 pyspmp-0.1.7/PKG-INFO
```

### Comparing `pyspmp-0.1.6/pyspmp/buscar_dados_pi.py` & `pyspmp-0.1.7/pyspmp/buscar_dados_pi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,112 @@
-import sys  
-import clr
-import os
-from datetime import datetime, timedelta
-import pandas as pd
-sys.path.append('C:\\Program Files (x86)\\PIPC\\AF\\PublicAssemblies\\4.0\\')
-clr.AddReference('OSIsoft.AFSDK')
-from OSIsoft.AF.PI import PIServer, PIPoint
-from OSIsoft.AF.Time import AFTimeRange, AFTimeSpan
-import warnings
-warnings.simplefilter(action='ignore', category=FutureWarning)
-warnings.simplefilter(action='ignore', category=pd.errors.PerformanceWarning)
-
-
-def buscar_dados(unidade, equipamento, server_name, inicio, final, time_span, df_parametros, path):
-
-    pi_server = PIServer.FindPIServer(server_name)
-    timerange = AFTimeRange(inicio, final)    
-    span = AFTimeSpan.Parse(time_span) # Intervalo na busca dos resultados
-
-    tag_date_out = []
-    tag_name_out = []
-    tag_point_in = []
-    tag_pl_out = []
-    tag_ph_out = []
-    df_day = pd.DataFrame.from_dict({
-                'Data': [],
-                'Point In': [],
-                'TAGs Out': [],
-                'Total TAGs': []
-            })
-
-    def daterange(start_date, end_date):
-        for n in range(int((end_date - start_date).days) + 1):
-            yield start_date + timedelta(n)
-
-    inicio_time = datetime.now()
-    start_date = datetime.strptime(inicio,'%d/%m/%Y %H:%M:%S')
-    end_date = datetime.strptime(final,'%d/%m/%Y %H:%M:%S')
-    for date_range in daterange(start_date, end_date):
-        point_in_t = 0
-        point_count_t = 0
-        tag_out = 0
-        if date_range == start_date:
-            data_i = inicio
-            data_f = str((date_range + timedelta(days=1)).strftime("%d/%m/%Y") + ' 00:00:00')
-        elif date_range == end_date:
-            data_i = str(date_range.strftime("%d/%m/%Y") + ' 00:00:00')
-            data_f = end_date
-        else:
-            data_i = str(date_range.strftime("%d/%m/%Y") + ' 00:00:00')
-            data_f = str((date_range + timedelta(days=1)).strftime("%d/%m/%Y") + ' 00:00:00')
-        
-        if date_range != datetime.strptime(final,'%d/%m/%Y 00:00:00'):
-
-            for row in range(0, df_parametros.shape[0]):
-                tagname = df_parametros.iat[row, 0]
-                pl = float(df_parametros.iat[row, 2])
-                ph = float(df_parametros.iat[row, 3])
-                tag = PIPoint.FindPIPoint(pi_server, tagname)  
-                timerange = AFTimeRange(data_i, data_f) 
-                V = []
-                V.append(tag.InterpolatedValues(timerange, span, "" , False,))    
-                T= []
-                t= []
-                for dado in V:
-                    for value in dado:
-                        if isinstance(value.Value,float):
-                            T.append(float(value.Value))
-                            t.append(datetime.strptime(str(value.Timestamp),'%d/%m/%Y %H:%M:%S'))
-                        else:
-                            T.append(0)
-                            t.append(datetime.strptime(str(value.Timestamp),'%d/%m/%Y %H:%M:%S'))
-
-                df_tags = pd.DataFrame({tagname:T}, index = t)
-                point_count= df_tags.count()
-                point_in = df_tags[(df_tags[tagname] >= pl) & (df_tags[tagname] <= ph)].count()
-                perc_in = point_in.item() / point_count.item()
-                
-                if perc_in < 1:
-                    tag_out = tag_out + 1
-                    tag_date_out.append(str(date_range.strftime("%d/%m/%Y")))
-                    tag_name_out.append(tagname)
-                    tag_point_in.append(perc_in)
-                    tag_pl_out.append(pl)
-                    tag_ph_out.append(ph)
-                    df_tags_out = pd.DataFrame({'Data':tag_date_out, 'TAGs':tag_name_out, 'Point In':tag_point_in , 'PL':tag_pl_out, 'PH':tag_ph_out})
-                point_in_t = point_in_t + point_in.item()
-                point_count_t = point_count_t + point_count.item()
-                
-            perc_in_t = point_in_t / point_count_t
+try:
+    import sys  
+    import clr
+    import os
+    from datetime import datetime, timedelta
+    import pandas as pd
+    sys.path.append('C:\\Program Files (x86)\\PIPC\\AF\\PublicAssemblies\\4.0\\')
+    clr.AddReference('OSIsoft.AFSDK')
+    from OSIsoft.AF.PI import PIServer, PIPoint
+    from OSIsoft.AF.Time import AFTimeRange, AFTimeSpan
+    import warnings
+    warnings.simplefilter(action='ignore', category=FutureWarning)
+    warnings.simplefilter(action='ignore', category=pd.errors.PerformanceWarning)
+
+
+    def buscar_dados(unidade, equipamento, server_name, inicio, final, time_span, df_parametros, path):
+
+        pi_server = PIServer.FindPIServer(server_name)
+        timerange = AFTimeRange(inicio, final)    
+        span = AFTimeSpan.Parse(time_span) # Intervalo na busca dos resultados
+
+        tag_date_out = []
+        tag_name_out = []
+        tag_point_in = []
+        tag_pl_out = []
+        tag_ph_out = []
+        df_day = pd.DataFrame.from_dict({
+                    'Data': [],
+                    'Point In': [],
+                    'TAGs Out': [],
+                    'Total TAGs': []
+                })
+
+        def daterange(start_date, end_date):
+            for n in range(int((end_date - start_date).days) + 1):
+                yield start_date + timedelta(n)
+
+        inicio_time = datetime.now()
+        start_date = datetime.strptime(inicio,'%d/%m/%Y %H:%M:%S')
+        end_date = datetime.strptime(final,'%d/%m/%Y %H:%M:%S')
+        for date_range in daterange(start_date, end_date):
+            point_in_t = 0
+            point_count_t = 0
+            tag_out = 0
+            if date_range == start_date:
+                data_i = inicio
+                data_f = str((date_range + timedelta(days=1)).strftime("%d/%m/%Y") + ' 00:00:00')
+            elif date_range == end_date:
+                data_i = str(date_range.strftime("%d/%m/%Y") + ' 00:00:00')
+                data_f = end_date
+            else:
+                data_i = str(date_range.strftime("%d/%m/%Y") + ' 00:00:00')
+                data_f = str((date_range + timedelta(days=1)).strftime("%d/%m/%Y") + ' 00:00:00')
             
-            df_day.loc[len(df_day)] = [str(date_range.strftime("%d/%m/%Y")), perc_in_t, tag_out, df_parametros.shape[0]]
+            if date_range != datetime.strptime(final,'%d/%m/%Y 00:00:00'):
+
+                for row in range(0, df_parametros.shape[0]):
+                    tagname = df_parametros.iat[row, 0]
+                    pl = float(df_parametros.iat[row, 2])
+                    ph = float(df_parametros.iat[row, 3])
+                    tag = PIPoint.FindPIPoint(pi_server, tagname)  
+                    timerange = AFTimeRange(data_i, data_f) 
+                    V = []
+                    V.append(tag.InterpolatedValues(timerange, span, "" , False,))    
+                    T= []
+                    t= []
+                    for dado in V:
+                        for value in dado:
+                            if isinstance(value.Value,float):
+                                T.append(float(value.Value))
+                                t.append(datetime.strptime(str(value.Timestamp),'%d/%m/%Y %H:%M:%S'))
+                            else:
+                                T.append(0)
+                                t.append(datetime.strptime(str(value.Timestamp),'%d/%m/%Y %H:%M:%S'))
+
+                    df_tags = pd.DataFrame({tagname:T}, index = t)
+                    point_count= df_tags.count()
+                    point_in = df_tags[(df_tags[tagname] >= pl) & (df_tags[tagname] <= ph)].count()
+                    perc_in = point_in.item() / point_count.item()
+                    
+                    if perc_in < 1:
+                        tag_out = tag_out + 1
+                        tag_date_out.append(str(date_range.strftime("%d/%m/%Y")))
+                        tag_name_out.append(tagname)
+                        tag_point_in.append(perc_in)
+                        tag_pl_out.append(pl)
+                        tag_ph_out.append(ph)
+                        df_tags_out = pd.DataFrame({'Data':tag_date_out, 'TAGs':tag_name_out, 'Point In':tag_point_in , 'PL':tag_pl_out, 'PH':tag_ph_out})
+                    point_in_t = point_in_t + point_in.item()
+                    point_count_t = point_count_t + point_count.item()
+                    
+                perc_in_t = point_in_t / point_count_t
+                
+                df_day.loc[len(df_day)] = [str(date_range.strftime("%d/%m/%Y")), perc_in_t, tag_out, df_parametros.shape[0]]
 
-    fim_time = datetime.now()
+        fim_time = datetime.now()
 
-    # Exportando df da para seleção de períodos
+        # Exportando df da para seleção de períodos
 
-    df_day.to_csv(os.path.join(path,r'df_sp_' + equipamento + '_' + unidade + '.csv'),',')
+        df_day.to_csv(os.path.join(path,r'df_sp_' + equipamento + '_' + unidade + '.csv'),',')
 
-    # Exportando df com as TAGs fora dos parâmetros
+        # Exportando df com as TAGs fora dos parâmetros
 
-    df_tags_out.to_csv(os.path.join(path,r'df_tagsout_' + equipamento + '_' + unidade + '.csv'),',')
+        df_tags_out.to_csv(os.path.join(path,r'df_tagsout_' + equipamento + '_' + unidade + '.csv'),',')
 
-    duration = fim_time - inicio_time
+        duration = fim_time - inicio_time
 
-    return duration
+        return duration
+except:
+    def buscar_dados(unidade, equipamento, server_name, inicio, final, time_span, df_parametros, path):
+        msg = 'Para usar essa função, instale-a usando pip install pyspmp[buscapi]'
+        return msg
```

### Comparing `pyspmp-0.1.6/pyspmp/carregar_csv.py` & `pyspmp-0.1.7/pyspmp/carregar_csv.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/dataset/dataset.csv` & `pyspmp-0.1.7/pyspmp/dataset/dataset.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/dataset.py` & `pyspmp-0.1.7/pyspmp/dataset.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/parametros/parametros.csv` & `pyspmp-0.1.7/pyspmp/parametros/parametros.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/parametros/parametros_pi.csv` & `pyspmp-0.1.7/pyspmp/parametros/parametros_pi.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/periodos.py` & `pyspmp-0.1.7/pyspmp/periodos.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/resultado_busca/df_sp_TGA_P62.csv` & `pyspmp-0.1.7/pyspmp/resultado_busca/df_sp_TGA_P62.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv` & `pyspmp-0.1.7/pyspmp/resultado_busca/df_tagsout_TGA_P62.csv`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/pyspmp/variaveis_out.py` & `pyspmp-0.1.7/pyspmp/variaveis_out.py`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/README.md` & `pyspmp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyspmp-0.1.6/setup.py` & `pyspmp-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pyspmp']
 
 package_data = \
 {'': ['*'], 'pyspmp': ['dataset/*', 'parametros/*', 'resultado_busca/*']}
 
 install_requires = \
-['clr>=1.0.3,<2.0.0', 'pandas>=1.4.3,<2.0.0']
+['pandas>=1.4.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyspmp',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos',
     'long_description': '# PySPMP GitLab\n\n## Descrição\n\nEste projeto tem como objetivo realizar buscas e pré seleção de períodos dentro dos parâmentros definidos pelo usuário para modelos de monitoramento e predição de máquinas e equipamentos, visando mitigar e reduzir o esforço de trabalho do usuário na busca de períodos adequados para um bom modelo de monitoramento e predição.\n\n## Fonte\n\nA fonte do PySPMP é [hospedado em\nGitLab.com](https://codigo-externo.petrobras.com.br/leandro.castro.prestserv/pyspmp).\n\n## Requisitos\n\npython = "^3.8.1"\npandas = "^1.4.3"\nclr = "^1.0.3"\n\n',
     'author': 'Leandro Ribeiro de Castro',
     'author_email': 'lr.castro@yahoo.com.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyspmp-0.1.6/PKG-INFO` & `pyspmp-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pyspmp
-Version: 0.1.6
+Version: 0.1.7
 Summary: Busca e pré seleção de períodos para modelos de monitoramento e predição de máquinas e equipamentos
 Author: Leandro Ribeiro de Castro
 Author-email: lr.castro@yahoo.com.br
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clr (>=1.0.3,<2.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PySPMP GitLab
 
 ## Descrição
```

