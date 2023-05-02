# Comparing `tmp/coinmetrics_api_client-2023.4.7.13.tar.gz` & `tmp/coinmetrics_api_client-2023.5.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinmetrics_api_client-2023.4.7.13.tar", max compression
+gzip compressed data, was "coinmetrics_api_client-2023.5.2.20.tar", max compression
```

## Comparing `coinmetrics_api_client-2023.4.7.13.tar` & `coinmetrics_api_client-2023.5.2.20.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     1088 2023-03-13 17:44:25.880253 coinmetrics_api_client-2023.4.7.13/LICENSE
--rw-r--r--   0        0        0    20460 2023-03-13 17:44:25.880253 coinmetrics_api_client-2023.4.7.13/README.md
--rw-r--r--   0        0        0       28 2023-04-07 13:55:31.202856 coinmetrics_api_client-2023.4.7.13/coinmetrics/__init__.py
--rw-r--r--   0        0        0    19494 2023-03-13 17:44:25.880253 coinmetrics_api_client-2023.4.7.13/coinmetrics/_catalogs.py
--rw-r--r--   0        0        0     8811 2023-04-07 13:55:31.202856 coinmetrics_api_client-2023.4.7.13/coinmetrics/_data_collection.py
--rw-r--r--   0        0        0     2328 2023-03-13 17:44:25.884253 coinmetrics_api_client-2023.4.7.13/coinmetrics/_exceptions.py
--rw-r--r--   0        0        0      699 2023-03-13 17:44:25.884253 coinmetrics_api_client-2023.4.7.13/coinmetrics/_typing.py
--rw-r--r--   0        0        0     3951 2023-03-13 17:44:25.884253 coinmetrics_api_client-2023.4.7.13/coinmetrics/_utils.py
--rw-r--r--   0        0        0   219839 2023-04-07 13:55:31.202856 coinmetrics_api_client-2023.4.7.13/coinmetrics/api_client.py
--rw-r--r--   0        0        0        0 2023-04-07 13:55:31.234856 coinmetrics_api_client-2023.4.7.13/coinmetrics/build.py
--rw-r--r--   0        0        0      148 2023-03-13 17:44:25.884253 coinmetrics_api_client-2023.4.7.13/coinmetrics/constants.py
--rw-r--r--   0        0        0    20520 2023-03-15 18:43:04.977129 coinmetrics_api_client-2023.4.7.13/coinmetrics/data_exporter.py
--rw-r--r--   0        0        0     8669 2023-03-13 17:44:25.884253 coinmetrics_api_client-2023.4.7.13/coinmetrics/typer_cli.py
--rw-r--r--   0        0        0     1236 2023-04-07 13:55:31.206856 coinmetrics_api_client-2023.4.7.13/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 13:55:31.246857 coinmetrics_api_client-2023.4.7.13/test/__init__.py
--rw-r--r--   0        0        0     1640 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_asset_pair_candles.csv
--rw-r--r--   0        0        0      412 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_asset_pairs.csv
--rw-r--r--   0        0        0     2097 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_assets_markets.csv
--rw-r--r--   0        0        0      605 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_assets_metrics.csv
--rw-r--r--   0        0        0      436 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_exchange_assets.csv
--rw-r--r--   0        0        0     3595 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_exchanges_markets.csv
--rw-r--r--   0        0        0      822 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_exchanges_metrics.csv
--rw-r--r--   0        0        0      556 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_indexes.csv
--rw-r--r--   0        0        0      223 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_institutions.csv
--rw-r--r--   0        0        0      178 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_market_orderbooks.csv
--rw-r--r--   0        0        0      254 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_market_quotes.csv
--rw-r--r--   0        0        0      297 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_market_trades.csv
--rw-r--r--   0        0        0      579 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_markets.csv
--rw-r--r--   0        0        0     2557 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/data/catalog_metrics.csv
--rw-r--r--   0        0        0    28915 2023-03-13 17:44:25.900253 coinmetrics_api_client-2023.4.7.13/test/test_api_client.py
--rw-r--r--   0        0        0    10311 2023-04-07 13:55:31.206856 coinmetrics_api_client-2023.4.7.13/test/test_api_methods.py
--rw-r--r--   0        0        0     2910 2023-03-15 19:40:48.344687 coinmetrics_api_client-2023.4.7.13/test/test_as_list.py
--rw-r--r--   0        0        0     1788 2023-04-07 13:55:31.206856 coinmetrics_api_client-2023.4.7.13/test/test_blockchain_methods.py
--rw-r--r--   0        0        0     2273 2023-03-13 17:44:25.904253 coinmetrics_api_client-2023.4.7.13/test/test_custom_exceptions.py
--rw-r--r--   0        0        0    13462 2023-03-13 17:44:25.904253 coinmetrics_api_client-2023.4.7.13/test/test_data_exporter.py
--rw-r--r--   0        0        0     1015 2023-03-13 17:44:25.904253 coinmetrics_api_client-2023.4.7.13/test/test_debugging.py
--rw-r--r--   0        0        0    11173 2023-03-13 17:44:25.904253 coinmetrics_api_client-2023.4.7.13/test/test_to_dataframe.py
--rw-r--r--   0        0        0     5783 2023-04-07 13:55:31.206856 coinmetrics_api_client-2023.4.7.13/test/test_websocket_methods.py
--rw-r--r--   0        0        0    21648 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.4.7.13/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/LICENSE
+-rw-r--r--   0        0        0    20460 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/README.md
+-rw-r--r--   0        0        0       28 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/coinmetrics/__init__.py
+-rw-r--r--   0        0        0    21093 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_catalogs.py
+-rw-r--r--   0        0        0     9947 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_data_collection.py
+-rw-r--r--   0        0        0     2328 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_exceptions.py
+-rw-r--r--   0        0        0     1181 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_models.py
+-rw-r--r--   0        0        0      699 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_typing.py
+-rw-r--r--   0        0        0     3951 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_utils.py
+-rw-r--r--   0        0        0   233224 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/coinmetrics/api_client.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:44:04.348483 coinmetrics_api_client-2023.5.2.20/coinmetrics/build.py
+-rw-r--r--   0        0        0      148 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/constants.py
+-rw-r--r--   0        0        0    20520 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/data_exporter.py
+-rw-r--r--   0        0        0     8669 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/typer_cli.py
+-rw-r--r--   0        0        0     1236 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 20:44:04.352483 coinmetrics_api_client-2023.5.2.20/test/__init__.py
+-rw-r--r--   0        0        0     1640 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pair_candles.csv
+-rw-r--r--   0        0        0      412 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pairs.csv
+-rw-r--r--   0        0        0     2097 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_markets.csv
+-rw-r--r--   0        0        0      605 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_metrics.csv
+-rw-r--r--   0        0        0      436 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchange_assets.csv
+-rw-r--r--   0        0        0     3595 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_markets.csv
+-rw-r--r--   0        0        0      822 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_metrics.csv
+-rw-r--r--   0        0        0      556 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_indexes.csv
+-rw-r--r--   0        0        0      223 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_institutions.csv
+-rw-r--r--   0        0        0      178 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_orderbooks.csv
+-rw-r--r--   0        0        0      254 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_quotes.csv
+-rw-r--r--   0        0        0      297 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_trades.csv
+-rw-r--r--   0        0        0      579 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_markets.csv
+-rw-r--r--   0        0        0     2557 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_metrics.csv
+-rw-r--r--   0        0        0    28915 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_api_client.py
+-rw-r--r--   0        0        0    10311 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_api_methods.py
+-rw-r--r--   0        0        0     2910 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_as_list.py
+-rw-r--r--   0        0        0     1788 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_blockchain_methods.py
+-rw-r--r--   0        0        0     2273 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_custom_exceptions.py
+-rw-r--r--   0        0        0    13462 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_data_exporter.py
+-rw-r--r--   0        0        0     1015 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_debugging.py
+-rw-r--r--   0        0        0     2142 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_models.py
+-rw-r--r--   0        0        0     1193 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/test/test_rate_limits.py
+-rw-r--r--   0        0        0    14167 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_to_dataframe.py
+-rw-r--r--   0        0        0     5829 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/test/test_websocket_methods.py
+-rw-r--r--   0        0        0    21648 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.5.2.20/PKG-INFO
```

### Comparing `coinmetrics_api_client-2023.4.7.13/LICENSE` & `coinmetrics_api_client-2023.5.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/README.md` & `coinmetrics_api_client-2023.5.2.20/README.md`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/_catalogs.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_catalogs.py`

 * *Files 9% similar despite different names*

```diff
@@ -139,14 +139,50 @@
         """
         Transforms catalog data in list form into a dataframe
         :return: Catalog Data
         """
         return convert_catalog_dtypes(pd.DataFrame(self))
 
 
+class CatalogAssetChainsData(List[Any]):
+    def to_dataframe(self) -> DataFrameType:
+        """
+        Transforms catalog data in list form into a dataframe
+        :return: Catalog Data
+        """
+        return convert_catalog_dtypes(pd.DataFrame(self))
+
+
+class CatalogMempoolFeeratesData(List[Any]):
+    def to_dataframe(self) -> DataFrameType:
+        """
+        Transforms catalog data in list form into a dataframe
+        :return: Catalog Data
+        """
+        return convert_catalog_dtypes(pd.DataFrame(self))
+
+
+class CatalogMiningPoolTipsData(List[Any]):
+    def to_dataframe(self) -> DataFrameType:
+        """
+        Transforms catalog data in list form into a dataframe
+        :return: Catalog Data
+        """
+        return convert_catalog_dtypes(pd.DataFrame(self))
+
+
+class CatalogTransactionTrackerData(List[Any]):
+    def to_dataframe(self) -> DataFrameType:
+        """
+        Transforms catalog data in list form into a dataframe
+        :return: Catalog Data
+        """
+        return convert_catalog_dtypes(pd.DataFrame(self))
+
+
 class CatalogMarketTradesData(List[Any]):
     def to_dataframe(self) -> DataFrameType:
         """
         Transforms catalog data in list form into a dataframe
         :return: Catalog Data
         """
         return convert_catalog_dtypes(pd.DataFrame(self))
@@ -569,7 +605,25 @@
             .assign(
                 max_time=lambda df: _expand_df(key="max_time", iterable=df.frequencies)
             )
             .reset_index(drop=True)
             .drop(["frequencies"], axis=1)
         )
         return convert_catalog_dtypes(df_catalog_asset_candles)
+
+
+class CatalogMarketContractPrices(List[Any]):
+    def to_dataframe(self) -> DataFrameType:
+        """
+        Transforms catalog data in list form into a dataframe
+        :return: Catalog Data
+        """
+        return convert_catalog_dtypes(pd.DataFrame(self))
+
+
+class CatalogMarketImpliedVolatility(List[Any]):
+    def to_dataframe(self) -> DataFrameType:
+        """
+        Transforms catalog data in list form into a dataframe
+        :return: Catalog Data
+        """
+        return convert_catalog_dtypes(pd.DataFrame(self))
```

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/_data_collection.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_data_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from copy import deepcopy
 from gzip import GzipFile
 from io import BytesIO
 from logging import getLogger
 from time import sleep
-from typing import Any, Dict, Iterable, Iterator, List, Optional, cast
+from typing import Any, Dict, Iterable, Iterator, List, Optional, cast, Type
 from dateutil.parser import isoparse
 
 import requests
 
 from coinmetrics._typing import (
     DataRetrievalFuncType,
     DataReturnType,
     FilePathOrBuffer,
     UrlParamTypes,
     DataFrameType,
 )
 from coinmetrics._utils import get_file_path_or_buffer
-
+from coinmetrics._models import AssetChainsData, CoinMetricsAPIModel, TransactionTrackerData
 try:
     import orjson as json
 except ImportError:
     import json  # type: ignore
 
 
 logger = getLogger("cm_client_data_collection")
@@ -42,14 +42,17 @@
     pass
 
 
 NUMBER_OF_RETRIES = 3
 
 
 class DataCollection:
+
+    API_RETURN_MODEL: Optional[Type[CoinMetricsAPIModel]] = None
+
     def __init__(
         self,
         data_retrieval_function: DataRetrievalFuncType,
         endpoint: str,
         url_params: Dict[str, UrlParamTypes],
         csv_export_supported: bool = True,
     ) -> None:
@@ -128,15 +131,18 @@
         first_data_el = None
         if columns_to_store is None:
             try:
                 first_data_el = next(self)
             except StopIteration:
                 logger.info("no data to export")
                 return
-            columns_to_store = list(first_data_el.keys())
+            if self.API_RETURN_MODEL:
+                columns_to_store = self.API_RETURN_MODEL.get_dataframe_cols()
+            else:
+                columns_to_store = list(first_data_el.keys())
 
         yield (",".join(columns_to_store) + "\n").encode()
 
         if first_data_el is not None:
             yield (
                 ",".join(
                     f'"{first_data_el.get(column)}"' or ""
@@ -165,14 +171,15 @@
 
     def _export_to_file(
         self,
         data_generator: Iterable[bytes],
         path_or_bufstr: FilePathOrBuffer = None,
         compress: bool = False,
     ) -> Optional[str]:
+
         if path_or_bufstr is None:
             path_or_bufstr_obj: FilePathOrBuffer = BytesIO()
         else:
             path_or_bufstr_obj = path_or_bufstr
 
         path_or_bufstr_obj = get_file_path_or_buffer(path_or_bufstr_obj)
         if hasattr(path_or_bufstr_obj, "write"):
@@ -225,14 +232,17 @@
                 f = BytesIO()
                 self.export_to_csv(f)
                 if f.getbuffer().nbytes == 0:
                     logger.warning("Response is empty.")
                     return pd.DataFrame()
                 else:
                     f.seek(0)
+                    # if self.API_RETURN_MODEL:
+                    #     columns = self.API_RETURN_MODEL.get_dataframe_cols()
+                    # else:
                     columns = (
                         BytesIO(f.getvalue())
                         .readlines(1)[0]
                         .decode()
                         .strip()
                         .split(",")
                     )
@@ -254,7 +264,28 @@
                         df.columns = header
                     return df
             else:
                 if dtype_mapper is None:
                     return pd.DataFrame(self)
                 else:
                     return pd.DataFrame(self).astype(dtype=dtype_mapper)
+
+
+class AssetChainsDataCollection(DataCollection):
+
+    API_RETURN_MODEL = AssetChainsData
+
+    def to_dataframe(
+        self,
+        header: Optional[List[str]] = None,
+        dtype_mapper: Optional[Dict[str, Any]] = None,
+        optimize_pandas_types: Optional[bool] = True,
+    ) -> DataFrameType:
+        df = super().to_dataframe(header=header, dtype_mapper=dtype_mapper, optimize_pandas_types=optimize_pandas_types)
+        if 'reorg' in df.columns:
+            df['reorg'] = df['reorg'].apply(lambda reorg: True if reorg == "true" else False)
+        return df
+
+
+class TransactionTrackerDataCollection(DataCollection):
+
+    API_RETURN_MODEL = TransactionTrackerData
```

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/_exceptions.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/_typing.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_typing.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/_utils.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_utils.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/api_client.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import socket
+import time
 from datetime import date, datetime
 from logging import getLogger
 from typing import Any, Dict, List, Optional, Union, cast
 from urllib.parse import urlencode
 
 import requests
 from requests import HTTPError, Response
@@ -20,15 +21,15 @@
     import json  # type: ignore
 
 from coinmetrics._typing import (
     DataReturnType,
     MessageHandlerType,
 )
 from coinmetrics.constants import PagingFrom, Backfill
-from coinmetrics._data_collection import DataCollection
+from coinmetrics._data_collection import DataCollection, AssetChainsDataCollection, TransactionTrackerDataCollection
 from coinmetrics._catalogs import (
     CatalogAssetsData,
     CatalogAssetAlertsData,
     CatalogAssetPairsData,
     CatalogAssetPairCandlesData,
     CatalogExchangeAssetsData,
     CatalogExchangesData,
@@ -39,14 +40,20 @@
     CatalogMarketMetricsData,
     CatalogMarketCandlesData,
     CatalogMarketTradesData,
     CatalogExchangeAssetMetricsData,
     CatalogPairMetricsData,
     CatalogInstitutionMetricsData,
     CatalogMarketOrderbooksData,
+    CatalogAssetChainsData,
+    CatalogMempoolFeeratesData,
+    CatalogMiningPoolTipsData,
+    CatalogTransactionTrackerData,
+    CatalogMarketContractPrices,
+    CatalogMarketImpliedVolatility
 )
 
 logger = getLogger("cm_client")
 
 try:
     import pandas as pd  # type: ignore
 except ImportError:
@@ -183,14 +190,78 @@
             "assets": assets,
             "alerts": alerts,
         }
         return CatalogAssetAlertsData(
             self._get_data("catalog/asset-alerts", params)["data"]
         )
 
+    def catalog_asset_chains(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogAssetChainsData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of asset chains assets
+        :rtype: CatalogAssetChainsData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogAssetChainsData(self._get_data("catalog/asset-chains", params)['data'])
+
+    def catalog_mempool_feerates(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogMempoolFeeratesData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of mempool feerates assets
+        :rtype: CatalogMempoolFeeratesData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogMempoolFeeratesData(self._get_data("catalog/mempool-feerates", params)['data'])
+
+    def catalog_mining_pool_tips_summaries(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogMiningPoolTipsData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of mining pool tips assets
+        :rtype: CatalogMiningPoolTipsData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogMiningPoolTipsData(self._get_data("catalog/mining-pool-tips-summary", params)['data'])
+
+    def catalog_transaction_tracker_assets(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogTransactionTrackerData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of transaction tracker assets
+        :rtype: CatalogTransactionTrackerData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogTransactionTrackerData(self._get_data("catalog/transaction-tracker", params)['data'])
+
     def catalog_asset_pairs(
         self, asset_pairs: Optional[Union[List[str], str]] = None
     ) -> CatalogAssetPairsData:
         """
         Returns meta information about _available_ asset-asset pairs
 
         :param asset_pairs: A single asset-asset pair (e.g. "btc-eth") or a list of asset-asset pairs to return info for. If none are provided, all available pairs are returned.
@@ -722,14 +793,110 @@
             "asset": asset,
             "symbol": symbol,
         }
         return CatalogMarketTradesData(
             self._get_data("catalog/market-funding-rates", params)["data"]
         )
 
+    def catalog_market_contract_prices(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            limit: Optional[str] = None,
+    ) -> CatalogMarketContractPrices:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param type: Type of markets.
+        :type type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param limit: Limit of response items. `none` means no limit.
+        :type limit: Optional[str]
+
+        :return: List of contract prices statistics.
+        :rtype: CatalogMarketContractPrices
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "limit": limit,
+        }
+        return CatalogMarketContractPrices(self._get_data("catalog/market-contract-prices", params)['data'])
+
+    def catalog_market_implied_volatility(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            limit: Optional[str] = None,
+    ) -> CatalogMarketImpliedVolatility:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param type: Type of markets.
+        :type type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param limit: Limit of response items. `none` means no limit.
+        :type limit: Optional[str]
+
+        :return: List of implied volatility statistics.
+        :rtype: CatalogMarketImpliedVolatility
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "limit": limit,
+        }
+        return CatalogMarketImpliedVolatility(self._get_data("catalog/market-implied-volatility", params)['data'])
+
     def catalog_market_greeks(
         self,
         markets: Optional[Union[List[str], str]] = None,
         market_type: Optional[str] = None,
         exchange: Optional[str] = None,
         base: Optional[str] = None,
         quote: Optional[str] = None,
@@ -919,14 +1086,78 @@
             "assets": assets,
             "alerts": alerts,
         }
         return CatalogAssetAlertsData(
             self._get_data("catalog-all/asset-alerts", params)["data"]
         )
 
+    def catalog_full_asset_chains(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogAssetChainsData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of asset chains assets
+        :rtype: CatalogAssetChainsData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogAssetChainsData(self._get_data("catalog-all/asset-chains", params)['data'])
+
+    def catalog_full_mempool_feerates(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogMempoolFeeratesData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of mempool feerates assets
+        :rtype: CatalogMempoolFeeratesData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogMempoolFeeratesData(self._get_data("catalog-all/mempool-feerates", params)['data'])
+
+    def catalog_full_mining_pool_tips_summaries(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogMiningPoolTipsData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of mining pool tips assets
+        :rtype: CatalogMiningPoolTipsData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogMiningPoolTipsData(self._get_data("catalog-all/mining-pool-tips-summary", params)['data'])
+
+    def catalog_full_transaction_tracker_assets(
+            self,
+            assets: Optional[Union[str, List[str]]] = None,
+    ) -> CatalogTransactionTrackerData:
+        """
+        :param assets: Comma separated list of assets. By default all assets are returned.
+        :type assets: Optional[Union[str, List[str]]]
+
+        :return: List of transaction tracker assets
+        :rtype: CatalogTransactionTrackerData
+        """
+        params: Dict[str, Any] = {
+            "assets": assets,
+        }
+        return CatalogTransactionTrackerData(self._get_data("catalog-all/transaction-tracker", params)['data'])
+
     def catalog_full_asset_pairs(
         self,
         asset_pairs: Optional[Union[List[str], str]] = None,
     ) -> CatalogAssetPairsData:
         """
         Returns meta information about _supported_ asset-asset pairs
 
@@ -1444,14 +1675,110 @@
             "asset": asset,
             "symbol": symbol,
         }
         return CatalogMarketTradesData(
             self._get_data("catalog-all/market-funding-rates", params)["data"]
         )
 
+    def catalog_full_market_contract_prices(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            limit: Optional[str] = None,
+    ) -> CatalogMarketContractPrices:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param type: Type of markets.
+        :type type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param limit: Limit of response items. `none` means no limit.
+        :type limit: Optional[str]
+
+        :return: List of contract prices statistics.
+        :rtype: CatalogMarketContractPrices
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "limit": limit,
+        }
+        return CatalogMarketContractPrices(self._get_data("catalog-all/market-contract-prices", params)['data'])
+
+    def catalog_full_market_implied_volatility(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            limit: Optional[str] = None,
+    ) -> CatalogMarketImpliedVolatility:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param type: Type of markets.
+        :type type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param limit: Limit of response items. `none` means no limit.
+        :type limit: Optional[str]
+
+        :return: List of implied volatility statistics.
+        :rtype: CatalogMarketImpliedVolatility
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "limit": limit,
+        }
+        return CatalogMarketImpliedVolatility(self._get_data("catalog-all/market-implied-volatility", params)['data'])
+
     def catalog_full_market_greeks(
         self,
         markets: Optional[Union[List[str], str]] = None,
         market_type: Optional[str] = None,
         exchange: Optional[str] = None,
         base: Optional[str] = None,
         quote: Optional[str] = None,
@@ -1686,15 +2013,15 @@
         page_size: Optional[int] = None,
         paging_from: Optional[Union[PagingFrom, str]] = "start",
         start_time: Optional[Union[datetime, date, str]] = None,
         end_time: Optional[Union[datetime, date, str]] = None,
         start_inclusive: Optional[bool] = None,
         end_inclusive: Optional[bool] = None,
         timezone: Optional[str] = None,
-    ) -> DataCollection:
+    ) -> AssetChainsDataCollection:
         """
         Returns the chains of blocks for the specified assets.
 
         :param assets: list of asset names, e.g. 'btc'
         :type assets: list(str), str
         :param page_size: number of items returned per page when calling the API. If the request times out, try using a smaller number.
         :type page_size: int
@@ -1707,28 +2034,28 @@
         :param start_inclusive: Flag to define if start timestamp must be included in the timeseries if present. True by default.
         :type start_inclusive: bool
         :param end_inclusive: Flag to define if end timestamp must be included in the timeseries if present. True by default.
         :type end_inclusive: bool
         :param timezone: timezone of the start/end times in db format for example: "America/Chicago". Default value is "UTC". For more details check out API documentation page.
         :type timezone: str
         :return: Asset chains timeseries.
-        :rtype: DataCollection
+        :rtype: AssetChainsDataCollection
         """
 
         params: Dict[str, Any] = {
             "assets": assets,
             "page_size": page_size,
             "paging_from": paging_from,
             "start_time": start_time,
             "end_time": end_time,
             "start_inclusive": start_inclusive,
             "end_inclusive": end_inclusive,
             "timezone": timezone,
         }
-        return DataCollection(self._get_data, "timeseries/asset-chains", params)
+        return AssetChainsDataCollection(self._get_data, "timeseries/asset-chains", params)
 
     def get_asset_metrics(
         self,
         assets: Union[List[str], str],
         metrics: Union[List[str], str],
         frequency: Optional[str] = None,
         page_size: Optional[int] = None,
@@ -4068,30 +4395,30 @@
             "start_inclusive": start_inclusive,
             "end_inclusive": end_inclusive,
             "timezone": timezone,
             "page_size": page_size,
             "paging_from": paging_from,
             "next_page_token": next_page_token,
         }
-        return DataCollection(self._get_data, f"/blockchain-v2/{asset}/accounts/{account}/balance-updates", params)
+        return DataCollection(self._get_data, f"blockchain-v2/{asset}/accounts/{account}/balance-updates", params)
 
     def get_transaction_tracker(
         self,
         asset: str,
         txids: Optional[Union[List[str], str]] = None,
         replacements_for_txids: Optional[Union[List[str], str]] = None,
         replacements_only: Optional[bool] = None,
         page_size: Optional[int] = None,
         paging_from: Optional[Union[PagingFrom, str]] = "start",
         start_time: Optional[Union[datetime, date, str]] = None,
         end_time: Optional[Union[datetime, date, str]] = None,
         start_inclusive: Optional[bool] = None,
         end_inclusive: Optional[bool] = None,
         timezone: Optional[str] = None,
-    ) -> DataCollection:
+    ) -> TransactionTrackerDataCollection:
         """
         Returns status updates for the specified or all transactions.
 
         :param asset: Asset name
         :type asset: str
         :param txids: Optional comma separated list of transaction identifiers (txid) to track.
         :type txids: str, list(str)
@@ -4110,30 +4437,30 @@
         :param start_inclusive: Flag to define if start timestamp must be included in the timeseries if present. True by default.
         :type start_inclusive: bool
         :param end_inclusive: Flag to define if end timestamp must be included in the timeseries if present. True by default.
         :type end_inclusive: bool
         :param timezone: timezone of the start/end times in db format for example: "America/Chicago". Default value is "UTC". For more details check out API documentation page.
         :type timezone: str
         :return: status updates for the specified or all transactions.
-        :rtype: DataCollection
+        :rtype: TransactionTrackerDataCollection
         """
         params: Dict[str, Any] = {
             "asset": asset,
             "txids": txids,
             "replacements_for_txids": replacements_for_txids,
             "replacements_only": replacements_only,
             "page_size": page_size,
             "paging_from": paging_from,
             "start_time": start_time,
             "end_time": end_time,
             "start_inclusive": start_inclusive,
             "end_inclusive": end_inclusive,
             "timezone": timezone,
         }
-        return DataCollection(
+        return TransactionTrackerDataCollection(
             self._get_data, f"blockchain/{asset}/transaction-tracker", params
         )
 
     def get_taxonomy_assets(
         self,
         assets: Optional[List[str]] = None,
         class_ids: Optional[List[str]] = None,
@@ -4318,13 +4645,19 @@
         actual_url = "{}/{}?{}{}".format(
             self._ws_api_base_url, url, self._api_key_url_str, params_str
         )
         return CmStream(ws_url=actual_url)
 
     @retry((socket.gaierror, HTTPError), retries=5, wait_time_between_retries=5)
     def _send_request(self, actual_url: str) -> Response:
-        return self._session.get(
+        response = self._session.get(
             actual_url,
             headers=self._session.headers,
             proxies=self._session.proxies,
             verify=self._session.verify,
         )
+        if response.status_code == 429 or response.headers.get("x-ratelimit-remaining", None) == "0":
+            logger.info("Sleeping for a rate limit window because 429 (too many requests) error was returned. Please"
+                        "see Coin Metrics APIV4 documentation for more information: https://docs.coinmetrics.io/api/v4/#tag/Rate-limits")
+            time.sleep(int(response.headers["x-ratelimit-reset"]))
+            response = self._send_request(actual_url=actual_url)
+        return response
```

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/data_exporter.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/coinmetrics/typer_cli.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/typer_cli.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/pyproject.toml` & `coinmetrics_api_client-2023.5.2.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinmetrics-api-client"
-version = "2023.4.7.13"
+version = "2023.5.2.20"
 description = "Python client for Coin Metrics API v4."
 authors = ["Coin Metrics <info@coinmetrics.io>", "Oleksandr Buchkovskyi <oleksandr@coinmetrics.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://coinmetrics.github.io/api-client-python/site/index.html"
 repository = "https://github.com/coinmetrics/api-client-python"
 packages = [{include = "coinmetrics"}]
```

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_asset_pair_candles.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pair_candles.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_assets_markets.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_assets_metrics.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_exchanges_markets.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_exchanges_metrics.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_indexes.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_indexes.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_markets.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/data/catalog_metrics.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_api_client.py` & `coinmetrics_api_client-2023.5.2.20/test/test_api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_api_methods.py` & `coinmetrics_api_client-2023.5.2.20/test/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_as_list.py` & `coinmetrics_api_client-2023.5.2.20/test/test_as_list.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_blockchain_methods.py` & `coinmetrics_api_client-2023.5.2.20/test/test_blockchain_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_custom_exceptions.py` & `coinmetrics_api_client-2023.5.2.20/test/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_data_exporter.py` & `coinmetrics_api_client-2023.5.2.20/test/test_data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_debugging.py` & `coinmetrics_api_client-2023.5.2.20/test/test_debugging.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_to_dataframe.py` & `coinmetrics_api_client-2023.5.2.20/test/test_to_dataframe.py`

 * *Files 23% similar despite different names*

```diff
@@ -303,10 +303,84 @@
     """
     aave_balance_sheets = client.get_defi_balance_sheets(
         defi_protocols="aave_v2_eth"
     ).to_dataframe()
     assert len(aave_balance_sheets) > 100
     assert aave_balance_sheets.iloc[:1]["defi_protocol"][0] == "aave_v2_eth"
 
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_asset_chains() -> None:
+    data = client.catalog_asset_chains().to_dataframe()
+    assert len(data) >= 2
+
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_asset_chains_all() -> None:
+    data = client.catalog_full_asset_chains().to_dataframe()
+    assert len(data) >= 2
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_mempool_feerates() -> None:
+    data = client.catalog_mempool_feerates().to_dataframe()
+    assert len(data) >= 1
+
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_mempool_feerates_full() -> None:
+    data = client.catalog_full_mempool_feerates().to_dataframe()
+    assert len(data) >= 1
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_mining_pool_tips() -> None:
+    data = client.catalog_mining_pool_tips_summaries().to_dataframe()
+    assert len(data) >= 1
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_mining_pool_tips_full() -> None:
+    data = client.catalog_full_mining_pool_tips_summaries().to_dataframe()
+    assert len(data) >= 1
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_transaction_tracker_catalog_full() -> None:
+    data = client.catalog_full_transaction_tracker_assets().to_dataframe()
+    assert len(data) >= 2
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_transaction_tracker_catalog() -> None:
+    data = client.catalog_transaction_tracker_assets().to_dataframe()
+    assert len(data) >= 2
+
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_market_contract_prices_catalog() -> None:
+    data = client.catalog_market_contract_prices(markets='deribit-BTC-11APR22-42000-C-option').to_dataframe()
+    assert len(data) == 1
+    expected_cols = ["market", "min_time", "max_time"]
+    assert all([col in data.columns for col in expected_cols])
+
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_market_contract_prices_catalog_all() -> None:
+    data = client.catalog_full_market_contract_prices(markets='deribit-BTC-11APR22-42000-C-option').to_dataframe()
+    assert len(data) == 1
+    expected_cols = ["market", "min_time", "max_time"]
+    assert all([col in data.columns for col in expected_cols])
+
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_market_implied_vol_catalog() -> None:
+    data = client.catalog_market_implied_volatility().to_dataframe()
+    assert len(data) > 100
+    expected_cols = ["market", "min_time", "max_time"]
+    assert all([col in data.columns for col in expected_cols])
+
+
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_market_implied_vol_catalog_full() -> None:
+    data = client.catalog_full_market_implied_volatility().to_dataframe()
+    assert len(data) > 100
+    expected_cols = ["market", "min_time", "max_time"]
+    assert all([col in data.columns for col in expected_cols])
+
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `coinmetrics_api_client-2023.4.7.13/test/test_websocket_methods.py` & `coinmetrics_api_client-2023.5.2.20/test/test_websocket_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,7 +186,11 @@
     stream.run(on_message=on_message_pair_quotes_test)
 
 
 @pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
 def test_get_asset_quotes_stream() -> None:
     stream = client.get_stream_asset_quotes(assets="btc")
     stream.run(on_message=on_message_assets_quotes_test)
+
+
+if __name__ == '__main__':
+    pytest.main()
```

### Comparing `coinmetrics_api_client-2023.4.7.13/PKG-INFO` & `coinmetrics_api_client-2023.5.2.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinmetrics-api-client
-Version: 2023.4.7.13
+Version: 2023.5.2.20
 Summary: Python client for Coin Metrics API v4.
 Home-page: https://coinmetrics.github.io/api-client-python/site/index.html
 License: MIT
 Keywords: coin metrics,coin,metrics,crypto,bitcoin,network-data,market-data,api,handy
 Author: Coin Metrics
 Author-email: info@coinmetrics.io
 Requires-Python: >=3.7.1,<4.0.0
```

