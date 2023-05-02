# Comparing `tmp/developergpt-0.2.4.tar.gz` & `tmp/developergpt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.2.4.tar", last modified: Tue Apr 25 16:13:46 2023, max compression
+gzip compressed data, was "developergpt-0.2.5.tar", last modified: Tue May  2 20:59:45 2023, max compression
```

## Comparing `developergpt-0.2.4.tar` & `developergpt-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.332788 developergpt-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 16:13:29.000000 developergpt-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-25 16:13:29.000000 developergpt-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-25 16:13:46.328788 developergpt-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 16:13:29.000000 developergpt-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.328788 developergpt-0.2.4/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-25 16:13:29.000000 developergpt-0.2.4/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.328788 developergpt-0.2.4/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 16:13:46.000000 developergpt-0.2.4/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:13:46.332788 developergpt-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-25 16:13:29.000000 developergpt-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:46.328788 developergpt-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:13:29.000000 developergpt-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 16:13:29.000000 developergpt-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 16:13:29.000000 developergpt-0.2.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 20:59:33.000000 developergpt-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 20:59:33.000000 developergpt-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-02 20:59:45.329928 developergpt-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-02 20:59:33.000000 developergpt-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-05-02 20:59:33.000000 developergpt-0.2.5/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 20:59:45.000000 developergpt-0.2.5/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:59:45.329928 developergpt-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-02 20:59:33.000000 developergpt-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:45.329928 developergpt-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:33.000000 developergpt-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 20:59:33.000000 developergpt-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-02 20:59:33.000000 developergpt-0.2.5/tests/test_cli.py
```

### Comparing `developergpt-0.2.4/LICENSE` & `developergpt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.4/PKG-INFO` & `developergpt-0.2.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: developergpt
-Version: 0.2.4
-Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
-Home-page: https://github.com/luo-anthony/DeveloperGPT/
-Author: luo-anthony
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
 
 
@@ -23,91 +12,124 @@
 By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
 In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
 **Supported Models:** GPT3.5 (default), BLOOM
+
+**Usage:** `developergpt cmd [your natural language command request]`
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
 **NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
 
 With both models, it is always good practice to manually verify the command output before running it.
 
 #### 2. Chat inside the Terminal
 **Supported Models:** GPT3.5 (default), BLOOM
+
+**Usage:** `developergpt chat`
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
 **NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
 
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
-By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. From limited testing, the GPT-3.5 model has the best results. 
 
-Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
+#### OpenAI GPT-3.5 (Default)
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use this model, you will need an OpenAI API Key.
 
+1. Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
+2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
 ```bash
-# Do this once 
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+#### BLOOM
+To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token as an environment variable using the steps below. Setting up a token is **not required (the BLOOM model will work without any token or key)**, but it will allow you to make more requests without being rate limited. 
 
 ```bash
-# Do this once 
-# set Hugging Face API token (using zsh for example)
+# [OPTIONAL] set Hugging Face API token (using zsh for example)
+# You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 ## Usage
 ```bash
 # see available commands
 $ developergpt 
 
+# give feedback
+$ developergpt feedback
+```
+
+#### Natural Language to Terminal Comands
+DeveloperGPT allows you to get and execute terminal commands using natural language. 
+```bash
+# Natural Language to Terminal Commands using OpenAI GPT-3.5 (default)
+$ developergpt cmd [your natural language command request]
+
+# Natural Language to Terminal Commands using OpenAI GPT-3.5 (default) with prompt
+$ developergpt cmd 
+
+# Example Usage
+$ developergpt cmd list all commits that contain the word "llm"
+```
+
+Use `developergpt --model bloom cmd` to use the BLOOM model instead of the GPT-3.5 model (used by default). 
+```bash
+# Natural Language to Terminal Commands using BLOOM model instead
+$ developergpt --model bloom cmd [your natural language command request]
+```
+
+Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
+```bash
+# Fast Mode (GPT-3.5): Commands are given without explanation (may be less accurate)
+$ developergpt cmd --fast [your natural language command request]
+
+# Fast Mode (BLOOM): Commands are given without explanation (may be less accurate)
+$ developergpt --model bloom cmd --fast [your natural language command request]
+```
+
+#### Chat inside the Terminal
+DeveloperGPT allows you to chat with either the GPT-3.5 model or the BLOOM model in the terminal. 
+
+```bash
 # chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
-# natural language to terminal commands using GPT-3.5 (default)
-$ developergpt cmd
-
 # chat with DeveloperGPT using BLOOM model instead
 $ developergpt --model bloom chat
-
-# natural langauge to terminal commands using BLOOM model instead
-$ developergpt --model bloom cmd
-
-# give feedback
-$ developergpt feedback
 ```
 
 **NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
-### Hugging-Face Usage (BLOOM)
+### Hugging-Face Inference API Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
-- Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
+- Add support for more open-source models (Alpaca, Vicuna, LLAMA, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.2.4/README.md` & `developergpt-0.2.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: developergpt
+Version: 0.2.5
+Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
+Home-page: https://github.com/luo-anthony/DeveloperGPT/
+Author: luo-anthony
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
 
 
@@ -12,91 +23,124 @@
 By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
 In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
 **Supported Models:** GPT3.5 (default), BLOOM
+
+**Usage:** `developergpt cmd [your natural language command request]`
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
 **NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
 
 With both models, it is always good practice to manually verify the command output before running it.
 
 #### 2. Chat inside the Terminal
 **Supported Models:** GPT3.5 (default), BLOOM
+
+**Usage:** `developergpt chat`
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
 **NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
 
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
-By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. From limited testing, the GPT-3.5 model has the best results. 
 
-Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
+#### OpenAI GPT-3.5 (Default)
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use this model, you will need an OpenAI API Key.
 
+1. Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
+2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
 ```bash
-# Do this once 
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+#### BLOOM
+To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token as an environment variable using the steps below. Setting up a token is **not required (the BLOOM model will work without any token or key)**, but it will allow you to make more requests without being rate limited. 
 
 ```bash
-# Do this once 
-# set Hugging Face API token (using zsh for example)
+# [OPTIONAL] set Hugging Face API token (using zsh for example)
+# You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 ## Usage
 ```bash
 # see available commands
 $ developergpt 
 
+# give feedback
+$ developergpt feedback
+```
+
+#### Natural Language to Terminal Comands
+DeveloperGPT allows you to get and execute terminal commands using natural language. 
+```bash
+# Natural Language to Terminal Commands using OpenAI GPT-3.5 (default)
+$ developergpt cmd [your natural language command request]
+
+# Natural Language to Terminal Commands using OpenAI GPT-3.5 (default) with prompt
+$ developergpt cmd 
+
+# Example Usage
+$ developergpt cmd list all commits that contain the word "llm"
+```
+
+Use `developergpt --model bloom cmd` to use the BLOOM model instead of the GPT-3.5 model (used by default). 
+```bash
+# Natural Language to Terminal Commands using BLOOM model instead
+$ developergpt --model bloom cmd [your natural language command request]
+```
+
+Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
+```bash
+# Fast Mode (GPT-3.5): Commands are given without explanation (may be less accurate)
+$ developergpt cmd --fast [your natural language command request]
+
+# Fast Mode (BLOOM): Commands are given without explanation (may be less accurate)
+$ developergpt --model bloom cmd --fast [your natural language command request]
+```
+
+#### Chat inside the Terminal
+DeveloperGPT allows you to chat with either the GPT-3.5 model or the BLOOM model in the terminal. 
+
+```bash
 # chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
-# natural language to terminal commands using GPT-3.5 (default)
-$ developergpt cmd
-
 # chat with DeveloperGPT using BLOOM model instead
 $ developergpt --model bloom chat
-
-# natural langauge to terminal commands using BLOOM model instead
-$ developergpt --model bloom cmd
-
-# give feedback
-$ developergpt feedback
 ```
 
 **NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
-### Hugging-Face Usage (BLOOM)
+### Hugging-Face Inference API Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
-- Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
+- Add support for more open-source models (Alpaca, Vicuna, LLAMA, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.2.4/developergpt/cli.py` & `developergpt-0.2.5/developergpt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """
 DeveloperGPT by luo-anthony
 """
 
-import copy
 import subprocess
 import sys
 from functools import wraps
 
 import click
 import inquirer
 import openai
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
-from prompt_toolkit.key_binding import KeyBindings
-from prompt_toolkit.key_binding.key_processor import KeyPressEvent
-from prompt_toolkit.keys import Keys
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich.console import Console
 
 from developergpt import config, huggingface_adapter, openai_adapter, utils
 
-console = Console()
-session: "PromptSession" = PromptSession()
+console: Console = Console()
+session: PromptSession = PromptSession()
 
 
 def handle_api_error(f):
     """Handle API errors gracefully"""
 
     @wraps(f)
     def internal(*args, **kwargs):
@@ -83,97 +79,108 @@
             "[bold yellow]Using Bloom 176B model: some features may have unexpected behavior and results may not be as good as using GPT-3.5.[/bold yellow]"
         )
 
     ctx.obj["temperature"] = temperature
     ctx.obj["model"] = model
 
 
-@click.command(help="Chat with DeveloperGPT")
+@main.command(help="Chat with DeveloperGPT")
 @click.pass_context
+@click.argument("user_input", nargs=-1)
 @handle_api_error
-def chat(ctx):
+def chat(ctx, user_input):
+    if user_input:
+        user_input = str(" ".join(user_input))
+        session.history.append_string(user_input)
+
     model = ctx.obj["model"]
 
     if model == config.GPT35:
         input_messages = [openai_adapter.INITIAL_CHAT_SYSTEM_MSG]
     elif model == config.BLOOM:
         input_messages = huggingface_adapter.BASE_INPUT_CHAT_MSGS
         api_token = ctx.obj.get("api_key", None)
     console.print("[gray]Type 'quit' to exit the chat[/gray]")
     while True:
-        user_input = utils.prompt_user_input(
-            "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
-        )
+        if not user_input:
+            user_input = utils.prompt_user_input(
+                "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
+            )
 
-        if len(user_input) == 0:
+        if not user_input:
             continue
 
         if model == config.GPT35:
             input_messages = openai_adapter.get_model_chat_response(
                 user_input, console, input_messages, ctx.obj["temperature"]
             )
         elif model == config.BLOOM:
             input_messages = huggingface_adapter.get_model_chat_response(
                 user_input, console, input_messages, api_token
             )
 
-
-kb = KeyBindings()
-
-
-@kb.add(Keys.Enter, eager=True)
-def _(event: KeyPressEvent):
-    buff = event.app.current_buffer
-    if buff.complete_state:
-        # during completion, enter will select the current completion instead of submitting input
-        if buff.complete_state.current_completion:
-            buff.apply_completion(buff.complete_state.current_completion)
-            return  # don't submit input
-    buff.validate_and_handle()
+        user_input = None
 
 
-@click.command(help="Execute commands using natural language")
+@main.command(help="Execute commands using natural language")
+@click.argument("user_input", nargs=-1)
+@click.option(
+    "--fast",
+    is_flag=True,
+    default=False,
+    help="Get commands without command or argument explanations (less accurate)",
+)
 @click.pass_context
 @handle_api_error
-def cmd(ctx):
+def cmd(ctx, user_input, fast):
     input_request = "\nDesired Command Request: "
 
-    model = ctx.obj["model"]
-    input_messages = copy.deepcopy(openai_adapter.BASE_INPUT_CMD_MSGS)
+    if fast:
+        console.print(
+            "[bold yellow]Using Fast Mode: Commands are given without explanation and may be less accurate[/bold yellow]"
+        )
 
-    console.print("[gray]Type 'quit' to exit[/gray]")
+    if user_input:
+        user_input = str(" ".join(user_input))
+        session.history.append_string(user_input)
+
+    model = ctx.obj["model"]
 
     if model == config.BLOOM:
         console.print(
             "[bold yellow]WARNING: Bloom 176B model command outputs are less accurate than GPT-3.5. Check all commands before running them.[/bold yellow]"
         )
         api_token = ctx.obj.get("api_key", None)
 
+    if not user_input:
+        console.print("[gray]Type 'quit' to exit[/gray]")
+
     while True:
-        user_input = utils.prompt_user_input(
-            input_request,
-            session,
-            console,
-            completer=utils.PathCompleter(),
-            complete_style=CompleteStyle.MULTI_COLUMN,
-            key_bindings=kb,
-        )
-        if len(user_input) == 0:
+        if not user_input:
+            user_input = utils.prompt_user_input(
+                input_request,
+                session,
+                console,
+                completer=utils.PathCompleter(),
+                complete_style=CompleteStyle.MULTI_COLUMN,
+                key_bindings=config.kb,
+            )
+
+        if not user_input:
             continue
 
         if model == config.GPT35:
-            model_output = openai_adapter.model_command(
-                user_input, console, input_messages
-            )
+            model_output = openai_adapter.model_command(user_input, console, fast)
         elif model == config.BLOOM:
             model_output = huggingface_adapter.model_command(
-                user_input, console, api_token
+                user_input, console, api_token, fast
             )
+        user_input = None  # clear input for next iteration
 
-        commands = utils.print_command_response(model_output, console)
+        commands = utils.print_command_response(model_output, console, fast, model)
         if not commands:
             continue
 
         # Give user options to revise query, execute command(s), or quit
         options = [
             "Revise Query",
             "Execute Command(s)",
@@ -194,47 +201,38 @@
             for idx, cmd in enumerate(commands):
                 if cmd:
                     console.print(
                         f"""[bold blue]Executing Command [{idx+1}]: {cmd}[/bold blue]"""
                     )
                     subprocess.run(cmd, shell=True)
 
-            console.print(
-                "[bold blue]Copied executed command(s) to clipboard[/bold blue]"
-            )
-            utils.copy_comands_to_cliboard(commands)
         elif selected_option == "Copy Command(s) to Clipboard":
             utils.copy_comands_to_cliboard(commands)
             console.print("[bold blue]Copied command(s) to clipboard[/bold blue]")
         else:
             console.print("[bold blue]Exiting...\n[/bold blue]")
 
         sys.exit(0)
 
 
-@click.command()
+# @main.command()
 @click.pass_context
 def test(ctx):
     pass
     # while True:
     #     user_input = utils.prompt_user_input(
     #         "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
     #     )
 
     #     if len(user_input) == 0:
     #         continue
 
 
-@click.command(help="Give feedback")
+@main.command(help="Give feedback")
 def feedback():
     console.print(
-        "Thanks for using DeveloperGPT! You can [bold blue][link=https://forms.gle/J36KbztsRAPHXnrKA]give feedback here[/link][/bold blue]!"
+        f"Thanks for using DeveloperGPT! You can [bold blue][link={config.FEEDBACK_LINK}]give feedback here[/link][/bold blue]!"
     )
 
 
-main.add_command(cmd)
-main.add_command(chat)
-main.add_command(feedback)
-# main.add_command(test)
-
 if __name__ == "__main__":
     main()
```

### Comparing `developergpt-0.2.4/developergpt/huggingface_adapter.py` & `developergpt-0.2.5/developergpt/huggingface_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,105 +1,88 @@
 """
 DeveloperGPT by luo-anthony
 """
 
-import copy
-import platform
 import re
 import sys
 
 import requests
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 # using: https://pypi.org/project/text-generation/
 from text_generation import InferenceAPIClient, errors
 
-from developergpt import config
+from developergpt import config, few_shot_prompts
 
-# TODO: add more hugging_face models: flan-ul2, Vicuna-13B?
-
-
-# TODO change the output format so that it doesn't use JSON and we don't need to deal with weird escaping issues with regex output
 BLOOM_CMD_PROMPT = """The following is a software development command line system that allows a user to get the command(s) to execute their request in natural language. 
-    The system gives the user a series of commands to be executed for the given platform in JSON format with explanations.\n"""
+    The system gives the user a series of commands to be executed for the given platform in Markdown format (escaping any special Markdown characters with \) along with explanations.\n"""
+TIMEOUT: int = 25  # seconds
 
-conda_output_example = """
-    {
-        "error": 0,
-        "commands": [
-            {
-                "cmd_to_execute": "curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh",
-                "cmd_explanations": ["The `curl` command is used to issue web requests, e.g. download web pages."],
-                "arg_explanations": [
-                                        "`-O` specifies that we want to save the response to a file.",
-                                        "`https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh` is the URL of the file we want to download."
-                                    ]
-            },
-            {
-                "cmd_to_execute": "bash Miniconda3-latest-MacOSX-x86_64.sh",
-                "cmd_explanations": ["The `bash` command is used to execute shell scripts."],
-                "arg_explanations": ["`Miniconda3-latest-MacOSX-x86_64.sh` is the name of the file we want to execute."]
-            }
-        ]
-    }
-"""
 
-search_output_example = """
-    {
-        "error" : 0,
-        "commands": [
-            {
-                "cmd_to_execute": "find ~/Documents/ -name 'test*.py'",
-                "cmd_explanations": ["`find` is used to list files."],
-                "arg_explanations": [
-                                        "``~/Documents` specifies the folder to search in.",
-                                        "`-name 'test.py'` specifies that we want to search for files starting with `test` and ending with `.py`."
-                                    ]
-            }
-        ]
-    }
-    """
+def format_user_cmd_request(
+    user_input: str, platform: str = config.USER_PLATFORM
+) -> str:
+    user_input.replace('"', "'")
+    return f"""User: Provide appropriate command-line commands that can be executed on a {platform} machine to: {user_input}."""
 
-unknown_query_output_example_one = """{"error": 1}"""
 
+def format_user_input(user_input: str) -> str:
+    return f"""User: {user_input}"""
 
-def format_user_cmd_request(user_input: str) -> str:
-    user_input.replace('"', "'")
-    return f"""User: Provide appropriate command-line commands that can be executed on a {platform.platform()} machine to: {user_input}."""
+
+def format_assistant_output(output: str) -> str:
+    return f"""Assistant: {output}"""
 
 
 BLOOM_EXAMPLE_CMDS = [
-    format_user_cmd_request("install conda"),
-    f"""Assistant: {conda_output_example}""",
     format_user_cmd_request(
-        "search ~/Documents directory for any .py file that begins with 'test'"
+        few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_output(few_shot_prompts.CONDA_OUTPUT_EXAMPLE),
+    format_user_cmd_request(
+        few_shot_prompts.SEARCH_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
-    f"""Assistant: {search_output_example}""",
+    format_assistant_output(few_shot_prompts.SEARCH_OUTPUT_EXAMPLE),
 ]
 
-
-TIMEOUT = 25  # seconds
+BLOOM_EXAMPLE_CMDS_FAST = [
+    format_user_cmd_request(
+        few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_output(few_shot_prompts.CONDA_OUTPUT_EXAMPLE_MARKDOWN),
+    format_user_cmd_request(
+        few_shot_prompts.SEARCH_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_output(few_shot_prompts.SEARCH_OUTPUT_EXAMPLE_MARKDOWN),
+    format_user_cmd_request(
+        few_shot_prompts.PROCESS_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_output(few_shot_prompts.PROCESS_OUTPUT_EXAMPLE_MARKDOWN),
+]
 
 
-def model_command(user_input: str, console: "Console", api_token: str) -> str:
-    model = "bigscience/bloom"
-    client = InferenceAPIClient(model, token=api_token, timeout=TIMEOUT)
+def model_command(
+    user_input: str, console: Console, api_token: str, fast_mode: bool
+) -> str:
+    MODEL = "bigscience/bloom"
+    client = InferenceAPIClient(MODEL, token=api_token, timeout=TIMEOUT)
     MAX_RESPONSE_TOKENS = 384
-
-    messages = copy.deepcopy(BLOOM_EXAMPLE_CMDS)
+    if fast_mode:
+        messages = list(BLOOM_EXAMPLE_CMDS_FAST)
+    else:
+        messages = list(BLOOM_EXAMPLE_CMDS)
     messages.append(format_user_cmd_request(user_input))
 
     model_input = model_input = (
         BLOOM_CMD_PROMPT + "\n" + "\n".join(messages) + "\nAssistant:"
     )
 
-    # console.log(model_input)
     with console.status("[bold blue]Decoding request") as _:
         try:
             exit = False
             output_text = ""
             for response in client.generate_stream(
                 model_input, max_new_tokens=MAX_RESPONSE_TOKENS
             ):
@@ -135,15 +118,15 @@
 
 
 BLOOM_CHAT_PROMPT = """The following is a conversation with a software development expert chatbot. 
     The chatbot should be able to understand and respond to questions and statements about a variety of topics related to Computer Science and Software Development. 
     The chatbot is conversational, flexible, and should be able to engage in casual, friendly conversation to assist the user.
     The chatbot should also be able to maintain context across multiple turns of conversation.\n"""
 
-raw_chat_msgs = [
+RAW_CHAT_MSGS = [
     "User: What is the difference between x86 and ARM architecture?",
     """Assistant: x86 and ARM are two different processor architectures used in modern computing devices. They have different instruction sets, 
     with x86 using a CISC instruction set and ARM using a RISC instruction set. x86 processors typically have higher clock speeds and can execute more instructions per clock cycle, while ARM processors are more power-efficient.
     x86 processors are compatible with a wide range of operating systems, while ARM processors are commonly used in mobile devices and are generally less expensive than x86 processors.""",
     "User: What are LDFLAGS in a Makefile?",
     """Assistant, LDFLAGS is a variable used in Makefiles that contains linker flags or options to pass to the linker program. 
     Linker flags control the behavior of the linker, which is responsible for linking together object files into an executable or library file. 
@@ -162,35 +145,27 @@
     ```""",
     "User: What is JIT?",
     """Assistant: A JIT (Just-In-Time) compiler is a type of compiler used in some programming languages that compiles code during runtime, rather than before the program is run. 
     JIT compilers can optimize the code based on the actual runtime behavior of the program, resulting in faster execution times. 
     JIT compilers are commonly used in languages such as Java, JavaScript, and .NET.""",
 ]
 
-BASE_INPUT_CHAT_MSGS = [re.sub(" +", " ", msg) for msg in raw_chat_msgs]
+BASE_INPUT_CHAT_MSGS = [re.sub(" +", " ", msg) for msg in RAW_CHAT_MSGS]
 
 
 def format_bloom_chat_input(messages: list) -> str:
     model_input = BLOOM_CHAT_PROMPT + "\n" + "\n".join(messages) + "\nAssistant:"
     return model_input
 
 
-def format_user_input(user_input: str) -> str:
-    return f"""User: {user_input}"""
-
-
-def format_assistant_output(output: str) -> str:
-    return f"""Assistant: {output}"""
-
-
 def get_model_chat_response(
-    user_input: str, console: "Console", input_messages: list, api_token: str
+    user_input: str, console: Console, input_messages: list, api_token: str
 ) -> list:
-    model = "bigscience/bloom"
-    client = InferenceAPIClient(model, token=api_token, timeout=TIMEOUT)
+    MODEL = "bigscience/bloom"
+    client = InferenceAPIClient(MODEL, token=api_token, timeout=TIMEOUT)
     MAX_RESPONSE_TOKENS = 384
 
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
 
     input_messages.append(format_user_input(user_input))
 
     model_input = format_bloom_chat_input(input_messages)
```

### Comparing `developergpt-0.2.4/developergpt/openai_adapter.py` & `developergpt-0.2.5/developergpt/openai_adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 DeveloperGPT by luo-anthony
 """
-import platform
 import sys
 from datetime import datetime
 
 import openai
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
-from developergpt import config, utils
+from developergpt import config, few_shot_prompts, utils
 
-json_cmd_format = """
+JSON_CMD_FORMAT = """
     {
         "input": "<user input>",
         "error": 0,
         "commands": [
             {
                 "seq": <Order of Command>,
                 "cmd_to_execute": "<commands and arguments to execute>",
@@ -30,138 +29,139 @@
                 "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
                 "arg_explanations": ["<explanation of argument 1>", "<explanation of argument 2>", ...]
             }
         ]
     }
     """
 
-json_invalid_format = """{"input": "<user input>", "error": 1}"""
-
-conda_output_example = """
+JSON_CMD_FORMAT_FAST = """
     {
-        "input": "install conda",
-        "error": 0,
-        "commands": [
-            {
-                "seq": 1,
-                "cmd_to_execute": "curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh",
-                "cmd_explanations": ["The `curl` command is used to issue web requests, e.g. download web pages."],
-                "arg_explanations": [
-                                        "`-O` specifies that we want to save the response to a file.",
-                                        "`https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh` is the URL of the file we want to download."
-                                    ]
-            },
-            {
-                "seq": 2,
-                "cmd_to_execute": "bash Miniconda3-latest-MacOSX-x86_64.sh",
-                "cmd_explanations": ["The `bash` command is used to execute shell scripts."],
-                "arg_explanations": ["`Miniconda3-latest-MacOSX-x86_64.sh` is the name of the file we want to execute."]
-            }
-        ]
+        "commands": ["<commands and arguments to execute>", "<commands and arguments to execute>", ...]
     }
     """
 
-search_output_example = """
-    {
-        "input": "search the ~/Documents/ directory for any .py file that begins with 'test'",
-        "error" : 0,
-        "commands": [
-            {
-                "seq": 1,
-                "cmd_to_execute": "find ~/Documents/ -name 'test*.py'",
-                "cmd_explanations": ["`find` is used to list files."],
-                "arg_explanations": [
-                                        "``~/Documents` specifies the folder to search in.",
-                                        "`-name 'test.py'` specifies that we want to search for files starting with `test` and ending with `.py`."
-                                    ]
-            }
-        ]
-    }
-    """
+JSON_INVALID_FORMAT = """{"input": "<user input>", "error": 1}"""
 
-unknown_query_output_example_one = (
-    """{"input": "the quick brown fox jumped over", "error": 1}"""
-)
+JSON_INVALID_FORMAT_FAST = """{"error": 1}"""
 
 INITIAL_CHAT_SYSTEM_MSG = {
     "role": "system",
     "content": f"""
-                You are DeveloperGPT, a helpful personal assistant for a programmer working on a {platform.platform()} machine. 
+                You are DeveloperGPT, a helpful personal assistant for a programmer working on a {config.USER_PLATFORM} machine. 
                 Your task is to assist the programmer with any programming-related tasks they may have. 
                 This could include providing advice on how to approach a programming problem, suggesting tools or libraries to use for a particular task, 
                 helping to troubleshoot errors or bugs in code, answering general programming questions, and providing code snippets or examples.
 
                 Please keep your answers short and concise and use a suitable format for printing on the terminal. 
                 If you provide code snippets, use ```<language> to specify the language. 
             """,
 }
 
 INITIAL_CMD_SYSTEM_MSG = {
     "role": "system",
     "content": f"""
-            As an assistant for a programmer on a {platform.platform()} machine, your task is to provide the appropriate command-line commands to execute a user request.
+            As an assistant for a programmer on a {config.USER_PLATFORM} machine, your task is to provide the appropriate command-line commands to execute a user request.
             """,
 }
 
-INITIAL_USER_CMD_MSG = {
-    "role": "user",
-    "content": f"""
-            Provide the appropriate command-line commands that can be executed on a {platform.platform()} machine for a user request.
-            Today's date/time is {datetime.now().strftime('%Y-%m-%d %H:%M:%S')}.
-            If the request is possible, please provide commands that can be executed in the command line and do not require a GUI.
-            Do not include commands that require a yes/no response.
-            For each command, explain the command and any arguments used.
-            Try to find the simplest command(s) that can be used to execute the request.
 
-            If the request is valid, format each command output in the following JSON format: {json_cmd_format}
+def format_initial_cmd_msg(cmd_format: str, invalid_format: str) -> dict:
+    return {
+        "role": "user",
+        "content": f"""
+                Provide the appropriate command-line commands that can be executed on a {config.USER_PLATFORM} machine for a user request.
+                Today's date/time is {datetime.now().strftime('%Y-%m-%d %H:%M:%S')}.
+                If the request is possible, please provide commands that can be executed in the command line and do not require a GUI.
+                Do not include commands that require a yes/no response.
+                For each command, explain the command and any arguments used.
+                Try to find the simplest command(s) that can be used to execute the request.
+
+                If the request is valid, format each command output in the following JSON format: {cmd_format}
 
-            If the request is invalid, please return the following JSON format: {json_invalid_format}
-            """,
-}
+                If the request is invalid, please return the following JSON format: {invalid_format}
+                """,
+    }
 
 
-def format_user_request(user_request: str) -> dict:
+INITIAL_USER_CMD_MSG = format_initial_cmd_msg(JSON_CMD_FORMAT, JSON_INVALID_FORMAT)
+
+INITIAL_USER_CMD_MSG_FAST = format_initial_cmd_msg(
+    JSON_CMD_FORMAT_FAST, JSON_INVALID_FORMAT_FAST
+)
+
+
+def format_user_request(
+    user_request: str, platform: str = config.USER_PLATFORM
+) -> dict:
     return {
         "role": "user",
-        "content": f"""Provide the appropriate command-line commands that can be executed on a {platform.platform()} machine for the user request: "{user_request}".""",
+        "content": f"""Provide the appropriate command-line commands that can be executed on a {platform} machine for the user request: "{user_request}".""",
     }
 
 
 def format_assistant_response(assistant_response: str) -> dict:
     return {"role": "assistant", "content": assistant_response}
 
 
-EXAMPLE_ONE = (
-    format_user_request("install conda"),
-    format_assistant_response(conda_output_example),
-)
-
-EXAMPLE_TWO = (
+BASE_INPUT_CMD_MSGS = [
+    INITIAL_CMD_SYSTEM_MSG,
+    INITIAL_USER_CMD_MSG,
     format_user_request(
-        "search ~/Documents directory for any .py file that begins with 'test'"
+        few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
-    format_assistant_response(search_output_example),
-)
-
-NEGATIVE_EXAMPLE_ONE = (
-    format_user_request("the quick brown fox jumped over"),
-    format_assistant_response(unknown_query_output_example_one),
-)
+    format_assistant_response(few_shot_prompts.CONDA_OUTPUT_EXAMPLE),
+    format_user_request(
+        few_shot_prompts.SEARCH_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_response(
+        few_shot_prompts.SEARCH_OUTPUT_EXAMPLE,
+    ),
+    format_user_request(
+        few_shot_prompts.UNKNOWN_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_response(
+        few_shot_prompts.UNKNOWN_QUERY_OUTPUT_EXAMPLE_ONE,
+    ),
+]
 
-BASE_INPUT_CMD_MSGS = [
+BASE_INPUT_CMD_MSGS_FAST = [
     INITIAL_CMD_SYSTEM_MSG,
-    INITIAL_USER_CMD_MSG,
-    *EXAMPLE_ONE,
-    *EXAMPLE_TWO,
-    *NEGATIVE_EXAMPLE_ONE,
+    INITIAL_USER_CMD_MSG_FAST,
+    format_user_request(
+        few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_response(
+        few_shot_prompts.CONDA_OUTPUT_EXAMPLE_FAST,
+    ),
+    format_user_request(
+        few_shot_prompts.SEARCH_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_response(
+        few_shot_prompts.SEARCH_OUTPUT_EXAMPLE_FAST,
+    ),
+    format_user_request(
+        few_shot_prompts.PROCESS_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_response(
+        few_shot_prompts.PROCESS_OUTPUT_EXAMPLE_FAST,
+    ),
+    format_user_request(
+        few_shot_prompts.UNKNOWN_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
+    ),
+    format_assistant_response(
+        few_shot_prompts.UNKNOWN_QUERY_OUTPUT_EXAMPLE_ONE_FAST,
+    ),
 ]
 
 
 def get_model_chat_response(
-    user_input: str, console: "Console", input_messages: list, temperature: float
+    user_input: str,
+    console: Console,
+    input_messages: list,
+    temperature: float,
 ) -> list:
     MODEL = "gpt-3.5-turbo"
     MAX_TOKENS = 4000
     RESERVED_OUTPUT_TOKENS = 1024
     MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
 
     input_messages.append({"role": "user", "content": user_input})
@@ -193,25 +193,30 @@
             msg = chunk["choices"][0]["delta"].get("content", "")
             collected_messages.append(msg)
             output_panel.renderable = Markdown(
                 "".join(collected_messages), inline_code_theme="monokai"
             )
 
     full_response = "".join(collected_messages)
-    input_messages.append({"role": "assistant", "content": full_response})
+    input_messages.append(format_assistant_response(full_response))
     return input_messages
 
 
-def model_command(user_input: str, console: "Console", input_messages: list) -> list:
+def model_command(user_input: str, console: Console, fast_mode: bool) -> list:
     MODEL = "gpt-3.5-turbo"
     MAX_TOKENS = 4000
     RESERVED_OUTPUT_TOKENS = 1024
     MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
     TEMP = 0.05
 
+    if fast_mode:
+        input_messages = list(BASE_INPUT_CMD_MSGS_FAST)
+    else:
+        input_messages = list(BASE_INPUT_CMD_MSGS)
+
     input_messages.append(format_user_request(user_input))
 
     n_input_tokens = utils.count_msg_tokens(input_messages, MODEL)
 
     if n_input_tokens > MAX_INPUT_TOKENS:
         input_messages, n_input_tokens = utils.remove_old_contexts(
             input_messages,
@@ -241,18 +246,7 @@
     try:
         _ = openai.Model.list()
     except openai.error.AuthenticationError:
         console.print(
             f"[bold red]Error: Invalid OpenAI API key. Check your {config.OPEN_AI_API_KEY} environment variable.[/bold red]"
         )
         sys.exit(-1)
-
-
-# def format_model_output(text: str) -> str:
-#     """Format the model output to be more readable."""
-#     text = re.sub(
-#         r"```(.+?)```", "[syntax]" + r"\1" + "[/syntax]", text, flags=re.DOTALL
-#     )
-#     text = re.sub(r"`(.+?)`", "[syntax]" + r"\1" +
-#                   "[/syntax]", text, flags=re.DOTALL)
-#     text.replace("```", "[syntax]")
-#     return text
```

### Comparing `developergpt-0.2.4/developergpt/utils.py` & `developergpt-0.2.5/developergpt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 import json
 import os
 import sys
 
 import pyperclip
 import requests
 import tiktoken
+from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import Completer, Completion
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config
 
 
-def pretty_print_commands(commands: list, console: "Console", panel_width: int):
+def pretty_print_commands(commands: list, console: Console, panel_width: int) -> None:
     # print all the commands in a panel
     commands_format = "\n\n".join([f"""- `{c}`""" for c in commands])
 
     cmd_out = Markdown(
         commands_format,
         inline_code_lexer="bash",
     )
@@ -33,73 +34,86 @@
             title="[bold blue]Command(s)[/bold blue]",
             title_align="left",
             width=panel_width,
         )
     )
 
 
-def print_command_response(model_output: str, console: "Console"):
+def print_command_response(
+    model_output: str, console: Console, fast_mode: bool, model: str
+) -> list:
     if not model_output:
         return []
 
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
 
-    try:
-        output_data = json.loads(model_output)
-    except json.decoder.JSONDecodeError:
-        console.print(
-            "[bold red]Error: Could not parse model response properly[/bold red]"
-        )
-        console.log(model_output)
-        return []
-
-    if output_data.get("error", 0) or "commands" not in output_data:
-        console.print(
-            "[bold red]Error: Could not find commands for this request[/bold red]"
-        )
-        return []
-
-    commands = output_data.get("commands", {})
-    cmd_strings = [cmd.get("cmd_to_execute", "") for cmd in commands]
+    if fast_mode and model == config.BLOOM:
+        cmd_strings = model_output.split("`\n")
+        cmd_strings = [c.replace("`", "") for c in cmd_strings]
+    else:
+        try:
+            output_data = json.loads(model_output)
+        except json.decoder.JSONDecodeError:
+            console.print(
+                "[bold red]Error: Could not parse model response properly[/bold red]"
+            )
+            console.log(model_output)
+            return []
+
+        if output_data.get("error", 0) or "commands" not in output_data:
+            console.print(
+                "[bold red]Error: Could not find commands for this request[/bold red]"
+            )
+            return []
+        commands = output_data.get("commands", {})
+        if fast_mode:
+            cmd_strings = commands
+        else:
+            cmd_strings = [cmd.get("cmd_to_execute", "") for cmd in commands]
 
     # print all the commands in a panel
     pretty_print_commands(cmd_strings, console, panel_width)
 
-    # print all the explanations in a panel
-    explanation_items = []
-    for cmd in commands:
-        explanation_items.extend([f"- {c}" for c in cmd.get("cmd_explanations", [])])
-        explanation_items.extend([f"\t- {c}" for c in cmd.get("arg_explanations", [])])
+    if not fast_mode:
+        # print all the explanations in a panel
+        explanation_items = []
+        for cmd in commands:
+            explanation_items.extend(
+                [f"- {c}" for c in cmd.get("cmd_explanations", [])]
+            )
+            explanation_items.extend(
+                [f"\t- {c}" for c in cmd.get("arg_explanations", [])]
+            )
 
-    arg_out = Markdown("\n".join(explanation_items))
+        arg_out = Markdown("\n".join(explanation_items))
 
-    console.print(
-        Panel(
-            arg_out,
-            title="[bold blue]Explanation[/bold blue]",
-            title_align="left",
-            width=panel_width,
+        console.print(
+            Panel(
+                arg_out,
+                title="[bold blue]Explanation[/bold blue]",
+                title_align="left",
+                width=panel_width,
+            )
         )
-    )
     return cmd_strings
 
 
 def copy_comands_to_cliboard(commands: list):
     pyperclip.copy("\n".join(commands))
 
 
 def prompt_user_input(
-    input_request,
-    session,
-    console,
+    input_request: str,
+    session: PromptSession,
+    console: Console,
     completer=None,
     complete_style=None,
     auto_suggest=None,
     key_bindings=None,
-):
+) -> str:
     user_input = session.prompt(
         input_request,
         style=config.INPUT_STYLE,
         completer=completer,
         complete_style=complete_style,
         auto_suggest=auto_suggest,
         key_bindings=key_bindings,
@@ -113,15 +127,15 @@
         sys.exit(0)
 
     return user_input
 
 
 def check_reduce_context(
     messages: list, token_limit: int, model: str, ctx_removal_index: int
-) -> tuple[list, int]:
+) -> tuple:
     """Check if token limit is exceeded and remove old context starting at ctx_removal_index if so."""
     n_tokens = count_msg_tokens(messages, model)
     if n_tokens > token_limit:
         messages, n_tokens = remove_old_contexts(
             messages, token_limit, n_tokens, model, ctx_removal_index
         )
     return messages, n_tokens
@@ -168,15 +182,15 @@
                 num_tokens += tokens_per_name
     num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
 
 
 def remove_old_contexts(
     messages: list, token_limit: int, n_tokens: int, model: str, ctx_removal_index: int
-) -> tuple[list, int]:
+) -> tuple:
     """Remove old contexts until token limit is not exceeded."""
     while n_tokens > token_limit:
         removed_ctx = messages.pop(ctx_removal_index)
         n_removed = count_msg_tokens([removed_ctx], model)
         n_tokens -= n_removed
 
     return messages, n_tokens
@@ -228,13 +242,13 @@
                 yield Completion(
                     completion,
                     display=os.path.basename(completion),
                     start_position=-len(text),
                 )
 
 
-def check_connectivity(url="http://www.google.com", timeout=8):
+def check_connectivity(url: str = "http://www.google.com", timeout: int = 8) -> bool:
     try:
         _ = requests.get(url, timeout=timeout)
         return True
     except requests.ConnectionError:
         return False
```

### Comparing `developergpt-0.2.4/developergpt.egg-info/PKG-INFO` & `developergpt-0.2.5/developergpt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.2.4
+Version: 0.2.5
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -23,91 +23,124 @@
 By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI (requires an OpenAI API Key), but it also supports the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Using BLOOM with DeveloperGPT is **completely free** and does **not require an API key** (rate-limited) thanks to the Hugging Face Inference API. 
 
 In our testing, GPT-3.5 (default) generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
 **Supported Models:** GPT3.5 (default), BLOOM
+
+**Usage:** `developergpt cmd [your natural language command request]`
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
 **NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
 
 With both models, it is always good practice to manually verify the command output before running it.
 
 #### 2. Chat inside the Terminal
 **Supported Models:** GPT3.5 (default), BLOOM
+
+**Usage:** `developergpt chat`
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
 **NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
 
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
-By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. From limited testing, the GPT-3.5 model has the best results. 
 
-Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
+#### OpenAI GPT-3.5 (Default)
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. To use this model, you will need an OpenAI API Key.
 
+1. Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
+2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
 ```bash
-# Do this once 
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+#### BLOOM
+To use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token as an environment variable using the steps below. Setting up a token is **not required (the BLOOM model will work without any token or key)**, but it will allow you to make more requests without being rate limited. 
 
 ```bash
-# Do this once 
-# set Hugging Face API token (using zsh for example)
+# [OPTIONAL] set Hugging Face API token (using zsh for example)
+# You only need to do this once
 $ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 ## Usage
 ```bash
 # see available commands
 $ developergpt 
 
+# give feedback
+$ developergpt feedback
+```
+
+#### Natural Language to Terminal Comands
+DeveloperGPT allows you to get and execute terminal commands using natural language. 
+```bash
+# Natural Language to Terminal Commands using OpenAI GPT-3.5 (default)
+$ developergpt cmd [your natural language command request]
+
+# Natural Language to Terminal Commands using OpenAI GPT-3.5 (default) with prompt
+$ developergpt cmd 
+
+# Example Usage
+$ developergpt cmd list all commits that contain the word "llm"
+```
+
+Use `developergpt --model bloom cmd` to use the BLOOM model instead of the GPT-3.5 model (used by default). 
+```bash
+# Natural Language to Terminal Commands using BLOOM model instead
+$ developergpt --model bloom cmd [your natural language command request]
+```
+
+Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
+```bash
+# Fast Mode (GPT-3.5): Commands are given without explanation (may be less accurate)
+$ developergpt cmd --fast [your natural language command request]
+
+# Fast Mode (BLOOM): Commands are given without explanation (may be less accurate)
+$ developergpt --model bloom cmd --fast [your natural language command request]
+```
+
+#### Chat inside the Terminal
+DeveloperGPT allows you to chat with either the GPT-3.5 model or the BLOOM model in the terminal. 
+
+```bash
 # chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
-# natural language to terminal commands using GPT-3.5 (default)
-$ developergpt cmd
-
 # chat with DeveloperGPT using BLOOM model instead
 $ developergpt --model bloom chat
-
-# natural langauge to terminal commands using BLOOM model instead
-$ developergpt --model bloom cmd
-
-# give feedback
-$ developergpt feedback
 ```
 
 **NOTE:** DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
-### Hugging-Face Usage (BLOOM)
+### Hugging-Face Inference API Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
-- Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
+- Add support for more open-source models (Alpaca, Vicuna, LLAMA, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
```

### Comparing `developergpt-0.2.4/developergpt.egg-info/SOURCES.txt` & `developergpt-0.2.5/developergpt.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.py
 developergpt/VERSION
 developergpt/__init__.py
 developergpt/__main__.py
 developergpt/cli.py
 developergpt/config.py
+developergpt/few_shot_prompts.py
 developergpt/huggingface_adapter.py
 developergpt/openai_adapter.py
 developergpt/utils.py
 developergpt.egg-info/PKG-INFO
 developergpt.egg-info/SOURCES.txt
 developergpt.egg-info/dependency_links.txt
 developergpt.egg-info/entry_points.txt
```

### Comparing `developergpt-0.2.4/setup.py` & `developergpt-0.2.5/setup.py`

 * *Files identical despite different names*

