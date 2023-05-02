# Comparing `tmp/code_genie-0.2.0.tar.gz` & `tmp/code_genie-0.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_genie-0.2.0.tar", last modified: Sat Apr 29 16:20:51 2023, max compression
+gzip compressed data, was "code_genie-0.2.1.dev0.tar", last modified: Tue May  2 05:53:02 2023, max compression
```

## Comparing `code_genie-0.2.0.tar` & `code_genie-0.2.1.dev0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      399 2023-04-29 16:20:39.492222 code_genie-0.2.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1871 2023-04-29 16:20:39.492906 code_genie-0.2.0/.gitignore
--rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0       91 2023-04-25 05:29:52.445152 code_genie-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.2.0/LICENSE
--rw-r--r--   0        0        0     1549 2023-04-29 16:20:39.493569 code_genie-0.2.0/README.md
--rw-r--r--   0        0        0      484 2023-04-29 16:20:39.494222 code_genie-0.2.0/TODO.md
--rw-r--r--   0        0        0      240 2023-04-29 16:20:39.494897 code_genie-0.2.0/code_genie/__init__.py
--rw-r--r--   0        0        0     3041 2023-04-29 16:20:39.495446 code_genie-0.2.0/code_genie/_cache.py
--rw-r--r--   0        0        0     1678 2023-04-29 16:20:39.496137 code_genie-0.2.0/code_genie/client.py
--rw-r--r--   0        0        0       89 2023-04-29 16:20:39.496555 code_genie-0.2.0/code_genie/genie/__init__.py
--rw-r--r--   0        0        0     4705 2023-04-29 16:20:39.497081 code_genie-0.2.0/code_genie/genie/base.py
--rw-r--r--   0        0        0      501 2023-04-29 16:20:39.497458 code_genie-0.2.0/code_genie/genie/genie.py
--rw-r--r--   0        0        0     3407 2023-04-29 16:20:39.497737 code_genie-0.2.0/code_genie/genie/pandas.py
--rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.2.0/docs/Makefile
--rw-r--r--   0        0        0       92 2023-04-27 10:15:39.151209 code_genie-0.2.0/docs/api.rst
--rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.2.0/docs/conf.py
--rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.2.0/docs/examples.rst
--rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.2.0/docs/generated/code_genie.client.rst
--rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.2.0/docs/generated/code_genie.genie.rst
--rw-r--r--   0        0        0      123 2023-04-27 10:15:39.154001 code_genie-0.2.0/docs/genie.rst
--rw-r--r--   0        0        0     1110 2023-04-27 10:15:39.154405 code_genie-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.2.0/docs/make.bat
--rw-r--r--   0        0        0    64853 2023-04-29 16:20:39.498904 code_genie-0.2.0/docs/notebooks/Starter.ipynb
--rw-r--r--   0        0        0     1619 2023-04-29 16:20:39.499378 code_genie-0.2.0/docs/notebooks/_cache_starter/_meta.json
--rw-r--r--   0        0        0      173 2023-04-29 16:20:39.499698 code_genie-0.2.0/docs/notebooks/_cache_starter/count_high_earners_86151.py
--rw-r--r--   0        0        0       90 2023-04-29 16:20:39.499976 code_genie-0.2.0/docs/notebooks/_cache_starter/count_missing_35951.py
--rw-r--r--   0        0        0      466 2023-04-29 16:20:39.500316 code_genie-0.2.0/docs/notebooks/_cache_starter/generate_employee_df_41317.py
--rw-r--r--   0        0        0      247 2023-04-29 16:20:39.500621 code_genie-0.2.0/docs/notebooks/_cache_starter/make_boxplots_25996.py
--rw-r--r--   0        0        0      485 2023-04-29 16:20:39.500926 code_genie-0.2.0/docs/notebooks/_cache_starter/make_salaries_missing_76197.py
--rw-r--r--   0        0        0      419 2023-04-29 16:20:39.501241 code_genie-0.2.0/docs/notebooks/_cache_starter/plot_salary_distribution_54098.py
--rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.2.0/docs/requirements.in
--rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     1212 2023-04-27 10:15:39.157311 code_genie-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1559 2023-04-29 16:20:39.502197 code_genie-0.2.0/tests/test_cache.py
--rw-r--r--   0        0        0      776 2023-04-29 16:20:39.502598 code_genie-0.2.0/tests/test_genie.py
--rw-r--r--   0        0        0      839 2023-04-29 16:20:39.503091 code_genie-0.2.0/tox.ini
--rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 code_genie-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      404 2023-05-02 05:52:48.260158 code_genie-0.2.1.dev0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1871 2023-04-29 16:20:39.492906 code_genie-0.2.1.dev0/.gitignore
+-rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.2.1.dev0/.readthedocs.yaml
+-rw-r--r--   0        0        0      251 2023-05-02 05:52:48.260947 code_genie-0.2.1.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.2.1.dev0/LICENSE
+-rw-r--r--   0        0        0     1554 2023-05-02 05:52:48.261659 code_genie-0.2.1.dev0/README.md
+-rw-r--r--   0        0        0      484 2023-04-30 09:58:38.245553 code_genie-0.2.1.dev0/TODO.md
+-rw-r--r--   0        0        0      245 2023-05-02 05:52:48.262694 code_genie-0.2.1.dev0/code_genie/__init__.py
+-rw-r--r--   0        0        0     3041 2023-04-29 16:20:39.495446 code_genie-0.2.1.dev0/code_genie/_cache.py
+-rw-r--r--   0        0        0     1678 2023-04-29 16:20:39.496137 code_genie-0.2.1.dev0/code_genie/client.py
+-rw-r--r--   0        0        0       89 2023-04-29 16:20:39.496555 code_genie-0.2.1.dev0/code_genie/genie/__init__.py
+-rw-r--r--   0        0        0     4755 2023-05-02 05:52:48.263526 code_genie-0.2.1.dev0/code_genie/genie/base.py
+-rw-r--r--   0        0        0      501 2023-04-29 16:20:39.497458 code_genie-0.2.1.dev0/code_genie/genie/genie.py
+-rw-r--r--   0        0        0     3407 2023-04-29 16:20:39.497737 code_genie-0.2.1.dev0/code_genie/genie/pandas.py
+-rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.2.1.dev0/docs/Makefile
+-rw-r--r--   0        0        0       92 2023-04-27 10:15:39.151209 code_genie-0.2.1.dev0/docs/api.rst
+-rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.2.1.dev0/docs/conf.py
+-rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.2.1.dev0/docs/examples.rst
+-rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.2.1.dev0/docs/generated/code_genie.client.rst
+-rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.2.1.dev0/docs/generated/code_genie.genie.rst
+-rw-r--r--   0        0        0      123 2023-04-27 10:15:39.154001 code_genie-0.2.1.dev0/docs/genie.rst
+-rw-r--r--   0        0        0     1110 2023-04-27 10:15:39.154405 code_genie-0.2.1.dev0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.2.1.dev0/docs/make.bat
+-rw-r--r--   0        0        0    57086 2023-05-02 05:52:48.264496 code_genie-0.2.1.dev0/docs/notebooks/Starter.ipynb
+-rw-r--r--   0        0        0     1695 2023-05-02 05:52:48.265032 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/_meta.json
+-rw-r--r--   0        0        0      232 2023-05-02 05:52:48.265457 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/boxplots_of_salary_by_department_12125.py
+-rw-r--r--   0        0        0      193 2023-05-02 05:52:48.265844 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/count_high_earners_61505.py
+-rw-r--r--   0        0        0       80 2023-05-02 05:52:48.266223 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/count_missing_values_28317.py
+-rw-r--r--   0        0        0      625 2023-05-02 05:52:48.266565 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/generate_employee_data_58297.py
+-rw-r--r--   0        0        0      518 2023-05-02 05:52:48.266983 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/generate_employee_dataframe_96513.py
+-rw-r--r--   0        0        0      318 2023-05-02 05:52:48.267382 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/make_salaries_missing_39233.py
+-rw-r--r--   0        0        0      452 2023-05-02 05:52:48.267772 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/plot_salary_distribution_47385.py
+-rw-r--r--   0        0        0      192 2023-05-02 05:52:48.268126 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/plot_salary_distribution_49433.py
+-rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.2.1.dev0/docs/requirements.in
+-rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.2.1.dev0/docs/requirements.txt
+-rw-r--r--   0        0        0     1212 2023-04-27 10:15:39.157311 code_genie-0.2.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.2.1.dev0/tests/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.2.1.dev0/tests/conftest.py
+-rw-r--r--   0        0        0     1559 2023-04-29 16:20:39.502197 code_genie-0.2.1.dev0/tests/test_cache.py
+-rw-r--r--   0        0        0      776 2023-04-29 16:20:39.502598 code_genie-0.2.1.dev0/tests/test_genie.py
+-rw-r--r--   0        0        0      839 2023-04-29 16:20:39.503091 code_genie-0.2.1.dev0/tox.ini
+-rw-r--r--   0        0        0     3031 1970-01-01 00:00:00.000000 code_genie-0.2.1.dev0/PKG-INFO
```

### Comparing `code_genie-0.2.0/.gitignore` & `code_genie-0.2.1.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/.readthedocs.yaml` & `code_genie-0.2.1.dev0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/LICENSE` & `code_genie-0.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/README.md` & `code_genie-0.2.1.dev0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.2.0
+Latest version: 0.2.1-dev0
 
 ## Documentation
 
 - [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
 - [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
 - [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
```

### Comparing `code_genie-0.2.0/code_genie/_cache.py` & `code_genie-0.2.1.dev0/code_genie/_cache.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/code_genie/client.py` & `code_genie-0.2.1.dev0/code_genie/client.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/code_genie/genie/base.py` & `code_genie-0.2.1.dev0/code_genie/genie/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,24 +41,25 @@
         self._instructions = instructions
         self._allowed_imports = allowed_imports
 
         # check cache
         cache = _CacheManager(cache_dir)
         cache_key = self._get_hash_str()
         cache_value = cache.get(cache_key)
-        self._filename = cache_value.filename if cache_value else self._generate_export_filename()
         if not override:
             if cache_value is not None:
-                print(f"Loading executor from cache file {cache_value.filename}, set override = True to rerun")
                 self._code = cache_value.code
                 self._fn_name = cache_value.fn_name
+                self._filename = cache_value.filename
+                print(f"Loading executor from cache file {cache_value.filename}, set override = True to rerun")
                 self._executor = self._extract_executable(self._code, self._fn_name)
                 return
         # override or cache not found
         self._code, self._fn_name = self._get_code(client=client or Client())
+        self._filename = self._generate_export_filename(self._fn_name)
         self._executor = self._extract_executable(self._code, self._fn_name)
         cache.update(cache_key, _CacheValue(code=self._code, fn_name=self._fn_name, filename=self._filename))
         print(f"Executor saved to cache file {self._filename}")
 
     @abstractmethod
     def _get_code(self, client: Client) -> Tuple[str, str]:
         raise NotImplementedError
@@ -74,17 +75,18 @@
         return self._executor(*args, **kwargs)
 
     @property
     def code(self):
         """The code generated by the genie"""
         return self._code
 
-    def _generate_export_filename(self) -> str:
+    @classmethod
+    def _generate_export_filename(cls, fn_name: str) -> str:
         # use fn name with random 5 digit suffix
-        return f"{self._fn_name}_{random.randint(10000, 99999)}.py"
+        return f"{fn_name}_{random.randint(10000, 99999)}.py"
 
     def _hash_attributes(self) -> List[Any]:
         return [self._instructions, self._inputs, self._allowed_imports]
 
     def _get_hash_str(self) -> str:
         sep = "::"
         hash_str = []
```

### Comparing `code_genie-0.2.0/code_genie/genie/pandas.py` & `code_genie-0.2.1.dev0/code_genie/genie/pandas.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/docs/Makefile` & `code_genie-0.2.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/docs/conf.py` & `code_genie-0.2.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/docs/index.rst` & `code_genie-0.2.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/docs/make.bat` & `code_genie-0.2.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/docs/notebooks/Starter.ipynb` & `code_genie-0.2.1.dev0/docs/notebooks/Starter.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893227026378173%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(1, \'\\n\'), (2, "Don\'t have an access token yet? [Sign '*

 * *            'up for free!](https://www.thismlguy.com/)\\n")]}}, 9: {\'execution_count\': 9, '*

 * *            "'outputs': {0: {'text': ['Executor saved to cache file "*

 * *            "generate_employee_data_58297.py\\n']}}, 'source': {insert: [(5, '                 "*

 * *            "override=True)')], delete: [5]}}, 10: {'execution_count': 10, 'outputs': {0: "*

 * *            "{'execution_count': 10}}}, 11: {'execution_cou […]*

```diff
@@ -24,14 +24,16 @@
         {
             "cell_type": "markdown",
             "id": "689a2a37-b0f1-4c0a-afe7-5252f5ccca3e",
             "metadata": {},
             "source": [
                 "## setup access token\n",
                 "\n",
+                "Don't have an access token yet? [Sign up for free!](https://www.thismlguy.com/)\n",
+                "\n",
                 "We're using dotenv library here, alternatively you can simply set the environment variable as:\n",
                 "```\n",
                 "import os\n",
                 "os.environ[\"CODE_GENIE_TOKEN\"] = \"your-access-token-here\"\n",
                 "```\n",
                 "\n",
                 "Though it is not recommended to do so as notebooks are typically shared with others and you should keep your access token private."
@@ -109,60 +111,60 @@
             "outputs": [],
             "source": [
                 "from code_genie.genie import Genie, PandasGenie"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 9,
             "id": "91de25d6-84dd-4019-bfd9-60fe3582d169",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Loading executor from cache file generate_employee_df_41317.py, set override = True to rerun\n"
+                        "Executor saved to cache file generate_employee_data_58297.py\n"
                     ]
                 }
             ],
             "source": [
                 "data_gen = Genie(instructions=[\"generate a pandas dataframe containing 100 rows with employee information with following columns:\",\n",
                 "                               \"id: random employee id\",\n",
                 "                               \"name: employee name\",\n",
                 "                               \"salary: salary per annum in USD\",\n",
                 "                               \"department: should be either engineering or product\"],\n",
-                "                override=False)"
+                "                 override=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 10,
             "id": "e7f67149-b53f-4c7f-9b4b-fc7e1972391f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(100, 4)"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = data_gen()\n",
                 "df.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 11,
             "id": "9c4897c3-19f0-41ba-80c1-57b2b5aef90d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -188,61 +190,61 @@
                             "      <th>salary</th>\n",
                             "      <th>department</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>9853</td>\n",
-                            "      <td>Employee_1</td>\n",
-                            "      <td>43446</td>\n",
+                            "      <td>391</td>\n",
+                            "      <td>Employee_0</td>\n",
+                            "      <td>80288</td>\n",
                             "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>2444</td>\n",
-                            "      <td>Employee_2</td>\n",
-                            "      <td>142980</td>\n",
+                            "      <td>289</td>\n",
+                            "      <td>Employee_1</td>\n",
+                            "      <td>74477</td>\n",
                             "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>1450</td>\n",
-                            "      <td>Employee_3</td>\n",
-                            "      <td>93806</td>\n",
-                            "      <td>engineering</td>\n",
+                            "      <td>817</td>\n",
+                            "      <td>Employee_2</td>\n",
+                            "      <td>134461</td>\n",
+                            "      <td>product</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>3799</td>\n",
-                            "      <td>Employee_4</td>\n",
-                            "      <td>125635</td>\n",
-                            "      <td>engineering</td>\n",
+                            "      <td>828</td>\n",
+                            "      <td>Employee_3</td>\n",
+                            "      <td>58336</td>\n",
+                            "      <td>product</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>3559</td>\n",
-                            "      <td>Employee_5</td>\n",
-                            "      <td>105519</td>\n",
+                            "      <td>139</td>\n",
+                            "      <td>Employee_4</td>\n",
+                            "      <td>111504</td>\n",
                             "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     id        name  salary   department\n",
-                            "0  9853  Employee_1   43446  engineering\n",
-                            "1  2444  Employee_2  142980  engineering\n",
-                            "2  1450  Employee_3   93806  engineering\n",
-                            "3  3799  Employee_4  125635  engineering\n",
-                            "4  3559  Employee_5  105519  engineering"
+                            "    id        name  salary   department\n",
+                            "0  391  Employee_0   80288  engineering\n",
+                            "1  289  Employee_1   74477  engineering\n",
+                            "2  817  Employee_2  134461      product\n",
+                            "3  828  Employee_3   58336      product\n",
+                            "4  139  Employee_4  111504  engineering"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.head()"
             ]
@@ -253,54 +255,54 @@
             "metadata": {},
             "source": [
                 "### add missing values"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 12,
             "id": "9b04199c-2abe-4de4-a74f-eda4b14f572a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file make_salaries_missing_76197.py\n"
+                        "Executor saved to cache file make_salaries_missing_39233.py\n"
                     ]
                 }
             ],
             "source": [
                 "data_gen_add_missing = PandasGenie(\"make salaries for around 10% of the employees missing\",\n",
                 "                                   columns=list(df.columns))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 13,
             "id": "1a408205-c16d-4799-b6a2-1ff0071972cc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "df_missing = data_gen_add_missing(df)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 14,
             "id": "d47d0c97-f170-4ff5-a011-d975ffebfb2a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "10"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df_missing[\"salary\"].isnull().sum()"
             ]
@@ -319,47 +321,47 @@
             "metadata": {},
             "source": [
                 "### find number of missing values in each column"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
             "id": "934df451-afaf-458c-a36c-a0c0277969b2",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file count_missing_35951.py\n"
+                        "Executor saved to cache file count_missing_values_28317.py\n"
                     ]
                 }
             ],
             "source": [
                 "num_missing = PandasGenie(\"find number of missing values in each column\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 16,
             "id": "5ad11b01-bffc-45ae-ae68-ce9d971d5c51",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "id             0\n",
                             "name           0\n",
                             "salary        10\n",
                             "department     0\n",
                             "dtype: int64"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "num_missing(df_missing)"
             ]
@@ -370,124 +372,164 @@
             "metadata": {},
             "source": [
                 "### plot distribution of salary"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 20,
             "id": "2b9d7bf3-1638-41e9-a44f-a138f1b4294e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file plot_salary_distribution_54098.py\n"
+                        "Executor saved to cache file plot_salary_distribution_49433.py\n"
                     ]
                 }
             ],
             "source": [
-                "dist_salary = PandasGenie(\"plot distribution of salary, create bins of 10K each\", columns=df_missing.columns)"
+                "dist_salary = PandasGenie(\"plot distribution of salary, create bins of 10K each\", columns=df_missing.columns,\n",
+                "                          override=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 21,
             "id": "465c1afb-4fa8-4644-8fcf-48c25f44a31b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjYAAAHHCAYAAACskBIUAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAABAuUlEQVR4nO3deZxN9ePH8fc1yzVmzIwls4ghRHZSIoVMyd6XsvxkjVJ8bSVUiJLlG5FE+coeSVKpaGwpX9mJyL5MZIlmxljGmPn8/ugx9+GaGeaOO3Ov4/V8PO7j4Zz7Oee873HHvJ17zrk2Y4wRAACABeTxdAAAAAB3odgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAXurNN9+UzWbLlW3Vq1dP9erVc0yvWbNGNptNixYtypXtd+7cWSVKlMiVbWVXYmKiunXrpvDwcNlsNvXt2zfXtp3297FmzZpc2yZwu6LYALlg5syZstlsjkfevHkVGRmphg0b6v3339f58+fdsp0TJ07ozTff1Pbt292yPnfy5mxZ8c4772jmzJl68cUXNWfOHHXo0CHTsVeuXNHEiRNVrVo1BQcHKzQ0VBUqVNDzzz+v33//PRdTA3ceX08HAO4kI0aMUMmSJZWcnKyTJ09qzZo16tu3r8aPH6+vv/5alStXdox94403NGjQIJfWf+LECQ0fPlwlSpRQ1apVs7zcDz/84NJ2suNG2aZNm6bU1NQcz3ArVq1apYceekjDhg276dhWrVrp+++/V7t27dS9e3clJyfr999/19KlS1W7dm2VK1cuFxIDdyaKDZCLGjVqpBo1ajimBw8erFWrVqlp06Zq3ry59uzZo4CAAEmSr6+vfH1z9kf04sWLypcvn/z9/XN0Ozfj5+fn0e1nxenTp1W+fPmbjtu0aZOWLl2qkSNH6rXXXnN67oMPPlBcXFwOJcy6CxcuKDAw0NMxgBzBR1GAhz322GMaMmSIjh49qrlz5zrmZ3SOTUxMjOrUqaPQ0FAFBQWpbNmyjl+ea9as0QMPPCBJ6tKli+Njr5kzZ0r65zyaihUrasuWLXr00UeVL18+x7LXn2OTJiUlRa+99prCw8MVGBio5s2bKzY21mlMiRIl1Llz53TLXrvOm2XL6BybCxcu6OWXX1axYsVkt9tVtmxZvfvuuzLGOI2z2Wzq1auXlixZoooVK8put6tChQpatmxZxjv8OqdPn9Zzzz2nsLAw5c2bV1WqVNGsWbMcz6ed33L48GF9++23juxHjhzJcH0HDx6UJD388MPpnvPx8VGhQoUc00ePHtVLL72ksmXLKiAgQIUKFdIzzzyT6bqv9dNPP+mZZ55R8eLFZbfbVaxYMfXr10+XLl1yGte5c2cFBQXp4MGDaty4sfLnz6/27dtr2LBh8vPz05kzZ9Kt+/nnn1doaKguX7580xyAt6HYAF4g7XyNG30k9Ntvv6lp06ZKSkrSiBEjNG7cODVv3lzr1q2TJN13330aMWKEpH9+Mc2ZM0dz5szRo48+6ljH2bNn1ahRI1WtWlUTJkxQ/fr1b5hr5MiR+vbbbzVw4ED17t1bMTExio6OTvfL82ayku1axhg1b95c7733np588kmNHz9eZcuW1YABA9S/f/9043/++We99NJLatu2rcaOHavLly+rVatWOnv27A1zXbp0SfXq1dOcOXPUvn17/ec//1FISIg6d+6siRMnOrLPmTNHhQsXVtWqVR3Z77rrrgzXGRUVJUmaN2+erl69esPtb9q0Sf/73//Utm1bvf/+++rRo4dWrlypevXq6eLFizdc9vPPP9fFixf14osvatKkSWrYsKEmTZqkjh07pht79epVNWzYUEWKFNG7776rVq1aqUOHDrp69ao+++wzp7FXrlzRokWL1KpVK+XNm/eGGQCvZADkuBkzZhhJZtOmTZmOCQkJMdWqVXNMDxs2zFz7I/ree+8ZSebMmTOZrmPTpk1GkpkxY0a65+rWrWskmalTp2b4XN26dR3Tq1evNpJM0aJFTUJCgmP+woULjSQzceJEx7yoqCjTqVOnm67zRtk6depkoqKiHNNLliwxkszbb7/tNO7pp582NpvNHDhwwDFPkvH393eat2PHDiPJTJo0Kd22rjVhwgQjycydO9cx78qVK6ZWrVomKCjI6bVHRUWZJk2a3HB9xhiTmprq2NdhYWGmXbt2ZvLkyebo0aPpxl68eDHdvPXr1xtJZvbs2Y55aX8fq1evvuGyo0aNMjabzWlbnTp1MpLMoEGD0o2vVauWqVmzptO8xYsXp9sWcDvhiA3gJYKCgm54dVRoaKgk6auvvsr2ibZ2u11dunTJ8viOHTsqf/78jumnn35aERER+u6777K1/az67rvv5OPjo969ezvNf/nll2WM0ffff+80Pzo6WqVKlXJMV65cWcHBwTp06NBNtxMeHq527do55vn5+al3795KTEzUjz/+6HJ2m82m5cuX6+2331aBAgU0f/589ezZU1FRUWrTpo3TOTZp51NJUnJyss6ePavSpUsrNDRUW7duveF2rl32woUL+uuvv1S7dm0ZY7Rt27Z041988cV08zp27KgNGzY4Pj6T/jnSVKxYMdWtW9eVlw14DYoN4CUSExOdSsT12rRpo4cffljdunVTWFiY2rZtq4ULF7pUcooWLerSicJlypRxmrbZbCpdunSWzgG5FUePHlVkZGS6/XHfffc5nr9W8eLF062jQIEC+vvvv2+6nTJlyihPHud/CjPbTlbZ7Xa9/vrr2rNnj06cOKH58+froYce0sKFC9WrVy/HuEuXLmno0KGO84gKFy6su+66S3FxcYqPj7/hNo4dO6bOnTurYMGCCgoK0l133eUoI9cv6+vrq7vvvjvdOtq0aSO73a558+Y5llu6dKnat2+fa/dQAtyNYgN4gT/++EPx8fEqXbp0pmMCAgK0du1arVixQh06dNCvv/6qNm3a6PHHH1dKSkqWtnPt//LdJbNfgFnN5A4+Pj4ZzjfXnWjsCREREWrbtq3Wrl2rMmXKaOHChY5zb/79739r5MiRat26tRYuXKgffvhBMTExKlSo0A0La0pKih5//HHH+U9LlixRTEyM42Ts65e12+3pypv0T/lr2rSpo9gsWrRISUlJevbZZ9306oHcR7EBvMCcOXMkSQ0bNrzhuDx58qhBgwYaP368du/erZEjR2rVqlVavXq1pMxLRnbt37/fadoYowMHDjhdwVSgQIEML2G+/miHK9mioqJ04sSJdB/Npd3cLu0E3VsVFRWl/fv3pysC7t6O9M9HXJUrV1ZycrL++usvSf8UiU6dOmncuHF6+umn9fjjj6tOnTo3vSR8586d2rdvn8aNG6eBAweqRYsWio6OVmRkpMu5OnbsqH379mnTpk2aN2+eqlWrpgoVKmTnJQJegWIDeNiqVav01ltvqWTJkmrfvn2m486dO5duXtqN7pKSkiTJcW8Sd90rZfbs2U7lYtGiRfrzzz/VqFEjx7xSpUrpl19+0ZUrVxzzli5dmu6ycFeyNW7cWCkpKfrggw+c5r/33nuy2WxO278VjRs3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oqOj1bt3bx08eNDd2RQREaHy5cs7zbvvvvt07NixTJcZPHiw4uPjHY/Y2Fi35wIAAN7J5WKzfPlylS9fXhs3blTlypVVuXJlbdiwQRUqVFBMTIxbwz388MPau3ev07x9+/YpKioq02XsdruCg4OdHgAA4M7g8kdRgwYNUr9+/TR69Oh08wcOHKjHH3/cbeH69eun2rVr65133lHr1q21ceNGffzxx/r444/dtg0AAGAdLh+x2bNnj5577rl087t27ardu3e7JVSaBx54QF9++aXmz5+vihUr6q233tKECRPUvn17t24HAABYg8tHbO666y5t375dZcqUcZq/ffv2HLlSqmnTpmratKnb1wsAAKzH5WLTvXt3Pf/88zp06JBq164tSVq3bp3GjBmj/v37uz0gAABAVrlcbIYMGaL8+fNr3LhxGjx4sCQpMjJSb775pnr37u32gAAAAFnlcrGx2Wzq16+f+vXrp/Pnz0uS8ufP7/ZgAAAArnK52FyLQgMAALxJtm7QBwAA4I0oNgAAwDIoNgAAwDJcKjbJyclq0KCB9u/fn1N5AAAAss2lYuPn56dff/01p7IAAADcEpc/inr22Wc1ffr0nMgCAABwS1y+3Pvq1av65JNPtGLFCt1///0KDAx0en78+PFuCwcAAOAKl4vNrl27VL16dUnSvn37nJ6z2WzuSQUAAJANLheb1atX50QOAACAW5bty70PHDig5cuX69KlS5IkY4zbQgEAAGSHy8Xm7NmzatCgge699141btxYf/75pyTpueee08svv+z2gAAAAFnlcrHp16+f/Pz8dOzYMeXLl88xv02bNlq2bJlbwwEAALjC5XNsfvjhBy1fvlx333230/wyZcro6NGjbgsGAADgKpeP2Fy4cMHpSE2ac+fOyW63uyUUAABAdrhcbB555BHNnj3bMW2z2ZSamqqxY8eqfv36bg0HAADgCpc/iho7dqwaNGigzZs368qVK3r11Vf122+/6dy5c1q3bl1OZAQAAMgSl4/YVKxYUfv27VOdOnXUokULXbhwQS1bttS2bdtUqlSpnMgIAACQJS4fsZGkkJAQvf766+7OAgAAcEuyVWz+/vtvTZ8+XXv27JEklS9fXl26dFHBggXdGg4AAMAVNuPiLYPXrl2rZs2aKSQkRDVq1JAkbdmyRXFxcfrmm2/06KOP5kjQ7EpI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+Ph41atXTxEREY7HZ5995uloAADAC3n1ERtjjKcjAACA24hXH7EBAABwBcUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYxm1RbCZPnqwSJUoob968qlmzpjZu3OjpSAAAwAt5fbH57LPP1L9/fw0bNkxbt25VlSpV1LBhQ50+fdrT0QAAgJfx+mIzfvx4de/eXV26dFH58uU1depU5cuXT5988omnowEAAC/j1cXmypUr2rJli6Kjox3z8uTJo+joaK1fv96DyQAAgDfy9XSAG/nrr7+UkpKisLAwp/lhYWH6/fffM1wmKSlJSUlJjun4+HhJUkJCgtvzpSZddPs6AQC4neTE79dr12uMcWk5ry422TFq1CgNHz483fxixYp5IA0AANYWMiFn13/+/HmFhIRkebxXF5vChQvLx8dHp06dcpp/6tQphYeHZ7jM4MGD1b9/f8d0amqqzp07p0KFCslms7ktW0JCgooVK6bY2FgFBwe7bb057XbMTebcQebcQebcQebckZOZjTE6f/68IiMjXVrOq4uNv7+/7r//fq1cuVJPPfWUpH+KysqVK9WrV68Ml7Hb7bLb7U7zQkNDcyxjcHDwbfMGvNbtmJvMuYPMuYPMuYPMuSOnMrtypCaNVxcbSerfv786deqkGjVq6MEHH9SECRN04cIFdenSxdPRAACAl/H6YtOmTRudOXNGQ4cO1cmTJ1W1alUtW7Ys3QnFAAAAXl9sJKlXr16ZfvTkKXa7XcOGDUv3sZe3ux1zkzl3kDl3kDl3kDl3eGNmm3H1OioAAAAv5dU36AMAAHAFxQYAAFgGxQYAAFgGxQYAAFjGHVtsRo8eLZvNpr59+zrmXb58WT179lShQoUUFBSkVq1apbvr8bFjx9SkSRPly5dPRYoU0YABA3T16lWnMWvWrFH16tVlt9tVunRpzZw5M932J0+erBIlSihv3ryqWbOmNm7cmGHON998UzabzelRrlw5r84sScePH9ezzz6rQoUKKSAgQJUqVdLmzZsdzxtjNHToUEVERCggIEDR0dHav3+/0zrOnTun9u3bKzg4WKGhoXruueeUmJjoNObXX3/VI488orx586pYsWIaO3Zsuiyff/65ypUrp7x586pSpUr67rvv0o0pUaJEuv1ss9nUs2dPr93PKSkpGjJkiEqWLKmAgACVKlVKb731ltP3qnjbfpb+uT163759FRUVpYCAANWuXVubNm3ymsxr165Vs2bNFBkZKZvNpiVLljgt4+l8GWUpVKiQfHx8ZLfbM8y8ePFiPfHEE447sG/fvj3dtnL7PR4eHi4fHx/5+/uny5ycnKyBAweqUqVKCgwMVGRkpDp27KgTJ054dD9HRETIbrfrrrvuUlhYWIb7+s0331S5cuUUGBioAgUKKDo6Whs2bPBo7pu9P67Vo0cP2Ww2TZgwwaOZb/TzdVPmDrRx40ZTokQJU7lyZdOnTx/H/B49ephixYqZlStXms2bN5uHHnrI1K5d2/H81atXTcWKFU10dLTZtm2b+e6770zhwoXN4MGDHWMOHTpk8uXLZ/r37292795tJk2aZHx8fMyyZcscYxYsWGD8/f3NJ598Yn777TfTvXt3Exoaak6dOpUu67Bhw0yFChXMn3/+6XicOXPGqzOfO3fOREVFmc6dO5sNGzaYQ4cOmeXLl5sDBw44xowePdqEhISYJUuWmB07dpjmzZubkiVLmkuXLjnGPPnkk6ZKlSrml19+MT/99JMpXbq0adeuneP5+Ph4ExYWZtq3b2927dpl5s+fbwICAsxHH33kGLNu3Trj4+Njxo4da3bv3m3eeOMN4+fnZ3bu3OmU+fTp0077OCYmxkgyq1ev9tr9PHLkSFOoUCGzdOlSc/jwYfP555+boKAgM3HiRK/dz8YY07p1a1O+fHnz448/mv3795thw4aZ4OBg88cff3hF5g8//NC8/vrrZvHixUaS+fLLL53yezrftfs0LcuQIUNM9+7dzQMPPGAkmc8++8wp8+zZs83w4cPNtGnTjCSzbdu2dH8vuf0e79u3r3n++edNdHS0kWRmzJjhGBMXF2eio6PNZ599Zn7//Xezfv168+CDD5r777/fKXNu7+clS5aYyZMnmzJlypgiRYpk+P6YN2+eiYmJMQcPHjS7du0yzz33nAkODjanT5/22vdHmsWLF5sqVaqYyMhI895773l8X2f283Uzd1yxOX/+vClTpoyJiYkxdevWdRSbuLg44+fnZz7//HPH2D179hhJZv369cYYY7777juTJ08ec/LkSceYKVOmmODgYJOUlGSMMebVV181FSpUcNpmmzZtTMOGDR3TDz74oOnZs6djOiUlxURGRppRo0alyzts2DBTpUqVDF+Lt2YeOHCgqVOnToaZjTEmNTXVhIeHm//85z9Or8Vut5v58+cbY4zZvXu3kWQ2bdrkGPP9998bm81mjh8/bowx5sMPPzQFChRwvI60bZctW9Yx3bp1a9OkSROn7desWdO88MILmeYzxpg+ffqYUqVKmdTUVK/dz02aNDFdu3Z1mteyZUvTvn17Y4x37ueLFy8aHx8fs3TpUqf51atXN6+//rrXZb7+F5c35cssiyTTv39/k5HDhw9nWGw8/R6XZJ599tkMM6fZuHGjkWSOHj1qjPH8frbb7RkWm+vFx8cbSWbFihVekTuz98cff/xhihYtanbt2mWioqKcio2nM1/785UVd9xHUT179lSTJk0UHR3tNH/Lli1KTk52ml+uXDkVL15c69evlyStX79elSpVcrrrccOGDZWQkKDffvvNMeb6dTds2NCxjitXrmjLli1OY/LkyaPo6GjHmOvt379fkZGRuueee9S+fXsdO3bMqzN//fXXqlGjhp555hkVKVJE1apV07Rp0xzPHz58WCdPnnRaX0hIiGrWrOmUOzQ0VDVq1HCMiY6OVp48eRyHddevX69HH31U/v7+Trn37t2rv//+O0uvLSNXrlzR3Llz1bVrV9lsNq/dz7Vr19bKlSu1b98+SdKOHTv0888/q1GjRl67n69evaqUlBTlzZvXaX5AQIB+/vlnr8x8LW/Kl1kWSdq7d2+mryEjnn6PZyVzfHy8bDab47v/PL2fa9asecO8aa/3448/VkhIiKpUqeIVuaX0+zo1NVUdOnTQgAEDVKFChXSvw9OZr/35yoo7qtgsWLBAW7du1ahRo9I9d/LkSfn7+6f7wsywsDCdPHnSMeb6r3JIm77ZmISEBF26dEl//fWXUlJSMhyTto5r1axZUzNnztSyZcs0ZcoUHT58WI888ojOnz/vtZkPHTqkKVOmqEyZMlq+fLlefPFF9e7dW7NmzXLa7o3Wd/LkSRUpUsTpeV9fXxUsWNAtry2j3GmWLFmiuLg4de7c2bEOb9zPgwYNUtu2bVWuXDn5+fmpWrVq6tu3r9q3b++0XW/az/nz51etWrX01ltv6cSJE0pJSdHcuXO1fv16/fnnn16Z+VrelC+zLJIUFxeX6WvI7HV58j1+s8yXL1/WwIED1a5dO8cXLXp6P9/oa32WLl2qoKAg5c2bV++9955iYmJUuHBhr8gtpd/XY8aMka+vr3r37p3h6/F05pv9XF7vtvhKBXeIjY1Vnz59FBMTk+5/i94s7X/fklS5cmXVrFlTUVFRWrhwoQICAjyYLHOpqamqUaOG3nnnHUlStWrVtGvXLk2dOlWdOnXycLqbmz59uho1aqTIyEhPR7mhhQsXat68efr0009VoUIFbd++XX379lVkZKRX7+c5c+aoa9euKlq0qHx8fFS9enW1a9dOW7Zs8XQ0eKHk5GS1bt1axhhNmTLF03GypH79+tq+fbv++usvTZs2Ta1bt9aGDRvSlQNvsGXLFk2cOFFbt26VzWbzdBy3uGOO2GzZskWnT59W9erV5evrK19fX/344496//335evrq7CwMF25ciVdkz116pTCw8MlSeHh4emuEkibvtmY4OBgBQQEqHDhwvLx8clwTNo6biQ0NFT33nuvDhw4oPDwcK/MHBERofLlyzvNu++++xwfoaUtc6P1hYeH6/Tp007PX716VefOnXPLa8tsXx89elQrVqxQt27dHPO8dT8PGDDAcdSmUqVK6tChg/r16+c4Iumt+7lUqVL68ccflZiYqNjYWG3cuFHJycm65557vDZzGm/Kl1kWSemOvNyMp9/jmWVOKzVHjx5VTEyM42hN2rY8uZ8zeg1pAgMDVbp0aT300EOaPn26fH19NX36dK/ILTnv659++kmnT59W8eLFHb8bjx49qpdfflklSpTwisxZ/f2Y5o4pNg0aNNDOnTu1fft2x6NGjRpq3769489+fn5auXKlY5m9e/fq2LFjqlWrliSpVq1a2rlzp9NfcNoPW9ov8lq1ajmtI21M2jr8/f11//33O41JTU3VypUrHWNuJDExUQcPHlRERITuv/9+r8z88MMPp/sMd9++fYqKipIklSxZUuHh4U7rS0hI0IYNG5xyx8XFOf0vftWqVUpNTXV8tl2rVi2tXbtWycnJTrnLli2rAgUKZOm1XW/GjBkqUqSImjRp4pjnrfv54sWLjvMT0vj4+Cg1NVWSd+9n6Z9//CMiIvT3339r+fLlatGihddn9qZ8mWWRpLJly2b6GjLi6fd4RpnTSs3+/fu1YsUKFSpUyOl5T+/n6y/hvpHU1FQlJSV5RW7JeV936NBBv/76q9PvxsjISA0YMEDLly/3iszX/nxlSZZPM7aga6+KMuafyx2LFy9uVq1aZTZv3mxq1aplatWq5Xg+7XLHJ554wmzfvt0sW7bM3HXXXRle7jhgwACzZ88eM3ny5Awvd7Tb7WbmzJlm9+7d5vnnnzehoaFOVxukefnll82aNWvM4cOHzbp160x0dLQpXLiw49JBb8y8ceNG4+vra0aOHGn2799v5s2bZ/Lly2fmzp3rGDN69GgTGhpqvvrqK/Prr7+aFi1aZHjJbLVq1cyGDRvMzz//bMqUKeN0eWFcXJwJCwszHTp0MLt27TILFiww+fLlS3d5oa+vr3n33XfNnj17zLBhwzK9DDklJcUUL17cDBw4MN1z3rifO3XqZIoWLeq43Hvx4sWmcOHC5tVXX/Xq/bxs2TLz/fffm0OHDpkffvjBVKlSxdSsWdNcuXLFKzJv2LDBbNu2zWzbts1IMuPHjzfbtm1zXI3j6XzXXxobGhpqFixYYBYuXGjq1atnJJkxY8Y4ZT579qzZtm2b+fbbb40ks2DBArNt2zbz559/OtaV2+/xqVOnmi+++MK0bNnSSDLDhw93ZL5y5Ypp3ry5ufvuu8327dudbsVw7VU3ub2fv/rqK/PLL7+YevXqmcjIyHTvj8TERDN48GCzfv16c+TIEbN582bTpUsXY7fbza5du7z2/XG966+K8tS+zuzn62YoNtcUm0uXLpmXXnrJFChQwOTLl8/861//cvrBN8aYI0eOmEaNGpmAgABTuHBh8/LLL5vk5GSnMatXrzZVq1Y1/v7+5p577nG6P0OaSZMmmeLFixt/f3/z4IMPml9++SXDjG3atDERERHG39/fFC1a1LRp08bpfjDemNkYY7755htTsWJFY7fbTbly5czHH3/s9HxqaqoZMmSICQsLM3a73TRo0MDs3bvXaczZs2dNu3btTFBQkAkODjZdunQx58+fdxqzY8cOU6dOHWO3203RokXN6NGj02VZuHChuffee42/v7+pUKGC+fbbbzPMvHz5ciMpXQ5jvHM/JyQkmD59+pjixYubvHnzmnvuuce8/vrrTv/we+N+/uyzz8w999xj/P39TXh4uOnZs6eJi4vzmsyrV682ktI9OnXq5BX5rpWWpUCBAjfMPGPGjAyfHzZsmGNduf0eT7sPTEaZ0y5Lz+iRdm8pT+znsLAw4+fnl2nuS5cumX/9618mMjLS+Pv7m4iICNO8eXOzceNGp/V52/vjehkVG0/s68x+vm7GZsw1tykFAAC4jd0x59gAAADro9gAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAuK3MnDnT5e9CAnDnoNgAyFVnzpzRiy++qOLFi8tutys8PFwNGzbUunXrPB0NgAX4ejoAgDtLq1atdOXKFc2aNUv33HOPTp06pZUrV+rs2bO5luHKlSvy9/fPte0ByD0csQGQa+Li4vTTTz9pzJgxql+/vqKiovTggw9q8ODBat68uSRp/PjxqlSpkgIDA1WsWDG99NJLSkxMzHSdBw8eVIsWLRQWFqagoCA98MADWrFihdOYEiVK6K233lLHjh0VHBys559/Xo899ph69erlNO7MmTPy9/dP9w3EAG4fFBsAuSYoKEhBQUFasmSJkpKSMhyTJ08evf/++/rtt980a9YsrVq1Sq+++mqm60xMTFTjxo21cuVKbdu2TU8++aSaNWumY8eOOY179913VaVKFW3btk1DhgxRt27d9OmnnzrlmDt3rooWLarHHnvMPS8YQK7jSzAB5KovvvhC3bt316VLl1S9enXVrVtXbdu2VeXKlTMcv2jRIvXo0UN//fWXpH9OHu7bt6/i4uIy3UbFihXVo0cPxxGZEiVKqFq1avryyy8dYy5fvqzIyEhNnTpVrVu3liRVqVJFLVu21LBhw9z0agHkNo7YAMhVrVq10okTJ/T111/rySef1Jo1a1S9enXNnDlTkrRixQo1aNBARYsWVf78+dWhQwedPXtWFy9ezHB9iYmJeuWVV3TfffcpNDRUQUFB2rNnT7ojNjVq1HCazps3rzp06KBPPvlEkrR161bt2rVLnTt3dvtrBpB7KDYAcl3evHn1+OOPa8iQIfrf//6nzp07a9iwYTpy5IiaNm2qypUr64svvtCWLVs0efJkSf+c8JuRV155RV9++aXeeecd/fTTT9q+fbsqVaqUbnxgYGC6Zbt166aYmBj98ccfmjFjhh577DFFRUW5/wUDyDVcFQXA48qXL68lS5Zoy5YtSk1N1bhx45Qnzz//71q4cOENl123bp06d+6sf/3rX5L+OYJz5MiRLG23UqVKqlGjhqZNm6ZPP/1UH3zwwS29DgCeR7EBkGvOnj2rZ555Rl27dlXlypWVP39+bd68WWPHjlWLFi1UunRpJScna9KkSWrWrJnWrVunqVOn3nCdZcqU0eLFi9WsWTPZbDYNGTJEqampWc7UrVs39erVS4GBgY5yBOD2xUdRAHJNUFCQatasqffee0+PPvqoKlasqCFDhqh79+764IMPVKVKFY0fP15jxoxRxYoVNW/ePI0aNeqG6xw/frwKFCig2rVrq1mzZmrYsKGqV6+e5Uzt2rWTr6+v2rVrp7x5897qSwTgYVwVBeCOduTIEZUqVUqbNm1yqRAB8E4UGwB3pOTkZJ09e1avvPKKDh8+zFc6ABbBR1EA7kjr1q1TRESENm3adNPzeADcPjhiAwAALIMjNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDL+H+EoGf6VNONaAAAAAElFTkSuQmCC\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjMAAAGwCAYAAABcnuQpAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA+OElEQVR4nO3deXxU9b3/8fcsyWSfhIRskIRF1oDsUMRWqCgCbtW6XaSov1qtKCK9lHIVt15FrbVYS6V6b0VvVbQVqHXBIoJIZRFCZAt7JCGQhJB9myzz/f2BTI3sMcnMCa/n4zGPMOd853w/30kyeXPO95xjM8YYAQAAWJTd3wUAAAB8F4QZAABgaYQZAABgaYQZAABgaYQZAABgaYQZAABgaYQZAABgaU5/F9DavF6vDh06pMjISNlsNn+XAwAAzoIxRhUVFUpOTpbdfvp9L+0+zBw6dEgpKSn+LgMAADRDbm6uOnfufNo27T7MREZGSjr2ZkRFRfm5GgAAcDbKy8uVkpLi+zt+Ou0+zBw/tBQVFUWYAQDAYs5miggTgAEAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKU5/V0AgBPl5OSoqKiozfuNi4tTampqm/cLAN8FYQYIMDk5Oerdp49qqqvbvO/QsDDtzMoi0ACwFMIMEGCKiopUU12tSbN+o4TU7m3Wb0HOPr3+9EwVFRURZgBYCmEGCFAJqd3VuUe6v8sAgIDHBGAAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBpfg0zq1ev1lVXXaXk5GTZbDYtXbr0hDZZWVm6+uqr5Xa7FR4ermHDhiknJ6ftiwUAAAHJr2GmqqpKAwYM0Pz580+6ft++fbr44ovVu3dvrVq1Slu2bNGcOXMUEhLSxpUCAIBA5fRn5+PHj9f48eNPuf7BBx/UhAkT9Mwzz/iWde/e/bTb9Hg88ng8vufl5eXfvVAAABCwAnbOjNfr1fvvv6+ePXtq3Lhxio+P14gRI056KOqb5s6dK7fb7XukpKS0TcEAAMAvAjbMFBYWqrKyUk899ZSuuOIK/fOf/9SPfvQjXXfddfr0009P+brZs2errKzM98jNzW3DqgEAQFvz62Gm0/F6vZKka665Rg888IAkaeDAgfr888+1YMECXXLJJSd9ncvlksvlarM6AQCAfwXsnpm4uDg5nU717du3yfI+ffpwNhMAAPAJ2DATHBysYcOGadeuXU2W7969W2lpaX6qCgAABBq/HmaqrKzU3r17fc+zs7OVmZmpDh06KDU1VTNnztRNN92kH/zgBxozZoyWLVumf/zjH1q1apX/igYAAAHFr2Fm48aNGjNmjO/5jBkzJElTpkzRwoUL9aMf/UgLFizQ3LlzNW3aNPXq1UvvvPOOLr74Yn+VDAAAAoxfw8zo0aNljDltmzvuuEN33HFHG1UEAACsJmDnzAAAAJwNwgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0v4aZ1atX66qrrlJycrJsNpuWLl16yrZ33323bDab5s2b12b1AQCAwOfXMFNVVaUBAwZo/vz5p223ZMkSrVu3TsnJyW1UGQAAsAqnPzsfP368xo8ff9o2eXl5uu+++/TRRx9p4sSJbVQZAACwCr+GmTPxer2aPHmyZs6cqfT09LN6jcfjkcfj8T0vLy9vrfIAAEAACOgJwE8//bScTqemTZt21q+ZO3eu3G6375GSktKKFQIAAH8L2DCzadMmPf/881q4cKFsNttZv2727NkqKyvzPXJzc1uxSgAA4G8BG2Y+++wzFRYWKjU1VU6nU06nUwcOHNAvfvELdenS5ZSvc7lcioqKavIAAADtV8DOmZk8ebLGjh3bZNm4ceM0efJk3X777X6qCgAABBq/hpnKykrt3bvX9zw7O1uZmZnq0KGDUlNTFRsb26R9UFCQEhMT1atXr7YuFQAABCi/hpmNGzdqzJgxvuczZsyQJE2ZMkULFy70U1UAAMBK/BpmRo8eLWPMWbf/6quvWq8YAABgSQE7ARgAAOBsEGYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAICl+TXMrF69WldddZWSk5Nls9m0dOlS37r6+nrNmjVL/fv3V3h4uJKTk/WTn/xEhw4d8l/BAAAg4Pg1zFRVVWnAgAGaP3/+Ceuqq6uVkZGhOXPmKCMjQ4sXL9auXbt09dVX+6FSAAAQqJz+7Hz8+PEaP378Sde53W4tX768ybI//OEPGj58uHJycpSamnrS13k8Hnk8Ht/z8vLylisYAAAEHEvNmSkrK5PNZlN0dPQp28ydO1dut9v3SElJabsCAQBAm7NMmKmtrdWsWbN0yy23KCoq6pTtZs+erbKyMt8jNze3DasEAABtza+Hmc5WfX29brzxRhlj9OKLL562rcvlksvlaqPKAACAvwV8mDkeZA4cOKBPPvnktHtlAADA+Segw8zxILNnzx6tXLlSsbGx/i4JAAAEGL+GmcrKSu3du9f3PDs7W5mZmerQoYOSkpL04x//WBkZGXrvvffU2Nio/Px8SVKHDh0UHBzsr7IBAEAA8WuY2bhxo8aMGeN7PmPGDEnSlClT9Oijj+rdd9+VJA0cOLDJ61auXKnRo0e3VZkAACCA+TXMjB49WsaYU64/3ToAAADJQqdmAwAAnAxhBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWJpfbzQJAGg7OTk5KioqavN+4+LilJqa2ub94vxBmAGA80BOTo569+mjmurqNu87NCxMO7OyCDRoNYQZADgPFBUVqaa6WpNm/UYJqd3brN+CnH16/emZKioqIsyg1RBmAOA8kpDaXZ17pPu7DKBFMQEYAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYml/DzOrVq3XVVVcpOTlZNptNS5cubbLeGKOHH35YSUlJ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AwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALC3gw8zcuXM1bNgwRUZGKj4+Xtdee6127drl77IAAECACPgw8+mnn2rq1Klat26dli9frvr6el1++eWqqqryd2kAACAAOP1dwJksW7asyfOFCxcqPj5emzZt0g9+8IMT2ns8Hnk8Ht/z8vLyVq8RAAD4T8Dvmfm2srIySVKHDh1Oun7u3Llyu92+R0pKSluWBwAA2pilwozX69X06dM1atQo9evX76RtZs+erbKyMt8jNze3jasEAABtKeAPM33T1KlTtW3bNq1Zs+aUbVwul1wuVxtWBQAA/MkyYebee+/Ve++9p9WrV6tz587+LgcAAASIgA8zxhjdd999WrJkiVatWqWuXbv6uyQAABBAAj7MTJ06VW+88Yb+/ve/KzIyUvn5+ZIkt9ut0NBQP1cHAAD8LeAnAL/44osqKyvT6NGjlZSU5Hu89dZb/i4NAAAEgIDfM2OM8XcJAAAggAX8nhkAAIDTIcwAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLs0SYmT9/vrp06aKQkBCNGDFCGzZs8HdJAAAgQAR8mHnrrbc0Y8YMPfLII8rIyNCAAQM0btw4FRYW+rs0AAAQAAI+zDz33HO68847dfvtt6tv375asGCBwsLC9Oc//9nfpQEAgADg9HcBp1NXV6dNmzZp9uzZvmV2u11jx47V2rVrT/oaj8cjj8fje15WViZJKi8vb5Ua8/PzlZ+f3yrbPh273S6v10u/7bDfXbt2SZIO7tkuT011m/Vb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GaKvvvpKaWlpp23r9XoVHR2tN954Q1deeaWkYxOAlyxZomuvvfakr3n22We1aNEibdy4UdKxPTNPPvmk8vLy1LFjR1+7e+65R1999ZU++OADSdJzzz2n+fPna+/evbLZbC0wUgBthT0zANrUgAEDdOmll6p///664YYb9PLLL6ukpESSVFBQoDvvvFM9evSQ2+1WVFSUKisrlZOTc8rtvfXWWxo1apQSExMVERGhhx566IT2aWlpTYKMJN1555365z//qby8PEnSwoULddtttxFkAAsizABoUw6HQ8uXL9eHH36ovn376oUXXlCvXr2UnZ2tKVOmKDMzU88//7w+//xzZWZmKjY29pSTdteuXatJkyZpwoQJeu+997R582Y9+OCDJ7QPDw8/4bWDBg3SgAED9Nprr2nTpk3avn27brvtttYYMoBW5vR3AQDOPzabTaNGjdKoUaP08MMPKy0tTUuWLNG//vUv/fGPf9SECRMkSbm5uSoqKjrldj7//HOlpaXpwQcf9C07cODAWdfx05/+VPPmzVNeXp7Gjh2rlJSU5g8KgN8QZgC0qfXr12vFihW6/PLLFR8fr/Xr1+vIkSPq06ePevToof/7v//T0KFDVV5erpkzZyo0NPSU2+rRo4dycnK0aNEiDRs2TO+//76WLFly1rX8x3/8h/7zP/9TL7/8sl577bWWGB4AP+AwE4A2FRUVpdWrV2vChAnq2bOnHnroIf32t7/V+PHj9b//+78qKSnR4MGDNXnyZE2bNk3x8fGn3NbVV1+tBx54QPfee68GDhyozz//XHPmzDnrWtxut66//npFREScckIxgMDH2UwAzmuXXnqp0tPT9fvf/97fpQBoJsIMgPNSSUmJVq1apR//+MfasWOHevXq5e+SADQTc2YAnJcGDRqkkpISPf300wQZwOLYMwMAACyNCcAAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDS/j9DaSi4hWz9FAAAAABJRU5ErkJggg==\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "dist_salary(df_missing)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 22,
             "id": "45559024-5905-43df-a021-19a2d0b77dff",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file make_boxplots_25996.py\n"
+                        "Executor saved to cache file boxplots_of_salary_by_department_12125.py\n"
                     ]
                 }
             ],
             "source": [
                 "dept_salary = PandasGenie(\"make boxplots of salary grouped by department\", columns=df_missing.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 23,
             "id": "637d39d9-c0bf-4a20-89bc-37af671c77cd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAtEAAAHWCAYAAACxJNUiAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAABQp0lEQVR4nO3deVhUdf//8dcAsogCriCpSGaKS+4L5lJJoeaCZq65FGmLlEsuWYloi3eau6WV31vNG0vtVjPNLbUoNVRcUkvTblNT0UoBUUGB8/uji/NjApWDyIA+H9c118Wcz/uc8z4zzvji8JkzNsMwDAEAAADINSdHNwAAAAAUNYRoAAAAwCJCNAAAAGARIRoAAACwiBANAAAAWESIBgAAACwiRAMAAAAWEaIBAAAAiwjRAAAAgEWEaAC33UMPPaSHHnrI0W3c1G+//SabzaYFCxaYy6KiomSz2Qpk//98nL755hvZbDZ9/vnnBbL/AQMGqEqVKgWyr6wK+jgBID8QogFks3//fnXr1k0BAQFyd3fXPffco0cffVSzZs1ydGtFwunTpxUVFaW9e/c6upVsCnNvt1vmL0SZt+LFi6ty5crq2LGj5s+fr9TUVEe3mGvvvPOOVq5c6eg2cmXbtm2KiopSQkKCo1sB8hUhGoCdbdu2qVGjRtq3b58GDhyo2bNn69lnn5WTk5NmzJjh6PYK3BtvvKErV65YWuf06dMaP3685aC6YcMGbdiwwdI6Vt2ot48//liHDx++rfsvDObMmaNFixZp1qxZevbZZ3X+/Hk988wzatKkiU6ePOno9nKlqIXo8ePHE6Jxx3FxdAMACpe3335b3t7e2rlzp3x8fOzGzp0755imskhLS1NGRoZcXV0LZH8uLi5ycbm9b5WXL19W8eLFC+yYrqdYsWIO3X9B6datm8qWLWvej4yMVHR0tPr166cnn3xSP/zwgwO7uz7DMJSSkiIPDw9HtwJAnIkG8A+//vqratWqlS1AS1L58uXt7s+fP1+PPPKIypcvLzc3N9WsWVNz5sy56T6uXr2qyMhINWzYUN7e3vL09FTLli21ZcsWu7rMOcrvvfeepk+frqpVq8rNzU07duyQp6enhgwZkm3bv//+u5ydnTVx4sQb9pCQkKABAwbI29tbPj4+6t+/f45nynKaE71x40a1aNFCPj4+KlGihKpXr67XXntN0t/zexs3bixJevrpp82pA5nzrB966CHVrl1bcXFxatWqlYoXL26ue7254+np6Xrttdfk5+cnT09PderUKdsZ0ypVqmjAgAHZ1s26zZv1ltOc6EuXLumVV15RpUqV5ObmpurVq+u9996TYRh2dTabTREREVq5cqVq164tNzc31apVS+vWrcvW0/Xc7DjHjRunYsWK6Y8//si27qBBg+Tj46OUlJRc7y+rPn366Nlnn1VsbKw2btxoNxYbG6u2bdvK29tbxYsXV+vWrbV161a7msx/J4cOHVL37t3l5eWlMmXKaMiQIdl6yu3rpkqVKurQoYPWr1+vRo0aycPDQx9++KFsNpsuXbqkhQsXms9h5nOf2ccvv/yip556St7e3ipXrpzGjh0rwzB08uRJde7cWV5eXvLz89OUKVOy7Tc1NVXjxo3TfffdJzc3N1WqVEmjRo3KNt0lN895VFSURo4cKUkKDAw0+/3tt99y/dwAhRVnogHYCQgI0Pbt23XgwAHVrl37hrVz5sxRrVq11KlTJ7m4uOjLL7/Uiy++qIyMDA0ePPi66yUlJWnevHnq1auXBg4cqIsXL+r//u//FBoaqh07dqhevXp29fPnz1dKSooGDRokNzc3Va5cWV26dNGSJUs0depUOTs7m7WffvqpDMNQnz59rrt/wzDUuXNnff/993r++ecVFBSkFStWqH///jd9fA4ePKgOHTrogQce0IQJE+Tm5qajR4+aoSooKEgTJkxQZGSkBg0apJYtW0qSmjdvbm7jr7/+Urt27dSzZ0899dRT8vX1veE+3377bdlsNo0ePVrnzp3T9OnTFRISor1791o6K5mb3rIyDEOdOnXSli1bFB4ernr16mn9+vUaOXKkTp06pWnTptnVf//991q+fLlefPFFlSxZUjNnztQTTzyhEydOqEyZMjft72bH2bdvX02YMEFLlixRRESEud7Vq1f1+eef64knnpC7u3uuH49/6tu3rz766CNt2LBBjz76qCRp8+bNateunRo2bKhx48bJycnJDMHfffedmjRpYreN7t27q0qVKpo4caJ++OEHzZw5UxcuXNAnn3xi1lh53Rw+fFi9evXSc889p4EDB6p69epatGiRnn32WTVp0kSDBg2SJFWtWtVuvR49eigoKEj/+te/tGbNGr311lsqXbq0PvzwQz3yyCN69913FR0d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xx+bQXngwIGqXr26GjVqpHLlymU7Ow5cj81gAiNQaDz66KPy8/PTokWLHN3KbZGRkaGgoCB1795db775pqPbAZBPHnroIdWrV4+v48ZdhekcgINcvnxZc+fOVWhoqJydnfXpp5/q66+/trvmc1F3/PhxbdiwQa1bt1Zqaqpmz56tY8eOqXfv3o5uDQCAW0KIBhwkc+rF22+/rZSUFFWvXl3//e9/FRIS4ujW8o2Tk5MWLFigESNGyDAM1a5dW19//bWCgoIc3RoAALeE6RwAAACARXywEAAAALCIEA0AAABYRIgGAAAALCJEAwAAABYRogEAAACLCNEAUAQ99NBDGjp0qKPbAIC7FiEaAJBnv/32m2w2m/bu3evoVkxVqlThm/MA3HaEaABAnly9etXRLQCAwxCiAaCQu3Tpkvr166cSJUqoQoUKmjJlit14amqqRowYoXvuuUeenp5q2rSpvvnmG3N8wYIF8vHx0cqVK1WtWjW5u7srNDRUJ0+eNGt+/fVXde7cWb6+vipRooQaN26sr7/+2m4/VapU0Ztvvql+/frJy8tLgwYNUmBgoCSpfv36stlseuihhyRJAwYMUFhYmN555x35+vrKx8dHEyZMUFpamkaOHKnSpUurYsWKmj9/vt0+Tp48qe7du8vHx0elS5dW586d9dtvv5njmdt97733VKFCBZUpU0aDBw/WtWvXJP09zeX48eMaNmyYbDabbDbbrT78AJAjQjQAFHIjR47Ut99+qy+++EIbNmzQN998o927d5vjERER2r59uz777DP9+OOPevLJJ9W2bVsdOXLErLl8+bLefvttffLJJ9q6dasSEhLUs2dPczw5OVnt27fXpk2btGfPHrVt21YdO3bUiRMn7Hp57733VLduXe3Zs0djx47Vjh07JElff/21zpw5o+XLl5u1mzdv1unTpxUTE6OpU6dq3Lhx6tChg0qVKqXY2Fg9//zzeu655/T7779Lkq5du6bQ0FCVLFlS3333nbZu3aoSJUqobdu2dme9t2zZol9//VVbtmzRwoULtWDBAi1YsECStHz5clWsWFETJkzQmTNndObMmfx7IgAgKwMAUGhdvHjRcHV1NZYuXWou++uvvwwPDw9jyJAhxvHjxw1nZ2fj1KlTduu1adPGGDNmjGEYhjF//nxDkvHDDz+Y4z///LMhyYiNjb3uvmvVqmXMmjXLvB8QEGCEhYXZ1Rw7dsyQZOzZs8duef/+/Y2AgAAjPT3dXFa9enWjZcuW5v20tDTD09PT+PTTTw3DMIxFixYZ1atXNzIyMsya1NRUw8PDw1i/fr3ddtPS0syaJ5980ujRo4ddn9OmTbvucQFAfnBxcIYHANzAr7/+qqtXr6pp06bmstKlS6t69eqSpP379ys9PV3333+/3XqpqakqU6aMed/FxUWNGzc279eoUUM+Pj76+eef1aRJEyUnJysqKkpr1qzRmTNnlJaWpitXrmQ7E92oUaNc916rVi05Of3/P3j6+vqqdu3a5n1nZ2eVKVNG586dkyTt27dPR48eVcmSJe22k5KSol9//dVuu87Ozub9ChUqaP/+/bnuCwDyAyEaAIqw5ORkOTs7Ky4uzi5YSlKJEiVyvZ0RI0Zo48aNeu+993TffffJw8ND3bp1y/bhQU9Pz1xvs1ixYnb3bTZbjssyMjLMY2nYsKGio6OzbatcuXI33G7mNgCgoBCiAaAQq1q1qooVK6bY2FhVrlxZknThwgX98ssvat26terXr6/09HSdO3dOLVu2vO520tLStGvXLjVp0kSSdPjwYSUkJCgoKEiStHXrVg0YMEBdunSR9HegzfqBvutxdXWVJKWnp9/KYUqSGjRooCVLlqh8+fLy8vLK83ZcXV3zpR8AuBE+WAgAhViJEiUUHh6ukSNHavPmzTpw4IAGDBhgTpO4//771adPH/Xr10/Lly/XsWPHtGPHDk2cOFFr1qwxt1OsWDG99NJLio2NVVxcnAYMGKBmzZqZobpatWpavny59u7dq3379ql37965Ortbvnx5eXh4aN26dTp79qwSExPzfKx9+vRR2bJl1blzZ3333Xc6duyYvvnmG7388svmhw9zo0qVKoqJidGpU6f0559/5rkfALgRQjQAFHKTJ09Wy5Yt1bFjR4WEhKhFixZq2LChOT5//nz169dPr7zyiqpXr66wsDDt3LnTPHMtScWLF9fo0aPVu3dvPfjggypRooSWLFlijk+dOlWlSpVS8+bN1bFjR4WGhqpBgwY37c3FxUUzZ87Uhx9+KH9/f3Xu3DnPx1m8eHHFxMSocuXK6tq1q4KCghQeHq6UlBRLZ6YnTJig3377TVWrVrWbBgIA+clmGIbh6CYAALfPggULNHToUCUkJDi6FQC4Y3AmGgAAALCIEA0AAABYxHQOAAAAwCLORAMAAAAWEaIBAAAAiwjRAAAAgEWEaAAAAMAiQjQAAABgESEaAAAAsIgQDQAAAFhEiAYAAAAs+n/GSxRjxNxtOgAAAABJRU5ErkJggg==\n",
+                        "image/png": "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48dr4MCBGjx4sKKjo1W/fn3FxcXd1j4CVd3gwYN16dIlde7cWSNGjNCoUaOsWydcT4cOHfTRRx/pww8/VOvWrTVp0iRNmTJFQ4cOtWoWL16s0NBQxcTE6KmnntLw4cPVuHFjl/W8++67KikpUceOHTV69Ohr/khq1KiRNm7cqIKCAsXExKhjx47685//bAWnYcOGKSIiQp06ddK99957zdEzVG0Ow8UXgIuf/OQnCg4O1vvvv+/uVu6IsrIyRUZG6rnnntPUqVPd3Q5gu0cffVTt2rXj62Nw13H6D7XaxYsXtXDhQsXFxcnT01MffPCB1q9fr9TUVHe3ZpujR49q3bp1iomJUVFRkd5++21lZ2dr0KBB7m4NAGoUQhVqtfJTdW+88YYKCwsVERGhv/3tb4qNjXV3a7bx8PDQkiVLNHbsWBlj1Lp1a61fv16RkZHubg0AahRO/wEAANiAC9UBAABsQKgCAACwAaEKAADABoQqAAAAGxCqAAAAbECoAlCtPfrooxo9erS72wAAQhUA2OGbb76Rw+G45gt03alZs2bcVRy4iwhVAHCbLl++7O4WAFQBhCoA1caFCxc0ePBg1a9fXyEhIZo9e7bLeFFRkcaOHav77rtP9erVU1RUlDZt2mSNL1myRAEBAVq1apWaN28up9OpuLg4HT9+3Ko5cuSI+vXrp6CgINWvX18PP/yw1q9f77KdZs2aaerUqRo8eLD8/Pw0fPhw60u827dvL4fDoUcffVSSNHToUMXHx+vNN99UUFCQAgICNGXKFJWUlGjcuHEKDAzU/fffr8WLF7ts4/jx43ruuecUEBCgwMBA9evXT9988401Xr7eWbNmKSQkRI0aNdKIESNUXFws6cpp0aNHj+qll16Sw+GQw+G43acfwE0QqgBUG+PGjdM//vEP/f3vf9e6deu0adMm7dy50xpPSkrS1q1b9eGHH2rv3r169tln1bt3bx06dMiquXjxot544w2999572rx5s3JzczVgwABrvKCgQI8//rg2bNigXbt2qXfv3urbt6+OHTvm0susWbPUtm1b7dq1SxMnTtT27dslSevXr9epU6f0ySefWLUbN27UyZMnlZaWprfeeku//e1v9eSTT6phw4ZKT0/Xr371K73wwgv69ttvJUnFxcWKi4tTgwYN9OWXX2rz5s2qX7++evfu7XJU7IsvvtCRI0f0xRdfaOnSpVqyZImWLFkiSfrkk090//33a8qUKTp16pROnTpl3y8CwPUZAKgGzp8/b7y9vc1HH31kzfv++++Nr6+vGTVqlDl69Kjx9PQ0J06ccFmuZ8+eZsKECcYYYxYvXmwkmW3btlnjBw4cMJJMenr6DbfdqlUrM3/+fGu6adOmJj4+3qUmOzvbSDK7du1ymT9kyBDTtGlTU1paas2LiIgw3bt3t6ZLSkpMvXr1zAcffGCMMeb99983ERERpqyszKopKioyvr6+5vPPP3dZb0lJiVXz7LPPmueff96lzzlz5txwvwDYiy9UBlAtHDlyRJcvX1ZUVJQ1LzAwUBEREZKkr776SqWlpXrooYdclisqKlKjRo2saS8vLz388MPWdIsWLRQQEKADBw6oc+fOKigoUHJystasWaNTp06ppKREly5duuZIVadOnSrce6tWreTh8X8nBoKCgtS6dWtr2tPTU40aNdKZM2ckSXv27NHhw4fVoEEDl/UUFhbqyJEjLuv19PS0pkNCQvTVV19VuC8A9iJUAagRCgoK5OnpqczMTJegIUn169ev8HrGjh2r1NRUzZo1Sw8++KB8fX31zDPPXHMxer169Sq8zjp16rhMOxyO684rKyuz9qVjx45atmzZNeu69957f3C95esAcPcRqgBUCw888IDq1Kmj9PR0NWnSRJJ07tw5ff3114qJiVH79u1VWlqqM2fOqHv37jdcT0lJiXbs2KHOnTtLkrKyspSbm6vIyEhJ0ubNmzV06FD1799f0pWAc/UF4jfi7e0tSSotLb2d3ZQkdejQQStWrFDjxo3l5+dX6fV4e3vb0g+AiuFCdQDVQv369ZWYmKhx48Zp48aN2rdvn4YOHWqdVnvooYeUkJCgwYMH65NPPlF2dra2b9+u6dOna82aNdZ66tSpoxdffFHp6enKzMzU0KFD1aVLFytkNW/eXJ988ol2796tPXv2aNCgQRU6+tO4cWP5+vpq7dq1On36tPLy8iq9rwkJCbrnnnvUr18/ffnll8rOztamTZs0cuRI62L2imjWrJnS0tJ04sQJfffdd5XuB0DFEKoAVBszZ85U9+7d1bdvX8XGxqpbt27q2LGjNb548WINHjxYL7/8siIiIhQfH6+MjAzryJYk1a1bV+PHj9egQYP0yCOPqH79+lqxYoU1/tZbb6lhw4bq2rWr+vbtq7i4OHXo0OGmvXl5eWnevHn605/+pNDQUPXr16/S+1m3bl2lpaWpSZMmeuqppxQZGanExEQVFhbe0pGrKVOm6JtvvtEDDzzgctoQwJ3hMMYYdzcBAHfDkiVLNHr0aOXm5rq7FQA1EEeqAAAAbECoAgAAsAGn/wAAAGzAkSoAAAAbEKoAAABsQKgCAACwAaEKAADABoQqAAAAGxCqAAAAbECoAgAAsAGhCgAAwAb/H0d+J2TIZjqsAAAAAElFTkSuQmCC\n",
                         "text/plain": [
-                            "<Figure size 800x500 with 1 Axes>"
+                            "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "dept_salary(df_missing)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 28,
             "id": "538ddd26-4b79-4251-9f40-d8a8fc57673f",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Loading executor from cache file count_high_earners_86151.py, set override = True to rerun\n"
+                        "Loading executor from cache file count_high_earners_61505.py, set override = True to rerun\n"
                     ]
                 }
             ],
             "source": [
                 "dept_100k = PandasGenie(\"how many people in each department make more than 100K?\", columns=df_missing.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 29,
             "id": "4e2e88e7-ac81-4710-8b45-cd94d3c44912",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>count</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>department</th>\n",
+                            "      <th></th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>engineering</th>\n",
+                            "      <td>20</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>product</th>\n",
+                            "      <td>24</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
                         "text/plain": [
-                            "department\n",
-                            "engineering    20\n",
-                            "product        18\n",
-                            "Name: id, dtype: int64"
+                            "             count\n",
+                            "department        \n",
+                            "engineering     20\n",
+                            "product         24"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dept_100k(df_missing)"
             ]
@@ -505,71 +547,77 @@
                 "2. `Loading executor from cache file count_high_earners_86151.py, set override = True to rerun`: this will be shown when we run the genie after its cached without setting `override=True`\n",
                 "\n",
                 "all cached py files for the starter notebook can be found [here](https://github.com/thismlguy/code-genie/tree/main/docs/notebooks/_cache_starter)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 26,
             "id": "b09e7679-9cc2-4b21-9d00-726a6035f570",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "import pandas as pd\n",
                         "import random\n",
                         "\n",
-                        "def generate_employee_df():\n",
-                        "    employee_data = {\"id\": [random.randint(1000,9999) for i in range(100)],\n",
-                        "                     \"name\": [\"Employee_\" + str(i) for i in range(1,101)],\n",
-                        "                     \"salary\": [random.randint(40000,150000) for i in range(100)],\n",
-                        "                     \"department\": [\"engineering\" if i<50 else \"product\" for i in range(100)]}\n",
+                        "def generate_employee_data():\n",
+                        "    employee_ids = []\n",
+                        "    employee_names = []\n",
+                        "    salaries = []\n",
+                        "    departments = []\n",
+                        "\n",
+                        "    departments_list = ['engineering', 'product']\n",
+                        "    \n",
+                        "    for i in range(100):\n",
+                        "        employee_ids.append(random.randint(100, 999))\n",
+                        "        employee_names.append('Employee_' + str(i))\n",
+                        "        salaries.append(random.randint(50000, 150000))\n",
+                        "        departments.append(random.choice(departments_list))\n",
+                        "\n",
+                        "    df = pd.DataFrame({\n",
+                        "        'id': employee_ids,\n",
+                        "        'name': employee_names,\n",
+                        "        'salary': salaries,\n",
+                        "        'department': departments\n",
+                        "    })\n",
                         "    \n",
-                        "    employee_df = pd.DataFrame(employee_data)\n",
-                        "    return employee_df\n",
+                        "    return df\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "# the code can be inspected using `code` property:\n",
                 "print(data_gen.code)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 27,
             "id": "410d75a1-c890-47e2-b09e-0a9c7654c231",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'generate_employee_df_41317.py'"
+                            "'generate_employee_data_58297.py'"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# the filename in which a genie is stored can be found using the `filename` property:\n",
                 "data_gen.filename"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "7a6435aa-4299-428a-b7df-842a31841e22",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "code-genie",
             "language": "python",
             "name": "code-genie"
```

### Comparing `code_genie-0.2.0/docs/notebooks/_cache_starter/_meta.json` & `code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/_meta.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555555%*

 * *Differences: {"'0c8c445e7d3df2205c953e4637cf27fdbff7ef5d0aa4fd4bb344da12960bcafe7e9e7e683588921480283373a6b6a0f0393ac51a3bf8b4bef3f0d10bc9840784'": "{'filename': "*

 * *                                                                                                                                       "'make_salaries_missing_39233.py'}",*

 * * "'295335dcc576497fb8dc10ec8004be1d84e7155617ecca9355d64dffb38d92d16d315c615c21b17ef77d95a49977a2f35ea08021ffa0072b05c4b6128e621245'": "{'filename': "*

 * *                                       […]*

```diff
@@ -1,27 +1,27 @@
 {
     "0c8c445e7d3df2205c953e4637cf27fdbff7ef5d0aa4fd4bb344da12960bcafe7e9e7e683588921480283373a6b6a0f0393ac51a3bf8b4bef3f0d10bc9840784": {
-        "filename": "make_salaries_missing_76197.py",
+        "filename": "make_salaries_missing_39233.py",
         "fn_name": "make_salaries_missing"
     },
     "295335dcc576497fb8dc10ec8004be1d84e7155617ecca9355d64dffb38d92d16d315c615c21b17ef77d95a49977a2f35ea08021ffa0072b05c4b6128e621245": {
-        "filename": "plot_salary_distribution_54098.py",
+        "filename": "plot_salary_distribution_49433.py",
         "fn_name": "plot_salary_distribution"
     },
     "308ea4408bf138110b1cf381763c19a747c3420981ddcdef83acbe7fd53a3aefc06f942dfe35daea93497bfefe1158a2c7d20776c3dd6e16213bd12e6f967f9a": {
-        "filename": "generate_employee_df_41317.py",
-        "fn_name": "generate_employee_df"
+        "filename": "generate_employee_data_58297.py",
+        "fn_name": "generate_employee_data"
     },
     "9c203807fc44999a07234202a84918cd67d699dff7f67f2a21f7d8b4a7faf855529c82b111890a97b248a7a72a12f9eea87d5ec1f315817bf0ed70ad0d1671e9": {
-        "filename": "count_missing_35951.py",
-        "fn_name": "count_missing"
+        "filename": "count_missing_values_28317.py",
+        "fn_name": "count_missing_values"
     },
     "afa88f466ce92056cb4e0b0dd9f15f72ba2a93cc23baa4c3e67238704be2cb9b228245f38ffce0cadd84228453d0c48cd55a7b898aef9ba60e01a9439254b4ac": {
-        "filename": "make_boxplots_25996.py",
-        "fn_name": "make_boxplots"
+        "filename": "boxplots_of_salary_by_department_12125.py",
+        "fn_name": "boxplots_of_salary_by_department"
     },
     "c4e1f86f22374f296b616a15dc7bfdc76e45d7c2bfc977926e4adc6cdf48a7a501b44188743929c4f0d70c825395cbbdd409ee4a3fc08cc1357531003486cc46": {
-        "code": "import pandas as pd\nimport numpy as np\n\ndef count_high_earners(df):\n    high_earners = df[df['salary'] > 100000].groupby('department')['id'].count()\n    return high_earners\n",
-        "filename": "count_high_earners_86151.py",
+        "code": "import pandas as pd\n\ndef count_high_earners(df):\n    high_earners = df[df['salary'] > 100000].groupby('department').count()[['id']]\n    high_earners.columns = ['count']\n    return high_earners\n",
+        "filename": "count_high_earners_61505.py",
         "fn_name": "count_high_earners"
     }
 }
```

### Comparing `code_genie-0.2.0/docs/requirements.txt` & `code_genie-0.2.1.dev0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/pyproject.toml` & `code_genie-0.2.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/tests/test_cache.py` & `code_genie-0.2.1.dev0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/tests/test_genie.py` & `code_genie-0.2.1.dev0/tests/test_genie.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/tox.ini` & `code_genie-0.2.1.dev0/tox.ini`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.0/PKG-INFO` & `code_genie-0.2.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_genie
-Version: 0.2.0
+Version: 0.2.1.dev0
 Summary: Copilot to supercharge your notebooks
 Keywords: copilot,jupyter
 Author-email: Aarshay Jain <aarshay.jain@columbia.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: notebook
 
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.2.0
+Latest version: 0.2.1-dev0
 
 ## Documentation
 
 - [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
 - [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
 - [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
```

