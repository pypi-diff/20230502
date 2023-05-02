# Comparing `tmp/finlogic-0.3.9.tar.gz` & `tmp/finlogic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.3.9.tar", last modified: Mon Apr 24 16:26:03 2023, max compression
+gzip compressed data, was "finlogic-0.4.0.tar", last modified: Tue May  2 00:32:29 2023, max compression
```

## Comparing `finlogic-0.3.9.tar` & `finlogic-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.3.9/LICENSE
--rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 finlogic-0.3.9/README.md
--rw-r--r--   0        0        0      423 2023-04-24 16:25:02.799288 finlogic-0.3.9/finlogic/__init__.py
--rw-r--r--   0        0        0    22892 2023-04-24 07:38:21.875678 finlogic-0.3.9/finlogic/company.py
--rw-r--r--   0        0        0     1024 2023-04-22 03:12:14.634867 finlogic-0.3.9/finlogic/config.py
--rw-r--r--   0        0        0     9283 2023-04-22 03:12:14.634867 finlogic-0.3.9/finlogic/cvm.py
--rw-r--r--   0        0        0     6806 2023-04-22 03:12:14.634867 finlogic-0.3.9/finlogic/database.py
--rw-r--r--   0        0        0      989 2023-04-24 16:26:03.864074 finlogic-0.3.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.3.9/tests/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 finlogic-0.3.9/tests/test_company.py
--rw-r--r--   0        0        0      598 2023-04-22 03:12:14.635867 finlogic-0.3.9/tests/test_database.py
--rw-r--r--   0        0        0    12080 1970-01-01 00:00:00.000000 finlogic-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 finlogic-0.4.0/README.md
+-rw-r--r--   0        0        0      423 2023-05-02 00:27:32.784880 finlogic-0.4.0/finlogic/__init__.py
+-rw-r--r--   0        0        0    23308 2023-05-02 00:27:32.784880 finlogic-0.4.0/finlogic/company.py
+-rw-r--r--   0        0        0      655 2023-05-02 00:27:32.785880 finlogic-0.4.0/finlogic/config.py
+-rw-r--r--   0        0        0     8076 2023-05-02 00:27:32.785880 finlogic-0.4.0/finlogic/cvm.py
+-rw-r--r--   0        0        0     7767 2023-05-02 00:27:32.785880 finlogic-0.4.0/finlogic/database.py
+-rw-r--r--   0        0        0     1010 2023-05-02 00:32:29.087499 finlogic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3396 2023-04-25 23:39:05.128133 finlogic-0.4.0/tests/test_company.py
+-rw-r--r--   0        0        0      887 2023-04-25 23:39:05.128133 finlogic-0.4.0/tests/test_database.py
+-rw-r--r--   0        0        0    12109 1970-01-01 00:00:00.000000 finlogic-0.4.0/PKG-INFO
```

### Comparing `finlogic-0.3.9/LICENSE` & `finlogic-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.9/README.md` & `finlogic-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `finlogic-0.3.9/finlogic/company.py` & `finlogic-0.4.0/finlogic/company.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,28 @@
 Classes:
     Company: Represents a company with its financial information and allows
     users to generate financial reports and indicators.
 
 Abreviations used in code:
     dfi = input dataframe
     dfo = output dataframe
+
+RuntimeWarning:
+    Pandas query + numexpr module -> Engine has switched to 'python' because
+    numexpr does not support extension array dtypes (category not supported
+    yet). Please set your engine to python manually. That means that the query
+    method has to use engine='python' to work with category dtype. N.B. Only
+    FinLogic Dataframe uses category dtype for efficiency.
+
 """
 from typing import Literal
 import numpy as np
 import pandas as pd
-from . import config as c
+from . import config as cf
+from .database import con
 
 
 class Company:
     """A class to represent a company financial data.
 
     This class provides methods to create financial reports and to calculate
     financial indicators based on a company's accounting data. The class also
@@ -73,27 +82,27 @@
             KeyError: If the given identifier isn't found in Finlogic Database.
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
-        df = (
-            c.finlogic_df[["co_id", "co_fiscal_id"]]
-            .drop_duplicates()
-            .astype({"co_id": int, "co_fiscal_id": str})
-        )
-        if identifier in df["co_id"].values:
+        query = """
+            SELECT DISTINCT co_id, co_fiscal_id
+            FROM reports
+        """
+        df = con.execute(query).df()
+        if identifier in df["co_id"].to_list():
             self._co_id = identifier
-            self._co_fiscal_id = df.loc[
-                df["co_id"] == identifier, "co_fiscal_id"
-            ].item()
-        elif identifier in df["co_fiscal_id"].values:
+            mask = df["co_id"] == identifier
+            self._co_fiscal_id = df.loc[mask, "co_fiscal_id"].item()
+        elif identifier in df["co_fiscal_id"].to_list():
             self._co_fiscal_id = identifier
-            self._co_id = df.loc[df["co_fiscal_id"] == identifier, "co_id"].item()
+            mask = df["co_fiscal_id"] == identifier
+            self._co_id = df.loc[mask, "co_id"].item()
         else:
             raise KeyError("Company 'identifier' not found in FinLogic Database")
         self._identifier = identifier
         # If object was already initialized, reset company dataframe
         if self._initialized:
             self._set_co_df()
 
@@ -111,15 +120,16 @@
             ValueError: If the accounting method is invalid.
         """
         return self._acc_unit
 
     @acc_method.setter
     def acc_method(self, value: Literal["consolidated", "separate"]):
         if value in {"consolidated", "separate"}:
-            self._acc_method = value
+            # Set accounting method to upper case as in FinLogic Database
+            self._acc_method = value.upper()
         else:
             raise ValueError("acc_method expects 'consolidated' or 'separate'")
         # If object was already initialized, reset company dataframe
         if self._initialized:
             self._set_co_df()
 
     @property
@@ -228,58 +238,57 @@
 
     def _set_co_df(self) -> pd.DataFrame:
         """Sets the company data frame.
 
         This method creates a data frame with the company's financial
         statements.
         """
-        # Create custom data frame for company selection
-        expr = "co_id == @self._co_id and acc_method == @self._acc_method"
-        co_df = (
-            c.finlogic_df.query(expr)
-            .astype(
-                {
-                    "co_name": str,
-                    "co_id": "UInt32",
-                    "co_fiscal_id": str,
-                    "report_type": str,
-                    "report_version": "UInt8",
-                    "period_reference": "datetime64[ns]",
-                    "period_begin": "datetime64[ns]",
-                    "period_end": "datetime64[ns]",
-                    "period_order": str,
-                    "acc_code": str,
-                    "acc_name": str,
-                    "acc_method": str,
-                    "acc_fixed": bool,
-                    "acc_value": float,
-                    "equity_statement_column": str,
-                }
-            )
-            .sort_values(by="acc_code", ignore_index=True)
-        )
+        # Create the company data frame
+        query = f"""
+            SELECT *
+            FROM reports
+            WHERE co_id = {self._co_id}
+            AND acc_method = '{self._acc_method}'            
+        """
+        co_df = con.execute(query).df().sort_values(by="acc_code", ignore_index=True)
 
         # Change acc_unit only for accounts different from 3.99
         co_df["acc_value"] = np.where(
             co_df["acc_code"].str.startswith("3.99"),
             co_df["acc_value"],
             co_df["acc_value"] / self._acc_unit,
         )
 
         self._name = co_df["co_name"].iloc[0]
-        expr = 'report_type == "annual"'
+        expr = 'report_type == "ANNUAL"'
         self._first_annual = co_df.query(expr)["period_end"].min()
         self._last_annual = co_df.query(expr)["period_end"].max()
-        expr = 'report_type == "quarterly"'
+        expr = 'report_type == "QUARTERLY"'
         self._last_quarterly = co_df.query(expr)["period_end"].max()
 
         # Drop columns that are already company properties
         co_df.drop(
             columns=["co_name", "co_id", "co_fiscal_id", "acc_method"], inplace=True
         )
+
+        # Keep only the newest 'report_version' in df
+        cols = [
+            "report_type",
+            "report_version",
+            "period_reference",
+            "period_order",
+            "acc_code",
+        ]
+        co_df.sort_values(by=cols, ignore_index=True, inplace=True)
+        cols = co_df.columns.tolist()
+        cols_remove = ["report_version", "acc_value", "acc_fixed"]
+        [cols.remove(col) for col in cols_remove]
+        # Ascending order --> last is the newest report_version
+        co_df.drop_duplicates(cols, keep="last", inplace=True, ignore_index=True)
+
         # Set company data frame
         self._co_df = co_df
 
     def info(self) -> dict:
         """Return a dictionay with company info."""
         company_info = {
             "Name": self._name,
@@ -294,23 +303,23 @@
             "Last Quarterly Report": self._last_quarterly.strftime("%Y-%m-%d"),
         }
         return company_info
 
     def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
         # keep only last quarterly fs
         if self._last_annual > self._last_quarterly:
-            df = dfi.query('report_type == "annual"').copy()
+            df = dfi.query('report_type == "ANNUAL"').copy()
             df.query(
                 "period_order == 'PREVIOUS' or \
                  period_end == @self._last_annual",
                 inplace=True,
             )
         else:
             df = dfi.query(
-                'report_type == "annual" or \
+                'report_type == "ANNUAL" or \
                  period_end == @self._last_quarterly'
             ).copy()
             df.query(
                 "period_order == 'PREVIOUS' or \
                  period_end == @self._last_quarterly or \
                  period_end == @self._last_annual",
                 inplace=True,
@@ -377,15 +386,15 @@
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
 
         if self._language == "English":
-            _pten_dict = dict(c.language_df.values)
+            _pten_dict = dict(cf.language_df.values)
             _pten_dict = MyDict(_pten_dict)
             df["acc_name"] = df["acc_name"].map(_pten_dict)
 
         # Filter dataframe for selected acc_level
         if acc_level:
             acc_code_limit = acc_level * 3 - 2  # noqa
             df.query("acc_code.str.len() <= @acc_code_limit", inplace=True)
@@ -444,15 +453,15 @@
             cols = report_df.columns.to_list()
             cols = cols[0:2] + cols[-num_years:]
             report_df = report_df[cols]
         return report_df
 
     def _calculate_ttm(self, dfi: pd.DataFrame) -> pd.DataFrame:
         if self._last_annual > self._last_quarterly:
-            return dfi.query('report_type == "annual"').copy()
+            return dfi.query('report_type == "ANNUAL"').copy()
 
         df1 = dfi.query("period_end == @self._last_quarterly").copy()
         df1.query("period_begin == period_begin.min()", inplace=True)
 
         df2 = dfi.query("period_reference == @self._last_quarterly").copy()
         df2.query("period_begin == period_begin.min()", inplace=True)
         df2["acc_value"] = -df2["acc_value"]
@@ -463,18 +472,18 @@
             pd.concat([df1, df2, df3], ignore_index=True)[["acc_code", "acc_value"]]
             .groupby(by="acc_code")
             .sum()
             .reset_index()
         )
         df1.drop(columns="acc_value", inplace=True)
         df_ttm = pd.merge(df1, df_ttm)
-        df_ttm["report_type"] = "quarterly"
+        df_ttm["report_type"] = "QUARTERLY"
         df_ttm["period_begin"] = self._last_quarterly - pd.DateOffset(years=1)
 
-        df_annual = dfi.query('report_type == "annual"').copy()
+        df_annual = dfi.query('report_type == "ANNUAL"').copy()
 
         return pd.concat([df_annual, df_ttm], ignore_index=True)
 
     def custom_report(
         self,
         acc_list: list[str],
         num_years: int = 0,
```

### Comparing `finlogic-0.3.9/finlogic/cvm.py` & `finlogic-0.4.0/finlogic/cvm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,30 @@
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from typing import List
 import zipfile as zf
 from pathlib import Path
 import pandas as pd
 import requests
 from . import config as cf
 
 URL_DFP = "http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/"
 URL_ITR = "http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/"
 
+CVM_DF_PATH = cf.DATA_PATH / "cvm_df.pkl"
+
+
+def get_cvm_df() -> pd.DataFrame:
+    """Get CVM files metadata."""
+    if CVM_DF_PATH.is_file():
+        cvm_df = pd.read_pickle(CVM_DF_PATH)
+    else:
+        columns = ["filename", "file_size", "etag", "last_modified"]
+        cvm_df = pd.DataFrame(columns=columns)
+    return cvm_df
+
 
 def list_urls() -> List[str]:
     """Update the CVM Portal file base.
     Urls with CVM raw files:
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/
     http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/
     Links example:
@@ -36,140 +48,133 @@
         if year >= first_year_itr:
             filename = f"itr_cia_aberta_{year}.zip"
             url = f"{URL_ITR}{filename}"
             urls.append(url)
     return urls
 
 
-def update_remote_file(url: str) -> Path:
+def update_cvm_file(url: str) -> Path:
     """Update raw file from CVM portal. Return a Path if file is updated."""
-    raw_path = Path(cf.RAW_DIR, url[-23:])  # filename = url final
+    cvm_filepath = Path(cf.CVM_DIR, url[-23:])  # filename = url final
     with requests.Session() as s:
         r = s.get(url, stream=True)
         if r.status_code != requests.codes.ok:
             return None
 
-    if Path.exists(raw_path):
-        local_file_size = raw_path.stat().st_size
+    if Path.exists(cvm_filepath):
+        local_file_size = cvm_filepath.stat().st_size
     else:
         local_file_size = 0
     url_file_size = int(r.headers["Content-Length"])
     if local_file_size == url_file_size:
         # File is already updated
         return None
-    with raw_path.open(mode="wb") as f:
+    with cvm_filepath.open(mode="wb") as f:
         f.write(r.content)
 
     # headers["Last-Modified"] -> 'Wed, 23 Jun 2021 12:19:24 GMT'
     ts_server = pd.to_datetime(
         r.headers["Last-Modified"], format="%a, %d %b %Y %H:%M:%S %Z"
     )
-    # Store URL files metadata
-    cf.cvm_df.loc[pd.Timestamp.now()] = [
-        raw_path.name,
+    # Store URL files metadata in a DataFrame
+    cvm_df = get_cvm_df()
+    cvm_df.loc[pd.Timestamp.now()] = [
+        cvm_filepath.name,
         r.headers["Content-Length"],
         r.headers["ETag"],
         ts_server,
     ]
-    print(f"    {cf.CHECKMARK} {raw_path.name} downloaded.")
-    return raw_path
+    cvm_df.to_pickle(CVM_DF_PATH)
+    return cvm_filepath.name
 
 
-def update_remote_files(urls: str) -> List[Path]:
+def update_cvm_files(urls: str) -> List[Path]:
     """Update local CVM raw files asynchronously."""
     with ThreadPoolExecutor() as executor:
-        results = executor.map(update_remote_file, urls)
-    cf.cvm_df.to_pickle(cf.CVM_DF_PATH)
-    updated_raw_paths = [r for r in results if r is not None]
-    return updated_raw_paths
+        results = executor.map(update_cvm_file, urls)
+    updated_filenames = [r for r in results if r is not None]
+    return updated_filenames
 
 
-def process_annual_df(raw_path: Path) -> Path:
+def read_cvm_file(cvm_filename: str) -> pd.DataFrame:
     """Read annual file, process it, save the result and return the file path."""
     df = pd.DataFrame()
-    annual_zipfile = zf.ZipFile(raw_path)
+    cvm_filepath = Path(cf.CVM_DIR, cvm_filename)
+    annual_zipfile = zf.ZipFile(cvm_filepath)
     child_filenames = annual_zipfile.namelist()
 
     df_list = []
     for child_filename in child_filenames[1:]:
-        # print(f"    {child_filename}")
         child_file = annual_zipfile.open(child_filename)
 
         # Only "DT_INI_EXERC" and "COLUNA_DF" have missing values.
         child_df = pd.read_csv(
             child_file,
             sep=";",
             encoding="iso-8859-1",
             true_values=["S"],
             false_values=["N"],
         )
         # Currency column has only one value (BRL) so it is not necessary.
         child_df = child_df.drop(columns=["MOEDA"])
 
-        # There are two types of CVM files: DFP (annual) and ITR (quarterly).
-        if raw_path.name.startswith("dfp"):
-            child_df["report_type"] = "annual"
+        # There are two types of CVM files: DFP (ANNUAL) and ITR (QUARTERLY).
+        if cvm_filepath.name.startswith("dfp"):
+            child_df["TIPO"] = "ANNUAL"
         else:
-            child_df["report_type"] = "quarterly"
+            child_df["TIPO"] = "QUARTERLY"
 
         df_list.append(child_df)
 
     df = pd.concat(df_list, ignore_index=True)
-
+    df["ARQUIVO"] = cvm_filepath.name
     # Convert string columns to categorical.
     columns = df.select_dtypes(include="object").columns
     df[columns] = df[columns].astype("category")
     return df
 
 
-def format_annual_df(df: pd.DataFrame) -> pd.DataFrame:
-    """Process a raw dataframe and return a formatted dataframe."""
+def format_cvm_df(df: pd.DataFrame) -> pd.DataFrame:
+    """Format a cvm dataframe."""
     columns_translation = {
-        "CNPJ_CIA": "co_fiscal_id",
-        "DT_REFER": "period_reference",
-        "VERSAO": "report_version",
         "DENOM_CIA": "co_name",
         "CD_CVM": "co_id",
-        "GRUPO_DFP": "report_group",
-        "ESCALA_MOEDA": "currency_unit",
-        "ORDEM_EXERC": "period_order",
+        "CNPJ_CIA": "co_fiscal_id",
+        "TIPO": "report_type",
+        "VERSAO": "report_version",
+        "DT_REFER": "period_reference",
+        "DT_INI_EXERC": "period_begin",
         "DT_FIM_EXERC": "period_end",
+        "ORDEM_EXERC": "period_order",
         "CD_CONTA": "acc_code",
         "DS_CONTA": "acc_name",
-        "VL_CONTA": "acc_value",
         "ST_CONTA_FIXA": "acc_fixed",
-        "DT_INI_EXERC": "period_begin",
+        "VL_CONTA": "acc_value",
         "COLUNA_DF": "equity_statement_column",
+        "ARQUIVO": "data_source",
+        # Columns below will be dropped after processing.
+        "GRUPO_DFP": "report_group",
+        "ESCALA_MOEDA": "currency_unit",
     }
-    df.rename(columns=columns_translation, inplace=True)
+    df = df.rename(columns=columns_translation)[columns_translation.values()]
 
-    adjust_data_types = {
-        "co_id": "UInt32",  # max. value = 600_000
-        "report_version": "UInt8",  # values are 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
-        "period_begin": "datetime64[ns]",
-        "period_end": "datetime64[ns]",
-        "period_reference": "datetime64[ns]",
-    }
-    df = df.astype(adjust_data_types)
     # currency_unit values are ['MIL', 'UNIDADE']
-    df["currency_unit"] = (
-        df["currency_unit"].map({"UNIDADE": 1, "MIL": 1000}).astype(int)
-    )
+    map_dict = {"UNIDADE": 1, "MIL": 1000}
+    df["currency_unit"] = df["currency_unit"].map(map_dict).astype(int)
 
     # Do not ajust acc_value for 3.99 codes.
     df["acc_value"] = df["acc_value"].where(
         df["acc_code"].str.startswith("3.99"),
         df["acc_value"] * df["currency_unit"],
     )
     df.drop(columns=["currency_unit"], inplace=True)
 
     # "period_order" values are: 'ÚLTIMO', 'PENÚLTIMO'
-    df["period_order"] = df["period_order"].map(
-        {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
-    )
+    map_dict = {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
+    df["period_order"] = df["period_order"].map(map_dict)
     """
     acc_method -> Financial Statemen Type
     Consolidated and Separate Financial Statements (IAS 27/2003)
     df['GRUPO_DFP'].unique() result:
         'DF Consolidado - Balanço Patrimonial Ativo',
         'DF Consolidado - Balanço Patrimonial Passivo',
         'DF Consolidado - Demonstração das Mutações do Patrimônio Líquido',
@@ -184,69 +189,26 @@
         'DF Individual - Demonstração de Valor Adicionado',
         'DF Individual - Demonstração do Fluxo de Caixa (Método Indireto)',
         'DF Individual - Demonstração do Resultado',
     Hence, with string position 3:6 we can make:
     if == 'Con' -> consolidated statement
     if == 'Ind' -> separate statement
     """
-    df["acc_method"] = (
-        df["report_group"].str[3:6].map({"Con": "consolidated", "Ind": "separate"})
-    )
+    map_dict = {"Con": "CONSOLIDATED", "Ind": "SEPARATE"}
+    df.insert(9, "acc_method", df["report_group"].str[3:6].map(map_dict))
     # 'GRUPO_DFP' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
     # Correct/harmonize some account texts.
     df["acc_name"].replace(to_replace=["\xa0ON\xa0", "On"], value="ON", inplace=True)
-    # Remove duplicated accounts
-    cols = list(df.columns)
-    # cols.remove("acc_value")
-    df.drop_duplicates(cols, keep="last", inplace=True)
-    columns_order = [
-        "co_name",
-        "co_id",
-        "co_fiscal_id",
-        "report_type",
-        "report_version",
-        "period_reference",
-        "period_begin",
-        "period_end",
-        "period_order",
-        "acc_code",
-        "acc_name",
-        "acc_method",
-        "acc_fixed",
-        "acc_value",
-        "equity_statement_column",
-    ]
-    df = df[columns_order]
-    # Most values in datetime and string columns are the same.
-    # So these remaining columns can be converted to category.
-    columns = df.select_dtypes(include=["datetime64[ns]", "object"]).columns
-    df[columns] = df[columns].astype("category")
+    # From 20_636_037 rows 2_383 were duplicated on 2023-04-30 -> remove duplicates
+    cols = df.columns.tolist()
+    cols.remove("acc_value")
+    df.drop_duplicates(subset=cols, keep="last", inplace=True)
 
     return df
 
 
-def process_annual_file(raw_path: Path) -> Path:
-    """Process the annual file and return the path to the processed file."""
-    df = process_annual_df(raw_path)
-    df = format_annual_df(df)
-    processed_filepath = cf.PROCESSED_DIR / raw_path.with_suffix(".pkl.zst").name
-    df.to_pickle(processed_filepath)
-    print(f"    {cf.CHECKMARK} {raw_path.name} processed.")
-    return processed_filepath
-
-
-def process_annual_files(
-    workers: int, raw_paths: List[Path], asynchronous: bool
-) -> List[Path]:
-    """
-    Execute function 'process_raw_file' and return
-    a list with filenames for the processed files.
-    """
-    if asynchronous:
-        with ProcessPoolExecutor(max_workers=workers) as executor:
-            results = executor.map(process_annual_file, raw_paths)
-        processed_paths = [r for r in results]
-    else:
-        processed_paths = [process_annual_file(raw_path) for raw_path in raw_paths]
-
-    return processed_paths
+def process_cvm_file(cvm_filename: str) -> pd.DataFrame:
+    """Read and format a CVM file."""
+    df = read_cvm_file(cvm_filename)
+    df = format_cvm_df(df)
+    return df
```

### Comparing `finlogic-0.3.9/pyproject.toml` & `finlogic-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "zstandard>=0.17.0",
+    "duckdb>=0.7.0",
 ]
-version = "0.3.9"
+version = "0.4.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `finlogic-0.3.9/PKG-INFO` & `finlogic-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.3.9
+Version: 0.4.0
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -31,14 +31,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic
 Requires-Python: >=3.10
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: zstandard>=0.17.0
+Requires-Dist: duckdb>=0.7.0
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finlogic Version: 0.3.9 Summary: Finance toolkit
+Metadata-Version: 2.1 Name: finlogic Version: 0.4.0 Summary: Finance toolkit
 for listed Brazilian companies Keywords: pandas, cvm, finance, investment,
 accounting Author-Email: Carlos Carvalho
 cj@outlook.com> License: MIT License Copyright (c) 2022 Carlos Carvalho
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -17,26 +17,27 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Classifier: Topic :: Office/Business :: Financial ::
 Accounting Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic Requires-Python:
 >=3.10 Requires-Dist: pandas>=1.4.0 Requires-Dist: requests>=2.27.0 Requires-
-Dist: zstandard>=0.17.0 Requires-Dist: pytest>=7.0.0; extra == "test" Provides-
-Extra: test Description-Content-Type: text/markdown [![PyPI version](https://
-img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic) [!
-[Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/
-version.svg)](https://anaconda.org/conda-forge/finlogic) [![PyPI Downloads]
-(https://img.shields.io/pypi/dm/finlogic.svg)](https://pypi.python.org/pypi/
-finlogic) [![Python Version](https://img.shields.io/pypi/pyversions/finlogic)]
-(https://www.python.org/) [![Anaconda License](https://anaconda.org/conda-
-forge/finlogic/badges/license.svg)](https://anaconda.org/conda-forge/finlogic)
-[![Code Style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black) ## FinLogic: finance data analysis
-toolkit for listed Brazilian companies
+Dist: zstandard>=0.17.0 Requires-Dist: duckdb>=0.7.0 Requires-Dist:
+pytest>=7.0.0; extra == "test" Provides-Extra: test Description-Content-Type:
+text/markdown [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)]
+(https://pypi.python.org/pypi/finlogic) [![Anaconda-Server Badge](https://
+anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/
+conda-forge/finlogic) [![PyPI Downloads](https://img.shields.io/pypi/dm/
+finlogic.svg)](https://pypi.python.org/pypi/finlogic) [![Python Version](https:
+//img.shields.io/pypi/pyversions/finlogic)](https://www.python.org/) [!
+[Anaconda License](https://anaconda.org/conda-forge/finlogic/badges/
+license.svg)](https://anaconda.org/conda-forge/finlogic) [![Code Style: black]
+(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+github.com/psf/black) ## FinLogic: finance data analysis toolkit for listed
+Brazilian companies
  ____________________________________________________________________________
 |#### \*\*\* IMPORTANT LEGAL DISCLAIMER \*\*\* --- **FinLogic** is **not**   |
 |affiliated, endorsed or vetted by the Securities and Exchange Commission of |
 |Brazil (CVM). It's an open-source tool that uses CVM publicly available data|
 |and is intended for research and educational purposes. This finance tool is |
 |distributed under the **MIT License** (see the [LICENSE](./LICENSE) file in |
 |the_release_for_details)._---_______________________________________________|
```

