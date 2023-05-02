# Comparing `tmp/fugle-trade-0.5.0.tar.gz` & `tmp/fugle-trade-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugle-trade-0.5.0.tar", max compression
+gzip compressed data, was "fugle-trade-0.5.1.tar", max compression
```

## Comparing `fugle-trade-0.5.0.tar` & `fugle-trade-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1075 2023-02-24 09:12:06.254393 fugle-trade-0.5.0/LICENSE
--rw-r--r--   0        0        0      776 2023-02-24 09:12:06.254393 fugle-trade-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-02-24 09:12:06.254393 fugle-trade-0.5.0/fugle_trade/__init__.py
--rw-r--r--   0        0        0      760 2023-02-24 09:12:06.254393 fugle-trade-0.5.0/fugle_trade/constant.py
--rw-r--r--   0        0        0      469 2023-02-24 09:12:06.254393 fugle-trade-0.5.0/fugle_trade/init.py
--rw-r--r--   0        0        0     2616 2023-02-24 09:12:06.258393 fugle-trade-0.5.0/fugle_trade/order.py
--rw-r--r--   0        0        0     8658 2023-02-24 09:12:06.258393 fugle-trade-0.5.0/fugle_trade/sdk.py
--rw-r--r--   0        0        0     1924 2023-02-24 09:12:06.258393 fugle-trade-0.5.0/fugle_trade/util.py
--rw-r--r--   0        0        0     1784 2023-02-24 09:12:06.258393 fugle-trade-0.5.0/fugle_trade/websocket.py
--rw-r--r--   0        0        0      772 2023-02-24 09:12:06.258393 fugle-trade-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1559 2023-02-24 09:12:28.327043 fugle-trade-0.5.0/setup.py
--rw-r--r--   0        0        0     1701 2023-02-24 09:12:28.327395 fugle-trade-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/LICENSE
+-rw-r--r--   0        0        0      776 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/__init__.py
+-rw-r--r--   0        0        0      760 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/constant.py
+-rw-r--r--   0        0        0      469 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/init.py
+-rw-r--r--   0        0        0     2616 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/order.py
+-rw-r--r--   0        0        0     8658 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/sdk.py
+-rw-r--r--   0        0        0     1924 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/util.py
+-rw-r--r--   0        0        0     1842 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/fugle_trade/websocket.py
+-rw-r--r--   0        0        0      772 2023-05-02 08:19:50.921872 fugle-trade-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1559 2023-05-02 08:20:03.063463 fugle-trade-0.5.1/setup.py
+-rw-r--r--   0        0        0     1701 2023-05-02 08:20:03.063759 fugle-trade-0.5.1/PKG-INFO
```

### Comparing `fugle-trade-0.5.0/LICENSE` & `fugle-trade-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugle-trade-0.5.0/README.md` & `fugle-trade-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fugle-trade-0.5.0/fugle_trade/constant.py` & `fugle-trade-0.5.1/fugle_trade/constant.py`

 * *Files identical despite different names*

### Comparing `fugle-trade-0.5.0/fugle_trade/order.py` & `fugle-trade-0.5.1/fugle_trade/order.py`

 * *Files identical despite different names*

### Comparing `fugle-trade-0.5.0/fugle_trade/sdk.py` & `fugle-trade-0.5.1/fugle_trade/sdk.py`

 * *Files identical despite different names*

### Comparing `fugle-trade-0.5.0/fugle_trade/util.py` & `fugle-trade-0.5.1/fugle_trade/util.py`

 * *Files identical despite different names*

### Comparing `fugle-trade-0.5.0/fugle_trade/websocket.py` & `fugle-trade-0.5.1/fugle_trade/websocket.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 handle websocket connection and callback registration
 """
 
 import json
 from websocket import WebSocketApp
 from fugle_trade_core.fugle_trade_core import convert_ws_object
 
+
 class WebsocketHandler():
     """Handle Websocket connection"""
     def __init__(self):
         self.__ws = None
-        default_fun = lambda x: print("in default function")
+        default_fun = lambda x, *y: print("in default function")
         self.on_order = default_fun
         self.on_dealt = default_fun
         self.on_error = default_fun
         self.on_close = default_fun
 
     def ws_on_message(self, _, in_message):
         """callback function for websocket message, pipe to order or dealt
@@ -29,28 +30,28 @@
         except:
             pass
 
     def ws_on_error(self, _, error):
         """callback function for websocket error"""
         self.on_error(error)
 
-    def ws_on_close(self, _, error):
+    def ws_on_close(self, ws, close_status_code, close_msg):
         """callback function for websocket close"""
-        self.on_close(error)
+        self.on_close(ws, close_status_code, close_msg)
 
     def set_callback(self, name, func):
         """for upper scope to set different types of callback function"""
         allowed_callback = ['order', 'dealt', 'error', 'close']
         if name in allowed_callback:
             setattr(self, "on_" + name, func)
         else:
             raise Exception("callback " + name + " not allowed")
 
-    def connect_websocket(self, urlEntry):
+    def connect_websocket(self, url_entry):
         """start to connect websocket"""
         self.__ws = WebSocketApp(
-            urlEntry,
+            url_entry,
             on_message=self.ws_on_message,
             on_error=self.ws_on_error,
             on_close=self.ws_on_close
         )
         self.__ws.run_forever()
```

### Comparing `fugle-trade-0.5.0/pyproject.toml` & `fugle-trade-0.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fugle-trade"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Fortuna Intelligence Co., Ltd. <development@fugle.tw>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fugle-dev/fugle-trade-python#readme"
 repository = "https://github.com/fugle-dev/fugle-trade-python"
 documentation = "https://developer.fugle.tw/docs/trading/intro"
```

### Comparing `fugle-trade-0.5.0/setup.py` & `fugle-trade-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['fugle-trade-core==0.5.0',
  'keyring==23.5.0',
  'keyrings.cryptfile==1.3.8',
  'websocket-client==1.2.1']
 
 setup_kwargs = {
     'name': 'fugle-trade',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': '',
     'long_description': '# Fugle Trade Python SDK\n\n## 事前準備\n\n可以參考 https://developer.fugle.tw/docs/trading/prerequisites 完成申請金鑰相關步驟\n\n## QuickStart\n\n```python\nfrom configparser import ConfigParser\nfrom fugle_trade.sdk import SDK\nfrom fugle_trade.order import OrderObject\nfrom fugle_trade.constant import (APCode, Trade, PriceFlag, BSFlag, Action)\n\nconfig = ConfigParser()\nconfig.read(\'./config.ini\')\nsdk = SDK(config)\nsdk.login()\n\norder = OrderObject(\n    buy_sell = Action.Buy,\n    price = 28.00,\n    stock_no = "2884",\n    quantity = 2,\n    ap_code = APCode.Common\n)\nsdk.place_order(order)\n\n```\n\n## Detail\n\n所有 function 跟 response 可以在專屬文件頁查到相關資訊\n\nhttps://developer.fugle.tw/docs/trading/reference/python\n\n\n## License\n\n[MIT](LICENSE)\n',
     'author': 'Fortuna Intelligence Co., Ltd.',
     'author_email': 'development@fugle.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fugle-dev/fugle-trade-python#readme',
```

### Comparing `fugle-trade-0.5.0/PKG-INFO` & `fugle-trade-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugle-trade
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Home-page: https://github.com/fugle-dev/fugle-trade-python#readme
 License: MIT
 Keywords: fugle,trade,stock
 Author: Fortuna Intelligence Co., Ltd.
 Author-email: development@fugle.tw
 Requires-Python: >=3.7,<4.0
```

