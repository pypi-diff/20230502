# Comparing `tmp/ghanashops-scraper-0.0.2.tar.gz` & `tmp/ghanashops-scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-0.0.2.tar", last modified: Tue May  2 21:40:14 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-0.0.3.tar", last modified: Tue May  2 21:50:34 2023, max compression
```

## Comparing `ghanashops-scraper-0.0.2.tar` & `ghanashops-scraper-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2115 2023-05-02 21:35:19.000000 ghanashops-scraper-0.0.2/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-0.0.2/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-0.0.2/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.2/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 21:39:34.000000 ghanashops-scraper-0.0.2/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:40:14.000000 ghanashops-scraper-0.0.2/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-0.0.2/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4768 2023-05-02 21:06:19.000000 ghanashops-scraper-0.0.2/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.2/tonaton/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2115 2023-05-02 21:46:49.000000 ghanashops-scraper-0.0.3/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-0.0.3/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-0.0.3/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.3/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 21:50:31.000000 ghanashops-scraper-0.0.3/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 21:50:34.000000 ghanashops-scraper-0.0.3/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-0.0.3/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4762 2023-05-02 21:50:25.000000 ghanashops-scraper-0.0.3/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.0.3/tonaton/utils.py
```

### Comparing `ghanashops-scraper-0.0.2/PKG-INFO` & `ghanashops-scraper-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to scrape data from Ghana online shops
 Home-page: https://github.com/donwany/ghanashops-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -18,15 +18,15 @@
         
         ### How to install
         ```shell
         pip install ghanashops-scraper
         ```
         
         ### Example Google Colab Notebook
-           Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing)
+           Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing)
         
         ### Outputs
           - All outputs will be saved in a `.csv` file. Other file formats not yet supported.
           - Format: 
             - ["product_description", "price", "location", "photo", "page_url"]
             - ![tv.png](tv.png)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.2 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.3 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
 python package to scrape data from [Tonaton](https://www.tonaton.com),
 [JumiaGH](https://www.jumia.com.gh). Affiliated to [Bank of Ghana Fx Rates]
 (https://pypi.org/project/bank-of-ghana-fx-rates/) [GhanaNews-Scraper](https://
 pypi.org/project/ghananews-scraper/). ### How to install ```shell pip install
 ghanashops-scraper ``` ### Example Google Colab Notebook Click Here: [![Google
 Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
-1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing) ### Outputs - All outputs will
+15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing) ### Outputs - All outputs will
 be saved in a `.csv` file. Other file formats not yet supported. - Format: -
 ["product_description", "price", "location", "photo", "page_url"] - ![tv.png]
 (tv.png) ### Usage + Scrape shop data from [Tonaton](https://tonaton.com) +
 Example of search queries: cars, laptops, phones, vehicles, rent, houses,
 tablets, shoes, refrigerator ```python import asyncio from tonaton.scraper
 import Tonaton search_query = "iphones" tonaton = Tonaton(query=search_query)
 asyncio.run(tonaton.download()) ``` ### Limiting the number of pages to scrape.
```

### Comparing `ghanashops-scraper-0.0.2/README.md` & `ghanashops-scraper-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ### How to install
 ```shell
 pip install ghanashops-scraper
 ```
 
 ### Example Google Colab Notebook
-   Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing)
+   Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing)
 
 ### Outputs
   - All outputs will be saved in a `.csv` file. Other file formats not yet supported.
   - Format: 
     - ["product_description", "price", "location", "photo", "page_url"]
     - ![tv.png](tv.png)
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 unofficial python package to scrape data from [Tonaton](https://
 www.tonaton.com), [JumiaGH](https://www.jumia.com.gh). Affiliated to [Bank of
 Ghana Fx Rates](https://pypi.org/project/bank-of-ghana-fx-rates/) [GhanaNews-
 Scraper](https://pypi.org/project/ghananews-scraper/). ### How to install
 ```shell pip install ghanashops-scraper ``` ### Example Google Colab Notebook
 Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/drive/
-1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing) ### Outputs - All outputs will
+15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing) ### Outputs - All outputs will
 be saved in a `.csv` file. Other file formats not yet supported. - Format: -
 ["product_description", "price", "location", "photo", "page_url"] - ![tv.png]
 (tv.png) ### Usage + Scrape shop data from [Tonaton](https://tonaton.com) +
 Example of search queries: cars, laptops, phones, vehicles, rent, houses,
 tablets, shoes, refrigerator ```python import asyncio from tonaton.scraper
 import Tonaton search_query = "iphones" tonaton = Tonaton(query=search_query)
 asyncio.run(tonaton.download()) ``` ### Limiting the number of pages to scrape.
```

### Comparing `ghanashops-scraper-0.0.2/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-0.0.3/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to scrape data from Ghana online shops
 Home-page: https://github.com/donwany/ghanashops-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -18,15 +18,15 @@
         
         ### How to install
         ```shell
         pip install ghanashops-scraper
         ```
         
         ### Example Google Colab Notebook
-           Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing)
+           Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing)
         
         ### Outputs
           - All outputs will be saved in a `.csv` file. Other file formats not yet supported.
           - Format: 
             - ["product_description", "price", "location", "photo", "page_url"]
             - ![tv.png](tv.png)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.2 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.0.3 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
 python package to scrape data from [Tonaton](https://www.tonaton.com),
 [JumiaGH](https://www.jumia.com.gh). Affiliated to [Bank of Ghana Fx Rates]
 (https://pypi.org/project/bank-of-ghana-fx-rates/) [GhanaNews-Scraper](https://
 pypi.org/project/ghananews-scraper/). ### How to install ```shell pip install
 ghanashops-scraper ``` ### Example Google Colab Notebook Click Here: [![Google
 Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
-1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing) ### Outputs - All outputs will
+15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing) ### Outputs - All outputs will
 be saved in a `.csv` file. Other file formats not yet supported. - Format: -
 ["product_description", "price", "location", "photo", "page_url"] - ![tv.png]
 (tv.png) ### Usage + Scrape shop data from [Tonaton](https://tonaton.com) +
 Example of search queries: cars, laptops, phones, vehicles, rent, houses,
 tablets, shoes, refrigerator ```python import asyncio from tonaton.scraper
 import Tonaton search_query = "iphones" tonaton = Tonaton(query=search_query)
 asyncio.run(tonaton.download()) ``` ### Limiting the number of pages to scrape.
```

### Comparing `ghanashops-scraper-0.0.2/jumia/scraper.py` & `ghanashops-scraper-0.0.3/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.0.2/jumia/utils.py` & `ghanashops-scraper-0.0.3/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.0.2/setup.py` & `ghanashops-scraper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-0.0.2/tonaton/scraper.py` & `ghanashops-scraper-0.0.3/tonaton/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,10 +109,10 @@
             print(f"error: {err}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Scrape complete!!!")
         print("Done!")
 
 
-# if __name__ == '__main__':
-#     tonaton = Tonaton(query="laptop", starting_page=1)
-#     asyncio.run(tonaton.download())
+if __name__ == '__main__':
+    tonaton = Tonaton(query="laptop", starting_page=1)
+    asyncio.run(tonaton.download())
```

### Comparing `ghanashops-scraper-0.0.2/tonaton/utils.py` & `ghanashops-scraper-0.0.3/tonaton/utils.py`

 * *Files identical despite different names*

