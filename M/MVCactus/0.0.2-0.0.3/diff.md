# Comparing `tmp/MVCactus-0.0.2.tar.gz` & `tmp/MVCactus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MVCactus-0.0.2.tar", last modified: Sat Mar 18 10:25:22 2023, max compression
+gzip compressed data, was "MVCactus-0.0.3.tar", last modified: Tue May  2 11:25:00 2023, max compression
```

## Comparing `MVCactus-0.0.2.tar` & `MVCactus-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-03-18 10:25:22.325359 MVCactus-0.0.2/
-drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-03-18 10:25:22.323845 MVCactus-0.0.2/MVCactus/
--rw-------   0 dekelcohen   (501) staff       (20)     9731 2023-03-18 10:23:30.000000 MVCactus-0.0.2/MVCactus/MVCactus.py
--rw-------   0 dekelcohen   (501) staff       (20)        0 2023-03-15 09:38:55.000000 MVCactus-0.0.2/MVCactus/__init__.py
-drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-03-18 10:25:22.324824 MVCactus-0.0.2/MVCactus.egg-info/
--rw-r--r--   0 dekelcohen   (501) staff       (20)     1380 2023-03-18 10:25:22.000000 MVCactus-0.0.2/MVCactus.egg-info/PKG-INFO
--rw-r--r--   0 dekelcohen   (501) staff       (20)      219 2023-03-18 10:25:22.000000 MVCactus-0.0.2/MVCactus.egg-info/SOURCES.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)        1 2023-03-18 10:25:22.000000 MVCactus-0.0.2/MVCactus.egg-info/dependency_links.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)        7 2023-03-18 10:25:22.000000 MVCactus-0.0.2/MVCactus.egg-info/requires.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)        9 2023-03-18 10:25:22.000000 MVCactus-0.0.2/MVCactus.egg-info/top_level.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)     1380 2023-03-18 10:25:22.325194 MVCactus-0.0.2/PKG-INFO
--rw-r--r--   0 dekelcohen   (501) staff       (20)      757 2023-03-18 10:25:05.000000 MVCactus-0.0.2/README.md
--rw-r--r--   0 dekelcohen   (501) staff       (20)       38 2023-03-18 10:25:22.325415 MVCactus-0.0.2/setup.cfg
--rw-------   0 dekelcohen   (501) staff       (20)      964 2023-03-18 10:15:47.000000 MVCactus-0.0.2/setup.py
+drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:25:00.224870 MVCactus-0.0.3/
+drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:25:00.223981 MVCactus-0.0.3/MVCactus/
+-rw-------   0 dekelcohen   (501) staff       (20)    10365 2023-05-02 11:23:43.000000 MVCactus-0.0.3/MVCactus/MVCactus.py
+-rw-------   0 dekelcohen   (501) staff       (20)        0 2023-03-15 09:38:55.000000 MVCactus-0.0.3/MVCactus/__init__.py
+drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:25:00.224579 MVCactus-0.0.3/MVCactus.egg-info/
+-rw-r--r--   0 dekelcohen   (501) staff       (20)     1380 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/PKG-INFO
+-rw-r--r--   0 dekelcohen   (501) staff       (20)      219 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/SOURCES.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)        1 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/dependency_links.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)        7 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/requires.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)        9 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/top_level.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)     1380 2023-05-02 11:25:00.224752 MVCactus-0.0.3/PKG-INFO
+-rw-r--r--   0 dekelcohen   (501) staff       (20)      757 2023-03-18 10:25:05.000000 MVCactus-0.0.3/README.md
+-rw-r--r--   0 dekelcohen   (501) staff       (20)       38 2023-05-02 11:25:00.224906 MVCactus-0.0.3/setup.cfg
+-rw-------   0 dekelcohen   (501) staff       (20)      964 2023-05-02 11:21:13.000000 MVCactus-0.0.3/setup.py
```

### Comparing `MVCactus-0.0.2/MVCactus/MVCactus.py` & `MVCactus-0.0.3/MVCactus/MVCactus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import cgi
 import http.server
 import mimetypes
 import os
 import re
 import socketserver
-import urllib
 import jinja2
 
 
 class MVCactus(http.server.BaseHTTPRequestHandler):
     """
-    MVCactus is a simple web framework that allows users to quickly develop and deploy web
+    MVCactus is a simple web micro-framework that allows users to quickly develop and deploy web
     applications. It uses the Jinja2 templating engine for rendering templates and provides a set of convenient
     methods for handling HTTP requests and responses.
 
     MVCactus includes a routing system that allows users to map URLs to Python functions, and it supports both
     GET and POST requests. It also provides a method for serving static files, and includes a basic file upload feature.
 
     To use MVCactus, create a new class that inherits from MVCactus, define your routes using the route decorator,
@@ -24,33 +23,31 @@
     For more information on how to use MVCactus, please refer to the documentation and examples on GitHub.
     """
     env = jinja2.Environment(loader=jinja2.FileSystemLoader('templates'))
     routes = []
 
     @classmethod
     def route(cls, pattern):
-        '''
+        """
         A decorator for registering a URL pattern and callback function to handle requests for that pattern.
-        '''
+        """
+
         def wrapper(callback):
-            cls.routes.append((pattern, callback))
+            # Add the '^' at the beginning and '$' at the end of the pattern to ensure a full match.
+            regex_pattern = f'^{pattern}$'
+            cls.routes.append((regex_pattern, callback))
             return callback
 
         return wrapper
 
-    def url_for_static(self, filename, port=None):
-        '''
-        Generates a URL for serving a static file from the 'static' directory, given the filename and optional port number.
-        :param filename: the name of the file to generate the URL for.
-        :param port: an optional port number to include in the URL. Default is None.
-        :return: a URL string.
-        '''
-        current_dir = os.getcwd()
-        path = os.path.join(current_dir, 'static', filename)
-        return f'http://localhost:{port}/static/{path}'
+    def url_for_static(self, filename):
+        """
+        Returns the URL for a static file.
+        """
+        return f'/static/{filename}'
 
     def handle_error(self, status, message, template_name='upload.html', context=None):
         """
         Handles errors by sending the specified status and message as a response
         and rendering the specified template with the given context.
 
         Args:
@@ -65,42 +62,65 @@
         self.send_error(status, message)
         if context is None:
             context = {}
         context['status'] = status
         context['message'] = message
         self.render_template(template_name, context)
 
+    def send_response_headers(self, content_type, content_length=None):
+        """
+        Sends the response headers.
+
+        Args:
+            content_type (str): The content type of the response.
+            content_length (int, optional): The content length of the response. Defaults to None.
+
+        Features:
+            - Access-Control-Allow-Origin: Sends the CORS header allowing any origin to access the resource.
+            - X-Content-Type-Options: Prevents browsers from interpreting files as a different MIME type.
+            - X-Frame-Options: Prevents the content from being embedded within an iframe, avoiding clickjacking attacks.
+            - X-XSS-Protection: Enables the Cross-site scripting (XSS) filter in the browser.
+            - Referrer-Policy: Controls the information sent in the Referer header, avoiding information leaks.
+            - Feature-Policy: Restricts the use of browser features such as geolocation, microphone, and camera.
+        """
+        self.send_response(200)
+        self.send_header('Content-Type', content_type)
+        if content_length is not None:
+            self.send_header('Content-Length', str(content_length))
+        self.send_header('Access-Control-Allow-Origin', '*')
+        self.send_header('X-Content-Type-Options', 'nosniff')
+        self.send_header('X-Frame-Options', 'SAMEORIGIN')
+        self.send_header('X-XSS-Protection', '1; mode=block')
+        self.send_header('Referrer-Policy', 'no-referrer')
+        self.send_header('Feature-Policy', "geolocation 'none'; microphone 'none'; camera 'none'")
+        self.end_headers()
+
     def do_GET(self):
-        '''
-        This method handles GET requests sent to the server. If the path starts with '/static/', it serves a static
-        file using the serve_static_file() method. If the path matches a pattern in self.routes, it calls the
-        corresponding callback function. If none of the patterns match, it sends a 404 error response.
-        '''
         if self.path.startswith('/static/'):
-            path = self.path[1:]
+            path = self.path[7:]
             self.serve_static_file(path)
             return
 
         for pattern, callback in self.routes:
             match = re.match(pattern, self.path)
             if match:
                 callback(self, match)
                 return
 
         self.send_response(404)
         self.end_headers()
 
     def do_POST(self):
-        '''
+        """
         This method handles POST requests sent to the server. It first checks if the request contains multipart form
         data. If it does, it saves the uploaded file and sends a success response. If it doesn't, it reads the
-        request body and searches for a callback function in self.routes with the matching path and function name. If
+        request body and searches for a callback function in self. routes with the matching path and function name. If
         it finds a match, it calls the function with the request body as a parameter. If no match is found,
         it sends a 404 error response.
-        '''
+        """
         content_length = int(self.headers['Content-Length'])
         content_type = self.headers['Content-Type']
 
         if 'multipart/form-data' in content_type:
             fields = cgi.FieldStorage(fp=self.rfile, headers=self.headers, environ={
                 'REQUEST_METHOD': 'POST',
                 'CONTENT_TYPE': content_type,
@@ -135,14 +155,15 @@
 
         Args:
             path (str): The path to associate the handler with.
 
         Returns: function: The decorator function that registers the given callback function as a POST request
         handler for the given path.
         """
+
         def wrapper(callback):
             """
             Wrapper function that registers the given callback function as a POST request handler for the path given
             to the outer function.
 
             Args:
                 callback (function): The function that handles the POST request.
@@ -169,37 +190,26 @@
         """
         handler.send_response(200)
         handler.send_header('Content-type', 'text/plain')
         handler.end_headers()
         handler.wfile.write(body.encode('utf-8'))
 
     def serve_static_file(self, path):
-        """
-        Serves a static file to the client with the given path.
-
-        Args:
-            path (str): The path of the file to serve.
-
-        Returns:
-            None
-        """
         try:
-            current_dir = os.getcwd()
-            file_path = os.path.join(current_dir, 'static', path)
+            current_dir = os.path.dirname(os.path.abspath(__file__))
+            file_path = f"{current_dir}/static{path}"
+            print(f'Serving static file: {file_path}')
 
             if not os.path.isfile(file_path):
                 raise IOError
 
-            self.send_response(200)
             mime_type, _ = mimetypes.guess_type(path)
-            if mime_type == 'text/css':
-                self.send_header('Cache-Control', 'max-age=86400')
-            self.send_header('Content-Type', mime_type)
-            self.send_header('Content-Length', str(os.path.getsize(file_path)))
-            self.end_headers()
+            content_length = os.path.getsize(file_path)
+
+            self.send_response_headers(mime_type, content_length)
 
             with open(file_path, 'rb') as f:
                 chunk_size = 8192
                 while True:
                     chunk = f.read(chunk_size)
                     if not chunk:
                         break
@@ -223,40 +233,38 @@
             if field not in data:
                 missing_fields.append(field)
         if missing_fields:
             self.send_error(400, f'Missing fields: {", ".join(missing_fields)}')
             return False
         return True
 
-    def render_template(self, template_name, context=None, css_url=None):
+    def render_template(self, template_name, context=None):
         """
         Renders a Jinja2 template with the given context and sends the resulting HTML to the client.
 
         Args:
             template_name (str): The name of the template file.
             context (dict, optional): The context to render the template with. Defaults to None.
-            css_url (str, optional): The URL of a CSS stylesheet to include in the template. Defaults to None.
 
         Returns:
             None
         """
         template = self.env.get_template(template_name)
         if context is None:
             context = {}
-        context['css_url'] = css_url
+        context['url_for_static'] = self.url_for_static
         html = template.render(context)
-        self.send_response(200)
-        self.send_header('Content-type', 'text/html')
-        self.end_headers()
+        self.send_response_headers('text/html', len(html.encode('utf-8')))
         self.wfile.write(html.encode('utf-8'))
 
 
 class MVCactusRun:
 
-    def __init__(self, port=8080):
+    def __init__(self, address='localhost', port=8080):
+        self.ADDRESS = address
         self.PORT = port
 
     def run(self, app_class):
-        with socketserver.TCPServer(("", self.PORT), app_class) as httpd:
-            print(f"Running on port {self.PORT}\nEnter here: http://localhost:{self.PORT}/")
+        with socketserver.TCPServer((self.ADDRESS, self.PORT), app_class) as httpd:
+            print(f"Running on {self.ADDRESS}:{self.PORT}\nEnter here: http://{self.ADDRESS}:{self.PORT}/")
 
             httpd.serve_forever()
```

### Comparing `MVCactus-0.0.2/MVCactus.egg-info/PKG-INFO` & `MVCactus-0.0.3/MVCactus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MVCactus
-Version: 0.0.2
+Version: 0.0.3
 Summary: MVCactus is a lightweight, open-source web framework for building small web applications in Python.
 Author: Dekel Cohen
 Author-email: <dcohen52@gmail.com>
 Keywords: python,web,framework,desktop,html,javascript,styles,js,API,microservices,REST
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MVCactus-0.0.2/PKG-INFO` & `MVCactus-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MVCactus
-Version: 0.0.2
+Version: 0.0.3
 Summary: MVCactus is a lightweight, open-source web framework for building small web applications in Python.
 Author: Dekel Cohen
 Author-email: <dcohen52@gmail.com>
 Keywords: python,web,framework,desktop,html,javascript,styles,js,API,microservices,REST
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MVCactus-0.0.2/README.md` & `MVCactus-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `MVCactus-0.0.2/setup.py` & `MVCactus-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'MVCactus is a lightweight, open-source web framework for building small web applications in Python.'
 
 # Setting up
 setup(
     name="MVCactus",
     version=VERSION,
     author="Dekel Cohen",
```

