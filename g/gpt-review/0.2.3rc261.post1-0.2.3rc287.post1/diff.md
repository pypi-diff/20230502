# Comparing `tmp/gpt-review-0.2.3rc261.post1.tar.gz` & `tmp/gpt-review-0.2.3rc287.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.2.3rc261.post1.tar", last modified: Mon May  1 21:56:15 2023, max compression
+gzip compressed data, was "gpt-review-0.2.3rc287.post1.tar", last modified: Tue May  2 04:57:56 2023, max compression
```

## Comparing `gpt-review-0.2.3rc261.post1.tar` & `gpt-review-0.2.3rc287.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      336 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1464 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2146 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4577 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/LICENSE
--rw-r--r--   0        0        0     1617 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/README.md
--rw-r--r--   0        0        0     5206 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/action.yml
--rw-r--r--   0        0        0     8232 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/review.py
--rw-r--r--   0        0        0      364 2023-05-01 21:56:14.719349 gpt-review-0.2.3rc261.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11461 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     1281 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/tests/conftest.py
--rw-r--r--   0        0        0     5449 2023-05-01 21:56:08.695310 gpt-review-0.2.3rc261.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc261.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1464 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2146 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4590 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/README.md
+-rw-r--r--   0        0        0     5206 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/action.yml
+-rw-r--r--   0        0        0     8232 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/review.py
+-rw-r--r--   0        0        0      364 2023-05-02 04:57:55.658790 gpt-review-0.2.3rc287.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11461 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1281 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5449 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc287.post1/PKG-INFO
```

### Comparing `gpt-review-0.2.3rc261.post1/.devcontainer/devcontainer.json` & `gpt-review-0.2.3rc287.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.2.3rc287.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/dependabot.yml` & `gpt-review-0.2.3rc287.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/pull_request_template.md` & `gpt-review-0.2.3rc287.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/workflows/codeql.yml` & `gpt-review-0.2.3rc287.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.2.3rc287.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.2.3rc287.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.github/workflows/python.yml` & `gpt-review-0.2.3rc287.post1/.github/workflows/python.yml`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
       with:
         ref: ${{ github.event.pull_request.head.sha }}
     - uses: actions/setup-python@v1
       with:
         python-version: '3.11'
         cache: 'pip' # caching pip dependencies
     - run: |
-        pip install pytest pytest-cov
+        pip install pytest pytest-cov pytest-xdist
         pip install -e .
     
     - run: pytest --cov=src --cov-report=xml --cov-fail-under 0 
     - uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         flags: unittests
```

### Comparing `gpt-review-0.2.3rc261.post1/.github/workflows/test-action.yml` & `gpt-review-0.2.3rc287.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.gitignore` & `gpt-review-0.2.3rc287.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/.vscode/settings.json` & `gpt-review-0.2.3rc287.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/LICENSE` & `gpt-review-0.2.3rc287.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/README.md` & `gpt-review-0.2.3rc287.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/action.yml` & `gpt-review-0.2.3rc287.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/pyproject.toml` & `gpt-review-0.2.3rc287.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/review.py` & `gpt-review-0.2.3rc287.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/src/gpt_review/_ask.py` & `gpt-review-0.2.3rc287.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.2.3rc287.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/tests/conftest.py` & `gpt-review-0.2.3rc287.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/tests/test_gpt_cli.py` & `gpt-review-0.2.3rc287.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc261.post1/PKG-INFO` & `gpt-review-0.2.3rc287.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.2.3rc261.post1
+Version: 0.2.3rc287.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc261.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc287.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

