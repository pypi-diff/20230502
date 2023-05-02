# Comparing `tmp/gpt-review-0.2.3rc291.post1.tar.gz` & `tmp/gpt-review-0.2.3rc293.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.2.3rc291.post1.tar", last modified: Tue May  2 06:06:16 2023, max compression
+gzip compressed data, was "gpt-review-0.2.3rc293.post1.tar", last modified: Tue May  2 06:11:59 2023, max compression
```

## Comparing `gpt-review-0.2.3rc291.post1.tar` & `gpt-review-0.2.3rc293.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      336 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1464 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2146 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4590 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/LICENSE
--rw-r--r--   0        0        0     1617 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/README.md
--rw-r--r--   0        0        0     5206 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/action.yml
--rw-r--r--   0        0        0     8232 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/review.py
--rw-r--r--   0        0        0      364 2023-05-02 06:06:15.861770 gpt-review-0.2.3rc291.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11461 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     1281 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/tests/conftest.py
--rw-r--r--   0        0        0     5554 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc291.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2146 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4577 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/README.md
+-rw-r--r--   0        0        0     5206 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/action.yml
+-rw-r--r--   0        0        0     8237 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/review.py
+-rw-r--r--   0        0        0      364 2023-05-02 06:11:58.464312 gpt-review-0.2.3rc293.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11461 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-02 06:11:47.104172 gpt-review-0.2.3rc293.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-02 06:11:47.108172 gpt-review-0.2.3rc293.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1281 2023-05-02 06:11:47.108172 gpt-review-0.2.3rc293.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5554 2023-05-02 06:11:47.108172 gpt-review-0.2.3rc293.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc293.post1/PKG-INFO
```

### Comparing `gpt-review-0.2.3rc291.post1/.devcontainer/devcontainer.json` & `gpt-review-0.2.3rc293.post1/.devcontainer/devcontainer.json`

 * *Files 26% similar despite different names*

```diff
@@ -5,36 +5,36 @@
   "build": {
     "dockerfile": "Dockerfile",
     "context": ".."
   },
   "customizations": {
     "vscode": {
       "extensions": [
-		"editorconfig.editorconfig",
-		"github.vscode-pull-request-github",
-		"ms-azuretools.vscode-docker",
-		"ms-python.python",
-		"ms-python.vscode-pylance",
-		"ms-python.pylint",
-		"ms-python.isort",
-		"ms-python.flake8",
-		"ms-python.black-formatter",
-		"ms-vsliveshare.vsliveshare",
-		"ryanluker.vscode-coverage-gutters",
-		"bungcip.better-toml",
-		"GitHub.copilot",
-		"GitHub.vscode-github-actions",
-		"ms-vscode.azurecli",
-		"ms-vscode.azure-account",
-		"zokugun.explicit-folding",
-		"MaxKless.git-squash-all",
-		"GitHub.copilot-labs",
-		"GitHub.codespaces",
-		"charliermarsh.ruff"
-	],
+        "editorconfig.editorconfig",
+        "github.vscode-pull-request-github",
+        "ms-azuretools.vscode-docker",
+        "ms-python.python",
+        "ms-python.vscode-pylance",
+        "ms-python.pylint",
+        "ms-python.isort",
+        "ms-python.flake8",
+        "ms-python.black-formatter",
+        "ms-vsliveshare.vsliveshare",
+        "ryanluker.vscode-coverage-gutters",
+        "bungcip.better-toml",
+        "GitHub.copilot",
+        "GitHub.vscode-github-actions",
+        "ms-vscode.azurecli",
+        "ms-vscode.azure-account",
+        "zokugun.explicit-folding",
+        "MaxKless.git-squash-all",
+        "GitHub.copilot-labs",
+        "GitHub.codespaces",
+        "charliermarsh.ruff"
+      ],
       "settings": {
         "python.defaultInterpreterPath": "/usr/local/bin/python",
         "black-formatter.path": [
           "/usr/local/py-utils/bin/black"
         ],
         "pylint.path": [
           "/usr/local/py-utils/bin/pylint"
```

### Comparing `gpt-review-0.2.3rc291.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.2.3rc293.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.github/dependabot.yml` & `gpt-review-0.2.3rc293.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.github/pull_request_template.md` & `gpt-review-0.2.3rc293.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.github/workflows/codeql.yml` & `gpt-review-0.2.3rc293.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.2.3rc293.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.2.3rc293.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.github/workflows/python.yml` & `gpt-review-0.2.3rc293.post1/.github/workflows/python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         with:
           ref: ${{ github.event.pull_request.head.sha }}
       - uses: Azure/login@v1.4.6
         continue-on-error: true
         with:
           creds: ${{ secrets.AZURE_CREDENTIALS }}
       - name: ${{ matrix.tools }}
-        uses: microsoft/action-python@0.4.0
+        uses: microsoft/action-python@0.6.0
         with:
           ${{ matrix.tools }}: true
           args: ${{ matrix.args }}
           workdir: '.'
           testdir: 'tests'
           python_version: '3.11.3'
 
@@ -62,15 +62,15 @@
 
       - name: Set Configurations
         if: steps.tag_version.outputs.release_type && github.event_name != 'release'
         shell: bash
         env:
           VERSION: ${{ steps.tag_version.outputs.new_version }}
         run: sed -ri 's/(__version__ = ")([0-9]+\.[0-9]+\.[0-9]+?(.*))(")/\1'"$VERSION"'\3/' "src/gpt_review/__init__.py" || exit 1
-        
+
       - name: Set Configurations
         if: steps.tag_version.outputs.release_type && github.event_name == 'release'
         shell: bash
         env:
           VERSION: ${{ steps.tag_version.outputs.previous_version }}
         run: sed -ri 's/(__version__ = ")([0-9]+\.[0-9]+\.[0-9]+?.*)(")/\1'"$VERSION"'\3/' "src/gpt_review/__init__.py" || exit 1
 
@@ -126,16 +126,16 @@
     - uses: actions/setup-python@v1
       with:
         python-version: '3.11'
         cache: 'pip' # caching pip dependencies
     - run: |
         pip install pytest pytest-cov pytest-xdist
         pip install -e .
-    
-    - run: pytest --cov=src --cov-report=xml --cov-fail-under 0 
+
+    - run: pytest --cov=src --cov-report=xml --cov-fail-under 0
     - uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         flags: unittests
 
     - run: pytest --cov=src --cov-report=xml --cov-fail-under 0 -m "integration"
     - uses: codecov/codecov-action@v3
```

### Comparing `gpt-review-0.2.3rc291.post1/.github/workflows/test-action.yml` & `gpt-review-0.2.3rc293.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.gitignore` & `gpt-review-0.2.3rc293.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/.vscode/settings.json` & `gpt-review-0.2.3rc293.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/LICENSE` & `gpt-review-0.2.3rc293.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/README.md` & `gpt-review-0.2.3rc293.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/action.yml` & `gpt-review-0.2.3rc293.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/pyproject.toml` & `gpt-review-0.2.3rc293.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     "flake8-pyproject",
     "pre-commit==3.2.2",
     "pylint==2.17.3",
     "pylint_junit",
     "pytest-cov>=3.0.0",
     "pytest-mock",
     "pytest-runner",
+    "pytest-xdist",
     "pytest>=7.2.2",
     "pytest-github-actions-annotate-failures",
     "shellcheck-py==0.9.0.2"
 ]
 
 [project.scripts]
 gpt = "gpt_review.main:__main__"
@@ -123,15 +124,15 @@
 pythonPlatform = "Linux"
 
 executionEnvironments = [
   { root = "src" }
 ]
 
 [tool.pytest.ini_options]
-# addopts = "--cov-report xml:coverage.xml --cov src --cov-fail-under 0 --cov-append -m 'not integration'"
+addopts = "--cov-report xml:coverage.xml --cov src --cov-fail-under 0 --cov-append -n auto"
 pythonpath = [
   "src"
 ]
 testpaths = "tests"
 # junit_family = "xunit2"
 markers = [
     "integration: marks as integration test",
```

### Comparing `gpt-review-0.2.3rc291.post1/review.py` & `gpt-review-0.2.3rc293.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/src/gpt_review/_ask.py` & `gpt-review-0.2.3rc293.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.2.3rc293.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/tests/conftest.py` & `gpt-review-0.2.3rc293.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/tests/test_gpt_cli.py` & `gpt-review-0.2.3rc293.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc291.post1/PKG-INFO` & `gpt-review-0.2.3rc293.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.2.3rc291.post1
+Version: 0.2.3rc293.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -32,14 +32,15 @@
 Requires-Dist: flake8-pyproject ; extra == "test"
 Requires-Dist: pre-commit==3.2.2 ; extra == "test"
 Requires-Dist: pylint==2.17.3 ; extra == "test"
 Requires-Dist: pylint_junit ; extra == "test"
 Requires-Dist: pytest-cov>=3.0.0 ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
+Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: pytest>=7.2.2 ; extra == "test"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
 Project-URL: Documentation, https://github.com/dciborow/action-gpt/tree/main#readme
 Project-URL: Source, https://github.com/dciborow/action-gpt
 Project-URL: Tracker, https://github.com/dciborow/action-gpt/issues
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc291.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc293.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -15,20 +15,21 @@
 manifest==0.49 ; extra == "test" Requires-Dist: flake8-bugbear==23.3.23 ; extra
 == "test" Requires-Dist: flake8-docstrings ; extra == "test" Requires-Dist:
 flake8-formatter_junit_xml ; extra == "test" Requires-Dist: flake8 ; extra ==
 "test" Requires-Dist: flake8-pyproject ; extra == "test" Requires-Dist: pre-
 commit==3.2.2 ; extra == "test" Requires-Dist: pylint==2.17.3 ; extra == "test"
 Requires-Dist: pylint_junit ; extra == "test" Requires-Dist: pytest-cov>=3.0.0
 ; extra == "test" Requires-Dist: pytest-mock ; extra == "test" Requires-Dist:
-pytest-runner ; extra == "test" Requires-Dist: pytest>=7.2.2 ; extra == "test"
-Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
-Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test" Project-URL:
-Documentation, https://github.com/dciborow/action-gpt/tree/main#readme Project-
-URL: Source, https://github.com/dciborow/action-gpt Project-URL: Tracker,
-https://github.com/dciborow/action-gpt/issues Provides-Extra: test # gpt-review
+pytest-runner ; extra == "test" Requires-Dist: pytest-xdist ; extra == "test"
+Requires-Dist: pytest>=7.2.2 ; extra == "test" Requires-Dist: pytest-github-
+actions-annotate-failures ; extra == "test" Requires-Dist: shellcheck-
+py==0.9.0.2 ; extra == "test" Project-URL: Documentation, https://github.com/
+dciborow/action-gpt/tree/main#readme Project-URL: Source, https://github.com/
+dciborow/action-gpt Project-URL: Tracker, https://github.com/dciborow/action-
+gpt/issues Provides-Extra: test # gpt-review
   [Actions_Status] [Coverage_Status] [License:_MIT] [PyPI] [Downloads] [Code
                                  style:_black]
 A Python based CLI and GitHub Action to use Open AI or Azure Open AI models to
 review contents of pull requests. ## How to use CLI: Install the package via
 `pip` and set the environment variables for your OpenAI API Key and
 Organization ID. To use Azure OpenAI, set the environment variable
 `AZURE_OPENAI_API_URL` and `AZURE_OPENAI_API_URL_KEY` to the URL and key for
```

