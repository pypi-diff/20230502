# Comparing `tmp/pyconverters-pubmedfetcher-0.5.93.tar.gz` & `tmp/pyconverters-pubmedfetcher-0.5.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconverters-pubmedfetcher-0.5.93.tar", last modified: Wed Oct 26 16:46:52 2022, max compression
+gzip compressed data, was "pyconverters-pubmedfetcher-0.5.95.tar", last modified: Thu Dec 15 20:02:57 2022, max compression
```

## Comparing `pyconverters-pubmedfetcher-0.5.93.tar` & `pyconverters-pubmedfetcher-0.5.95.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      502 2022-10-04 08:09:07.296708 pyconverters-pubmedfetcher-0.5.93/.bumpversion.cfg
--rw-r--r--   0        0        0     1386 2022-10-04 08:09:07.297708 pyconverters-pubmedfetcher-0.5.93/.github/workflows/main.yml
--rw-r--r--   0        0        0     1750 2022-10-04 08:09:07.298708 pyconverters-pubmedfetcher-0.5.93/.gitignore
--rw-r--r--   0        0        0      478 2022-10-04 08:09:07.299708 pyconverters-pubmedfetcher-0.5.93/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2022-10-04 08:09:07.299708 pyconverters-pubmedfetcher-0.5.93/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      304 2022-10-04 08:09:07.300708 pyconverters-pubmedfetcher-0.5.93/.idea/modules.xml
--rw-r--r--   0        0        0      180 2022-10-04 08:09:07.301708 pyconverters-pubmedfetcher-0.5.93/.idea/vcs.xml
--rw-r--r--   0        0        0      419 2022-10-04 08:09:07.303708 pyconverters-pubmedfetcher-0.5.93/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2022-10-04 08:09:07.307708 pyconverters-pubmedfetcher-0.5.93/.readthedocs.yml
--rw-r--r--   0        0        0      122 2022-10-04 08:09:07.311708 pyconverters-pubmedfetcher-0.5.93/AUTHORS.md
--rw-r--r--   0        0        0      268 2022-10-04 08:09:07.315708 pyconverters-pubmedfetcher-0.5.93/CHANGELOG.md
--rw-r--r--   0        0        0      461 2022-10-04 08:09:07.317708 pyconverters-pubmedfetcher-0.5.93/Dockerfile
--rw-r--r--   0        0        0    10235 2022-10-25 12:07:35.454798 pyconverters-pubmedfetcher-0.5.93/Jenkinsfile
--rw-r--r--   0        0        0     1082 2022-10-04 08:09:07.324708 pyconverters-pubmedfetcher-0.5.93/LICENSE
--rw-r--r--   0        0        0     1612 2022-10-04 08:09:07.325708 pyconverters-pubmedfetcher-0.5.93/README.md
--rw-r--r--   0        0        0      951 2022-10-04 08:09:07.327709 pyconverters-pubmedfetcher-0.5.93/RELEASE.md
--rw-r--r--   0        0        0     1559 2022-10-04 08:09:07.334709 pyconverters-pubmedfetcher-0.5.93/bumpversion.py
--rw-r--r--   0        0        0       62 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.93/docs/.gitignore
--rw-r--r--   0        0        0      268 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.93/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.93/docs/LICENSE
--rw-r--r--   0        0        0        0 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.93/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-10-04 08:09:07.337709 pyconverters-pubmedfetcher-0.5.93/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2904 2022-10-04 08:09:07.338709 pyconverters-pubmedfetcher-0.5.93/docs/conf.py
--rw-r--r--   0        0        0      147 2022-10-04 08:09:07.341709 pyconverters-pubmedfetcher-0.5.93/docs/index.rst
--rw-r--r--   0        0        0       98 2022-10-04 08:09:07.344709 pyconverters-pubmedfetcher-0.5.93/mypy.ini
--rw-r--r--   0        0        0     2292 2022-10-04 08:09:07.346709 pyconverters-pubmedfetcher-0.5.93/pyproject.toml
--rw-r--r--   0        0        0      988 2022-10-26 16:41:08.971258 pyconverters-pubmedfetcher-0.5.93/results.xml
--rw-r--r--   0        0        0       47 2022-10-26 16:46:51.611319 pyconverters-pubmedfetcher-0.5.93/src/pyconverters_pubmedfetcher/__init__.py
--rw-r--r--   0        0        0     9452 2022-10-26 16:41:08.971258 pyconverters-pubmedfetcher-0.5.93/src/pyconverters_pubmedfetcher/pubmedfetcher.py
--rw-r--r--   0        0        0     4101 2022-10-04 08:09:07.358709 pyconverters-pubmedfetcher-0.5.93/tests/data/DOIs-only.txt
--rwxr-xr-x   0        0        0  1242426 2022-10-04 08:09:07.368709 pyconverters-pubmedfetcher-0.5.93/tests/data/MedLine2021-09-06-19-04-11.xml
--rw-r--r--   0        0        0       97 2022-10-26 16:41:08.973258 pyconverters-pubmedfetcher-0.5.93/tests/data/list.txt
--rw-r--r--   0        0        0     2466 2022-10-25 12:07:35.457798 pyconverters-pubmedfetcher-0.5.93/tests/test_pubmedfetcher.py
--rw-r--r--   0        0        0      927 2022-10-04 08:09:07.381710 pyconverters-pubmedfetcher-0.5.93/tox.ini
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 pyconverters-pubmedfetcher-0.5.93/setup.py
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 pyconverters-pubmedfetcher-0.5.93/PKG-INFO
+-rw-r--r--   0        0        0      502 2022-10-04 08:09:07.296708 pyconverters-pubmedfetcher-0.5.95/.bumpversion.cfg
+-rw-r--r--   0        0        0     1386 2022-10-04 08:09:07.297708 pyconverters-pubmedfetcher-0.5.95/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1750 2022-10-04 08:09:07.298708 pyconverters-pubmedfetcher-0.5.95/.gitignore
+-rw-r--r--   0        0        0      478 2022-10-04 08:09:07.299708 pyconverters-pubmedfetcher-0.5.95/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2022-10-04 08:09:07.299708 pyconverters-pubmedfetcher-0.5.95/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      304 2022-10-04 08:09:07.300708 pyconverters-pubmedfetcher-0.5.95/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2022-10-04 08:09:07.301708 pyconverters-pubmedfetcher-0.5.95/.idea/vcs.xml
+-rw-r--r--   0        0        0      419 2022-10-04 08:09:07.303708 pyconverters-pubmedfetcher-0.5.95/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2022-10-04 08:09:07.307708 pyconverters-pubmedfetcher-0.5.95/.readthedocs.yml
+-rw-r--r--   0        0        0      122 2022-10-04 08:09:07.311708 pyconverters-pubmedfetcher-0.5.95/AUTHORS.md
+-rw-r--r--   0        0        0      268 2022-10-04 08:09:07.315708 pyconverters-pubmedfetcher-0.5.95/CHANGELOG.md
+-rw-r--r--   0        0        0      461 2022-10-04 08:09:07.317708 pyconverters-pubmedfetcher-0.5.95/Dockerfile
+-rw-r--r--   0        0        0    10324 2022-12-15 19:41:59.660333 pyconverters-pubmedfetcher-0.5.95/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2022-10-04 08:09:07.324708 pyconverters-pubmedfetcher-0.5.95/LICENSE
+-rw-r--r--   0        0        0     1612 2022-10-04 08:09:07.325708 pyconverters-pubmedfetcher-0.5.95/README.md
+-rw-r--r--   0        0        0      951 2022-10-04 08:09:07.327709 pyconverters-pubmedfetcher-0.5.95/RELEASE.md
+-rw-r--r--   0        0        0     1559 2022-10-04 08:09:07.334709 pyconverters-pubmedfetcher-0.5.95/bumpversion.py
+-rw-r--r--   0        0        0       62 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.95/docs/.gitignore
+-rw-r--r--   0        0        0      268 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.95/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.95/docs/LICENSE
+-rw-r--r--   0        0        0        0 2022-10-04 08:09:07.335709 pyconverters-pubmedfetcher-0.5.95/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-10-04 08:09:07.337709 pyconverters-pubmedfetcher-0.5.95/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2904 2022-10-04 08:09:07.338709 pyconverters-pubmedfetcher-0.5.95/docs/conf.py
+-rw-r--r--   0        0        0      147 2022-10-04 08:09:07.341709 pyconverters-pubmedfetcher-0.5.95/docs/index.rst
+-rw-r--r--   0        0        0       98 2022-10-04 08:09:07.344709 pyconverters-pubmedfetcher-0.5.95/mypy.ini
+-rw-r--r--   0        0        0     2292 2022-10-04 08:09:07.346709 pyconverters-pubmedfetcher-0.5.95/pyproject.toml
+-rw-r--r--   0        0        0      988 2022-12-15 19:41:59.662333 pyconverters-pubmedfetcher-0.5.95/results.xml
+-rw-r--r--   0        0        0       47 2022-12-15 20:02:20.272673 pyconverters-pubmedfetcher-0.5.95/src/pyconverters_pubmedfetcher/__init__.py
+-rw-r--r--   0        0        0     9452 2022-10-26 16:41:08.971258 pyconverters-pubmedfetcher-0.5.95/src/pyconverters_pubmedfetcher/pubmedfetcher.py
+-rw-r--r--   0        0        0     4101 2022-10-04 08:09:07.358709 pyconverters-pubmedfetcher-0.5.95/tests/data/DOIs-only.txt
+-rwxr-xr-x   0        0        0  1242426 2022-10-04 08:09:07.368709 pyconverters-pubmedfetcher-0.5.95/tests/data/MedLine2021-09-06-19-04-11.xml
+-rw-r--r--   0        0        0       97 2022-10-26 16:41:08.973258 pyconverters-pubmedfetcher-0.5.95/tests/data/list.txt
+-rw-r--r--   0        0        0     2466 2022-10-25 12:07:35.457798 pyconverters-pubmedfetcher-0.5.95/tests/test_pubmedfetcher.py
+-rw-r--r--   0        0        0      927 2022-10-04 08:09:07.381710 pyconverters-pubmedfetcher-0.5.95/tox.ini
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 pyconverters-pubmedfetcher-0.5.95/setup.py
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 pyconverters-pubmedfetcher-0.5.95/PKG-INFO
```

### Comparing `pyconverters-pubmedfetcher-0.5.93/.github/workflows/main.yml` & `pyconverters-pubmedfetcher-0.5.95/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/.gitignore` & `pyconverters-pubmedfetcher-0.5.95/.gitignore`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/Jenkinsfile` & `pyconverters-pubmedfetcher-0.5.95/Jenkinsfile`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
             // remove any previous folder dist
             sh 'rm -rf dist'
             // create (as root) folder dist
             sh 'mkdir dist'
             // pull recent updates of file __init__.py
             withCredentials([gitUsernamePassword(credentialsId: 'bitbucket-user', gitToolName: 'git-tool')]) {
               sh 'git config --global pull.rebase false'
+              sh "git config --global --add safe.directory ${PATH_HOME}/${env.JOB_NAME}"
               sh 'git pull'
             }
             // put back owner of pulled file
             sh 'chown 1000:1000 src/pyconverters_pubmedfetcher/__init__.py'
             // get git status
             sh 'git status'
             // publish on PyPI
```

### Comparing `pyconverters-pubmedfetcher-0.5.93/LICENSE` & `pyconverters-pubmedfetcher-0.5.95/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/README.md` & `pyconverters-pubmedfetcher-0.5.95/README.md`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/RELEASE.md` & `pyconverters-pubmedfetcher-0.5.95/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/bumpversion.py` & `pyconverters-pubmedfetcher-0.5.95/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/docs/LICENSE` & `pyconverters-pubmedfetcher-0.5.95/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/docs/conf.py` & `pyconverters-pubmedfetcher-0.5.95/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/pyproject.toml` & `pyconverters-pubmedfetcher-0.5.95/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/results.xml` & `pyconverters-pubmedfetcher-0.5.95/results.xml`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/src/pyconverters_pubmedfetcher/pubmedfetcher.py` & `pyconverters-pubmedfetcher-0.5.95/src/pyconverters_pubmedfetcher/pubmedfetcher.py`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/tests/data/DOIs-only.txt` & `pyconverters-pubmedfetcher-0.5.95/tests/data/DOIs-only.txt`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/tests/data/MedLine2021-09-06-19-04-11.xml` & `pyconverters-pubmedfetcher-0.5.95/tests/data/MedLine2021-09-06-19-04-11.xml`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/tests/test_pubmedfetcher.py` & `pyconverters-pubmedfetcher-0.5.95/tests/test_pubmedfetcher.py`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/tox.ini` & `pyconverters-pubmedfetcher-0.5.95/tox.ini`

 * *Files identical despite different names*

### Comparing `pyconverters-pubmedfetcher-0.5.93/setup.py` & `pyconverters-pubmedfetcher-0.5.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           'tox']}
 
 entry_points = \
 {'pyconverters.plugins': ['pubmedfetcher = '
                           'pyconverters_pubmedfetcher.pubmedfetcher:PubmedFetcherConverter']}
 
 setup(name='pyconverters-pubmedfetcher',
-      version='0.5.93',
+      version='0.5.95',
       description='Pubmed converter.',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyconverters_pubmedfetcher/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyconverters-pubmedfetcher-0.5.93/PKG-INFO` & `pyconverters-pubmedfetcher-0.5.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconverters-pubmedfetcher
-Version: 0.5.93
+Version: 0.5.95
 Summary: Pubmed converter.
 Home-page: https://github.com/oterrier/pyconverters_pubmedfetcher/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

