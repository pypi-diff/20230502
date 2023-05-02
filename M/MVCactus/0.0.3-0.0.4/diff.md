# Comparing `tmp/MVCactus-0.0.3.tar.gz` & `tmp/MVCactus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MVCactus-0.0.3.tar", last modified: Tue May  2 11:25:00 2023, max compression
+gzip compressed data, was "MVCactus-0.0.4.tar", last modified: Tue May  2 11:59:23 2023, max compression
```

## Comparing `MVCactus-0.0.3.tar` & `MVCactus-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:25:00.224870 MVCactus-0.0.3/
-drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:25:00.223981 MVCactus-0.0.3/MVCactus/
--rw-------   0 dekelcohen   (501) staff       (20)    10365 2023-05-02 11:23:43.000000 MVCactus-0.0.3/MVCactus/MVCactus.py
--rw-------   0 dekelcohen   (501) staff       (20)        0 2023-03-15 09:38:55.000000 MVCactus-0.0.3/MVCactus/__init__.py
-drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:25:00.224579 MVCactus-0.0.3/MVCactus.egg-info/
--rw-r--r--   0 dekelcohen   (501) staff       (20)     1380 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/PKG-INFO
--rw-r--r--   0 dekelcohen   (501) staff       (20)      219 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/SOURCES.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)        1 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/dependency_links.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)        7 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/requires.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)        9 2023-05-02 11:25:00.000000 MVCactus-0.0.3/MVCactus.egg-info/top_level.txt
--rw-r--r--   0 dekelcohen   (501) staff       (20)     1380 2023-05-02 11:25:00.224752 MVCactus-0.0.3/PKG-INFO
--rw-r--r--   0 dekelcohen   (501) staff       (20)      757 2023-03-18 10:25:05.000000 MVCactus-0.0.3/README.md
--rw-r--r--   0 dekelcohen   (501) staff       (20)       38 2023-05-02 11:25:00.224906 MVCactus-0.0.3/setup.cfg
--rw-------   0 dekelcohen   (501) staff       (20)      964 2023-05-02 11:21:13.000000 MVCactus-0.0.3/setup.py
+drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:59:23.601817 MVCactus-0.0.4/
+drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:59:23.600836 MVCactus-0.0.4/MVCactus/
+-rw-------   0 dekelcohen   (501) staff       (20)    10877 2023-05-02 11:58:11.000000 MVCactus-0.0.4/MVCactus/MVCactus.py
+-rw-------   0 dekelcohen   (501) staff       (20)        0 2023-03-15 09:38:55.000000 MVCactus-0.0.4/MVCactus/__init__.py
+drwxr-xr-x   0 dekelcohen   (501) staff       (20)        0 2023-05-02 11:59:23.601504 MVCactus-0.0.4/MVCactus.egg-info/
+-rw-r--r--   0 dekelcohen   (501) staff       (20)     1415 2023-05-02 11:59:23.000000 MVCactus-0.0.4/MVCactus.egg-info/PKG-INFO
+-rw-r--r--   0 dekelcohen   (501) staff       (20)      219 2023-05-02 11:59:23.000000 MVCactus-0.0.4/MVCactus.egg-info/SOURCES.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)        1 2023-05-02 11:59:23.000000 MVCactus-0.0.4/MVCactus.egg-info/dependency_links.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)        7 2023-05-02 11:59:23.000000 MVCactus-0.0.4/MVCactus.egg-info/requires.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)        9 2023-05-02 11:59:23.000000 MVCactus-0.0.4/MVCactus.egg-info/top_level.txt
+-rw-r--r--   0 dekelcohen   (501) staff       (20)     1415 2023-05-02 11:59:23.601688 MVCactus-0.0.4/PKG-INFO
+-rw-r--r--   0 dekelcohen   (501) staff       (20)      757 2023-03-18 10:25:05.000000 MVCactus-0.0.4/README.md
+-rw-r--r--   0 dekelcohen   (501) staff       (20)       38 2023-05-02 11:59:23.601863 MVCactus-0.0.4/setup.cfg
+-rw-------   0 dekelcohen   (501) staff       (20)     1023 2023-05-02 11:59:11.000000 MVCactus-0.0.4/setup.py
```

### Comparing `MVCactus-0.0.3/MVCactus/MVCactus.py` & `MVCactus-0.0.4/MVCactus/MVCactus.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,31 +22,33 @@
 
     For more information on how to use MVCactus, please refer to the documentation and examples on GitHub.
     """
     env = jinja2.Environment(loader=jinja2.FileSystemLoader('templates'))
     routes = []
 
     @classmethod
+    @classmethod
     def route(cls, pattern):
-        """
+        '''
         A decorator for registering a URL pattern and callback function to handle requests for that pattern.
-        """
+        '''
 
         def wrapper(callback):
             # Add the '^' at the beginning and '$' at the end of the pattern to ensure a full match.
             regex_pattern = f'^{pattern}$'
             cls.routes.append((regex_pattern, callback))
             return callback
 
         return wrapper
 
     def url_for_static(self, filename):
-        """
+        '''
         Returns the URL for a static file.
-        """
+        '''
+        # print(f'/static/{filename}')
         return f'/static/{filename}'
 
     def handle_error(self, status, message, template_name='upload.html', context=None):
         """
         Handles errors by sending the specified status and message as a response
         and rendering the specified template with the given context.
 
@@ -106,21 +108,21 @@
                 callback(self, match)
                 return
 
         self.send_response(404)
         self.end_headers()
 
     def do_POST(self):
-        """
+        '''
         This method handles POST requests sent to the server. It first checks if the request contains multipart form
         data. If it does, it saves the uploaded file and sends a success response. If it doesn't, it reads the
         request body and searches for a callback function in self. routes with the matching path and function name. If
         it finds a match, it calls the function with the request body as a parameter. If no match is found,
         it sends a 404 error response.
-        """
+        '''
         content_length = int(self.headers['Content-Length'])
         content_type = self.headers['Content-Type']
 
         if 'multipart/form-data' in content_type:
             fields = cgi.FieldStorage(fp=self.rfile, headers=self.headers, environ={
                 'REQUEST_METHOD': 'POST',
                 'CONTENT_TYPE': content_type,
@@ -191,16 +193,16 @@
         handler.send_response(200)
         handler.send_header('Content-type', 'text/plain')
         handler.end_headers()
         handler.wfile.write(body.encode('utf-8'))
 
     def serve_static_file(self, path):
         try:
-            current_dir = os.path.dirname(os.path.abspath(__file__))
-            file_path = f"{current_dir}/static{path}"
+            current_dir = os.path.abspath("static")
+            file_path = f"{current_dir}{path}"
             print(f'Serving static file: {file_path}')
 
             if not os.path.isfile(file_path):
                 raise IOError
 
             mime_type, _ = mimetypes.guess_type(path)
             content_length = os.path.getsize(file_path)
@@ -261,10 +263,20 @@
 
     def __init__(self, address='localhost', port=8080):
         self.ADDRESS = address
         self.PORT = port
 
     def run(self, app_class):
         with socketserver.TCPServer((self.ADDRESS, self.PORT), app_class) as httpd:
-            print(f"Running on {self.ADDRESS}:{self.PORT}\nEnter here: http://{self.ADDRESS}:{self.PORT}/")
+            print(f"Running on {self.ADDRESS}:{self.PORT}")
+            print(f"Enter here: http://{self.ADDRESS}:{self.PORT}/")
+            if "static" or "templates" not in os.listdir():
+                if "static" not in os.listdir():
+                    os.mkdir("static")
+                    print("* Static folder created")
+                elif "templates" not in os.listdir():
+                    os.mkdir("templates")
+                    print("* Templates folder created")
+            print("* Press Ctrl+C to stop")
+            print("========================================")
 
             httpd.serve_forever()
```

### Comparing `MVCactus-0.0.3/MVCactus.egg-info/PKG-INFO` & `MVCactus-0.0.4/MVCactus.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: MVCactus
-Version: 0.0.3
+Version: 0.0.4
 Summary: MVCactus is a lightweight, open-source web framework for building small web applications in Python.
 Author: Dekel Cohen
 Author-email: <dcohen52@gmail.com>
-Keywords: python,web,framework,desktop,html,javascript,styles,js,API,microservices,REST
+Keywords: python,web,framework,microframework,micro-framework,desktop,html,javascript,styles,js,API,microservices,REST,css
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `MVCactus-0.0.3/PKG-INFO` & `MVCactus-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: MVCactus
-Version: 0.0.3
+Version: 0.0.4
 Summary: MVCactus is a lightweight, open-source web framework for building small web applications in Python.
 Author: Dekel Cohen
 Author-email: <dcohen52@gmail.com>
-Keywords: python,web,framework,desktop,html,javascript,styles,js,API,microservices,REST
+Keywords: python,web,framework,microframework,micro-framework,desktop,html,javascript,styles,js,API,microservices,REST,css
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `MVCactus-0.0.3/README.md` & `MVCactus-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `MVCactus-0.0.3/setup.py` & `MVCactus-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'MVCactus is a lightweight, open-source web framework for building small web applications in Python.'
 
 # Setting up
 setup(
     name="MVCactus",
     version=VERSION,
     author="Dekel Cohen",
     author_email="<dcohen52@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
     packages=find_packages(),
     install_requires=['Jinja2'],
-    keywords=['python', 'web', 'framework', 'desktop', 'html', 'javascript', 'styles', 'js', 'API', 'microservices',
-              'REST'],
+    keywords=['python', 'web', 'framework', 'microframework', 'micro-framework', 'desktop', 'html', 'javascript',
+              'styles', 'js', 'API', 'microservices',
+              'REST', 'css'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

