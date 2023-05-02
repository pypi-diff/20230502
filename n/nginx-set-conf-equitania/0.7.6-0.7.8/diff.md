# Comparing `tmp/nginx-set-conf-equitania-0.7.6.tar.gz` & `tmp/nginx-set-conf-equitania-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.7.6.tar", last modified: Sun Jul 10 08:20:16 2022, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.7.8.tar", last modified: Tue May  2 12:53:20 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.7.6.tar` & `nginx-set-conf-equitania-0.7.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-07-10 08:20:16.600470 nginx-set-conf-equitania-0.7.6/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.7.6/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3354 2022-07-10 08:20:16.600358 nginx-set-conf-equitania-0.7.6/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2816 2022-05-19 13:19:31.000000 nginx-set-conf-equitania-0.7.6/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-07-10 08:20:16.599459 nginx-set-conf-equitania-0.7.6/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    21450 2022-07-10 08:18:30.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4006 2022-05-01 15:48:47.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2022-05-01 15:47:21.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-07-10 08:20:16.600206 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3354 2022-07-10 08:20:16.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2022-07-10 08:20:16.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2022-07-10 08:20:16.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2022-07-10 08:20:16.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       25 2022-07-10 08:20:16.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2022-07-10 08:20:16.000000 nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2022-07-10 08:20:16.600505 nginx-set-conf-equitania-0.7.6/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      901 2022-07-10 08:14:25.000000 nginx-set-conf-equitania-0.7.6/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 12:53:20.184376 nginx-set-conf-equitania-0.7.8/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.7.8/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 12:53:20.184199 nginx-set-conf-equitania-0.7.8/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.7.8/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 12:53:20.182392 nginx-set-conf-equitania-0.7.8/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    21510 2023-05-02 12:47:22.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     4005 2023-05-02 12:42:36.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7077 2023-05-02 12:43:15.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 12:53:20.183931 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-02 12:53:20.184426 nginx-set-conf-equitania-0.7.8/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-02 12:43:01.000000 nginx-set-conf-equitania-0.7.8/setup.py
```

### Comparing `nginx-set-conf-equitania-0.7.6/LICENSE.txt` & `nginx-set-conf-equitania-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.7.6/PKG-INFO` & `nginx-set-conf-equitania-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.7.6
+Version: 0.7.8
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -19,15 +17,15 @@
   
 ## Installation
   
 ### Nginx-set-conf requires:
   
 - Python (>= 3.6)  
 - click (>= 8.1.3)  
-- PyYaml (>= 6.0)  
+- PyYaml (>= 5.4.1)  
   
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install nginx-set-conf.
   
 ```bash
 pip install nginx-set-conf-equitania
 ```
 
@@ -85,8 +83,7 @@
 ```
   
 ## Compile your nginx with PageSpeed   
   
 At github you can find the script to do that: [nginx build script](https://github.com/equitania/myodoo-docker/tree/2022/scripts/build_nginx)  
   
 This project is licensed under the terms of the **AGPLv3** license.  
-
```

### Comparing `nginx-set-conf-equitania-0.7.6/README.md` & `nginx-set-conf-equitania-0.7.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   
 ## Installation
   
 ### Nginx-set-conf requires:
   
 - Python (>= 3.6)  
 - click (>= 8.1.3)  
-- PyYaml (>= 6.0)  
+- PyYaml (>= 5.4.1)  
   
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install nginx-set-conf.
   
 ```bash
 pip install nginx-set-conf-equitania
 ```
```

### Comparing `nginx-set-conf-equitania-0.7.6/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.7.8/nginx_set_conf/config_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 config_template_dict = {
 "ngx_code_server": """# Template for code-server configuration nginx incl. SSL/http2
-# Version 3.6 from 10.07.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -65,18 +65,18 @@
     }
     # Pagespeed
     pagespeed off;
 }
 """,
 
 "ngx_fast_report": """# Template for FastReport configuration nginx incl. SSL/http2
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -134,18 +134,18 @@
     }
     # Pagespeed
     pagespeed off;
 }
 """,
 
 "ngx_nextcloud": """# Template for NextCloud configuration nginx incl. SSL/http2
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -214,18 +214,18 @@
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 
 "ngx_portainer": """# Template for Portainer configuration nginx incl. SSL/http2
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -270,18 +270,18 @@
         proxy_pass http://127.0.0.1:oldport;
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_odoo_http": """# Template for Odoo configuration nginx
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     client_max_body_size 8192m;
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
@@ -337,18 +337,18 @@
         proxy_pass http://127.0.0.1:oldport;
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_odoo_ssl": """# Template for Odoo configuration nginx incl. SSL
-# Version 3.6 from 01.05.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -427,18 +427,18 @@
     pagespeed off;
 }
 
 """,
 
 "ngx_odoo_ssl_pagespeed": """# Template for Odoo configuration nginx incl. SSL/http2 and Google PageSpeed
 # source: https://github.com/apache/incubator-pagespeed-ngx/blob/master/scripts/build_ngx_pagespeed.sh
-# Version 3.4 from 18.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -517,18 +517,18 @@
 
     include "pagespeed_main.conf";
     # Pagespeed
     pagespeed on;
 }""",
 
 "ngx_pgadmin": """# Template for pgAdmin configuration nginx incl. SSL/http2
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -578,18 +578,18 @@
     }
     # Pagespeed
     pagespeed off;
 }
 """,
 
 "ngx_pwa": """# Template for Progressive Web App .NET Core configuration nginx incl. SSL/http2
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
@@ -658,18 +658,18 @@
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_redirect_ssl": """# Template for Redirect domain configuration nginx ssl/http2
-# Version 3.5 from 25.04.2022
-upstream server.domain.de {
-    server ip.ip.ip.ip weight=1 fail_timeout=0;
-}
+# Version 3.7 from 02.05.2023
+# upstream server.domain.de {
+#     server ip.ip.ip.ip weight=1 fail_timeout=0;
+# }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
```

### Comparing `nginx-set-conf-equitania-0.7.6/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.7.8/nginx_set_conf/nginx_set_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright 2014-now Equitania Software GmbH - Pforzheim - Germany
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
-from .utils import parse_yaml_folder, retrieve_valid_input, execute_commands
+from utils import parse_yaml_folder, retrieve_valid_input, execute_commands
 import click
 import os
 
 def welcome():
     click.echo("Welcome to the nginx_set_conf!")
```

### Comparing `nginx-set-conf-equitania-0.7.6/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.7.8/nginx_set_conf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2014-now Equitania Software GmbH - Pforzheim - Germany
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 import yaml
 import os
-from .config_templates import get_config_template
+from config_templates import get_config_template
 
 def fire_all_functions(function_list: list):
     """
         Execute each function in a list
         :param function_list: List of functions
     """
     for func in function_list:
```

### Comparing `nginx-set-conf-equitania-0.7.6/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.7.6
+Version: 0.7.8
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -19,15 +17,15 @@
   
 ## Installation
   
 ### Nginx-set-conf requires:
   
 - Python (>= 3.6)  
 - click (>= 8.1.3)  
-- PyYaml (>= 6.0)  
+- PyYaml (>= 5.4.1)  
   
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install nginx-set-conf.
   
 ```bash
 pip install nginx-set-conf-equitania
 ```
 
@@ -85,8 +83,7 @@
 ```
   
 ## Compile your nginx with PageSpeed   
   
 At github you can find the script to do that: [nginx build script](https://github.com/equitania/myodoo-docker/tree/2022/scripts/build_nginx)  
   
 This project is licensed under the terms of the **AGPLv3** license.  
-
```

### Comparing `nginx-set-conf-equitania-0.7.6/setup.py` & `nginx-set-conf-equitania-0.7.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.7.6",
+    version="0.7.8",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx with/without pagespeed for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
@@ -20,10 +20,10 @@
     python_requires='>=3.6',
     entry_points='''
     [console_scripts]
     nginx-set-conf=nginx_set_conf.nginx_set_conf:start_nginx_set_conf
     ''',
     install_requires=[
         'click>=8.1.3',
-        'PyYaml>=6.0'
+        'PyYaml>=5.4.1'
     ]
 )
```

