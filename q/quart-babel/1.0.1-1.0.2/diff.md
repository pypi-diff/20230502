# Comparing `tmp/quart_babel-1.0.1.tar.gz` & `tmp/quart_babel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_babel-1.0.1.tar", max compression
+gzip compressed data, was "quart_babel-1.0.2.tar", max compression
```

## Comparing `quart_babel-1.0.1.tar` & `quart_babel-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1081 2023-02-04 02:05:28.083294 quart_babel-1.0.1/README.md
--rw-r--r--   0        0        0      575 2023-02-04 23:23:04.806825 quart_babel-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1629 2023-02-04 22:56:13.072819 quart_babel-1.0.1/quart_babel/__init__.py
--rw-r--r--   0        0        0      769 2023-02-04 01:40:45.406910 quart_babel-1.0.1/quart_babel/const.py
--rw-r--r--   0        0        0     5560 2023-02-04 01:40:45.524909 quart_babel-1.0.1/quart_babel/context.py
--rw-r--r--   0        0        0     9560 2023-02-04 01:40:45.579909 quart_babel-1.0.1/quart_babel/core.py
--rw-r--r--   0        0        0    12680 2023-02-04 01:40:45.682909 quart_babel-1.0.1/quart_babel/domain.py
--rw-r--r--   0        0        0    11535 2023-02-04 01:40:45.740909 quart_babel-1.0.1/quart_babel/formatters.py
--rw-r--r--   0        0        0     2455 2023-02-04 23:01:40.098052 quart_babel-1.0.1/quart_babel/locale.py
--rw-r--r--   0        0        0     4091 2023-02-04 01:40:45.878909 quart_babel-1.0.1/quart_babel/middleware.py
--rw-r--r--   0        0        0     2145 2023-02-04 01:40:45.982910 quart_babel-1.0.1/quart_babel/speaklater.py
--rw-r--r--   0        0        0     3551 2023-02-04 22:47:56.261566 quart_babel-1.0.1/quart_babel/timezone.py
--rw-r--r--   0        0        0     1290 2023-02-04 01:40:46.158909 quart_babel-1.0.1/quart_babel/typing.py
--rw-r--r--   0        0        0     6217 2023-02-04 01:40:46.215910 quart_babel-1.0.1/quart_babel/utils.py
--rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 quart_babel-1.0.1/setup.py
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 quart_babel-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-30 21:43:53.220523 quart_babel-1.0.2/README.md
+-rw-r--r--   0        0        0      575 2023-05-02 01:44:34.885232 quart_babel-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1562 2023-04-30 23:35:23.300044 quart_babel-1.0.2/quart_babel/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-30 21:43:53.224523 quart_babel-1.0.2/quart_babel/const.py
+-rw-r--r--   0        0        0     5560 2023-04-30 23:10:39.097401 quart_babel-1.0.2/quart_babel/context.py
+-rw-r--r--   0        0        0     9214 2023-04-30 23:33:11.679807 quart_babel-1.0.2/quart_babel/core.py
+-rw-r--r--   0        0        0    12680 2023-04-30 23:33:41.166608 quart_babel-1.0.2/quart_babel/domain.py
+-rw-r--r--   0        0        0    11535 2023-04-30 23:34:10.775248 quart_babel-1.0.2/quart_babel/formatters.py
+-rw-r--r--   0        0        0     2455 2023-04-30 23:34:51.958204 quart_babel-1.0.2/quart_babel/locale.py
+-rw-r--r--   0        0        0     3922 2023-05-02 01:48:37.765650 quart_babel-1.0.2/quart_babel/middleware.py
+-rw-r--r--   0        0        0     2145 2023-04-30 21:43:53.225523 quart_babel-1.0.2/quart_babel/speaklater.py
+-rw-r--r--   0        0        0     2980 2023-04-30 23:07:03.579587 quart_babel-1.0.2/quart_babel/timezone.py
+-rw-r--r--   0        0        0     1235 2023-04-30 23:40:18.654048 quart_babel-1.0.2/quart_babel/typing.py
+-rw-r--r--   0        0        0     4340 2023-04-30 23:10:08.626876 quart_babel-1.0.2/quart_babel/utils.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 quart_babel-1.0.2/PKG-INFO
```

### Comparing `quart_babel-1.0.1/README.md` & `quart_babel-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quart_babel-1.0.1/pyproject.toml` & `quart_babel-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "quart_babel"
-version = "1.0.1"
+version = "1.0.2"
 description = "Implements i18n and l10n support for Quart."
 authors = ["Chris Rood <quart.addons@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 quart = "^0.18.3"
 Babel = "^2.11.0"
-asgi-tools = "^0.64.8"
-ipapi = "^1.0.4"
 importlib-metadata = "^6.0.0"
+pytz = "^2023.3"
+asgi-tools = "^0.73.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 Sphinx = ">=3.4 <6.0.0"
 pydata-sphinx-theme = "^0.12.0"
```

### Comparing `quart_babel-1.0.1/quart_babel/__init__.py` & `quart_babel-1.0.2/quart_babel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 support for date formatting with timezone support as well as a very simple and
 friendly interface :mod:`gettext` translations.
 """
 from .core import Babel
 
 from .domain import (
     Domain,
-    get_domain, 
+    get_domain,
     gettext,
     ngettext,
     pgettext,
     npgettext,
     lazy_gettext,
     lazy_ngettext,
     lazy_pgettext
@@ -41,16 +41,15 @@
     )
 
 from .timezone import (
     get_timezone,
     switch_timezone,
     refresh_timezone,
     to_user_timezone,
-    to_utc,
-    select_timezone_by_request
+    to_utc
     )
 
 __all__ = (
     'Babel',
     'Domain',
     'get_domain',
     'gettext',
@@ -74,10 +73,9 @@
     'switch_locale',
     'refresh_locale',
     'select_locale_by_request',
     'get_timezone',
     'switch_timezone',
     'refresh_timezone',
     'to_user_timezone',
-    'to_utc',
-    'select_timezone_by_request'
+    'to_utc'
 )
```

### Comparing `quart_babel-1.0.1/quart_babel/const.py` & `quart_babel-1.0.2/quart_babel/const.py`

 * *Files identical despite different names*

### Comparing `quart_babel-1.0.1/quart_babel/context.py` & `quart_babel-1.0.2/quart_babel/context.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 Contexts and context helpers for Quart Babel.
 """
 from contextvars import ContextVar, Token
 
 from .typing import Locale, BaseTzInfo
 from .utils import convert_locale, convert_timezone
 
-__all__ = (
-    'LocaleStorageContext',
-    'TimezoneStorageContext'
-)
-
 class LocaleStorageContext:
     """
     Locale Context Storage for Quart Babel.
 
     This class is used to store the locale
     context. It also provides functions to
     work with the context variable.
@@ -170,7 +165,12 @@
             value: The value to set the timezone.
         """
         if value:
             value = convert_timezone(value)
             self.set(value)
         else:
             self.set(self.default_timezone)
+
+__all__ = (
+    'LocaleStorageContext',
+    'TimezoneStorageContext'
+)
```

### Comparing `quart_babel-1.0.1/quart_babel/core.py` & `quart_babel-1.0.2/quart_babel/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,79 +69,73 @@
         self,
         app: Quart | None = None,
         default_locale: str = DEFAULT_LOCALE,
         default_timezone: str = DEFAULT_TIMEZONE,
         date_formats: Quart | t.Dict = None,
         configure_jinja: bool = True,
         default_domain: Domain | None = None,
-        ipapi_key: str | None = None,
         locale_selector: LocaleSelectorFunc | None = None,
         timezone_selector: TimezoneSelectorFunc | None = None
         ) -> None:
         """
         Construct an instance of :class:`quart_babel.Babel`.
 
         Arguments:
             app: The Quart application to use. Defaults to ``None``.
             default_locale: The default locale to be used, defaults to 'en'.
             default_timezone: The default timezone to be used, defaults to 'UTC'.
             date_formats: A mapping of Babel datetime form strings. Defaults to ``None``.
             configure_jinja: Sets if Jinja2 filters are added to the app. Defaults to ``True``.
             default_domain: The default translation domain. Defaults to ``None``.
-            ipapi_key: The IP API key to use. Defaults to ``None``.
             locale_selector: The custom locale selector. Defaults to ``None``.
             timezone_selector: The custom timezone selector. Defaults to ``None``.
         """
         if app is not None:
             self.init_app(
                 app,
                 default_locale,
                 default_timezone,
                 date_formats,
                 configure_jinja,
                 default_domain,
-                ipapi_key,
                 locale_selector,
                 timezone_selector
             )
 
     def init_app(
         self,
         app: Quart,
         default_locale: str = DEFAULT_LOCALE,
         default_timezone: str = DEFAULT_TIMEZONE,
         date_formats: t.Dict | None = None,
         configure_jinja: bool = True,
         default_domain: Domain | None = None,
-        ipapi_key: str | None = None,
         locale_selector: LocaleSelectorFunc | None = None,
         timezone_selector: TimezoneSelectorFunc | None = None
         ) -> None:
         """
         Initialize the Quart-Babel extension with the application.
 
         Arguments:
             app: The Quart application to use. Defaults to ``None``.
             default_locale: The default locale to be used, defaults to 'en'.
             default_timezone: The default timezone to be used, defaults to 'UTC'.
             date_formats: A mapping of Babel datetime form strings. Defaults to ``None``.
             configure_jinja: Sets if Jinja2 filters are added to the app. Defaults to ``True``.
             default_domain: The default translation domain. Defaults to ``None``.
-            ipapi_key: The IP API key to use. Defaults to ``None``.
             locale_selector: The custom locale selector. Defaults to ``None``.
             timezone_selector: The custom timezone selector. Defaults to ``None``.
         """
         if default_domain is None:
             default_domain = Domain()
 
         app.config.setdefault('BABEL_DEFAULT_LOCALE', default_locale)
         app.config.setdefault('BABEL_DEFAULT_TIMEZONE', default_timezone)
         app.config.setdefault('BABEL_CONFIGURE_JINJA', configure_jinja)
         app.config.setdefault('BABEL_DOMAIN', default_domain)
-        app.config.setdefault('BABEL_IPAPI_KEY', ipapi_key)
 
         app.extensions['babel'] = BabelState(
             self, app, app.config['BABEL_DOMAIN']
         )
 
         if self.locale_selector is None and locale_selector is not None:
             self.locale_selector = locale_selector
@@ -185,15 +179,14 @@
             )
 
         app.asgi_app = QuartBabelMiddleware(
             app.asgi_app,
             app.config.get('BABEL_DEFAULT_LOCALE'),
             self.locale_selector,
             app.config.get('BABEL_DEFAULT_TIMEZONE'),
-            app.config.get('BABEL_IPAPI_KEY'),
             self.timezone_selector
         )
 
     @property
     def translations(self) -> Translations:
         """
         Get the translations to use in the template. It will get the domain
```

### Comparing `quart_babel-1.0.1/quart_babel/domain.py` & `quart_babel-1.0.2/quart_babel/domain.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,26 +12,14 @@
 from .speaklater import LazyString
 from .typing import Translations
 from .utils import get_state
 
 if t.TYPE_CHECKING:
     from quart import Quart
 
-__all__ = (
-    'Domain',
-    'get_domain',
-    'gettext',
-    'ngettext',
-    'pgettext',
-    'npgettext',
-    'lazy_gettext',
-    'lazy_ngettext',
-    'lazy_pgettext'
-)
-
 class Domain:
     """
     Localization domain. By default it will look for tranlations in the
     Quart application directory and "messages" domain - all message
     catalogs should be called ``messages.mo``.
     """
     def __init__(
@@ -408,7 +396,19 @@
 
     Arguments:
         context: The context to use.
         singular: The string of the text.
         variables: Kwargs variables for the translation.
     """
     return LazyString(pgettext, context, string, **variables)
+
+__all__ = (
+    'Domain',
+    'get_domain',
+    'gettext',
+    'ngettext',
+    'pgettext',
+    'npgettext',
+    'lazy_gettext',
+    'lazy_ngettext',
+    'lazy_pgettext'
+)
```

### Comparing `quart_babel-1.0.1/quart_babel/formatters.py` & `quart_babel-1.0.2/quart_babel/formatters.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,27 +10,14 @@
 from babel import dates, numbers
 
 from .locale import get_locale
 from .timezone import get_timezone, to_user_timezone
 from .typing import DateTimeFormats, Granularity
 from .utils import get_state
 
-__all__ = (
-    'format_datetime',
-    'format_date',
-    'format_time',
-    'format_timedelta',
-    'format_interval',
-    'format_number',
-    'format_decimal',
-    'format_currency',
-    'format_percent',
-    'format_scientific'
-)
-
 def _date_format(
     formatter: t.Callable,
     obj: t.Any,
     format: str,
     rebase: bool,
     **extra
 ) -> str:
@@ -342,7 +329,20 @@
         format: The format to use.
         decimal_quantization: Truncate and round high-precision numbers to the format
             pattern.
     """
     return numbers.format_scientific(
         number, format=format, locale=get_locale(), decimal_quantization=decimal_quantization
         )
+
+__all__ = (
+    'format_datetime',
+    'format_date',
+    'format_time',
+    'format_timedelta',
+    'format_interval',
+    'format_number',
+    'format_decimal',
+    'format_currency',
+    'format_percent',
+    'format_scientific'
+)
```

### Comparing `quart_babel-1.0.1/quart_babel/locale.py` & `quart_babel-1.0.2/quart_babel/locale.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,14 @@
 from contextlib import contextmanager
 import typing as t
 
 from .context import LocaleStorageContext
 from .typing import ASGIRequest, Locale
 from .utils import convert_locale, parse_accept_header
 
-__all__ = (
-    'setup_locale_context',
-    'get_locale',
-    'set_locale',
-    'switch_locale',
-    'refresh_locale',
-    'select_locale_by_request'
-)
-
 _current_locale = LocaleStorageContext()
 
 def setup_locale_context(default_locale: Locale | str) -> None:
     """
      Setups context with the default locale value using
     `LocaleStorageContext.setup_context` method.
 
@@ -89,7 +80,16 @@
     locale_header = request.headers.get("accept-language")
 
     if locale_header:
         ulocales = list(parse_accept_header(locale_header))
         if ulocales:
             return ulocales[0][1]
     return None
+
+__all__ = (
+    'setup_locale_context',
+    'get_locale',
+    'set_locale',
+    'switch_locale',
+    'refresh_locale',
+    'select_locale_by_request'
+)
```

### Comparing `quart_babel-1.0.1/quart_babel/middleware.py` & `quart_babel-1.0.2/quart_babel/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 quart_babel.middleware
 
 Provides middleware for Babel to use with `Quart`.
 """
 from asgi_tools import Request
 
 from .locale import setup_locale_context, set_locale, select_locale_by_request
-from .timezone import setup_timezone_context, set_timezone, select_timezone_by_request
+from .timezone import setup_timezone_context, set_timezone
 
 from .typing import (
     ASGIApp,
     ASGIRequest,
     Receive,
     Scope,
     Send,
@@ -29,35 +29,32 @@
     """
     def __init__(
         self,
         app: ASGIApp,
         default_locale: str,
         locale_selector: LocaleSelectorFunc | None,
         default_timezone: str,
-        ipapi_key: str | None,
         timezone_selector: TimezoneSelectorFunc | None
         ) -> None:
         """
         Construct an instance of the class.
 
         Attributes:
             app: ASGI Application.
             default_locale: The default locale to use.
             locale_selector: Custom locale selector function.
             default_timezone: The default timezone to use.
-            ipapi_key: The IP API key to use.
             timezone_selector: Custom timezone selector function.
         """
         self.app = app
 
         self.default_locale = default_locale
         self.locale_selector = locale_selector
 
         self.default_timezone = default_timezone
-        self.ipapi_key = ipapi_key
         self.timezone_selector = timezone_selector
 
         setup_locale_context(self.default_locale)
         setup_timezone_context(self.default_timezone)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> ASGIApp:
         """
@@ -72,15 +69,15 @@
         """
         if scope["type"] not in ("http", "websocket"):
             return await self.app(scope, receive, send)
 
         if isinstance(scope, Request):
             request = scope
         else:
-            request = Request(scope)
+            request = Request(scope, receive, send)
 
         await self.detect_locale(request)
         await self.detect_timezone(request)
 
         return await self.app(scope, receive, send)
 
     async def detect_locale(self, request: ASGIRequest) -> None:
@@ -110,16 +107,16 @@
         then the timezone will be determined by the request (scope)
         using the :func:`quart_babel.select_timezone_by_request` function.
 
         Arguments:
             request (`ASGIRequest`): ASGI Request object.
         """
         if self.timezone_selector is not None:
-            tz_info = await self.timezone_selector(request, self.ipapi_key)
-        else:
-            tz_info = await select_timezone_by_request(request, self.ipapi_key)
+            tz_info = await self.timezone_selector(request)
 
-        if tz_info is None:
+            if tz_info is None:
+                tz_info = self.default_timezone
+        else:
             tz_info = self.default_timezone
 
         set_timezone(tz_info)
```

### Comparing `quart_babel-1.0.1/quart_babel/speaklater.py` & `quart_babel-1.0.2/quart_babel/speaklater.py`

 * *Files identical despite different names*

### Comparing `quart_babel-1.0.1/quart_babel/timezone.py` & `quart_babel-1.0.2/quart_babel/timezone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,19 @@
 """
 quart_babel.timezone
 
 Provides helpers for timezone.
 """
 from contextlib import contextmanager
 from datetime import datetime
-import typing as t
-
-import ipapi
+from typing import Generator
 
 from .const import UTC
 from .context import TimezoneStorageContext
-from .typing import ASGIRequest, BaseTzInfo
-from .utils import get_ip_address
-
-__all__ = (
-    'setup_timezone_context',
-    'get_timezone',
-    'set_timezone',
-    'switch_timezone',
-    'refresh_timezone',
-    'to_user_timezone',
-    'to_utc',
-    'select_timezone_by_request'
-)
+from .typing import BaseTzInfo
 
 _current_timezone = TimezoneStorageContext()
 
 def setup_timezone_context(default_timezone: BaseTzInfo | str) -> None:
     """
      Setups context with the default locale value using
     :func:`LocaleStorageContext.setup_context` method.
@@ -51,15 +37,15 @@
 
     Arguments:
         timezone: The timezone to set.
     """
     _current_timezone.set(timezone)
 
 @contextmanager
-def switch_timezone(timezone: str | BaseTzInfo) -> t.Generator[None, None, None]:
+def switch_timezone(timezone: str | BaseTzInfo) -> Generator[None, None, None]:
     """
     Temporary switch current timezone for a code block. The previous timezone
     will be restored after exiting the manager.
 
     Arguments:
         timezone: The timezone to switch to.
     """
@@ -105,25 +91,16 @@
     Arguments:
         dttime (`datetime`): The datetime object to convert.
     """
     if dtime.tzinfo is None:
         dtime = get_timezone().localize(dtime)
     return dtime.astimezone(UTC).replace(tzinfo=None)
 
-async def select_timezone_by_request(
-    request: ASGIRequest,
-    ipapi_key: str | None = None
-    ) -> str | None:
-    """
-    Select the user timezone by a given request.
-
-    Arguments:
-        request: The ASGI Request object.
-        ipapi_key: The IP API key to use.
-    """
-    tzone = None
-    ip_addr = get_ip_address(request)
-
-    if ip_addr is not None:
-        ip_info = ipapi.location(ip_addr, ipapi_key)
-        tzone = ip_info.get('timezone', None)
-    return tzone
+__all__ = (
+    'setup_timezone_context',
+    'get_timezone',
+    'set_timezone',
+    'switch_timezone',
+    'refresh_timezone',
+    'to_user_timezone',
+    'to_utc'
+)
```

### Comparing `quart_babel-1.0.1/quart_babel/typing.py` & `quart_babel-1.0.2/quart_babel/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 Locale = _Locale
 LocaleSelectorFunc = Callable[[ASGIRequest], Awaitable[Optional[str]]]
 ParsedHeader = Iterator[Tuple[float, str]]
 Translations = Union[support.Translations, support.NullTranslations]
 
 # TIMEZONE TYPES - Types used for Timezones.
 BaseTzInfo = _BaseTzInfo
-IPApiKey = NewType("IPApiKey", str)
-TimezoneSelectorFunc = Callable[[ASGIRequest, Optional[IPApiKey]], Awaitable[Optional[str]]]
+TimezoneSelectorFunc = Callable[[ASGIRequest,], Awaitable[Optional[str]]]
 
 # DATETIME TYPES
 DateTimeFormats = Literal["short", "medium", "long", "full"]
 
 TimeDeltaFormats = Literal["narrow", "short", "long"]
 
 Granularity = Literal["year", "month", "week", "day", "hour", "minute", "second"]
```

### Comparing `quart_babel-1.0.1/PKG-INFO` & `quart_babel-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: quart-babel
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implements i18n and l10n support for Quart.
 License: MIT
 Author: Chris Rood
 Author-email: quart.addons@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Babel (>=2.11.0,<3.0.0)
-Requires-Dist: asgi-tools (>=0.64.8,<0.65.0)
+Requires-Dist: asgi-tools (>=0.73.2,<0.74.0)
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
-Requires-Dist: ipapi (>=1.0.4,<2.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: quart (>=0.18.3,<0.19.0)
 Description-Content-Type: text/markdown
 
 # Quart Babel
 
 ![Quart Uploads Logo](logos/logo.png)
```

