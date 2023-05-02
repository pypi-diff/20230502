# Comparing `tmp/blackboxopt-4.9.0.tar.gz` & `tmp/blackboxopt-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxopt-4.9.0.tar", max compression
+gzip compressed data, was "blackboxopt-4.9.1.tar", max compression
```

## Comparing `blackboxopt-4.9.0.tar` & `blackboxopt-4.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11476 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/LICENSE
--rw-r--r--   0        0        0     4392 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/README.md
--rw-r--r--   0        0        0      346 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/__init__.py
--rw-r--r--   0        0        0     8378 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/base.py
--rw-r--r--   0        0        0     7044 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/evaluation.py
--rw-r--r--   0        0        0     1408 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/examples/dask_distributed.py
--rw-r--r--   0        0        0        0 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimization_loops/__init__.py
--rw-r--r--   0        0        0     6094 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimization_loops/dask_distributed.py
--rw-r--r--   0        0        0     4814 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimization_loops/sequential.py
--rw-r--r--   0        0        0     2370 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimization_loops/testing.py
--rw-r--r--   0        0        0     3677 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimization_loops/utils.py
--rw-r--r--   0        0        0        0 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/__init__.py
--rw-r--r--   0        0        0     5209 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/bohb.py
--rw-r--r--   0        0        0    22290 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/botorch_base.py
--rw-r--r--   0        0        0     3151 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/hyperband.py
--rw-r--r--   0        0        0     1822 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/random_search.py
--rw-r--r--   0        0        0     1488 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/space_filling.py
--rw-r--r--   0        0        0        0 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/__init__.py
--rw-r--r--   0        0        0    18551 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/bohb.py
--rw-r--r--   0        0        0     1276 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/configuration_sampler.py
--rw-r--r--   0        0        0     2284 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/hyperband.py
--rw-r--r--   0        0        0     6471 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/iteration.py
--rw-r--r--   0        0        0     4572 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/optimizer.py
--rw-r--r--   0        0        0     2636 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/staged/utils.py
--rw-r--r--   0        0        0    15463 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/optimizers/testing.py
--rw-r--r--   0        0        0        0 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/py.typed
--rw-r--r--   0        0        0     3393 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/utils.py
--rw-r--r--   0        0        0        0 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/visualizations/__init__.py
--rw-r--r--   0        0        0     1869 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/visualizations/to_html_patch.js
--rw-r--r--   0        0        0     7092 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/visualizations/utils.py
--rw-r--r--   0        0        0    20427 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/blackboxopt/visualizations/visualizer.py
--rw-r--r--   0        0        0     3200 2023-02-10 10:25:08.000000 blackboxopt-4.9.0/pyproject.toml
--rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 blackboxopt-4.9.0/setup.py
--rw-r--r--   0        0        0     6443 1970-01-01 00:00:00.000000 blackboxopt-4.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11476 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/LICENSE
+-rw-r--r--   0        0        0     4392 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/README.md
+-rw-r--r--   0        0        0      346 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/__init__.py
+-rw-r--r--   0        0        0     8378 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/base.py
+-rw-r--r--   0        0        0     7044 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/evaluation.py
+-rw-r--r--   0        0        0     1408 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/examples/dask_distributed.py
+-rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/__init__.py
+-rw-r--r--   0        0        0     6094 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/dask_distributed.py
+-rw-r--r--   0        0        0     4814 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/sequential.py
+-rw-r--r--   0        0        0     2370 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/testing.py
+-rw-r--r--   0        0        0     3677 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimization_loops/utils.py
+-rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/__init__.py
+-rw-r--r--   0        0        0     5209 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/bohb.py
+-rw-r--r--   0        0        0    22290 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/botorch_base.py
+-rw-r--r--   0        0        0     3151 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/hyperband.py
+-rw-r--r--   0        0        0     1822 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/random_search.py
+-rw-r--r--   0        0        0     1488 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/space_filling.py
+-rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/__init__.py
+-rw-r--r--   0        0        0    18551 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/bohb.py
+-rw-r--r--   0        0        0     1276 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/configuration_sampler.py
+-rw-r--r--   0        0        0     2284 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/hyperband.py
+-rw-r--r--   0        0        0     6471 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/iteration.py
+-rw-r--r--   0        0        0     4572 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/optimizer.py
+-rw-r--r--   0        0        0     2636 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/staged/utils.py
+-rw-r--r--   0        0        0    15463 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/optimizers/testing.py
+-rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/py.typed
+-rw-r--r--   0        0        0     3393 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/utils.py
+-rw-r--r--   0        0        0        0 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/__init__.py
+-rw-r--r--   0        0        0     1869 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/to_html_patch.js
+-rw-r--r--   0        0        0     7092 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/utils.py
+-rw-r--r--   0        0        0    20427 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/blackboxopt/visualizations/visualizer.py
+-rw-r--r--   0        0        0     3206 2023-02-14 09:20:42.000000 blackboxopt-4.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 blackboxopt-4.9.1/setup.py
+-rw-r--r--   0        0        0     6441 1970-01-01 00:00:00.000000 blackboxopt-4.9.1/PKG-INFO
```

### Comparing `blackboxopt-4.9.0/LICENSE` & `blackboxopt-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/README.md` & `blackboxopt-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/base.py` & `blackboxopt-4.9.1/blackboxopt/base.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/evaluation.py` & `blackboxopt-4.9.1/blackboxopt/evaluation.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/examples/dask_distributed.py` & `blackboxopt-4.9.1/blackboxopt/examples/dask_distributed.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimization_loops/dask_distributed.py` & `blackboxopt-4.9.1/blackboxopt/optimization_loops/dask_distributed.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimization_loops/sequential.py` & `blackboxopt-4.9.1/blackboxopt/optimization_loops/sequential.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimization_loops/testing.py` & `blackboxopt-4.9.1/blackboxopt/optimization_loops/testing.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimization_loops/utils.py` & `blackboxopt-4.9.1/blackboxopt/optimization_loops/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/bohb.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/bohb.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/botorch_base.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/botorch_base.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/hyperband.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/hyperband.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/random_search.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/random_search.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/space_filling.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/space_filling.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/staged/bohb.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/staged/bohb.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/staged/configuration_sampler.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/staged/configuration_sampler.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/staged/hyperband.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/staged/hyperband.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/staged/iteration.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/staged/iteration.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/staged/optimizer.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/staged/optimizer.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/staged/utils.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/staged/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/optimizers/testing.py` & `blackboxopt-4.9.1/blackboxopt/optimizers/testing.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/utils.py` & `blackboxopt-4.9.1/blackboxopt/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/visualizations/to_html_patch.js` & `blackboxopt-4.9.1/blackboxopt/visualizations/to_html_patch.js`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/visualizations/utils.py` & `blackboxopt-4.9.1/blackboxopt/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/blackboxopt/visualizations/visualizer.py` & `blackboxopt-4.9.1/blackboxopt/visualizations/visualizer.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-4.9.0/pyproject.toml` & `blackboxopt-4.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackboxopt"
-version = "4.9.0"
+version = "4.9.1"
 description = "A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts."
 readme = "README.md"
 repository = "https://github.com/boschresearch/blackboxopt"
 authors = ["Bosch Center for AI, Robert Bosch GmbH"]
 license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-parameterspace = "^0.7.2"
+parameterspace = ">=0.7.2,<0.9"
 numpy = {version = "^1.22.0", optional = true}
 plotly = {version = "^5.10.0", optional = true}
 scipy = {version = "^1.6.0", optional = true}
 statsmodels = {version = "^0.13.2", optional = true}
 dask = {version = "^2023.1.0", optional = true}
 distributed = {version = "^2023.1.0", optional = true}
 pandas = {version = "^1.2.4", optional = true}
```

### Comparing `blackboxopt-4.9.0/setup.py` & `blackboxopt-4.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  'blackboxopt.optimizers.staged',
  'blackboxopt.visualizations']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['parameterspace>=0.7.2,<0.8.0']
+['parameterspace>=0.7.2,<0.9']
 
 extras_require = \
 {'all': ['numpy>=1.22.0,<2.0.0',
          'plotly>=5.10.0,<6.0.0',
          'scipy>=1.6.0,<2.0.0',
          'statsmodels>=0.13.2,<0.14.0',
          'dask>=2023.1.0,<2024.0.0',
@@ -34,15 +34,15 @@
  'testing': ['numpy>=1.22.0,<2.0.0'],
  'visualization': ['plotly>=5.10.0,<6.0.0',
                    'scipy>=1.6.0,<2.0.0',
                    'pandas>=1.2.4,<2.0.0']}
 
 setup_kwargs = {
     'name': 'blackboxopt',
-    'version': '4.9.0',
+    'version': '4.9.1',
     'description': 'A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts.',
     'long_description': '# Blackbox Optimization\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)\n[![CI/CD](https://github.com/boschresearch/blackboxopt/workflows/ci-cd-pipeline/badge.svg)](https://github.com/boschresearch/blackboxopt/actions?query=workflow%3Aci-cd-pipeline+branch%3Amain)\n\nVarious blackbox optimization algorithms with a common interface along with useful\nhelpers like parallel optimization loops, analysis and visualization scripts.\n\nRandom search is provided as an example optimizer along with tests for the interface.\n\nNew optimizers can require `blackboxopt` as a dependency, which is just the light-weight\ninterface definition.\nIf you want all optimizer implementations that come with this package, install\n`blackboxopt[all]`\nAlternatively, you can get individual optimizers with e.g. `blackboxopt[bohb]`\n\nThis software is a research prototype.\nThe software is not ready for production use.\nIt has neither been developed nor tested for a specific use case.\nHowever, the license conditions of the applicable Open Source licenses allow you to\nadapt the software to your needs.\nBefore using it in a safety relevant setting, make sure that the software fulfills your\nrequirements and adjust it according to any applicable safety standards\n(e.g. ISO 26262).\n\n## Documentation\n\n**Visit [boschresearch.github.io/blackboxopt](https://boschresearch.github.io/blackboxopt/)**\n\n## Development\n\nInstall poetry\n\n```\npip install poetry\n```\n\nInstall the `blackboxopt` package from source by running the following from the root\ndirectory of _this_ repository\n\n```\npoetry install\n```\n\n(Optional) Install [pre-commit](https://pre-commit.com) hooks to check code standards\nbefore committing changes:\n\n```\npoetry run pre-commit install\n```\n\n## Test\n\nMake sure to install all extras before running tests\n\n```\npoetry install -E testing\npoetry run pytest tests/\n```\n\nFor HTML test coverage reports run\n\n```\npoetry run pytest tests/ --cov --cov-report html:htmlcov\n```\n\n### Custom Optimizers\n\nWhen you develop an optimizer based on the interface defined as part of\n`blackboxopt.base`, you can use `blackboxopt.testing` to directly test whether your\nimplementation follows the specification by adding a test like this to your test suite.\n\n```python\nfrom blackboxopt.testing import ALL_REFERENCE_TESTS\n\n@pytest.mark.parametrize("reference_test", ALL_REFERENCE_TESTS)\ndef test_all_reference_tests(reference_test):\n    reference_test(CustomOptimizer, custom_optimizer_init_kwargs)\n```\n\n## Building Documentation\n\nMake sure to install _all_ necessary dependencies:\n\n```\npoetry install --extras=all\n```\n\nThe documentation can be built from the repository root as follows:\n\n```\npoetry run mkdocs build --clean --no-directory-urls\n```\n\nFor serving it locally while working on the documentation run:\n\n```\npoetry run mkdocs serve\n```\n\n## Architectural Decision Records\n\n### Create evaluation result from specification\n\nIn the context of initializing an evaluation result from a specification, facing the\nconcern that having a constructor with a specification argument while the specification\nattributes end up as toplevel attributes and not summarized under a specification\nattribute we decided for unpacking the evaluation specification like a dictionary into\nthe result constructor to prevent the said cognitive dissonance, accepting that the\nunpacking operator can feel unintuitive and that users might tend to matching the\nattributes explictly to the init arguments.\n\n### Report multiple evaluations\n\nIn the context of many optimizers just sequentally reporting the individual evaluations\nwhen multiple evaluations are reported at once and thus not leveraging any batch\nreporting benefits, facing the concern that representing that common behaviour in the\noptimizer base class requires the definition of an abstract report single and an\nabstract report multi method for which the report single does not need to be implemented\nif the report multi is, we decided to refactor the arising redundancy into a function\n`call_functions_with_evaluations_and_collect_errors`, accepting that this increases the\ncognitive load when reading the code.\n\n## License\n\n`blackboxopt` is open-sourced under the Apache-2.0 license. See the [LICENSE](LICENSE)\nfile for details.\n\nFor a list of other open source components included in `blackboxopt`, see the file\n[3rd-party-licenses.txt](3rd-party-licenses.txt).\n',
     'author': 'Bosch Center for AI, Robert Bosch GmbH',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/boschresearch/blackboxopt',
```

### Comparing `blackboxopt-4.9.0/PKG-INFO` & `blackboxopt-4.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxopt
-Version: 4.9.0
+Version: 4.9.1
 Summary: A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts.
 Home-page: https://github.com/boschresearch/blackboxopt
 License: Apache-2.0
 Author: Bosch Center for AI, Robert Bosch GmbH
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 Provides-Extra: visualization
 Requires-Dist: botorch (>=0.7.1,<0.8.0) ; extra == "all" or extra == "botorch"
 Requires-Dist: dask (>=2023.1.0,<2024.0.0) ; extra == "all" or extra == "dask"
 Requires-Dist: distributed (>=2023.1.0,<2024.0.0) ; extra == "all" or extra == "dask"
 Requires-Dist: numpy (>=1.22.0,<2.0.0) ; extra == "all" or extra == "hyperband" or extra == "bohb" or extra == "space-fill" or extra == "testing"
 Requires-Dist: pandas (>=1.2.4,<2.0.0) ; extra == "all" or extra == "visualization"
-Requires-Dist: parameterspace (>=0.7.2,<0.8.0)
+Requires-Dist: parameterspace (>=0.7.2,<0.9)
 Requires-Dist: plotly (>=5.10.0,<6.0.0) ; extra == "all" or extra == "visualization"
 Requires-Dist: scipy (>=1.6.0,<2.0.0) ; extra == "all" or extra == "bohb" or extra == "space-fill" or extra == "visualization"
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0) ; extra == "all" or extra == "bohb"
 Project-URL: Repository, https://github.com/boschresearch/blackboxopt
 Description-Content-Type: text/markdown
 
 # Blackbox Optimization
```

