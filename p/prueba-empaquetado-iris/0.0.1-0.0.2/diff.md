# Comparing `tmp/prueba_empaquetado_iris-0.0.1.tar.gz` & `tmp/prueba_empaquetado_iris-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prueba_empaquetado_iris-0.0.1.tar", last modified: Tue May  2 21:27:52 2023, max compression
+gzip compressed data, was "prueba_empaquetado_iris-0.0.2.tar", last modified: Tue May  2 21:37:17 2023, max compression
```

## Comparing `prueba_empaquetado_iris-0.0.1.tar` & `prueba_empaquetado_iris-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:27:52.955309 prueba_empaquetado_iris-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-02 18:24:18.000000 prueba_empaquetado_iris-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      475 2023-05-02 21:27:52.954309 prueba_empaquetado_iris-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-02 17:36:54.000000 prueba_empaquetado_iris-0.0.1/README.md
--rw-rw-rw-   0        0        0      454 2023-05-02 21:27:22.000000 prueba_empaquetado_iris-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 21:27:52.956309 prueba_empaquetado_iris-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 21:27:52.924312 prueba_empaquetado_iris-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-05-02 18:17:02.000000 prueba_empaquetado_iris-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:27:52.931310 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris/
--rw-rw-rw-   0        0        0        0 2023-05-02 18:19:06.000000 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris/__init__.py
--rw-rw-rw-   0        0        0      106 2023-05-02 21:24:32.000000 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris/example.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:27:52.949310 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris.egg-info/
--rw-rw-rw-   0        0        0      475 2023-05-02 21:27:52.000000 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-02 21:27:52.000000 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:27:52.000000 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-02 21:27:52.000000 prueba_empaquetado_iris-0.0.1/src/prueba_empaquetado_iris.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:17.259460 prueba_empaquetado_iris-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-02 18:24:18.000000 prueba_empaquetado_iris-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      475 2023-05-02 21:37:17.256463 prueba_empaquetado_iris-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-02 17:36:54.000000 prueba_empaquetado_iris-0.0.2/README.md
+-rw-rw-rw-   0        0        0      454 2023-05-02 21:36:42.000000 prueba_empaquetado_iris-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:37:17.260461 prueba_empaquetado_iris-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:17.221457 prueba_empaquetado_iris-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-05-02 18:17:02.000000 prueba_empaquetado_iris-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:17.230459 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris/
+-rw-rw-rw-   0        0        0        0 2023-05-02 18:19:06.000000 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-05-02 21:32:12.000000 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris/example.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:17.250459 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris.egg-info/
+-rw-rw-rw-   0        0        0      475 2023-05-02 21:37:17.000000 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-02 21:37:17.000000 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:37:17.000000 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-02 21:37:17.000000 prueba_empaquetado_iris-0.0.2/src/prueba_empaquetado_iris.egg-info/top_level.txt
```

### Comparing `prueba_empaquetado_iris-0.0.1/LICENSE` & `prueba_empaquetado_iris-0.0.2/LICENSE`

 * *Files identical despite different names*

