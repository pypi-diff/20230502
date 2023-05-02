# Comparing `tmp/scrape-google-scholar-py-0.3.3.tar.gz` & `tmp/scrape-google-scholar-py-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrape-google-scholar-py-0.3.3.tar", last modified: Thu Apr 13 06:22:53 2023, max compression
+gzip compressed data, was "scrape-google-scholar-py-0.3.4.tar", last modified: Tue May  2 08:44:15 2023, max compression
```

## Comparing `scrape-google-scholar-py-0.3.3.tar` & `scrape-google-scholar-py-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.988462 scrape-google-scholar-py-0.3.3/
--rw-rw-rw-   0        0        0       42 2023-03-30 07:33:49.000000 scrape-google-scholar-py-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    36317 2023-04-13 06:22:53.988462 scrape-google-scholar-py-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    34997 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.958562 scrape-google-scholar-py-0.3.3/google_scholar_py/
--rw-rw-rw-   0        0        0      825 2023-04-13 06:09:47.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.980488 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/
--rw-rw-rw-   0        0        0     8787 2023-04-13 06:10:14.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/author_info_all_articles.py
--rw-rw-rw-   0        0        0     1492 2023-03-30 09:37:52.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/cite_results.py
--rw-rw-rw-   0        0        0     2468 2023-03-30 09:37:56.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
--rw-rw-rw-   0        0        0     6795 2023-04-13 06:10:48.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/organic_search.py
--rw-rw-rw-   0        0        0     8311 2023-04-13 06:11:27.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/profiles_results.py
--rw-rw-rw-   0        0        0     5860 2023-04-13 06:17:03.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_mandates_metrics.py
--rw-rw-rw-   0        0        0     6930 2023-04-13 06:18:17.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_article_citations.py
--rw-rw-rw-   0        0        0     6062 2023-04-13 06:21:42.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.984478 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/
--rw-rw-rw-   0        0        0     5098 2023-03-30 09:37:03.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/author_results.py
--rw-rw-rw-   0        0        0     3533 2023-03-30 08:25:43.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_cite_results.py
--rw-rw-rw-   0        0        0     3692 2023-03-30 09:37:07.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_results.py
--rw-rw-rw-   0        0        0     3248 2023-03-30 09:37:08.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/profile_results.py
--rw-rw-rw-   0        0        0      127 2023-03-30 06:54:12.000000 scrape-google-scholar-py-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0     1606 2023-03-30 10:09:31.000000 scrape-google-scholar-py-0.3.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.987464 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/
--rw-rw-rw-   0        0        0    36317 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:22:53.988462 scrape-google-scholar-py-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-04-13 06:18:08.000000 scrape-google-scholar-py-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:44:15.054120 scrape-google-scholar-py-0.3.4/
+-rw-rw-rw-   0        0        0     1095 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       42 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    37176 2023-05-02 08:44:15.054120 scrape-google-scholar-py-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    35833 2023-05-02 08:40:25.000000 scrape-google-scholar-py-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 08:44:15.030112 scrape-google-scholar-py-0.3.4/google_scholar_py/
+-rw-rw-rw-   0        0        0      925 2023-05-02 08:40:25.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:44:15.041112 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/
+-rw-rw-rw-   0        0        0     8787 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/author_info_all_articles.py
+-rw-rw-rw-   0        0        0     1492 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/cite_results.py
+-rw-rw-rw-   0        0        0     2468 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
+-rw-rw-rw-   0        0        0     6795 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/organic_search.py
+-rw-rw-rw-   0        0        0     8311 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/profiles_results.py
+-rw-rw-rw-   0        0        0     5860 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_mandates_metrics.py
+-rw-rw-rw-   0        0        0     6889 2023-05-02 08:40:25.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_publications_article.py
+-rw-rw-rw-   0        0        0     6538 2023-05-02 08:40:25.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_publications_article_citation.py
+-rw-rw-rw-   0        0        0     6062 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_publications_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:44:15.047111 scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/
+-rw-rw-rw-   0        0        0     5098 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/author_results.py
+-rw-rw-rw-   0        0        0     3533 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/organic_cite_results.py
+-rw-rw-rw-   0        0        0     3692 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/organic_results.py
+-rw-rw-rw-   0        0        0     3248 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/profile_results.py
+-rw-rw-rw-   0        0        0      127 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1606 2023-05-02 07:29:49.000000 scrape-google-scholar-py-0.3.4/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 08:44:15.053113 scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/
+-rw-rw-rw-   0        0        0    37176 2023-05-02 08:44:14.000000 scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1099 2023-05-02 08:44:15.000000 scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 08:44:14.000000 scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-05-02 08:44:14.000000 scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:44:14.000000 scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 08:44:15.055112 scrape-google-scholar-py-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-05-02 08:40:25.000000 scrape-google-scholar-py-0.3.4/setup.py
```

### Comparing `scrape-google-scholar-py-0.3.3/PKG-INFO` & `scrape-google-scholar-py-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-google-scholar-py
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar
 Author: Dmitiry Zub
 Author-email: dimitryzub@gmail.com
 Maintainer: Dmitiry Zub
 Maintainer-email: dimitryzub@gmail.com
 License: MIT
@@ -20,28 +20,44 @@
 Classifier: Topic :: Internet
 Classifier: Natural Language :: English
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
-<p>Sponsor of the project:</p>
+<p>Special thanks to:</p>
 <div>
-   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="140" alt="SerpApi">
+   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="60" alt="SerpApi">
 </div>
 <a href="https://serpapi.com">
 	<b>API to get search engine results with ease.</b>
 </a>
 </div>
 
-_____
+____
+
+<h3 align="center">
+  Scrape data from all Google Scholar pages from a single Python module.
+</h3>
+
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/78694043/231677340-8980c44d-389a-497d-b021-b1d4ab846a77.svg" width="600" alt="scrape-google-scholar-py-logo">
+</div>
+
+
+<div align="center">
+
+  <a href="https://pepy.tech/project/scrape-google-scholar-py">![Downloads](https://static.pepy.tech/badge/scrape-google-scholar-py/month)</a>
+  <a href="">![licence](https://img.shields.io/github/license/dimitryzub/scrape-google-scholar-py?color=blue)</a>
+
+</div>
 
-This repository is meant to extract data from all Google Scholar pages.
 
 <details>
 <summary>🧐 Why two backends?</summary>
 
 1. If you don't want to pay for API. However, I'm not 100% sure if [`selenium-stealth`](https://pypi.org/project/selenium-stealth/) could handle all CAPTCHAs (although it handles CAPTCHA by Cloudflare) and similar blocks.
 2. If you know about SerpApi but don't want to figure out pagination.
 
@@ -58,15 +74,15 @@
 <summary>🧩 Custom backend supports</summary>
 
 1. [Organic results](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=blizzard&btnG=&oq=blizz) (with pagination).
 2. [Profile results](https://scholar.google.com/citations?view_op=search_authors&mauthors=blizzard&hl=en&oi=drw) (with pagination).
 3. [Author + author articles](https://scholar.google.com/citations?user=6IQ8pQwAAAAJ&hl=en&oi=sra) (with pagination), everything except "cited by" graph.
 4. [Public access mandates metrics](https://scholar.google.com/citations?view_op=mandates_leaderboard&hl=en). Yes, you can download CSV with one click, however, it doesn't contain a funder link. Script here has it and saves to CSV/JSON.
 5. [Top publications metrics](https://scholar.google.com/citations?view_op=top_venues&hl=en). Categories is also supported (as function argument). Saves to CSV/JSON. Sub-categories are not yet supported.
-6. soon: [journal articles](https://github.com/dimitryzub/scrape-google-scholar/issues/2).
+6. [Journal articles](https://github.com/dimitryzub/scrape-google-scholar/issues/2) (with pagination).
 
 You can use [`scholary`](https://github.com/scholarly-python-package/scholarly) to parse the data instead. However, it only extracts first 3 points below.  
 
   <details>
   <summary>Things custom backend doesn't support yet</summary>
 
   1. Organic results filters (case law, sorting, period ranges). You can add those URL parameters yourself ([if installing from source](https://github.com/dimitryzub/scrape-google-scholar-py#installing)) easily to the `google_scholar_py/custom_backend/organic_search.py` file (line [`147`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/organic_search.py#L147) or [`136`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/organic_search.py#L160)), where `driver.get()` is being called.
@@ -82,43 +98,53 @@
 
 - [Google Scholar Organic](https://serpapi.com/google-scholar-organic-results)
 - [Google Scholar Profiles](https://serpapi.com/google-scholar-profilesapi)
 - [Google Scholar Author](https://serpapi.com/google-scholar-author-api)
 - [Google Scholar Cite](https://serpapi.com/google-scholar-cite-api)
 </details>
 
-
 <details>
 <summary>🏗 Custom backend depends on</summary>
 
-- [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to bypass CAPTCHAs.
+- [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to bypass CAPTCHAs and render some HTML (like cite results from organic result).
 - [`selectolax`](https://github.com/rushter/selectolax) - to parse HTML fast. Its the fastest Python parser wrapped around [`lexbor`](https://github.com/lexbor/lexbor) (parser in pure C).
 - [`pandas`](https://pandas.pydata.org/) - to save extracted data to CSV or JSON, or if you want to analyze the data right away. Save options is used in organic results and top publications, public access mandates pages for now.
-- [`google-search-results`](https://github.com/serpapi/google-search-results-python) - Python wrapper for SerpApi backend.
-- [other packages in the `requirements.txt`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/8de484e0eec71478e330303fb405a22e0178f068/requirements.txt).
 
 All scripts are using headless [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) to bypass CAPTCHA that appears on Google Scholar, so you need to have a `chromedriver`. If you're on Linux you may need to do additional troubleshooting if `chromedriver` won't run properly.
 </details>
 
 ## 📥Installing
 
 Install via `pip`:
 
 ```bash
 $ pip install scrape-google-scholar-py
 ```
 
-Install for development from source:
+Install from source:
 
 ```bash
 $ git clone https://github.com/dimitryzub/scrape-google-scholar-py.git
 $ cd scrape-google-scholar-py
+$ python -m venv env && source env/Scripts/activate # windows activation
 $ pip install -r requirements.txt
 ```
 
+### Possible errors that you might encounter
+
+<details>
+<summary>LINUX USERS: If it throws "Web-driver exits unexpectedly" error</summary>
+
+  Try installing extra dependencies to run `chromedriver`:	
+  ```bash
+  $ apt-get install -y libglib2.0-0 libnss3 libgconf-2-4 libfontconfig1
+  ```
+
+  See resolved issue: [[Linux] Web-driver exits unexpectedly using CustomGoogleScholarOrganic() #7](https://github.com/dimitryzub/scrape-google-scholar-py/issues/7)	
+</details>
 
 <details>
 <summary>If it throws an error with `selenium-stealth`</summary>
 
   ```bash
   error: The 'selenium' distribution was not found and is required by selenium-stealth
   ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.4 Summary:
 Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar Author: Dmitiry
 Zub Author-email: dimitryzub@gmail.com Maintainer: Dmitiry Zub Maintainer-
 email: dimitryzub@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/dimitryzub/scrape-google-scholar#example-usage-custom-backend
 Project-URL: Source, https://github.com/dimitryzub/scrape-google-scholar
 Project-URL: Tracker, https://github.com/dimitryzub/scrape-google-scholar/
@@ -11,20 +11,26 @@
 scraping,research,lexbor,selectolax,selenium,selenium-stealth,pandas
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet Classifier: Natural Language :: English
 Classifier: Topic :: Utilities Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-                            Sponsor of the project:
+Description-Content-Type: text/markdown License-File: LICENSE
+                              Special thanks to:
                                    [SerpApi]
                   API_to_get_search_engine_results_with_ease.
-_____ This repository is meant to extract data from all Google Scholar pages.
-ð§ Why two backends? 1. If you don't want to pay for API. However, I'm not
+____
+  **** Scrape data from all Google Scholar pages from a single Python module.
+                                     ****
+                        [scrape-google-scholar-py-logo]
+ ![Downloads](https://static.pepy.tech/badge/scrape-google-scholar-py/month) !
+   [licence](https://img.shields.io/github/license/dimitryzub/scrape-google-
+                            scholar-py?color=blue)
+ ð§ Why two backends? 1. If you don't want to pay for API. However, I'm not
 100% sure if [`selenium-stealth`](https://pypi.org/project/selenium-stealth/
 ) could handle all CAPTCHAs (although it handles CAPTCHA by Cloudflare) and
 similar blocks. 2. If you know about SerpApi but don't want to figure out
 pagination. SerpApi backend is more reliable because of: - dedicated team of
 maintainers - pool of proxies - CAPTCHA solvers - legal part of scraping and
 more.   ð§© Custom backend supports 1. [Organic results](https://
 scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=blizzard&btnG=&oq=blizz) (with
@@ -34,21 +40,21 @@
 citations?user=6IQ8pQwAAAAJ&hl=en&oi=sra) (with pagination), everything except
 "cited by" graph. 4. [Public access mandates metrics](https://
 scholar.google.com/citations?view_op=mandates_leaderboard&hl=en). Yes, you can
 download CSV with one click, however, it doesn't contain a funder link. Script
 here has it and saves to CSV/JSON. 5. [Top publications metrics](https://
 scholar.google.com/citations?view_op=top_venues&hl=en). Categories is also
 supported (as function argument). Saves to CSV/JSON. Sub-categories are not yet
-supported. 6. soon: [journal articles](https://github.com/dimitryzub/scrape-
-google-scholar/issues/2). You can use [`scholary`](https://github.com/
-scholarly-python-package/scholarly) to parse the data instead. However, it only
-extracts first 3 points below.  Things custom backend doesn't support yet 1.
-Organic results filters (case law, sorting, period ranges). You can add those
-URL parameters yourself ([if installing from source](https://github.com/
-dimitryzub/scrape-google-scholar-py#installing)) easily to the
+supported. 6. [Journal articles](https://github.com/dimitryzub/scrape-google-
+scholar/issues/2) (with pagination). You can use [`scholary`](https://
+github.com/scholarly-python-package/scholarly) to parse the data instead.
+However, it only extracts first 3 points below.  Things custom backend doesn't
+support yet 1. Organic results filters (case law, sorting, period ranges). You
+can add those URL parameters yourself ([if installing from source](https://
+github.com/dimitryzub/scrape-google-scholar-py#installing)) easily to the
 `google_scholar_py/custom_backend/organic_search.py` file (line [`147`](https:/
 /github.com/dimitryzub/scrape-google-scholar-py/blob/
 a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/
 organic_search.py#L147) or [`136`](https://github.com/dimitryzub/scrape-google-
 scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/
 custom_backend/organic_search.py#L160)), where `driver.get()` is being called.
 2. Author page -> cited by graph. 3. Extracting [journal articles page](https:/
@@ -62,43 +68,46 @@
 jhjzd72UJ%3Ascholar.google.com%2F%26output%3Dcite%26scirp%3D7%26hl%3Den) page
 extraction.    ð® SerpApi backend supports - [Google Scholar Organic](https:/
 /serpapi.com/google-scholar-organic-results) - [Google Scholar Profiles](https:
 //serpapi.com/google-scholar-profilesapi) - [Google Scholar Author](https://
 serpapi.com/google-scholar-author-api) - [Google Scholar Cite](https://
 serpapi.com/google-scholar-cite-api)   ð Custom backend depends on -
 [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to
-bypass CAPTCHAs. - [`selectolax`](https://github.com/rushter/selectolax) - to
-parse HTML fast. Its the fastest Python parser wrapped around [`lexbor`](https:
-//github.com/lexbor/lexbor) (parser in pure C). - [`pandas`](https://
-pandas.pydata.org/) - to save extracted data to CSV or JSON, or if you want to
-analyze the data right away. Save options is used in organic results and top
-publications, public access mandates pages for now. - [`google-search-results`]
-(https://github.com/serpapi/google-search-results-python) - Python wrapper for
-SerpApi backend. - [other packages in the `requirements.txt`](https://
-github.com/dimitryzub/scrape-google-scholar-py/blob/
-8de484e0eec71478e330303fb405a22e0178f068/requirements.txt). All scripts are
-using headless [`selenium-stealth`](https://github.com/diprajpatra/selenium-
-stealth) to bypass CAPTCHA that appears on Google Scholar, so you need to have
-a `chromedriver`. If you're on Linux you may need to do additional
-troubleshooting if `chromedriver` won't run properly.  ## ð¥Installing
-Install via `pip`: ```bash $ pip install scrape-google-scholar-py ``` Install
-for development from source: ```bash $ git clone https://github.com/dimitryzub/
-scrape-google-scholar-py.git $ cd scrape-google-scholar-py $ pip install -
-r requirements.txt ```  If it throws an error with `selenium-stealth` ```bash
-error: The 'selenium' distribution was not found and is required by selenium-
-stealth ``` Use: ```bash $ pip install selenium-stealth ```  ## ðExample
-usage custom backend ```python from google_scholar_py import
-CustomGoogleScholarProfiles import json parser = CustomGoogleScholarProfiles()
-data = parser.scrape_google_scholar_profiles( query='blizzard',
-pagination=False, save_to_csv=False, save_to_json=False ) print(json.dumps
-(data, indent=2)) ```  Google Scholar search operators could also be used
-```lang-none label:computer_vision "Michigan State University"|"U.Michigan" ```
-This query will search all profiles from 2 universities based on "computer
-vision" query.   JSON output ```json [ { "name": "Adam Lobel", "link": "https:/
-/scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
+bypass CAPTCHAs and render some HTML (like cite results from organic result). -
+[`selectolax`](https://github.com/rushter/selectolax) - to parse HTML fast. Its
+the fastest Python parser wrapped around [`lexbor`](https://github.com/lexbor/
+lexbor) (parser in pure C). - [`pandas`](https://pandas.pydata.org/) - to save
+extracted data to CSV or JSON, or if you want to analyze the data right away.
+Save options is used in organic results and top publications, public access
+mandates pages for now. All scripts are using headless [`selenium-stealth`]
+(https://github.com/diprajpatra/selenium-stealth) to bypass CAPTCHA that
+appears on Google Scholar, so you need to have a `chromedriver`. If you're on
+Linux you may need to do additional troubleshooting if `chromedriver` won't run
+properly.  ## ð¥Installing Install via `pip`: ```bash $ pip install scrape-
+google-scholar-py ``` Install from source: ```bash $ git clone https://
+github.com/dimitryzub/scrape-google-scholar-py.git $ cd scrape-google-scholar-
+py $ python -m venv env && source env/Scripts/activate # windows activation $
+pip install -r requirements.txt ``` ### Possible errors that you might
+encounter  LINUX USERS: If it throws "Web-driver exits unexpectedly" error Try
+installing extra dependencies to run `chromedriver`: ```bash $ apt-get install
+-y libglib2.0-0 libnss3 libgconf-2-4 libfontconfig1 ``` See resolved issue: [
+[Linux] Web-driver exits unexpectedly using CustomGoogleScholarOrganic() #7]
+(https://github.com/dimitryzub/scrape-google-scholar-py/issues/7)   If it
+throws an error with `selenium-stealth` ```bash error: The 'selenium'
+distribution was not found and is required by selenium-stealth ``` Use: ```bash
+$ pip install selenium-stealth ```  ## ðExample usage custom backend
+```python from google_scholar_py import CustomGoogleScholarProfiles import json
+parser = CustomGoogleScholarProfiles() data =
+parser.scrape_google_scholar_profiles( query='blizzard', pagination=False,
+save_to_csv=False, save_to_json=False ) print(json.dumps(data, indent=2)) ```
+Google Scholar search operators could also be used ```lang-none label:
+computer_vision "Michigan State University"|"U.Michigan" ``` This query will
+search all profiles from 2 universities based on "computer vision" query.
+JSON output ```json [ { "name": "Adam Lobel", "link": "https://
+scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
 "Blizzard Entertainment", "interests": [ "Gaming", "Emotion regulation" ],
 "email": "Verified email at AdamLobel.com", "cited_by_count": 3593 }, { "name":
 "Daniel Blizzard", "link": "https://scholar.google.com/
 citations?hl=en&user=dk4LWEgAAAAJ", "affiliations": "", "interests": null,
 "email": null, "cited_by_count": 1041 }, { "name": "Shuo Chen", "link": "https:
 //scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ", "affiliations":
 "Senior Data Scientist, Blizzard Entertainment", "interests": [ "Machine
```

### Comparing `scrape-google-scholar-py-0.3.3/README.md` & `scrape-google-scholar-py-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 <div align="center">
-<p>Sponsor of the project:</p>
+<p>Special thanks to:</p>
 <div>
-   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="140" alt="SerpApi">
+   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="60" alt="SerpApi">
 </div>
 <a href="https://serpapi.com">
 	<b>API to get search engine results with ease.</b>
 </a>
 </div>
 
-_____
+____
+
+<h3 align="center">
+  Scrape data from all Google Scholar pages from a single Python module.
+</h3>
+
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/78694043/231677340-8980c44d-389a-497d-b021-b1d4ab846a77.svg" width="600" alt="scrape-google-scholar-py-logo">
+</div>
+
+
+<div align="center">
+
+  <a href="https://pepy.tech/project/scrape-google-scholar-py">![Downloads](https://static.pepy.tech/badge/scrape-google-scholar-py/month)</a>
+  <a href="">![licence](https://img.shields.io/github/license/dimitryzub/scrape-google-scholar-py?color=blue)</a>
+
+</div>
 
-This repository is meant to extract data from all Google Scholar pages.
 
 <details>
 <summary>🧐 Why two backends?</summary>
 
 1. If you don't want to pay for API. However, I'm not 100% sure if [`selenium-stealth`](https://pypi.org/project/selenium-stealth/) could handle all CAPTCHAs (although it handles CAPTCHA by Cloudflare) and similar blocks.
 2. If you know about SerpApi but don't want to figure out pagination.
 
@@ -31,15 +46,15 @@
 <summary>🧩 Custom backend supports</summary>
 
 1. [Organic results](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=blizzard&btnG=&oq=blizz) (with pagination).
 2. [Profile results](https://scholar.google.com/citations?view_op=search_authors&mauthors=blizzard&hl=en&oi=drw) (with pagination).
 3. [Author + author articles](https://scholar.google.com/citations?user=6IQ8pQwAAAAJ&hl=en&oi=sra) (with pagination), everything except "cited by" graph.
 4. [Public access mandates metrics](https://scholar.google.com/citations?view_op=mandates_leaderboard&hl=en). Yes, you can download CSV with one click, however, it doesn't contain a funder link. Script here has it and saves to CSV/JSON.
 5. [Top publications metrics](https://scholar.google.com/citations?view_op=top_venues&hl=en). Categories is also supported (as function argument). Saves to CSV/JSON. Sub-categories are not yet supported.
-6. soon: [journal articles](https://github.com/dimitryzub/scrape-google-scholar/issues/2).
+6. [Journal articles](https://github.com/dimitryzub/scrape-google-scholar/issues/2) (with pagination).
 
 You can use [`scholary`](https://github.com/scholarly-python-package/scholarly) to parse the data instead. However, it only extracts first 3 points below.  
 
   <details>
   <summary>Things custom backend doesn't support yet</summary>
 
   1. Organic results filters (case law, sorting, period ranges). You can add those URL parameters yourself ([if installing from source](https://github.com/dimitryzub/scrape-google-scholar-py#installing)) easily to the `google_scholar_py/custom_backend/organic_search.py` file (line [`147`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/organic_search.py#L147) or [`136`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/organic_search.py#L160)), where `driver.get()` is being called.
@@ -55,43 +70,53 @@
 
 - [Google Scholar Organic](https://serpapi.com/google-scholar-organic-results)
 - [Google Scholar Profiles](https://serpapi.com/google-scholar-profilesapi)
 - [Google Scholar Author](https://serpapi.com/google-scholar-author-api)
 - [Google Scholar Cite](https://serpapi.com/google-scholar-cite-api)
 </details>
 
-
 <details>
 <summary>🏗 Custom backend depends on</summary>
 
-- [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to bypass CAPTCHAs.
+- [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to bypass CAPTCHAs and render some HTML (like cite results from organic result).
 - [`selectolax`](https://github.com/rushter/selectolax) - to parse HTML fast. Its the fastest Python parser wrapped around [`lexbor`](https://github.com/lexbor/lexbor) (parser in pure C).
 - [`pandas`](https://pandas.pydata.org/) - to save extracted data to CSV or JSON, or if you want to analyze the data right away. Save options is used in organic results and top publications, public access mandates pages for now.
-- [`google-search-results`](https://github.com/serpapi/google-search-results-python) - Python wrapper for SerpApi backend.
-- [other packages in the `requirements.txt`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/8de484e0eec71478e330303fb405a22e0178f068/requirements.txt).
 
 All scripts are using headless [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) to bypass CAPTCHA that appears on Google Scholar, so you need to have a `chromedriver`. If you're on Linux you may need to do additional troubleshooting if `chromedriver` won't run properly.
 </details>
 
 ## 📥Installing
 
 Install via `pip`:
 
 ```bash
 $ pip install scrape-google-scholar-py
 ```
 
-Install for development from source:
+Install from source:
 
 ```bash
 $ git clone https://github.com/dimitryzub/scrape-google-scholar-py.git
 $ cd scrape-google-scholar-py
+$ python -m venv env && source env/Scripts/activate # windows activation
 $ pip install -r requirements.txt
 ```
 
+### Possible errors that you might encounter
+
+<details>
+<summary>LINUX USERS: If it throws "Web-driver exits unexpectedly" error</summary>
+
+  Try installing extra dependencies to run `chromedriver`:	
+  ```bash
+  $ apt-get install -y libglib2.0-0 libnss3 libgconf-2-4 libfontconfig1
+  ```
+
+  See resolved issue: [[Linux] Web-driver exits unexpectedly using CustomGoogleScholarOrganic() #7](https://github.com/dimitryzub/scrape-google-scholar-py/issues/7)	
+</details>
 
 <details>
 <summary>If it throws an error with `selenium-stealth`</summary>
 
   ```bash
   error: The 'selenium' distribution was not found and is required by selenium-stealth
   ```
```

#### html2text {}

```diff
@@ -1,12 +1,18 @@
-                            Sponsor of the project:
+                              Special thanks to:
                                    [SerpApi]
                   API_to_get_search_engine_results_with_ease.
-_____ This repository is meant to extract data from all Google Scholar pages.
-ð§ Why two backends? 1. If you don't want to pay for API. However, I'm not
+____
+  **** Scrape data from all Google Scholar pages from a single Python module.
+                                     ****
+                        [scrape-google-scholar-py-logo]
+ ![Downloads](https://static.pepy.tech/badge/scrape-google-scholar-py/month) !
+   [licence](https://img.shields.io/github/license/dimitryzub/scrape-google-
+                            scholar-py?color=blue)
+ ð§ Why two backends? 1. If you don't want to pay for API. However, I'm not
 100% sure if [`selenium-stealth`](https://pypi.org/project/selenium-stealth/
 ) could handle all CAPTCHAs (although it handles CAPTCHA by Cloudflare) and
 similar blocks. 2. If you know about SerpApi but don't want to figure out
 pagination. SerpApi backend is more reliable because of: - dedicated team of
 maintainers - pool of proxies - CAPTCHA solvers - legal part of scraping and
 more.   ð§© Custom backend supports 1. [Organic results](https://
 scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=blizzard&btnG=&oq=blizz) (with
@@ -16,21 +22,21 @@
 citations?user=6IQ8pQwAAAAJ&hl=en&oi=sra) (with pagination), everything except
 "cited by" graph. 4. [Public access mandates metrics](https://
 scholar.google.com/citations?view_op=mandates_leaderboard&hl=en). Yes, you can
 download CSV with one click, however, it doesn't contain a funder link. Script
 here has it and saves to CSV/JSON. 5. [Top publications metrics](https://
 scholar.google.com/citations?view_op=top_venues&hl=en). Categories is also
 supported (as function argument). Saves to CSV/JSON. Sub-categories are not yet
-supported. 6. soon: [journal articles](https://github.com/dimitryzub/scrape-
-google-scholar/issues/2). You can use [`scholary`](https://github.com/
-scholarly-python-package/scholarly) to parse the data instead. However, it only
-extracts first 3 points below.  Things custom backend doesn't support yet 1.
-Organic results filters (case law, sorting, period ranges). You can add those
-URL parameters yourself ([if installing from source](https://github.com/
-dimitryzub/scrape-google-scholar-py#installing)) easily to the
+supported. 6. [Journal articles](https://github.com/dimitryzub/scrape-google-
+scholar/issues/2) (with pagination). You can use [`scholary`](https://
+github.com/scholarly-python-package/scholarly) to parse the data instead.
+However, it only extracts first 3 points below.  Things custom backend doesn't
+support yet 1. Organic results filters (case law, sorting, period ranges). You
+can add those URL parameters yourself ([if installing from source](https://
+github.com/dimitryzub/scrape-google-scholar-py#installing)) easily to the
 `google_scholar_py/custom_backend/organic_search.py` file (line [`147`](https:/
 /github.com/dimitryzub/scrape-google-scholar-py/blob/
 a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/
 organic_search.py#L147) or [`136`](https://github.com/dimitryzub/scrape-google-
 scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/
 custom_backend/organic_search.py#L160)), where `driver.get()` is being called.
 2. Author page -> cited by graph. 3. Extracting [journal articles page](https:/
@@ -44,43 +50,46 @@
 jhjzd72UJ%3Ascholar.google.com%2F%26output%3Dcite%26scirp%3D7%26hl%3Den) page
 extraction.    ð® SerpApi backend supports - [Google Scholar Organic](https:/
 /serpapi.com/google-scholar-organic-results) - [Google Scholar Profiles](https:
 //serpapi.com/google-scholar-profilesapi) - [Google Scholar Author](https://
 serpapi.com/google-scholar-author-api) - [Google Scholar Cite](https://
 serpapi.com/google-scholar-cite-api)   ð Custom backend depends on -
 [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to
-bypass CAPTCHAs. - [`selectolax`](https://github.com/rushter/selectolax) - to
-parse HTML fast. Its the fastest Python parser wrapped around [`lexbor`](https:
-//github.com/lexbor/lexbor) (parser in pure C). - [`pandas`](https://
-pandas.pydata.org/) - to save extracted data to CSV or JSON, or if you want to
-analyze the data right away. Save options is used in organic results and top
-publications, public access mandates pages for now. - [`google-search-results`]
-(https://github.com/serpapi/google-search-results-python) - Python wrapper for
-SerpApi backend. - [other packages in the `requirements.txt`](https://
-github.com/dimitryzub/scrape-google-scholar-py/blob/
-8de484e0eec71478e330303fb405a22e0178f068/requirements.txt). All scripts are
-using headless [`selenium-stealth`](https://github.com/diprajpatra/selenium-
-stealth) to bypass CAPTCHA that appears on Google Scholar, so you need to have
-a `chromedriver`. If you're on Linux you may need to do additional
-troubleshooting if `chromedriver` won't run properly.  ## ð¥Installing
-Install via `pip`: ```bash $ pip install scrape-google-scholar-py ``` Install
-for development from source: ```bash $ git clone https://github.com/dimitryzub/
-scrape-google-scholar-py.git $ cd scrape-google-scholar-py $ pip install -
-r requirements.txt ```  If it throws an error with `selenium-stealth` ```bash
-error: The 'selenium' distribution was not found and is required by selenium-
-stealth ``` Use: ```bash $ pip install selenium-stealth ```  ## ðExample
-usage custom backend ```python from google_scholar_py import
-CustomGoogleScholarProfiles import json parser = CustomGoogleScholarProfiles()
-data = parser.scrape_google_scholar_profiles( query='blizzard',
-pagination=False, save_to_csv=False, save_to_json=False ) print(json.dumps
-(data, indent=2)) ```  Google Scholar search operators could also be used
-```lang-none label:computer_vision "Michigan State University"|"U.Michigan" ```
-This query will search all profiles from 2 universities based on "computer
-vision" query.   JSON output ```json [ { "name": "Adam Lobel", "link": "https:/
-/scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
+bypass CAPTCHAs and render some HTML (like cite results from organic result). -
+[`selectolax`](https://github.com/rushter/selectolax) - to parse HTML fast. Its
+the fastest Python parser wrapped around [`lexbor`](https://github.com/lexbor/
+lexbor) (parser in pure C). - [`pandas`](https://pandas.pydata.org/) - to save
+extracted data to CSV or JSON, or if you want to analyze the data right away.
+Save options is used in organic results and top publications, public access
+mandates pages for now. All scripts are using headless [`selenium-stealth`]
+(https://github.com/diprajpatra/selenium-stealth) to bypass CAPTCHA that
+appears on Google Scholar, so you need to have a `chromedriver`. If you're on
+Linux you may need to do additional troubleshooting if `chromedriver` won't run
+properly.  ## ð¥Installing Install via `pip`: ```bash $ pip install scrape-
+google-scholar-py ``` Install from source: ```bash $ git clone https://
+github.com/dimitryzub/scrape-google-scholar-py.git $ cd scrape-google-scholar-
+py $ python -m venv env && source env/Scripts/activate # windows activation $
+pip install -r requirements.txt ``` ### Possible errors that you might
+encounter  LINUX USERS: If it throws "Web-driver exits unexpectedly" error Try
+installing extra dependencies to run `chromedriver`: ```bash $ apt-get install
+-y libglib2.0-0 libnss3 libgconf-2-4 libfontconfig1 ``` See resolved issue: [
+[Linux] Web-driver exits unexpectedly using CustomGoogleScholarOrganic() #7]
+(https://github.com/dimitryzub/scrape-google-scholar-py/issues/7)   If it
+throws an error with `selenium-stealth` ```bash error: The 'selenium'
+distribution was not found and is required by selenium-stealth ``` Use: ```bash
+$ pip install selenium-stealth ```  ## ðExample usage custom backend
+```python from google_scholar_py import CustomGoogleScholarProfiles import json
+parser = CustomGoogleScholarProfiles() data =
+parser.scrape_google_scholar_profiles( query='blizzard', pagination=False,
+save_to_csv=False, save_to_json=False ) print(json.dumps(data, indent=2)) ```
+Google Scholar search operators could also be used ```lang-none label:
+computer_vision "Michigan State University"|"U.Michigan" ``` This query will
+search all profiles from 2 universities based on "computer vision" query.
+JSON output ```json [ { "name": "Adam Lobel", "link": "https://
+scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
 "Blizzard Entertainment", "interests": [ "Gaming", "Emotion regulation" ],
 "email": "Verified email at AdamLobel.com", "cited_by_count": 3593 }, { "name":
 "Daniel Blizzard", "link": "https://scholar.google.com/
 citations?hl=en&user=dk4LWEgAAAAJ", "affiliations": "", "interests": null,
 "email": null, "cited_by_count": 1041 }, { "name": "Shuo Chen", "link": "https:
 //scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ", "affiliations":
 "Senior Data Scientist, Blizzard Entertainment", "interests": [ "Machine
```

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/__init__.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .custom_backend.organic_search import CustomGoogleScholarOrganic
 from .custom_backend.profiles_results import CustomGoogleScholarProfiles
 from .custom_backend.author_info_all_articles import CustomGoogleScholarAuthor
 from .custom_backend.top_mandates_metrics import CustomGoogleScholarTopMandates
 from .custom_backend.top_publications_metrics import CustomGoogleScholarTopPublications
-from .custom_backend.top_publications_article_citations import CustomGoogleScholarTopPublicationCitations
+from .custom_backend.top_publications_article import CustomGoogleScholarTopPublicationArticle
+from .custom_backend.top_publications_article_citation import CustomGoogleScholarTopPublicationArticleCitation
 
 # serpapi backend
 from .serpapi_backend.organic_results import SerpApiGoogleScholarOrganic
 from .serpapi_backend.profile_results import SerpApiGoogleScholarProfiles
 from .serpapi_backend.organic_cite_results import SerpApiGoogleScholarOrganicCite
 from .serpapi_backend.author_results import SerpApiGoogleScholarAuthor
```

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/author_info_all_articles.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/author_info_all_articles.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/cite_results.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/cite_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/organic_search.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/organic_search.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/profiles_results.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/profiles_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_mandates_metrics.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_mandates_metrics.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_article_citations.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_publications_article_citation.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriverManager
 from selectolax.lexbor import LexborHTMLParser
 from typing import List, Dict, Callable, Union
 import pandas as pd
 import time, random
 
-class CustomGoogleScholarTopPublicationCitations:
+class CustomGoogleScholarTopPublicationArticleCitation:
     def __init__(self) -> None:
         pass
     
 
     def parse(self, parser: Callable, publication_citation_data: Callable):
         '''
         Arugments:
-        - parser:  Lexbor parser from scrape_google_scholar_top_publication_citations() function.
-        - publication_citation_data: List to append data to. List origin location is scrape_google_scholar_top_publication_citations() function. Line 104.
+        - parser:  Lexbor parser from scrape_google_scholar_top_publication_article_citations() function.
+        - publication_citation_data: List to append data to. List origin location is scrape_google_scholar_top_publication_article_citations() function. Line 104.
         
         This function parses data from Google Scholar Organic results and appends data to a List.
         
-        It's used by scrape_google_scholar_top_publication_citations().
+        It's used by scrape_google_scholar_top_publication_article_citations().
         '''
         
         # selects the whole table without the first row (header row) 
         for result in parser.css('tr:not(:first-child)'):
             try:
                 title: str = result.css_first('.gsc_mp_anchor_lrge').text()
             except: title = None
@@ -38,72 +38,62 @@
             except: authors = None
             
             try:
                 published_at: str = result.css_first('.gs_gray+ .gs_gray').text()
             except: published_at = None
             
             try:
-                cited_by_count: int = int(result.css_first('.gsc_mpat_c .gsc_mp_anchor').text())
-            except: cited_by_count = None
-
-            try:
-                cited_by_link: str = f"https://scholar.google.com{result.css_first('.gsc_mpat_c a.gsc_mp_anchor').attrs['href']}"
-            except: cited_by_link = None
-            
-            try:
                 year: int = int(result.css_first('.gsc_mp_anchor.gs_nph').text())
             except: year = None
             
             
             publication_citation_data.append({
                 'title': title,
                 'title_link': title_link,
                 'authors': authors,
-                'cited_by_link': cited_by_link,
-                'cited_by_count': cited_by_count,
-                'year': year,
+                'year': year,   
                 'published_at': published_at
             })
 
     #TODO: add lang support. https://serpapi.com/google-languages
-    def scrape_google_scholar_top_publication_citations(
+    def scrape_google_scholar_top_publication_article_citations(
             self,
             journal_publications_link: str,
             pagination: bool = False,
             save_to_csv: bool = False, 
             save_to_json: bool = False
         ) -> List[Dict[str, Union[str, List[str], int]]]:
         '''
-        Results comes from (for example): https://scholar.google.com/citations?hl=en&venue=H--JoiVp8x8J.2022&vq=en&view_op=hcore_citedby&hcore_pos=0
+        Results comes from (for example): https://scholar.google.com/citations?hl=en&venue=k6hd2dUel5kJ.2022&vq=en&view_op=hcore_citedby&hcore_pos=18
         
         Extracts data from Google Scholar Top Publication Metrics Citation page:
         - title: str
         - title_link: str
         - authors: list 
-        - cited_by_count: int
-        - cited_by_link: str 
-        - year: int
         - published_at: str
+        - year: int
     
         Arguments:
         - journal_publications_link: str. Search query. 
         - pagination: bool. Enables or disables pagination. Default is False.
         - save_to_csv: bool. True of False. Default is False.
         - save_to_json: bool. True of False. Default is False.
         
         Usage:
         
-        from google_scholar_py import CustomGoogleScholarTopPublicationCitations
-
-        parser = CustomGoogleScholarTopPublicationCitations()
-        data = parser.scrape_google_scholar_top_publication_citations(
-            journal_publications_link='https://scholar.google.com/citations?hl=en&venue=H--JoiVp8x8J.2022&vq=en&view_op=hcore_citedby&hcore_pos=0', # or link variable that stores the link
+        from google_scholar_py import CustomGoogleScholarTopPublicationArticleCitation
+        import json 
+        
+        parser = CustomGoogleScholarTopPublicationArticleCitation()
+        data = parser.scrape_google_scholar_top_publication_article_citations(
+            journal_publications_link='https://scholar.google.com/citations?hl=en&venue=k6hd2dUel5kJ.2022&vq=en&view_op=hcore_citedby&hcore_pos=18', # or link variable that stores the link
             pagination=False,
             save_to_csv=True
         )
+        print(json.dumps(data, indent=2))
         
         for citations in data:
             print(citations['title'], citations['year'], citations['published_at'], sep='\\n')
         '''
         
         # selenium stealth
         options = webdriver.ChromeOptions()
```

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_metrics.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/custom_backend/top_publications_metrics.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/author_results.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/author_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_cite_results.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/organic_cite_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_results.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/organic_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/profile_results.py` & `scrape-google-scholar-py-0.3.4/google_scholar_py/serpapi_backend/profile_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/requirements.txt` & `scrape-google-scholar-py-0.3.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/PKG-INFO` & `scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-google-scholar-py
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar
 Author: Dmitiry Zub
 Author-email: dimitryzub@gmail.com
 Maintainer: Dmitiry Zub
 Maintainer-email: dimitryzub@gmail.com
 License: MIT
@@ -20,28 +20,44 @@
 Classifier: Topic :: Internet
 Classifier: Natural Language :: English
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
-<p>Sponsor of the project:</p>
+<p>Special thanks to:</p>
 <div>
-   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="140" alt="SerpApi">
+   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="60" alt="SerpApi">
 </div>
 <a href="https://serpapi.com">
 	<b>API to get search engine results with ease.</b>
 </a>
 </div>
 
-_____
+____
+
+<h3 align="center">
+  Scrape data from all Google Scholar pages from a single Python module.
+</h3>
+
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/78694043/231677340-8980c44d-389a-497d-b021-b1d4ab846a77.svg" width="600" alt="scrape-google-scholar-py-logo">
+</div>
+
+
+<div align="center">
+
+  <a href="https://pepy.tech/project/scrape-google-scholar-py">![Downloads](https://static.pepy.tech/badge/scrape-google-scholar-py/month)</a>
+  <a href="">![licence](https://img.shields.io/github/license/dimitryzub/scrape-google-scholar-py?color=blue)</a>
+
+</div>
 
-This repository is meant to extract data from all Google Scholar pages.
 
 <details>
 <summary>🧐 Why two backends?</summary>
 
 1. If you don't want to pay for API. However, I'm not 100% sure if [`selenium-stealth`](https://pypi.org/project/selenium-stealth/) could handle all CAPTCHAs (although it handles CAPTCHA by Cloudflare) and similar blocks.
 2. If you know about SerpApi but don't want to figure out pagination.
 
@@ -58,15 +74,15 @@
 <summary>🧩 Custom backend supports</summary>
 
 1. [Organic results](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=blizzard&btnG=&oq=blizz) (with pagination).
 2. [Profile results](https://scholar.google.com/citations?view_op=search_authors&mauthors=blizzard&hl=en&oi=drw) (with pagination).
 3. [Author + author articles](https://scholar.google.com/citations?user=6IQ8pQwAAAAJ&hl=en&oi=sra) (with pagination), everything except "cited by" graph.
 4. [Public access mandates metrics](https://scholar.google.com/citations?view_op=mandates_leaderboard&hl=en). Yes, you can download CSV with one click, however, it doesn't contain a funder link. Script here has it and saves to CSV/JSON.
 5. [Top publications metrics](https://scholar.google.com/citations?view_op=top_venues&hl=en). Categories is also supported (as function argument). Saves to CSV/JSON. Sub-categories are not yet supported.
-6. soon: [journal articles](https://github.com/dimitryzub/scrape-google-scholar/issues/2).
+6. [Journal articles](https://github.com/dimitryzub/scrape-google-scholar/issues/2) (with pagination).
 
 You can use [`scholary`](https://github.com/scholarly-python-package/scholarly) to parse the data instead. However, it only extracts first 3 points below.  
 
   <details>
   <summary>Things custom backend doesn't support yet</summary>
 
   1. Organic results filters (case law, sorting, period ranges). You can add those URL parameters yourself ([if installing from source](https://github.com/dimitryzub/scrape-google-scholar-py#installing)) easily to the `google_scholar_py/custom_backend/organic_search.py` file (line [`147`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/organic_search.py#L147) or [`136`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/organic_search.py#L160)), where `driver.get()` is being called.
@@ -82,43 +98,53 @@
 
 - [Google Scholar Organic](https://serpapi.com/google-scholar-organic-results)
 - [Google Scholar Profiles](https://serpapi.com/google-scholar-profilesapi)
 - [Google Scholar Author](https://serpapi.com/google-scholar-author-api)
 - [Google Scholar Cite](https://serpapi.com/google-scholar-cite-api)
 </details>
 
-
 <details>
 <summary>🏗 Custom backend depends on</summary>
 
-- [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to bypass CAPTCHAs.
+- [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to bypass CAPTCHAs and render some HTML (like cite results from organic result).
 - [`selectolax`](https://github.com/rushter/selectolax) - to parse HTML fast. Its the fastest Python parser wrapped around [`lexbor`](https://github.com/lexbor/lexbor) (parser in pure C).
 - [`pandas`](https://pandas.pydata.org/) - to save extracted data to CSV or JSON, or if you want to analyze the data right away. Save options is used in organic results and top publications, public access mandates pages for now.
-- [`google-search-results`](https://github.com/serpapi/google-search-results-python) - Python wrapper for SerpApi backend.
-- [other packages in the `requirements.txt`](https://github.com/dimitryzub/scrape-google-scholar-py/blob/8de484e0eec71478e330303fb405a22e0178f068/requirements.txt).
 
 All scripts are using headless [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) to bypass CAPTCHA that appears on Google Scholar, so you need to have a `chromedriver`. If you're on Linux you may need to do additional troubleshooting if `chromedriver` won't run properly.
 </details>
 
 ## 📥Installing
 
 Install via `pip`:
 
 ```bash
 $ pip install scrape-google-scholar-py
 ```
 
-Install for development from source:
+Install from source:
 
 ```bash
 $ git clone https://github.com/dimitryzub/scrape-google-scholar-py.git
 $ cd scrape-google-scholar-py
+$ python -m venv env && source env/Scripts/activate # windows activation
 $ pip install -r requirements.txt
 ```
 
+### Possible errors that you might encounter
+
+<details>
+<summary>LINUX USERS: If it throws "Web-driver exits unexpectedly" error</summary>
+
+  Try installing extra dependencies to run `chromedriver`:	
+  ```bash
+  $ apt-get install -y libglib2.0-0 libnss3 libgconf-2-4 libfontconfig1
+  ```
+
+  See resolved issue: [[Linux] Web-driver exits unexpectedly using CustomGoogleScholarOrganic() #7](https://github.com/dimitryzub/scrape-google-scholar-py/issues/7)	
+</details>
 
 <details>
 <summary>If it throws an error with `selenium-stealth`</summary>
 
   ```bash
   error: The 'selenium' distribution was not found and is required by selenium-stealth
   ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.4 Summary:
 Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar Author: Dmitiry
 Zub Author-email: dimitryzub@gmail.com Maintainer: Dmitiry Zub Maintainer-
 email: dimitryzub@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/dimitryzub/scrape-google-scholar#example-usage-custom-backend
 Project-URL: Source, https://github.com/dimitryzub/scrape-google-scholar
 Project-URL: Tracker, https://github.com/dimitryzub/scrape-google-scholar/
@@ -11,20 +11,26 @@
 scraping,research,lexbor,selectolax,selenium,selenium-stealth,pandas
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet Classifier: Natural Language :: English
 Classifier: Topic :: Utilities Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-                            Sponsor of the project:
+Description-Content-Type: text/markdown License-File: LICENSE
+                              Special thanks to:
                                    [SerpApi]
                   API_to_get_search_engine_results_with_ease.
-_____ This repository is meant to extract data from all Google Scholar pages.
-ð§ Why two backends? 1. If you don't want to pay for API. However, I'm not
+____
+  **** Scrape data from all Google Scholar pages from a single Python module.
+                                     ****
+                        [scrape-google-scholar-py-logo]
+ ![Downloads](https://static.pepy.tech/badge/scrape-google-scholar-py/month) !
+   [licence](https://img.shields.io/github/license/dimitryzub/scrape-google-
+                            scholar-py?color=blue)
+ ð§ Why two backends? 1. If you don't want to pay for API. However, I'm not
 100% sure if [`selenium-stealth`](https://pypi.org/project/selenium-stealth/
 ) could handle all CAPTCHAs (although it handles CAPTCHA by Cloudflare) and
 similar blocks. 2. If you know about SerpApi but don't want to figure out
 pagination. SerpApi backend is more reliable because of: - dedicated team of
 maintainers - pool of proxies - CAPTCHA solvers - legal part of scraping and
 more.   ð§© Custom backend supports 1. [Organic results](https://
 scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=blizzard&btnG=&oq=blizz) (with
@@ -34,21 +40,21 @@
 citations?user=6IQ8pQwAAAAJ&hl=en&oi=sra) (with pagination), everything except
 "cited by" graph. 4. [Public access mandates metrics](https://
 scholar.google.com/citations?view_op=mandates_leaderboard&hl=en). Yes, you can
 download CSV with one click, however, it doesn't contain a funder link. Script
 here has it and saves to CSV/JSON. 5. [Top publications metrics](https://
 scholar.google.com/citations?view_op=top_venues&hl=en). Categories is also
 supported (as function argument). Saves to CSV/JSON. Sub-categories are not yet
-supported. 6. soon: [journal articles](https://github.com/dimitryzub/scrape-
-google-scholar/issues/2). You can use [`scholary`](https://github.com/
-scholarly-python-package/scholarly) to parse the data instead. However, it only
-extracts first 3 points below.  Things custom backend doesn't support yet 1.
-Organic results filters (case law, sorting, period ranges). You can add those
-URL parameters yourself ([if installing from source](https://github.com/
-dimitryzub/scrape-google-scholar-py#installing)) easily to the
+supported. 6. [Journal articles](https://github.com/dimitryzub/scrape-google-
+scholar/issues/2) (with pagination). You can use [`scholary`](https://
+github.com/scholarly-python-package/scholarly) to parse the data instead.
+However, it only extracts first 3 points below.  Things custom backend doesn't
+support yet 1. Organic results filters (case law, sorting, period ranges). You
+can add those URL parameters yourself ([if installing from source](https://
+github.com/dimitryzub/scrape-google-scholar-py#installing)) easily to the
 `google_scholar_py/custom_backend/organic_search.py` file (line [`147`](https:/
 /github.com/dimitryzub/scrape-google-scholar-py/blob/
 a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/custom_backend/
 organic_search.py#L147) or [`136`](https://github.com/dimitryzub/scrape-google-
 scholar-py/blob/a6b3b39042eabdc84851e3c1ca3c246e55bf19d1/google_scholar_py/
 custom_backend/organic_search.py#L160)), where `driver.get()` is being called.
 2. Author page -> cited by graph. 3. Extracting [journal articles page](https:/
@@ -62,43 +68,46 @@
 jhjzd72UJ%3Ascholar.google.com%2F%26output%3Dcite%26scirp%3D7%26hl%3Den) page
 extraction.    ð® SerpApi backend supports - [Google Scholar Organic](https:/
 /serpapi.com/google-scholar-organic-results) - [Google Scholar Profiles](https:
 //serpapi.com/google-scholar-profilesapi) - [Google Scholar Author](https://
 serpapi.com/google-scholar-author-api) - [Google Scholar Cite](https://
 serpapi.com/google-scholar-cite-api)   ð Custom backend depends on -
 [`selenium-stealth`](https://github.com/diprajpatra/selenium-stealth) - to
-bypass CAPTCHAs. - [`selectolax`](https://github.com/rushter/selectolax) - to
-parse HTML fast. Its the fastest Python parser wrapped around [`lexbor`](https:
-//github.com/lexbor/lexbor) (parser in pure C). - [`pandas`](https://
-pandas.pydata.org/) - to save extracted data to CSV or JSON, or if you want to
-analyze the data right away. Save options is used in organic results and top
-publications, public access mandates pages for now. - [`google-search-results`]
-(https://github.com/serpapi/google-search-results-python) - Python wrapper for
-SerpApi backend. - [other packages in the `requirements.txt`](https://
-github.com/dimitryzub/scrape-google-scholar-py/blob/
-8de484e0eec71478e330303fb405a22e0178f068/requirements.txt). All scripts are
-using headless [`selenium-stealth`](https://github.com/diprajpatra/selenium-
-stealth) to bypass CAPTCHA that appears on Google Scholar, so you need to have
-a `chromedriver`. If you're on Linux you may need to do additional
-troubleshooting if `chromedriver` won't run properly.  ## ð¥Installing
-Install via `pip`: ```bash $ pip install scrape-google-scholar-py ``` Install
-for development from source: ```bash $ git clone https://github.com/dimitryzub/
-scrape-google-scholar-py.git $ cd scrape-google-scholar-py $ pip install -
-r requirements.txt ```  If it throws an error with `selenium-stealth` ```bash
-error: The 'selenium' distribution was not found and is required by selenium-
-stealth ``` Use: ```bash $ pip install selenium-stealth ```  ## ðExample
-usage custom backend ```python from google_scholar_py import
-CustomGoogleScholarProfiles import json parser = CustomGoogleScholarProfiles()
-data = parser.scrape_google_scholar_profiles( query='blizzard',
-pagination=False, save_to_csv=False, save_to_json=False ) print(json.dumps
-(data, indent=2)) ```  Google Scholar search operators could also be used
-```lang-none label:computer_vision "Michigan State University"|"U.Michigan" ```
-This query will search all profiles from 2 universities based on "computer
-vision" query.   JSON output ```json [ { "name": "Adam Lobel", "link": "https:/
-/scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
+bypass CAPTCHAs and render some HTML (like cite results from organic result). -
+[`selectolax`](https://github.com/rushter/selectolax) - to parse HTML fast. Its
+the fastest Python parser wrapped around [`lexbor`](https://github.com/lexbor/
+lexbor) (parser in pure C). - [`pandas`](https://pandas.pydata.org/) - to save
+extracted data to CSV or JSON, or if you want to analyze the data right away.
+Save options is used in organic results and top publications, public access
+mandates pages for now. All scripts are using headless [`selenium-stealth`]
+(https://github.com/diprajpatra/selenium-stealth) to bypass CAPTCHA that
+appears on Google Scholar, so you need to have a `chromedriver`. If you're on
+Linux you may need to do additional troubleshooting if `chromedriver` won't run
+properly.  ## ð¥Installing Install via `pip`: ```bash $ pip install scrape-
+google-scholar-py ``` Install from source: ```bash $ git clone https://
+github.com/dimitryzub/scrape-google-scholar-py.git $ cd scrape-google-scholar-
+py $ python -m venv env && source env/Scripts/activate # windows activation $
+pip install -r requirements.txt ``` ### Possible errors that you might
+encounter  LINUX USERS: If it throws "Web-driver exits unexpectedly" error Try
+installing extra dependencies to run `chromedriver`: ```bash $ apt-get install
+-y libglib2.0-0 libnss3 libgconf-2-4 libfontconfig1 ``` See resolved issue: [
+[Linux] Web-driver exits unexpectedly using CustomGoogleScholarOrganic() #7]
+(https://github.com/dimitryzub/scrape-google-scholar-py/issues/7)   If it
+throws an error with `selenium-stealth` ```bash error: The 'selenium'
+distribution was not found and is required by selenium-stealth ``` Use: ```bash
+$ pip install selenium-stealth ```  ## ðExample usage custom backend
+```python from google_scholar_py import CustomGoogleScholarProfiles import json
+parser = CustomGoogleScholarProfiles() data =
+parser.scrape_google_scholar_profiles( query='blizzard', pagination=False,
+save_to_csv=False, save_to_json=False ) print(json.dumps(data, indent=2)) ```
+Google Scholar search operators could also be used ```lang-none label:
+computer_vision "Michigan State University"|"U.Michigan" ``` This query will
+search all profiles from 2 universities based on "computer vision" query.
+JSON output ```json [ { "name": "Adam Lobel", "link": "https://
+scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
 "Blizzard Entertainment", "interests": [ "Gaming", "Emotion regulation" ],
 "email": "Verified email at AdamLobel.com", "cited_by_count": 3593 }, { "name":
 "Daniel Blizzard", "link": "https://scholar.google.com/
 citations?hl=en&user=dk4LWEgAAAAJ", "affiliations": "", "interests": null,
 "email": null, "cited_by_count": 1041 }, { "name": "Shuo Chen", "link": "https:
 //scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ", "affiliations":
 "Senior Data Scientist, Blizzard Entertainment", "interests": [ "Machine
```

### Comparing `scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/SOURCES.txt` & `scrape-google-scholar-py-0.3.4/scrape_google_scholar_py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 google_scholar_py/__init__.py
 google_scholar_py/custom_backend/author_info_all_articles.py
 google_scholar_py/custom_backend/cite_results.py
 google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
 google_scholar_py/custom_backend/organic_search.py
 google_scholar_py/custom_backend/profiles_results.py
 google_scholar_py/custom_backend/top_mandates_metrics.py
-google_scholar_py/custom_backend/top_publications_article_citations.py
+google_scholar_py/custom_backend/top_publications_article.py
+google_scholar_py/custom_backend/top_publications_article_citation.py
 google_scholar_py/custom_backend/top_publications_metrics.py
 google_scholar_py/serpapi_backend/author_results.py
 google_scholar_py/serpapi_backend/organic_cite_results.py
 google_scholar_py/serpapi_backend/organic_results.py
 google_scholar_py/serpapi_backend/profile_results.py
 scrape_google_scholar_py.egg-info/PKG-INFO
 scrape_google_scholar_py.egg-info/SOURCES.txt
```

### Comparing `scrape-google-scholar-py-0.3.3/setup.py` & `scrape-google-scholar-py-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     README = readme_file.read()
 
 setup(
     name='scrape-google-scholar-py',
     description = 'Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.',
     url='https://github.com/dimitryzub/scrape-google-scholar',
-    version='0.3.3',
+    version='0.3.4',
     license='MIT',
     author='Dmitiry Zub',
     author_email='dimitryzub@gmail.com',
     maintainer='Dmitiry Zub',
     maintainer_email='dimitryzub@gmail.com',
     long_description_content_type='text/markdown',
     long_description=README,
```

