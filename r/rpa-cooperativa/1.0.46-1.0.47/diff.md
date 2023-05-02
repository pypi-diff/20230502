# Comparing `tmp/rpa_cooperativa-1.0.46.tar.gz` & `tmp/rpa_cooperativa-1.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.46.tar", last modified: Thu Apr 27 12:44:56 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.47.tar", last modified: Tue May  2 13:00:02 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.46.tar` & `rpa_cooperativa-1.0.47.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:44:56.191722 rpa_cooperativa-1.0.46/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.46/LICENSE
--rw-rw-rw-   0        0        0     6237 2023-04-27 12:44:56.189723 rpa_cooperativa-1.0.46/PKG-INFO
--rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.46/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:44:55.957647 rpa_cooperativa-1.0.46/rpa_coop/
--rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.46/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:44:56.121074 rpa_cooperativa-1.0.46/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.46/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.46/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.46/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.46/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.46/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.46/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    71299 2023-04-24 14:17:17.000000 rpa_cooperativa-1.0.46/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:44:56.184727 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6237 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-04-27 12:44:55.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 12:44:54.000000 rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 12:44:56.193735 rpa_cooperativa-1.0.46/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-04-27 12:44:30.000000 rpa_cooperativa-1.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:00:02.543623 rpa_cooperativa-1.0.47/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.47/LICENSE
+-rw-rw-rw-   0        0        0     6909 2023-05-02 13:00:02.540596 rpa_cooperativa-1.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0     5760 2023-05-02 12:58:58.000000 rpa_cooperativa-1.0.47/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 13:00:02.299176 rpa_cooperativa-1.0.47/rpa_coop/
+-rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.47/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:00:02.481488 rpa_cooperativa-1.0.47/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.47/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.47/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.47/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.47/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.47/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.47/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.47/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.47/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.47/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.47/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.47/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    71397 2023-05-02 12:46:27.000000 rpa_cooperativa-1.0.47/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:00:02.533520 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6909 2023-05-02 13:00:01.000000 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-05-02 13:00:01.000000 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:00:01.000000 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-02 13:00:01.000000 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-05-02 13:00:01.000000 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 13:00:01.000000 rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:00:02.544623 rpa_cooperativa-1.0.47/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-05-02 12:59:06.000000 rpa_cooperativa-1.0.47/setup.py
```

### Comparing `rpa_cooperativa-1.0.46/LICENSE` & `rpa_cooperativa-1.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/PKG-INFO` & `rpa_cooperativa-1.0.47/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.46
+Version: 1.0.47
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -36,14 +36,30 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
+## metodo de envio de email
+```python
+from rpa_coop import mail
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg') \n\n
+
+lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']\n
+mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')\n\n
+
+anexos = ['notas.txt', 'README.md']\n
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)\n\n
+
+anexos = ['notas.txt', 'README.md', 'imagem.PNG']\n
+html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'\n
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)\n
+```
+
 ## manipulacao selenium: automaÃ§Ã£o web
 ```python
 from rpa_coop import selenium
 import time
 
 driver = selenium.driver_edge()
 url = 'http://www.google.com.br'
```

### Comparing `rpa_cooperativa-1.0.46/README.md` & `rpa_cooperativa-1.0.47/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,30 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
+## metodo de envio de email
+```python
+from rpa_coop import mail
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg') \n\n
+
+lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']\n
+mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')\n\n
+
+anexos = ['notas.txt', 'README.md']\n
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)\n\n
+
+anexos = ['notas.txt', 'README.md', 'imagem.PNG']\n
+html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'\n
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)\n
+```
+
 ## manipulacao selenium: automação web
 ```python
 from rpa_coop import selenium
 import time
 
 driver = selenium.driver_edge()
 url = 'http://www.google.com.br'
```

### Comparing `rpa_cooperativa-1.0.46/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.47/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.47/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.47/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.47/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.47/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.47/rpa_coop/rpa_coop.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
     
     def __init__(self):
         self.user_mail = gerador_pwd('api_email', 'usuario')
         self.password_mail = gerador_pwd('api_email', 'sistema')
         self.smtpsrv = gerador_pwd('api_email', 'ip_host')
 
 
-    def enviar_email(self, destinatarios, assunto: str, mensagem: str, anexo=None, html_text_img=None, com_copia=None):
+    def enviar_email(self, destinatarios, assunto: str, mensagem: str, anexo=None, html_text_img=None, cc=None, cco=None):
         '''
         mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg') \n\n
         
         lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']\n
         mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')\n\n
         
         anexos = ['notas.txt', 'README.md']\n
@@ -1020,17 +1020,18 @@
         mail_content = mensagem
         smtpserver = self.smtplib.SMTP(self.smtpsrv,587)
         msg = self.MIMEMultipart('mixed')
         msg = self.MIMEMultipart('alternative')
         
         msg['Subject'] = assunto
         msg['From'] = self.user_mail 
-        msg['To'] = destinatarios if type(destinatarios) == str else ", ".join(destinatarios)
+        msg['To'] = destinatarios if type(destinatarios) == str else ",".join(destinatarios)
 
-        if com_copia: msg['Cc'] = com_copia
+        if cc: msg['Cc'] = cc if type(cc) == str else ",".join(cc)
+        if cco: msg['Bcc'] = cco if type(cco) == str else ",".join(cco)
         msg.attach(self.MIMEText(mail_content,'plain','utf8'))
 
         msg.attach(self.MIMEText(html_text_img, 'html', 'utf-8'))
         
         if type(anexo) == str:
             if anexo:
                 attachmentPath = anexo
```

### Comparing `rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.46
+Version: 1.0.47
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -36,14 +36,30 @@
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
 ```
 
+## metodo de envio de email
+```python
+from rpa_coop import mail
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg') \n\n
+
+lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']\n
+mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')\n\n
+
+anexos = ['notas.txt', 'README.md']\n
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)\n\n
+
+anexos = ['notas.txt', 'README.md', 'imagem.PNG']\n
+html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'\n
+mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)\n
+```
+
 ## manipulacao selenium: automaÃ§Ã£o web
 ```python
 from rpa_coop import selenium
 import time
 
 driver = selenium.driver_edge()
 url = 'http://www.google.com.br'
```

### Comparing `rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.47/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.46/setup.py` & `rpa_cooperativa-1.0.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.46",
+    version="1.0.47",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

