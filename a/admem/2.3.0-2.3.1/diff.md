# Comparing `tmp/admem-2.3.0.tar.gz` & `tmp/admem-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admem-2.3.0.tar", last modified: Fri Apr 28 09:19:35 2023, max compression
+gzip compressed data, was "admem-2.3.1.tar", last modified: Tue May  2 15:21:16 2023, max compression
```

## Comparing `admem-2.3.0.tar` & `admem-2.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.503958 admem-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-20 07:45:29.000000 admem-2.3.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-28 09:19:35.503958 admem-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-28 09:19:35.507958 admem-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.487958 admem-2.3.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.499958 admem-2.3.0/source/admem/
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-28 09:14:04.000000 admem-2.3.0/source/admem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_backend_manager_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     6684 2023-04-28 09:16:24.000000 admem-2.3.0/source/admem/_create_django_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     8304 2023-04-28 09:04:15.000000 admem-2.3.0/source/admem/_django_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_inspect_dataclass.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-28 09:04:15.000000 admem-2.3.0/source/admem/_path_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-27 21:17:11.000000 admem-2.3.0/source/admem/_protocols.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-04-26 22:14:31.000000 admem-2.3.0/source/admem/_store_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-27 21:17:11.000000 admem-2.3.0/source/admem/_sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_util.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.503958 admem-2.3.0/source/admem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:19:17.000000 admem-2.3.0/source/admem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.617513 admem-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-05-02 14:46:08.000000 admem-2.3.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 15:21:16.617513 admem-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-02 15:21:16.621513 admem-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.601512 admem-2.3.1/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.613512 admem-2.3.1/source/admem/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_backend_manager_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_create_django_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8282 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_django_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_inspect_dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-05-02 15:02:28.000000 admem-2.3.1/source/admem/_path_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_store_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.617513 admem-2.3.1/source/admem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:20:57.000000 admem-2.3.1/source/admem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/top_level.txt
```

### Comparing `admem-2.3.0/LICENSE.txt` & `admem-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/setup.cfg` & `admem-2.3.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [options.package_data]
 * = *.typed
 admem = 
 	source/admem/py.typed
 
 [options.extras_require]
 dev = 
-	adaux==2.4.0
+	adaux==2.4.4
 	pre-commit>=2.20
 	mypy==1.1.1
 	pylint==2.17.1
 	django-stubs==1.12.0
 test = 
 	pytest>=7.2
 	pytest-cov~=4.0
```

### Comparing `admem-2.3.0/source/admem/__init__.py` & `admem-2.3.1/source/admem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     + _sync_store.__all__
     + _store_setup.__all__
     + _create_django_model.__all__
     + _inspect_dataclass.__all__
 )
 
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
```

### Comparing `admem-2.3.0/source/admem/_backend_manager_proxy.py` & `admem-2.3.1/source/admem/_backend_manager_proxy.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem/_create_django_model.py` & `admem-2.3.1/source/admem/_create_django_model.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem/_decorator.py` & `admem-2.3.1/source/admem/_decorator.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem/_django_store.py` & `admem-2.3.1/source/admem/_django_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,22 +126,21 @@
         raise NotImplementedError(val)
 
     def create_dj_path(
         self, model: type[models.Model], dc_field: dc.Field[Path]
     ) -> tp.Callable[[FieldFile], DjangoPath]:
         # pylint: disable=protected-access
         dj_field = model._meta.get_field(dc_field.name)
-        prefix = None
+        prefix: str | None = None
         if hasattr(dj_field, "upload_to"):
             prefix = getattr(dj_field, "upload_to")
 
         def inner(fieldfile: FieldFile) -> DjangoPath:
             assert fieldfile.name
-            res = DjangoPath(fieldfile.name)
-            res._prefix = prefix  # type: ignore
+            res = DjangoPath.create(fieldfile.name, prefix)
             return res
 
         return inner
 
     def django_to_dataclass(self, dj_obj: models.Model) -> tp.Any:
         dataclass = BACKEND_LINKER.backend_to_dc[type(dj_obj)]
         obj_kwgs = {}
```

### Comparing `admem-2.3.0/source/admem/_inspect_dataclass.py` & `admem-2.3.1/source/admem/_inspect_dataclass.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem/_protocols.py` & `admem-2.3.1/source/admem/_protocols.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem/_store_setup.py` & `admem-2.3.1/source/admem/_store_setup.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem/_sync_store.py` & `admem-2.3.1/source/admem/_sync_store.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.0/source/admem.egg-info/SOURCES.txt` & `admem-2.3.1/source/admem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

