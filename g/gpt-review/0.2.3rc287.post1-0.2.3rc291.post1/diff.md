# Comparing `tmp/gpt-review-0.2.3rc287.post1.tar.gz` & `tmp/gpt-review-0.2.3rc291.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.2.3rc287.post1.tar", last modified: Tue May  2 04:57:56 2023, max compression
+gzip compressed data, was "gpt-review-0.2.3rc291.post1.tar", last modified: Tue May  2 06:06:16 2023, max compression
```

## Comparing `gpt-review-0.2.3rc287.post1.tar` & `gpt-review-0.2.3rc291.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      336 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1464 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2146 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4590 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/LICENSE
--rw-r--r--   0        0        0     1617 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/README.md
--rw-r--r--   0        0        0     5206 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/action.yml
--rw-r--r--   0        0        0     8232 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/review.py
--rw-r--r--   0        0        0      364 2023-05-02 04:57:55.658790 gpt-review-0.2.3rc287.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11461 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     1281 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/tests/conftest.py
--rw-r--r--   0        0        0     5449 2023-05-02 04:57:49.678679 gpt-review-0.2.3rc287.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc287.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1464 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2146 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4590 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-02 06:06:05.169598 gpt-review-0.2.3rc291.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/README.md
+-rw-r--r--   0        0        0     5206 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/action.yml
+-rw-r--r--   0        0        0     8232 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/review.py
+-rw-r--r--   0        0        0      364 2023-05-02 06:06:15.861770 gpt-review-0.2.3rc291.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11461 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1281 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5554 2023-05-02 06:06:05.173598 gpt-review-0.2.3rc291.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc291.post1/PKG-INFO
```

### Comparing `gpt-review-0.2.3rc287.post1/.devcontainer/devcontainer.json` & `gpt-review-0.2.3rc291.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.2.3rc291.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/dependabot.yml` & `gpt-review-0.2.3rc291.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/pull_request_template.md` & `gpt-review-0.2.3rc291.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/workflows/codeql.yml` & `gpt-review-0.2.3rc291.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.2.3rc291.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.2.3rc291.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/workflows/python.yml` & `gpt-review-0.2.3rc291.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.github/workflows/test-action.yml` & `gpt-review-0.2.3rc291.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.gitignore` & `gpt-review-0.2.3rc291.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/.vscode/settings.json` & `gpt-review-0.2.3rc291.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/LICENSE` & `gpt-review-0.2.3rc291.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/README.md` & `gpt-review-0.2.3rc291.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/action.yml` & `gpt-review-0.2.3rc291.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/pyproject.toml` & `gpt-review-0.2.3rc291.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/review.py` & `gpt-review-0.2.3rc291.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/src/gpt_review/_ask.py` & `gpt-review-0.2.3rc291.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.2.3rc291.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/tests/conftest.py` & `gpt-review-0.2.3rc291.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc287.post1/tests/test_gpt_cli.py` & `gpt-review-0.2.3rc291.post1/tests/test_gpt_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,90 +21,90 @@
     CLICase("--help"),
 ]
 
 ASK_COMMANDS = [
     CLICase("ask --help"),
     CLICase("ask how are you"),
     CLICase("ask --fast how are you"),
-    CLICase(f"ask how are you --max-tokens={C.MAX_TOKENS_DEFAULT}"),
+    CLICase(f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT}"),
     CLICase(
-        "ask how are you --max-tokens",
+        "ask how are you --fast --max-tokens",
         """usage: gpt ask [-h] [--verbose] [--debug] [--only-show-errors]
                [--output {json,jsonc,yaml,yamlc,table,tsv,none}]
                [--query JMESPATH] [--max-tokens MAX_TOKENS]
                [--temperature TEMPERATURE] [--top-p TOP_P]
                [--frequency-penalty FREQUENCY_PENALTY]
                [--presence-penalty PRESENCE_PENALTY]
                <QUESTION> [<QUESTION> ...]
 gpt ask: error: argument --max-tokens: expected one argument
 """,
         2,
     ),
     CLICase(
-        "ask how are you --max-tokens 'test'",
+        "ask how are you --fast --max-tokens 'test'",
         """usage: gpt ask [-h] [--verbose] [--debug] [--only-show-errors]
                [--output {json,jsonc,yaml,yamlc,table,tsv,none}]
                [--query JMESPATH] [--max-tokens MAX_TOKENS]
                [--temperature TEMPERATURE] [--top-p TOP_P]
                [--frequency-penalty FREQUENCY_PENALTY]
                [--presence-penalty PRESENCE_PENALTY]
                <QUESTION> [<QUESTION> ...]
 gpt ask: error: argument --max-tokens: invalid int value: \"'test'\"
 """,
         2,
     ),
     CLICase(
-        f"ask how are you --max-tokens {C.MAX_TOKENS_MIN-1}",
+        f"ask how are you --fast --max-tokens {C.MAX_TOKENS_MIN-1}",
         f"ERROR: --max-tokens must be a(n) int between {C.MAX_TOKENS_MIN} and {C.MAX_TOKENS_MAX}\n",
         1,
     ),
-    CLICase(f"ask how are you --temperature {C.TEMPERATURE_DEFAULT}"),
+    CLICase(f"ask how are you --fast --temperature {C.TEMPERATURE_DEFAULT}"),
     CLICase(
         f"ask how are you --temperature {C.TEMPERATURE_MAX+8}",
         f"ERROR: --temperature must be a(n) float between {C.TEMPERATURE_MIN} and {C.TEMPERATURE_MAX}\n",
         1,
     ),
-    CLICase(f"ask how are you --top-p {C.TOP_P_DEFAULT}"),
+    CLICase(f"ask how are you --fast --top-p {C.TOP_P_DEFAULT}"),
     CLICase(
         f"ask how are you --top-p {C.TOP_P_MAX+3.5}",
         f"ERROR: --top-p must be a(n) float between {C.TOP_P_MIN} and {C.TOP_P_MAX}\n",
         1,
     ),
-    CLICase(f"ask how are you --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT}"),
+    CLICase(f"ask how are you --fast --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT}"),
     CLICase(
         f"ask how are you --frequency-penalty {C.FREQUENCY_PENALTY_MAX+2}",
         f"ERROR: --frequency-penalty must be a(n) float between {C.FREQUENCY_PENALTY_MIN} and {C.FREQUENCY_PENALTY_MAX}\n",
         1,
     ),
-    CLICase(f"ask how are you --presence-penalty {C.PRESENCE_PENALTY_DEFAULT}"),
+    CLICase(f"ask how are you --fast --presence-penalty {C.PRESENCE_PENALTY_DEFAULT}"),
     CLICase(
         f"ask how are you --presence-penalty {C.PRESENCE_PENALTY_MAX+7.7}",
         f"ERROR: --presence-penalty must be a(n) float between {C.PRESENCE_PENALTY_MIN} and {C.PRESENCE_PENALTY_MAX}\n",
         1,
     ),
-    CLICase(f"ask how are you --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT}"),
-    CLICase(f"ask how are you --max-tokens={C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT}"),
+    CLICase(f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT}"),
+    CLICase(f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT}"),
     CLICase(
-        f"ask how are you --max-tokens {C.MAX_TOKENS_MAX+1} --top-p {C.TOP_P_DEFAULT}",
+        f"ask how are you --fast --max-tokens {C.MAX_TOKENS_MAX+1} --top-p {C.TOP_P_DEFAULT}",
         f"ERROR: --max-tokens must be a(n) int between {C.MAX_TOKENS_MIN} and {C.MAX_TOKENS_MAX}\n",
         1,
     ),
     CLICase(
-        f"ask how are you --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.PRESENCE_PENALTY_DEFAULT}"
+        f"ask how are you --fast --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.PRESENCE_PENALTY_DEFAULT}"
     ),
     CLICase(
-        f"ask how are you --frequency-penalty {C.FREQUENCY_PENALTY_MAX+3} --presence-penalty {C.PRESENCE_PENALTY_MAX+7.7}",
+        f"ask how are you --fast --frequency-penalty {C.FREQUENCY_PENALTY_MAX+3} --presence-penalty {C.PRESENCE_PENALTY_MAX+7.7}",
         f"ERROR: --frequency-penalty must be a(n) float between {C.FREQUENCY_PENALTY_MIN} and {C.FREQUENCY_PENALTY_MAX}\n",
         1,
     ),
     CLICase(
-        f"ask how are you --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"
+        f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"
     ),
     CLICase(
-        f"""ask how are you --max-tokens {C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"""
+        f"""ask how are you --fast --max-tokens {C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"""
     ),
     CLICase("ask --files review.py --files review.py what programming language is this code written in?"),
 ]
 
 ARGS = ROOT_COMMANDS + ASK_COMMANDS
```

### Comparing `gpt-review-0.2.3rc287.post1/PKG-INFO` & `gpt-review-0.2.3rc291.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.2.3rc287.post1
+Version: 0.2.3rc291.post1
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
-Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc287.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc291.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

