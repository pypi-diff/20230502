# Comparing `tmp/blacklist-checker-0.0.3.tar.gz` & `tmp/blacklist-checker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacklist-checker-0.0.3.tar", last modified: Mon May  1 17:15:35 2023, max compression
+gzip compressed data, was "blacklist-checker-0.0.4.tar", last modified: Tue May  2 17:44:07 2023, max compression
```

## Comparing `blacklist-checker-0.0.3.tar` & `blacklist-checker-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-01 17:15:35.766784 blacklist-checker-0.0.3/
--rw-r--r--   0 benoit     (501) staff       (20)    11357 2023-05-01 16:18:52.000000 blacklist-checker-0.0.3/LICENSE
--rw-r--r--   0 benoit     (501) staff       (20)    13516 2023-05-01 17:15:35.766115 blacklist-checker-0.0.3/PKG-INFO
--rw-r--r--   0 benoit     (501) staff       (20)       20 2023-05-01 16:16:27.000000 blacklist-checker-0.0.3/README.md
--rw-r--r--   0 benoit     (501) staff       (20)      881 2023-05-01 17:15:10.000000 blacklist-checker-0.0.3/pyproject.toml
--rw-r--r--   0 benoit     (501) staff       (20)       38 2023-05-01 17:15:35.766945 blacklist-checker-0.0.3/setup.cfg
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-01 17:15:35.749122 blacklist-checker-0.0.3/src/
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-01 16:48:21.000000 blacklist-checker-0.0.3/src/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-01 17:15:35.760593 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/
--rw-r--r--   0 benoit     (501) staff       (20)    13516 2023-05-01 17:15:35.000000 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/PKG-INFO
--rw-r--r--   0 benoit     (501) staff       (20)      464 2023-05-01 17:15:35.000000 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benoit     (501) staff       (20)        1 2023-05-01 17:15:35.000000 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benoit     (501) staff       (20)       43 2023-05-01 17:15:35.000000 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/entry_points.txt
--rw-r--r--   0 benoit     (501) staff       (20)      100 2023-05-01 17:15:35.000000 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/requires.txt
--rw-r--r--   0 benoit     (501) staff       (20)       34 2023-05-01 17:15:35.000000 blacklist-checker-0.0.3/src/blacklist_checker.egg-info/top_level.txt
--rw-r--r--   0 benoit     (501) staff       (20)     1214 2023-05-01 16:49:23.000000 blacklist-checker-0.0.3/src/main.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-01 17:15:35.762517 blacklist-checker-0.0.3/src/messaging/
--rw-r--r--   0 benoit     (501) staff       (20)     7473 2023-05-01 12:57:49.000000 blacklist-checker-0.0.3/src/messaging/Mailer.py
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-29 16:38:19.000000 blacklist-checker-0.0.3/src/messaging/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-01 17:15:35.764430 blacklist-checker-0.0.3/src/requester/
--rw-r--r--   0 benoit     (501) staff       (20)     2200 2023-05-01 12:31:50.000000 blacklist-checker-0.0.3/src/requester/Black_list_checker.py
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-24 12:19:29.000000 blacklist-checker-0.0.3/src/requester/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-01 17:15:35.764860 blacklist-checker-0.0.3/test/
--rw-r--r--   0 benoit     (501) staff       (20)      412 2023-05-01 11:54:04.000000 blacklist-checker-0.0.3/test/test_mailer.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.302311 blacklist-checker-0.0.4/
+-rw-r--r--   0 benoit     (501) staff       (20)    11357 2023-05-01 16:18:52.000000 blacklist-checker-0.0.4/LICENSE
+-rw-r--r--   0 benoit     (501) staff       (20)    13516 2023-05-02 17:44:07.301538 blacklist-checker-0.0.4/PKG-INFO
+-rw-r--r--   0 benoit     (501) staff       (20)       20 2023-05-01 16:16:27.000000 blacklist-checker-0.0.4/README.md
+-rw-r--r--   0 benoit     (501) staff       (20)      910 2023-05-02 17:43:55.000000 blacklist-checker-0.0.4/pyproject.toml
+-rw-r--r--   0 benoit     (501) staff       (20)       38 2023-05-02 17:44:07.302476 blacklist-checker-0.0.4/setup.cfg
+-rw-r--r--   0 benoit     (501) staff       (20)       47 2023-05-02 17:14:58.000000 blacklist-checker-0.0.4/setup.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.291481 blacklist-checker-0.0.4/src/
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-01 16:48:21.000000 blacklist-checker-0.0.4/src/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.291783 blacklist-checker-0.0.4/src/blacklist_checker/
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-02 17:30:59.000000 blacklist-checker-0.0.4/src/blacklist_checker/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.295194 blacklist-checker-0.0.4/src/blacklist_checker/cli/
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-02 17:25:00.000000 blacklist-checker-0.0.4/src/blacklist_checker/cli/__init__.py
+-rw-r--r--   0 benoit     (501) staff       (20)     1251 2023-05-02 17:37:54.000000 blacklist-checker-0.0.4/src/blacklist_checker/cli/mycli.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.296887 blacklist-checker-0.0.4/src/blacklist_checker/messaging/
+-rw-r--r--   0 benoit     (501) staff       (20)     7492 2023-05-02 16:41:33.000000 blacklist-checker-0.0.4/src/blacklist_checker/messaging/Mailer.py
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-29 16:38:19.000000 blacklist-checker-0.0.4/src/blacklist_checker/messaging/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.298216 blacklist-checker-0.0.4/src/blacklist_checker/requester/
+-rw-r--r--   0 benoit     (501) staff       (20)     2200 2023-05-01 12:31:50.000000 blacklist-checker-0.0.4/src/blacklist_checker/requester/Black_list_checker.py
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-24 12:19:29.000000 blacklist-checker-0.0.4/src/blacklist_checker/requester/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.294428 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/
+-rw-r--r--   0 benoit     (501) staff       (20)    13516 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benoit     (501) staff       (20)      640 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit     (501) staff       (20)        1 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit     (501) staff       (20)       71 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benoit     (501) staff       (20)      100 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/requires.txt
+-rw-r--r--   0 benoit     (501) staff       (20)       27 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.298756 blacklist-checker-0.0.4/test/
+-rw-r--r--   0 benoit     (501) staff       (20)      502 2023-05-02 16:28:55.000000 blacklist-checker-0.0.4/test/test_mailer.py
```

### Comparing `blacklist-checker-0.0.3/LICENSE` & `blacklist-checker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blacklist-checker-0.0.3/PKG-INFO` & `blacklist-checker-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacklist-checker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Check if a specific domain is in mail blaclist 
 Author-email: Benoit Chenal <ben57univ@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blacklist-checker-0.0.3/pyproject.toml` & `blacklist-checker-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blacklist-checker"
-version = "0.0.3"
+version = "0.0.4"
 description = "Check if a specific domain is in mail blaclist "
 readme = "README.md"
 authors = [{ name = "Benoit Chenal", email = "ben57univ@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 
 
+
 keywords = ["blacklist", "domain", "mail"]
 dependencies = [
     "requests",
     "configparser",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.9"
@@ -30,8 +31,8 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/benochen/blacklist-checker.git"
 
 [project.scripts]
-blacklist-checker = "main"
+blacklist-checker = "blacklist_checker.cli.mycli:main"
```

### Comparing `blacklist-checker-0.0.3/src/blacklist_checker.egg-info/PKG-INFO` & `blacklist-checker-0.0.4/src/blacklist_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacklist-checker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Check if a specific domain is in mail blaclist 
 Author-email: Benoit Chenal <ben57univ@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blacklist-checker-0.0.3/src/main.py` & `blacklist-checker-0.0.4/src/blacklist_checker/cli/mycli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typer
-from src.requester.Black_list_checker import BlackListListChecker
-from src.messaging.Mailer import MyMailer
+import sys
+from requester.Black_list_checker import BlackListListChecker
+from messaging.Mailer import MyMailer
 app = typer.Typer()
 
 @app.command()
 def checkdns(domain:str = typer.Option("", help=("domain to test")),config:str=typer.Option("",help=("Configuration file")),reporting:bool=typer.Option(False,help=("If set a reporting is sent ")),provider:str=typer.Option("",help=("provider file"))):
     try:
         if config=="":
             config_file="config.ini"
@@ -27,9 +28,12 @@
         print(e)
 
 
 @app.command()
 def check_web_site(domain:str = typer.Option("", help=("domain to test"))):
     pass
 
+def main():
+    app()
+
 if __name__ == "__main__":
-    app()
+    sys.exit(main())
```

### Comparing `blacklist-checker-0.0.3/src/messaging/Mailer.py` & `blacklist-checker-0.0.4/src/blacklist_checker/messaging/Mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import configparser
 import json
 import smtplib, ssl
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
-
+'''
+'''
 class MyMailer():
-    def load_smtp_config(self,config_smtp):
+    def load_smtp_config(self,config_smtp:str)->None:
 
         if "smtp_host" not in config_smtp.keys():
             raise Exception("The SMTP host is missing")
         else:
             self.smtp_host=config_smtp["smtp_host"]
 
         if "smtp_port" not in config_smtp.keys():
@@ -126,14 +127,22 @@
                 line = f.readline()
                 if not line:
                     break
                 else:
                     lines=lines+line
         return lines
 
+    def send_alert_report(self,report):
+        self.set_complete_template_path("alert")
+        html_mail_body_template=self.load_alert_report_template()
+        report_html_table=self.transform_json_to_html_table(report)
+        html_mail_body= self.replace_template_placeholder(html_mail_body_template,report_html_table)
+        self.send_mail(self.smtp_alert_report_receivers,self.smtp_alert_report_subject,html_mail_body)
+
+
     def send_regular_report(self):
         self.set_complete_template_path("daily")
         html_mail_body_template=self.load_daily_report_template()
         html_mail_body= self.replace_template_placeholder(html_mail_body_template,None)
         self.send_mail(self.smtp_daily_report_receivers,self.smtp_daily_report_subject,html_mail_body)
 
     def replace_template_placeholder(self,html_body_template,report_html_table):
@@ -161,13 +170,7 @@
         with smtplib.SMTP(self.smtp_host, self.smtp_port) as server:
             server.login(self.smtp_user, self.smtp_pass)
             server.sendmail(
                 self.smtp_sender, receiver_email, message.as_string()
             )
 
 
-    def send_alert_report(self,report):
-        self.set_complete_template_path("alert")
-        html_mail_body_template=self.load_alert_report_template()
-        report_html_table=self.transform_json_to_html_table(report)
-        html_mail_body= self.replace_template_placeholder(html_mail_body_template,report_html_table)
-        self.send_mail(self.smtp_alert_report_receivers,self.smtp_alert_report_subject,html_mail_body)
```

### Comparing `blacklist-checker-0.0.3/src/requester/Black_list_checker.py` & `blacklist-checker-0.0.4/src/blacklist_checker/requester/Black_list_checker.py`

 * *Files identical despite different names*

