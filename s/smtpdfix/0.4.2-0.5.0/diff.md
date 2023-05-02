# Comparing `tmp/smtpdfix-0.4.2.tar.gz` & `tmp/smtpdfix-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smtpdfix-0.4.2.tar", last modified: Sat Mar 25 21:35:04 2023, max compression
+gzip compressed data, was "smtpdfix-0.5.0.tar", last modified: Tue May  2 17:47:10 2023, max compression
```

## Comparing `smtpdfix-0.4.2.tar` & `smtpdfix-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-03-25 21:35:04.944757 smtpdfix-0.4.2/
--rw-r--r--   0 james     (1000) james     (1000)     1089 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/LICENSE
--rw-r--r--   0 james     (1000) james     (1000)    10806 2023-03-25 21:35:04.944757 smtpdfix-0.4.2/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)     9808 2022-09-05 12:39:41.000000 smtpdfix-0.4.2/README.md
--rw-r--r--   0 james     (1000) james     (1000)       90 2023-01-05 22:40:35.000000 smtpdfix-0.4.2/pyproject.toml
--rw-r--r--   0 james     (1000) james     (1000)     2062 2023-03-25 21:35:04.954757 smtpdfix-0.4.2/setup.cfg
--rw-r--r--   0 james     (1000) james     (1000)       41 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/setup.py
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-03-25 21:35:04.934757 smtpdfix-0.4.2/smtpdfix/
--rw-r--r--   0 james     (1000) james     (1000)      363 2023-03-25 21:34:35.000000 smtpdfix-0.4.2/smtpdfix/__init__.py
--rw-r--r--   0 james     (1000) james     (1000)     1041 2022-11-12 12:17:37.000000 smtpdfix-0.4.2/smtpdfix/authenticator.py
--rw-r--r--   0 james     (1000) james     (1000)     3063 2022-09-05 11:25:36.000000 smtpdfix-0.4.2/smtpdfix/certs.py
--rw-r--r--   0 james     (1000) james     (1000)     5176 2022-11-12 12:25:54.000000 smtpdfix-0.4.2/smtpdfix/configuration.py
--rw-r--r--   0 james     (1000) james     (1000)     8044 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/smtpdfix/controller.py
--rw-r--r--   0 james     (1000) james     (1000)      640 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/smtpdfix/event_handler.py
--rw-r--r--   0 james     (1000) james     (1000)     2505 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/smtpdfix/fixture.py
--rw-r--r--   0 james     (1000) james     (1000)     3400 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/smtpdfix/handlers.py
--rw-r--r--   0 james     (1000) james     (1000)        0 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/smtpdfix/py.typed
--rw-r--r--   0 james     (1000) james     (1000)     1660 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/smtpdfix/smtp.py
--rw-r--r--   0 james     (1000) james     (1000)      673 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/smtpdfix/typing.py
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-03-25 21:35:04.934757 smtpdfix-0.4.2/smtpdfix.egg-info/
--rw-r--r--   0 james     (1000) james     (1000)    10806 2023-03-25 21:35:04.000000 smtpdfix-0.4.2/smtpdfix.egg-info/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      633 2023-03-25 21:35:04.000000 smtpdfix-0.4.2/smtpdfix.egg-info/SOURCES.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2023-03-25 21:35:04.000000 smtpdfix-0.4.2/smtpdfix.egg-info/dependency_links.txt
--rw-r--r--   0 james     (1000) james     (1000)       36 2023-03-25 21:35:04.000000 smtpdfix-0.4.2/smtpdfix.egg-info/entry_points.txt
--rw-r--r--   0 james     (1000) james     (1000)      242 2023-03-25 21:35:04.000000 smtpdfix-0.4.2/smtpdfix.egg-info/requires.txt
--rw-r--r--   0 james     (1000) james     (1000)       15 2023-03-25 21:35:04.000000 smtpdfix-0.4.2/smtpdfix.egg-info/top_level.txt
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-03-25 21:35:04.944757 smtpdfix-0.4.2/tests/
--rw-r--r--   0 james     (1000) james     (1000)        0 2022-06-28 23:27:52.000000 smtpdfix-0.4.2/tests/__init__.py
--rw-r--r--   0 james     (1000) james     (1000)     1191 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/tests/conftest.py
--rw-r--r--   0 james     (1000) james     (1000)     3341 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/tests/test_configuration.py
--rw-r--r--   0 james     (1000) james     (1000)     5446 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/tests/test_controller.py
--rw-r--r--   0 james     (1000) james     (1000)     7914 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/tests/test_fixture.py
--rw-r--r--   0 james     (1000) james     (1000)     3057 2022-10-30 00:06:09.000000 smtpdfix-0.4.2/tests/test_smtp.py
--rw-r--r--   0 james     (1000) james     (1000)     1068 2022-12-03 17:17:56.000000 smtpdfix-0.4.2/tests/test_smtpdfix.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/
+-rw-r--r--   0 james     (1000) james     (1000)     1089 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/LICENSE
+-rw-r--r--   0 james     (1000) james     (1000)    10715 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)     9715 2023-05-02 16:10:21.000000 smtpdfix-0.5.0/README.md
+-rw-r--r--   0 james     (1000) james     (1000)       90 2023-01-05 22:40:35.000000 smtpdfix-0.5.0/pyproject.toml
+-rw-r--r--   0 james     (1000) james     (1000)     2113 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/setup.cfg
+-rw-r--r--   0 james     (1000) james     (1000)       41 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/setup.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.721994 smtpdfix-0.5.0/smtpdfix/
+-rw-r--r--   0 james     (1000) james     (1000)      342 2023-05-02 17:45:20.000000 smtpdfix-0.5.0/smtpdfix/__init__.py
+-rw-r--r--   0 james     (1000) james     (1000)     1041 2022-11-12 12:17:37.000000 smtpdfix-0.5.0/smtpdfix/authenticator.py
+-rw-r--r--   0 james     (1000) james     (1000)     3063 2022-09-05 11:25:36.000000 smtpdfix-0.5.0/smtpdfix/certs.py
+-rw-r--r--   0 james     (1000) james     (1000)     5027 2023-05-02 16:10:21.000000 smtpdfix-0.5.0/smtpdfix/configuration.py
+-rw-r--r--   0 james     (1000) james     (1000)     8008 2023-05-02 16:10:16.000000 smtpdfix-0.5.0/smtpdfix/controller.py
+-rw-r--r--   0 james     (1000) james     (1000)      640 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/event_handler.py
+-rw-r--r--   0 james     (1000) james     (1000)     2606 2023-05-02 16:10:21.000000 smtpdfix-0.5.0/smtpdfix/fixture.py
+-rw-r--r--   0 james     (1000) james     (1000)     3400 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/handlers.py
+-rw-r--r--   0 james     (1000) james     (1000)        0 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/py.typed
+-rw-r--r--   0 james     (1000) james     (1000)     1660 2023-04-10 17:16:42.000000 smtpdfix-0.5.0/smtpdfix/smtp.py
+-rw-r--r--   0 james     (1000) james     (1000)      673 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/smtpdfix/typing.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.731994 smtpdfix-0.5.0/smtpdfix.egg-info/
+-rw-r--r--   0 james     (1000) james     (1000)    10715 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)      633 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/SOURCES.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/dependency_links.txt
+-rw-r--r--   0 james     (1000) james     (1000)       36 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/entry_points.txt
+-rw-r--r--   0 james     (1000) james     (1000)      239 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/requires.txt
+-rw-r--r--   0 james     (1000) james     (1000)       15 2023-05-02 17:47:10.000000 smtpdfix-0.5.0/smtpdfix.egg-info/top_level.txt
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-02 17:47:10.741994 smtpdfix-0.5.0/tests/
+-rw-r--r--   0 james     (1000) james     (1000)        0 2022-06-28 23:27:52.000000 smtpdfix-0.5.0/tests/__init__.py
+-rw-r--r--   0 james     (1000) james     (1000)     1191 2022-12-03 17:17:56.000000 smtpdfix-0.5.0/tests/conftest.py
+-rw-r--r--   0 james     (1000) james     (1000)     3016 2023-04-03 11:16:42.000000 smtpdfix-0.5.0/tests/test_configuration.py
+-rw-r--r--   0 james     (1000) james     (1000)     4789 2023-04-03 11:16:42.000000 smtpdfix-0.5.0/tests/test_controller.py
+-rw-r--r--   0 james     (1000) james     (1000)     7914 2023-04-01 17:11:44.000000 smtpdfix-0.5.0/tests/test_fixture.py
+-rw-r--r--   0 james     (1000) james     (1000)     3057 2023-04-10 17:11:14.000000 smtpdfix-0.5.0/tests/test_smtp.py
+-rw-r--r--   0 james     (1000) james     (1000)     1068 2023-04-08 16:47:14.000000 smtpdfix-0.5.0/tests/test_smtpdfix.py
```

### Comparing `smtpdfix-0.4.2/LICENSE` & `smtpdfix-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/PKG-INFO` & `smtpdfix-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtpdfix
-Version: 0.4.2
+Version: 0.5.0
 Summary: A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 Home-page: https://github.com/bebleo/smtpdfix
 Author: James Warne
 Author-email: bebleo@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/bebleo/smtpdfix
 Project-URL: Documentation, https://github.com/bebleo/smtpdfix#readme
@@ -145,26 +145,24 @@
 ### Configuration
 
 Configuration is handled through properties in the `config` of the fixture and are initially set from environment variables:
 
 Property         | Variable               | Default              | Description
 -----------------|------------------------|----------------------|------------
 `host`           | `SMTPD_HOST`           | `127.0.0.1` or `::1` | The hostname that the fixture will listen on.
-`port`           | `SMTPD_PORT`           | `8025`               | The port that the fixture will listen on.
+`port`           | `SMTPD_PORT`           | `a random free port` | The port that the fixture will listen on.
 `ready_timeout`  | `SMTPD_READY_TIMEOUT`  | `10.0`               | The seconds the server will wait to start before raising a `TimeoutError`.
 `login_username` | `SMTPD_LOGIN_NAME`     | `user`               | Username for default authentication.
 `login_password` | `SMTPD_LOGIN_PASSWORD` | `password`           | Password for default authentication.
 `use_ssl`        | `SMTPD_USE_SSL`        | `False`              | Whether the fixture should use fixed TLS/SSL for transactions. If using smtplib requires that `SMTP_SSL` be used instead of `SMTP`.
 `use_starttls`   | `SMTPD_USE_STARTTLS`   | `False`              | Whether the fixture should use StartTLS to encrypt the connections. If using `smtplib` requires that `SMTP.starttls()` is called before other commands are issued. Overrides `use_tls` as the preferred method for securing communications with the client.
 `enforce_auth`   | `SMTPD_ENFORCE_AUTH`   | `False`              | If set to true then the fixture refuses MAIL, RCPT, DATA commands until authentication is completed.
 `ssl_cert_path`  | `SMTPD_SSL_CERTS_PATH` | `./certs/`           | The path to the key and certificate in PEM format for encryption with SSL/TLS or StartTLS.
 `ssl_cert_files` | `SMTPD_SSL_CERT_FILE` and `SMTPD_SSL_KEY_FILE` | `("cert.pem", None)` | A tuple of the path for the certificate file and key file in PEM format. See [Resolving certificate and key paths](#resolving-certificate-and-key-paths) for more details.
 
-> If environment variables are included in a `.env` file they'll be loaded automatically.
-
 ### Resolving certificate and key paths
 
 In order to resolve the certificate and key paths for the SSL/TLS context SMTPDFix does the following:
 
 1. On initialization of a `smtpdfix.Config` the `ssl_cert_path` is set by the `SMTPD_SSL_CERTS_PATH` environment variable and the `ssl_cert_files` is set to a tuple of `(SMTPD_SSL_CERT_FILE and SMTPD_SSL_KEY_FILE)`. If the environment variables are not set the deafults are used.
 2. If an SSL Context is needed, when the `smptdfix.AuthController` is initialized it will attempt to find the files in the following sequence for both the certificate file and the key file:
    1. If the value in `ssl_cert_files` is `None` then `None` is returned. Setting the key file to be none assumes that it has been included in the certificate file.
```

### Comparing `smtpdfix-0.4.2/README.md` & `smtpdfix-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,26 +116,24 @@
 ### Configuration
 
 Configuration is handled through properties in the `config` of the fixture and are initially set from environment variables:
 
 Property         | Variable               | Default              | Description
 -----------------|------------------------|----------------------|------------
 `host`           | `SMTPD_HOST`           | `127.0.0.1` or `::1` | The hostname that the fixture will listen on.
-`port`           | `SMTPD_PORT`           | `8025`               | The port that the fixture will listen on.
+`port`           | `SMTPD_PORT`           | `a random free port` | The port that the fixture will listen on.
 `ready_timeout`  | `SMTPD_READY_TIMEOUT`  | `10.0`               | The seconds the server will wait to start before raising a `TimeoutError`.
 `login_username` | `SMTPD_LOGIN_NAME`     | `user`               | Username for default authentication.
 `login_password` | `SMTPD_LOGIN_PASSWORD` | `password`           | Password for default authentication.
 `use_ssl`        | `SMTPD_USE_SSL`        | `False`              | Whether the fixture should use fixed TLS/SSL for transactions. If using smtplib requires that `SMTP_SSL` be used instead of `SMTP`.
 `use_starttls`   | `SMTPD_USE_STARTTLS`   | `False`              | Whether the fixture should use StartTLS to encrypt the connections. If using `smtplib` requires that `SMTP.starttls()` is called before other commands are issued. Overrides `use_tls` as the preferred method for securing communications with the client.
 `enforce_auth`   | `SMTPD_ENFORCE_AUTH`   | `False`              | If set to true then the fixture refuses MAIL, RCPT, DATA commands until authentication is completed.
 `ssl_cert_path`  | `SMTPD_SSL_CERTS_PATH` | `./certs/`           | The path to the key and certificate in PEM format for encryption with SSL/TLS or StartTLS.
 `ssl_cert_files` | `SMTPD_SSL_CERT_FILE` and `SMTPD_SSL_KEY_FILE` | `("cert.pem", None)` | A tuple of the path for the certificate file and key file in PEM format. See [Resolving certificate and key paths](#resolving-certificate-and-key-paths) for more details.
 
-> If environment variables are included in a `.env` file they'll be loaded automatically.
-
 ### Resolving certificate and key paths
 
 In order to resolve the certificate and key paths for the SSL/TLS context SMTPDFix does the following:
 
 1. On initialization of a `smtpdfix.Config` the `ssl_cert_path` is set by the `SMTPD_SSL_CERTS_PATH` environment variable and the `ssl_cert_files` is set to a tuple of `(SMTPD_SSL_CERT_FILE and SMTPD_SSL_KEY_FILE)`. If the environment variables are not set the deafults are used.
 2. If an SSL Context is needed, when the `smptdfix.AuthController` is initialized it will attempt to find the files in the following sequence for both the certificate file and the key file:
    1. If the value in `ssl_cert_files` is `None` then `None` is returned. Setting the key file to be none assumes that it has been included in the certificate file.
```

### Comparing `smtpdfix-0.4.2/setup.cfg` & `smtpdfix-0.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 description = A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bebleo/smtpdfix
 author = James Warne
 author_email = bebleo@yahoo.com
 license = MIT
-license_file = LICENSE
+license_files = 
+	LICENSE
 classifiers = 
 	Framework :: Pytest
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
@@ -30,16 +31,16 @@
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
 	aiosmtpd
 	cryptography;python_implementation!="PyPy"
 	cryptography >= 39.0.1, < 40.0.0;python_implementation=="PyPy"
+	portpicker
 	pytest
-	python-dotenv
 python_requires = >=3.7
 
 [options.entry_points]
 pytest11 = 
 	smtpd = smtpdfix.fixture
 
 [options.extras_require]
@@ -78,11 +79,14 @@
 no_implicit_reexport = True
 warn_redundant_casts = True
 warn_unused_configs = True
 warn_unused_ignores = True
 warn_return_any = True
 follow_imports = skip
 
+[mypy-portpicker.*]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `smtpdfix-0.4.2/smtpdfix/authenticator.py` & `smtpdfix-0.5.0/smtpdfix/authenticator.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/smtpdfix/certs.py` & `smtpdfix-0.5.0/smtpdfix/certs.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/smtpdfix/configuration.py` & `smtpdfix-0.5.0/smtpdfix/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 from pathlib import Path
 from typing import Any, Optional, Tuple, Union
 
-from dotenv import load_dotenv
+import portpicker
 
 from .event_handler import EventHandler
 from .typing import PathType
 
 _current_dir = Path(__file__).parent
-load_dotenv()
 
 
 def _strtobool(val: str) -> bool:
     """Convert a string representation of truth to true (1) or false (0).
 
     True values are "y", "yes", "t", "true", "on", and "1"; false values are
     "n", "no", "f", "false", "off", and "0".  Raises ValueError if "val" is
@@ -26,24 +25,22 @@
     elif val in ("n", "no", "f", "false", "off", "0"):
         return False
     else:
         raise ValueError(f"invalid truth value {val}")
 
 
 class Config():
-    def __init__(self,
-                 filename: Optional[PathType] = None,
-                 override: bool = False) -> None:
-        if filename:
-            load_dotenv(filename, override=override)
+    def __init__(self) -> None:
 
         self.OnChanged = EventHandler()
 
         self._host = os.getenv("SMTPD_HOST")
-        self._port = int(os.getenv("SMTPD_PORT", 8025))
+        self._port = int(
+            os.getenv("SMTPD_PORT", portpicker.pick_unused_port())
+        )
         self._ready_timeout = float(os.getenv("SMTPD_READY_TIMEOUT", 10.0))
         self._login_username = os.getenv("SMTPD_LOGIN_NAME", "user")
         self._login_password = os.getenv("SMTPD_LOGIN_PASSWORD", "password")
         self._enforce_auth = _strtobool(os.getenv("SMTPD_ENFORCE_AUTH",
                                                   "False"))
         self._auth_require_tls = _strtobool(os.getenv("SMTPD_AUTH_REQUIRE_TLS",
                                                       "True"))
```

### Comparing `smtpdfix-0.4.2/smtpdfix/controller.py` & `smtpdfix-0.5.0/smtpdfix/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,15 @@
                          ready_timeout=_ready_timeout,
                          ssl_context=context_or_none(),
                          authenticator=self._authenticator,
                          **kwargs)
 
         # The event handler for changes to the config goes here to prevent it
         # firing when the obkect is initialized.
-        if hostname is not None:
-            self.config.host = hostname
+        self.config.host = _hostname
         if port is not None:
             self.config.port = port
         self.config.OnChanged += self.reset
         log.info(f"SMTPDFix running on {self.hostname}:{self.port}")
 
     def factory(self) -> _SMTP:
         use_starttls = self.config.use_starttls
```

### Comparing `smtpdfix-0.4.2/smtpdfix/event_handler.py` & `smtpdfix-0.5.0/smtpdfix/event_handler.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/smtpdfix/fixture.py` & `smtpdfix-0.5.0/smtpdfix/fixture.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 from typing import Any, Generator, Optional
 
+import portpicker
 import pytest
 
 from .authenticator import Authenticator
 from .certs import _generate_certs
 from .configuration import Config
 from .controller import AuthController
 from .typing import TempPathFactory
@@ -34,18 +35,22 @@
     def get_password(self, username: Optional[str]) -> str:
         return str(self.config.login_password)
 
 
 class SMTPDFix():
     def __init__(self,
                  hostname: Optional[str] = None,
-                 port: int = 8025,
+                 port: Optional[int] = None,
                  config: Optional[Config] = None) -> None:
         self.hostname = hostname
-        self.port = int(port) if port is not None else 8025
+        self.port = (
+            int(port)
+            if port is not None
+            else portpicker.pick_unused_port()
+        )
         self.config = config or Config()
 
     def __enter__(self) -> AuthController:
         self.controller = AuthController(
             hostname=self.hostname,
             port=self.port,
             config=self.config,
```

### Comparing `smtpdfix-0.4.2/smtpdfix/handlers.py` & `smtpdfix-0.5.0/smtpdfix/handlers.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/smtpdfix/smtp.py` & `smtpdfix-0.5.0/smtpdfix/smtp.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/smtpdfix/typing.py` & `smtpdfix-0.5.0/smtpdfix/typing.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/smtpdfix.egg-info/PKG-INFO` & `smtpdfix-0.5.0/smtpdfix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtpdfix
-Version: 0.4.2
+Version: 0.5.0
 Summary: A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 Home-page: https://github.com/bebleo/smtpdfix
 Author: James Warne
 Author-email: bebleo@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/bebleo/smtpdfix
 Project-URL: Documentation, https://github.com/bebleo/smtpdfix#readme
@@ -145,26 +145,24 @@
 ### Configuration
 
 Configuration is handled through properties in the `config` of the fixture and are initially set from environment variables:
 
 Property         | Variable               | Default              | Description
 -----------------|------------------------|----------------------|------------
 `host`           | `SMTPD_HOST`           | `127.0.0.1` or `::1` | The hostname that the fixture will listen on.
-`port`           | `SMTPD_PORT`           | `8025`               | The port that the fixture will listen on.
+`port`           | `SMTPD_PORT`           | `a random free port` | The port that the fixture will listen on.
 `ready_timeout`  | `SMTPD_READY_TIMEOUT`  | `10.0`               | The seconds the server will wait to start before raising a `TimeoutError`.
 `login_username` | `SMTPD_LOGIN_NAME`     | `user`               | Username for default authentication.
 `login_password` | `SMTPD_LOGIN_PASSWORD` | `password`           | Password for default authentication.
 `use_ssl`        | `SMTPD_USE_SSL`        | `False`              | Whether the fixture should use fixed TLS/SSL for transactions. If using smtplib requires that `SMTP_SSL` be used instead of `SMTP`.
 `use_starttls`   | `SMTPD_USE_STARTTLS`   | `False`              | Whether the fixture should use StartTLS to encrypt the connections. If using `smtplib` requires that `SMTP.starttls()` is called before other commands are issued. Overrides `use_tls` as the preferred method for securing communications with the client.
 `enforce_auth`   | `SMTPD_ENFORCE_AUTH`   | `False`              | If set to true then the fixture refuses MAIL, RCPT, DATA commands until authentication is completed.
 `ssl_cert_path`  | `SMTPD_SSL_CERTS_PATH` | `./certs/`           | The path to the key and certificate in PEM format for encryption with SSL/TLS or StartTLS.
 `ssl_cert_files` | `SMTPD_SSL_CERT_FILE` and `SMTPD_SSL_KEY_FILE` | `("cert.pem", None)` | A tuple of the path for the certificate file and key file in PEM format. See [Resolving certificate and key paths](#resolving-certificate-and-key-paths) for more details.
 
-> If environment variables are included in a `.env` file they'll be loaded automatically.
-
 ### Resolving certificate and key paths
 
 In order to resolve the certificate and key paths for the SSL/TLS context SMTPDFix does the following:
 
 1. On initialization of a `smtpdfix.Config` the `ssl_cert_path` is set by the `SMTPD_SSL_CERTS_PATH` environment variable and the `ssl_cert_files` is set to a tuple of `(SMTPD_SSL_CERT_FILE and SMTPD_SSL_KEY_FILE)`. If the environment variables are not set the deafults are used.
 2. If an SSL Context is needed, when the `smptdfix.AuthController` is initialized it will attempt to find the files in the following sequence for both the certificate file and the key file:
    1. If the value in `ssl_cert_files` is `None` then `None` is returned. Setting the key file to be none assumes that it has been included in the certificate file.
```

### Comparing `smtpdfix-0.4.2/smtpdfix.egg-info/SOURCES.txt` & `smtpdfix-0.5.0/smtpdfix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/tests/conftest.py` & `smtpdfix-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/tests/test_configuration.py` & `smtpdfix-0.5.0/tests/test_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import functools
-import os
-from pathlib import Path
 from typing import Any, Generator, List
 
 import pytest
 
 from smtpdfix.configuration import Config, _strtobool
 from smtpdfix.event_handler import EventHandler
 
@@ -66,25 +64,14 @@
 
 
 def test_init() -> None:
     config = Config()
     assert isinstance(config, Config)
 
 
-def test_init_envfile() -> None:
-    original_env = os.environ.copy()
-    config_file = Path(__file__).parent.joinpath("assets/.test.env")
-    config = Config(filename=config_file, override=True)
-
-    assert config.port == 5025
-
-    os.environ.clear()
-    os.environ.update(original_env)
-
-
 @pytest.mark.parametrize("attr, value, expected, type", values)
 def test_set_values(attr: str, value: Any, expected: Any, type: Any) -> None:
     config = Config()
     setattr(config, attr, value)
     assert isinstance(getattr(config, attr), type)
     assert getattr(config, attr) == expected
```

### Comparing `smtpdfix-0.4.2/tests/test_controller.py` & `smtpdfix-0.5.0/tests/test_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
-import os
 import ssl
 from email.message import EmailMessage
-from pathlib import Path
 from smtplib import SMTP, SMTP_SSL, SMTPSenderRefused, SMTPServerDisconnected
 
 import pytest
 from pytest import FixtureRequest, TempPathFactory
 
 from smtpdfix.certs import _generate_certs
 from smtpdfix.configuration import Config
@@ -120,33 +118,14 @@
         with SMTP(server.hostname, server.port) as client:
             # this should return a 523 Encryption required error
             # but instead returns an SMTPServerDisconnected Error
             client.send_message(msg)
             assert len(server.messages) == 1
 
 
-def test_config_file(request: FixtureRequest, msg: EmailMessage) -> None:
-    _original_env = os.environ.copy()
-    config_file = Path(__file__).parent.joinpath("assets/.test.env")
-    _config = Config(filename=config_file, override=True)
-    server = AuthController(hostname=_config.host,
-                            port=_config.port,
-                            config=_config)
-    request.addfinalizer(server.stop)
-    server.start()
-
-    with SMTP(server.hostname, server.port) as client:
-        client.send_message(msg)
-
-    assert server.port == 5025
-
-    os.environ.clear()
-    os.environ.update(_original_env)
-
-
 def test_exception_handler(request: FixtureRequest, msg: EmailMessage) -> None:
     def raise_error() -> None:
         raise Exception("Deliberately raised error.")
 
     server = AuthController()
     request.addfinalizer(server.stop)
     server.start()
```

### Comparing `smtpdfix-0.4.2/tests/test_fixture.py` & `smtpdfix-0.5.0/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/tests/test_smtp.py` & `smtpdfix-0.5.0/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.4.2/tests/test_smtpdfix.py` & `smtpdfix-0.5.0/tests/test_smtpdfix.py`

 * *Files identical despite different names*

