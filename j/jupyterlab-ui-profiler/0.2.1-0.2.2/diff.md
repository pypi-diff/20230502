# Comparing `tmp/jupyterlab_ui_profiler-0.2.1.tar.gz` & `tmp/jupyterlab_ui_profiler-0.2.2.tar.gz`

## Comparing `jupyterlab_ui_profiler-0.2.1.tar` & `jupyterlab_ui_profiler-0.2.2.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.eslintignore
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.eslintrc.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.stylelintrc
--rw-r--r--   0        0        0    10523 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/babel.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jest.config.js
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/package.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/readthedocs.yml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/setup.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/tsconfig.json
--rw-r--r--   0        0        0   400810 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/yarn.lock
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/make.bat
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/changelog.rst
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/index.rst
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyter-config/nb-config/jupyterlab_ui_profiler.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyter-config/server-config/jupyterlab_ui_profiler.json
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/_version.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/package.json
--rw-r--r--   0        0        0    66876 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/148.386a0716eefd6e346348.js
--rw-r--r--   0        0        0   373774 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js.LICENSE.txt
--rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/remoteEntry.b7edad4eeff456a5f798.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/style.js
--rw-r--r--   0        0        0    58872 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/benchmark.ts
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/browserProfiler.d.ts
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/css.ts
--rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/dramaturg.ts
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/index.ts
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/jsBenchmarks.ts
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/lumino.tsx
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/profiler.ts
--rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/scenarios.ts
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/statistics.ts
--rw-r--r--   0        0        0    17780 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/styleBenchmarks.tsx
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/table.ts
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/templates.tsx
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/tokens.ts
--rw-r--r--   0        0        0    40154 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/ui.tsx
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/utils.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/__tests__/jupyterlab-ui-profiler.spec.ts
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/__tests__/statistics.spec.ts
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-base.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-execution.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-profile.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-group.json
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-usage.json
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-base.json
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-completer.json
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-debugger.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-menu-open.json
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-scroll.json
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-sidebars.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-tabs.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-base.ts
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-execution.ts
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-profile.ts
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-group.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-usage.ts
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule.ts
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-base.ts
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-completer.ts
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-debugger.ts
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-menu-open.ts
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-scroll.ts
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-sidebars.ts
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-tabs.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/index.ts
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/package.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   131668 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts
--rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28608 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png
--rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png
--rw-r--r--   0        0        0   103844 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png
--rw-r--r--   0        0        0   109606 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png
--rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png
--rw-r--r--   0        0        0    64015 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png
--rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png
--rw-r--r--   0        0        0   117877 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png
--rw-r--r--   0        0        0   102798 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png
--rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png
--rw-r--r--   0        0        0    58453 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/LICENSE
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/README.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/.eslintignore
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/.eslintrc.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/.stylelintrc
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/babel.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jest.config.js
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/package.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/readthedocs.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/setup.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0   400810 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/yarn.lock
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/docs/make.bat
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/docs/source/changelog.rst
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/docs/source/conf.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/docs/source/index.rst
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyter-config/nb-config/jupyterlab_ui_profiler.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyter-config/server-config/jupyterlab_ui_profiler.json
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/_version.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/package.json
+-rw-r--r--   0        0        0   373774 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js.LICENSE.txt
+-rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js
+-rw-r--r--   0        0        0    67728 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/894.c1224529783339629936.js
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/remoteEntry.edbfe3921863735c974c.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/style.js
+-rw-r--r--   0        0        0    58872 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/benchmark.ts
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/browserProfiler.d.ts
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/css.ts
+-rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/dramaturg.ts
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/index.ts
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/jsBenchmarks.ts
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/lumino.tsx
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/profiler.ts
+-rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/scenarios.ts
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/statistics.ts
+-rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/styleBenchmarks.tsx
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/table.ts
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/templates.tsx
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/tokens.ts
+-rw-r--r--   0        0        0    40154 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/ui.tsx
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/utils.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/__tests__/jupyterlab-ui-profiler.spec.ts
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/__tests__/statistics.spec.ts
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-base.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-execution.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-profile.json
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-rule-group.json
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-rule-usage.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-rule.json
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-sheet.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-base.json
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-completer.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-debugger.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-menu-open.json
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-scroll.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-sidebars.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/schema/scenario-tabs.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-base.ts
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-execution.ts
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-profile.ts
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-rule-group.ts
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-rule-usage.ts
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-rule.ts
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-sheet.ts
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-base.ts
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-completer.ts
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-debugger.ts
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-menu-open.ts
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-scroll.ts
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-sidebars.ts
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/_scenario-tabs.ts
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/src/types/index.ts
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/package.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   131668 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/profiler.spec.ts
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28608 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png
+-rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png
+-rw-r--r--   0        0        0   103844 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png
+-rw-r--r--   0        0        0   109606 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png
+-rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png
+-rw-r--r--   0        0        0    64015 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png
+-rw-r--r--   0        0        0   117877 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png
+-rw-r--r--   0        0        0   102798 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png
+-rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png
+-rw-r--r--   0        0        0    58453 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.2/PKG-INFO
```

### Comparing `jupyterlab_ui_profiler-0.2.1/.eslintrc.js` & `jupyterlab_ui_profiler-0.2.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/CHANGELOG.md` & `jupyterlab_ui_profiler-0.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.2
+
+([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.2.1...61c99c34b8de4ff8f0ac0da4b1af50e774cd543a))
+
+### Enhancements made
+
+- Allow to filter sheet and rule benchmarks to only include some rules [#50](https://github.com/jupyterlab/ui-profiler/pull/50) ([@krassowski](https://github.com/krassowski))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/ui-profiler/graphs/contributors?from=2023-04-30&to=2023-05-01&type=c))
+
+[@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Akrassowski+updated%3A2023-04-30..2023-05-01&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.2.1
 
 ([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.2.0...308598c8f2f2c344fee6d9ccffd1c379f8b8ecbc))
 
 ### Enhancements made
 
 - Expose option types for more convenient use downstream [#49](https://github.com/jupyterlab/ui-profiler/pull/49) ([@krassowski](https://github.com/krassowski))
@@ -16,16 +32,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/ui-profiler/graphs/contributors?from=2023-04-23&to=2023-04-30&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Agithub-actions+updated%3A2023-04-23..2023-04-30&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Akrassowski+updated%3A2023-04-23..2023-04-30&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.2.0
 
 ([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.1.8...3c4d2c8f2f80ba5e81c16b1dea2b77d76c209766))
 
 ### Enhancements made
 
 - Separate profiler out of the user interface [#46](https://github.com/jupyterlab/ui-profiler/pull/46) ([@krassowski](https://github.com/krassowski))
```

### Comparing `jupyterlab_ui_profiler-0.2.1/RELEASE.md` & `jupyterlab_ui_profiler-0.2.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/jest.config.js` & `jupyterlab_ui_profiler-0.2.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/package.json` & `jupyterlab_ui_profiler-0.2.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.1/tsconfig.json` & `jupyterlab_ui_profiler-0.2.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/yarn.lock` & `jupyterlab_ui_profiler-0.2.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/docs/Makefile` & `jupyterlab_ui_profiler-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/docs/make.bat` & `jupyterlab_ui_profiler-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/docs/source/conf.py` & `jupyterlab_ui_profiler-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/docs/source/_static/logo-icon.png` & `jupyterlab_ui_profiler-0.2.2/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/__init__.py` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/package.json` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.edbfe3921863735c974c.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -47,15 +47,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/jupyterlab/ui-profiler",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b7edad4eeff456a5f798.js",
+            "load": "static/remoteEntry.edbfe3921863735c974c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_ui_profiler/labextension",
         "sharedPackages": {
             "@lumino/datagrid": {
                 "bundled": false,
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/148.386a0716eefd6e346348.js` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/894.c1224529783339629936.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 "use strict";
 (self.webpackChunk_jupyterlab_ui_profiler = self.webpackChunk_jupyterlab_ui_profiler || []).push([
-    [148], {
-        8148: (e, t, n) => {
+    [894], {
+        4894: (e, t, n) => {
             n.r(t), n.d(t, {
                 IUIProfiler: () => we,
                 default: () => He
             });
             var s = n(5687),
                 i = n(3033),
                 r = n(7986),
                 o = n(7280),
                 a = n(1467),
                 l = n(3169),
                 c = n(2502),
                 u = n(3443),
-                p = n(6271),
-                d = n.n(p),
+                d = n(6271),
+                p = n.n(d),
                 m = n(8820),
                 h = n(2583),
                 f = n(1526),
                 g = n(8142),
                 w = n(1840),
                 y = n(1641);
 
@@ -29,39 +29,39 @@
                 for (const n of e.values()) {
                     const e = n.tagName.toLocaleLowerCase();
                     Object.prototype.hasOwnProperty.call(t, e) ? t[e] += 1 : t[e] = 1
                 }
                 return t
             }
 
-            function k(e) {
+            function v(e) {
                 if (isNaN(e)) return "-";
                 const t = e / 1e3,
                     n = Math.floor(t / 60);
                 let s = Math.round(t - 60 * n) + " seconds";
                 if (n < 1) return s;
                 const i = Math.floor(n / 60);
                 return s = Math.round(n - 60 * i) + " minutes " + s, i < 1 || (s = Math.round(i) + " hours " + s), s
             }
 
-            function* v(e) {
-                for (const t of e.childNodes) yield t, yield* v(t)
+            function* k(e) {
+                for (const t of e.childNodes) yield t, yield* k(t)
             }
 
             function* S(e) {
                 for (const t of e) {
                     yield t.target;
                     for (const e of t.addedNodes)
                         if (e !== document.body) {
                             yield e;
-                            for (const t of v(e)) yield t
+                            for (const t of k(e)) yield t
                         } for (const e of t.removedNodes)
                         if (e !== document.body) {
                             yield e;
-                            for (const t of v(e)) yield t
+                            for (const t of k(e)) yield t
                         }
                 }
             }
             const E = 1 / (2 * Math.PI) ** .5;
             var x;
             ! function(e) {
                 function t(e) {
@@ -131,34 +131,34 @@
                 }))))
             }
             class C {
                 constructor(e) {
                     this.element = e
                 }
                 $(e) {
-                    return A(e, this.element)
+                    return P(e, this.element)
                 }
                 click() {
-                    return R(this.element)
+                    return B(this.element)
                 }
                 async focus() {
                     return this.element.focus()
                 }
                 press(e, t = {
                     delay: 0
                 }) {
-                    return B(e, t, this.element)
+                    return R(e, t, this.element)
                 }
                 type(e, t = {
                     delay: 0
                 }) {
                     return async function(e, t = {
                         delay: 0
                     }, n = null) {
-                        for (const s of e) await B(s, t, n)
+                        for (const s of e) await R(s, t, n)
                     }(e, t, this.element)
                 }
                 async isVisible() {
                     const e = this.element.getBoundingClientRect();
                     return !(0 === e.width || 0 === e.height)
                 }
                 waitForSelector(e, t) {
@@ -229,58 +229,58 @@
                 }
                 const s = t.timeout || 5e3;
                 return Promise.race([n, new Promise(((n, i) => {
                     setTimeout((() => i(`Selector ${e} not found in ${t.state} state in ${s/1e3}s`)), s)
                 }))])
             }
             const I = (0, j.Vc)(),
-                _ = I._codes,
-                T = Object.fromEntries(Object.entries(_).map((e => e.reverse())));
-            async function B(e, t = {
+                T = I._codes,
+                _ = Object.fromEntries(Object.entries(T).map((e => e.reverse())));
+            async function R(e, t = {
                 delay: 0
             }, n = null) {
                 n || (n = document.activeElement || document.body);
                 const s = e.split("+"),
                     i = s.filter((e => I.isModifierKey(e))),
                     r = s.filter((e => !I.isModifierKey(e)))[0],
                     o = {
-                        keyCode: T[r],
+                        keyCode: _[r],
                         shiftKey: i.includes("Shift"),
                         ctrlKey: i.includes("Ctrl"),
                         metaKey: i.includes("Meta"),
                         key: r
                     };
                 n.dispatchEvent(new KeyboardEvent("keydown", o)), n.dispatchEvent(new KeyboardEvent("keypress", o)), t.delay && await new Promise((e => setTimeout(e, t.delay))), n.dispatchEvent(new KeyboardEvent("keyup", o))
             }
-            async function R(e) {
+            async function B(e) {
                 const t = e.getBoundingClientRect(),
                     n = {
                         clientX: t.x + t.width / 2,
                         clientY: t.x + t.height / 2,
                         bubbles: !0
                     };
                 e.dispatchEvent(new MouseEvent("mousedown", n)), e.dispatchEvent(new MouseEvent("mouseup", n)), e.click()
             }
-            async function A(e, t) {
+            async function P(e, t) {
                 const n = t ? t.querySelector(e) : document.querySelector(e);
                 return n ? new C(n) : null
             }
-            const P = {
+            const A = {
                 waitForSelector: O,
-                press: B,
-                $: A,
+                press: R,
+                $: P,
                 type: async (e, t, n = {
                     delay: 0
                 }) => (await O(e, {
                     state: "visible"
                 })).type(t, n),
                 click: async e => {
                     await O(e, {
                         state: "attached"
-                    }), R((await O(e, {
+                    }), B((await O(e, {
                         state: "visible"
                     })).element)
                 },
                 focus: async e => {
                     (await O(e, {
                         state: "visible"
                     })).element.focus()
@@ -346,89 +346,89 @@
                             i = x.quartile(e.times, 3),
                             r = i - s,
                             o = Math.min(s + 1.5 * r, t),
                             a = Math.max(i - 1.5 * r, n),
                             l = 200 / 3,
                             c = e => e / t * 750,
                             u = e.times.map((t => x.kernelDensityEstimate(e.times, t))),
-                            p = Math.max(...u),
+                            d = Math.max(...u),
                             m = Math.round(375),
                             h = t,
                             f = Math.ceil((h - 0) / m),
                             g = Array.from(Array(m), (() => [])),
                             w = new Array(e.times.length);
                         for (let t = 0; t < e.times.length; t++) {
                             const n = e.times[t],
                                 s = Math.floor(n / f);
                             g[s].push(t), w[t] = s
                         }
                         const y = e.times.map(((e, t) => {
                                 const n = w[t],
                                     s = g[n],
-                                    i = (s.indexOf(t) / s.length - .5) * u[t] / p * l;
-                                return d().createElement("g", null, d().createElement("title", null, x.round(e, 2), " ms, ", X(t), " repeat"), d().createElement("circle", {
+                                    i = (s.indexOf(t) / s.length - .5) * u[t] / d * l;
+                                return p().createElement("g", null, p().createElement("title", null, x.round(e, 2), " ms, ", X(t), " repeat"), p().createElement("circle", {
                                     cx: c(e),
                                     cy: 100 + i,
                                     r: 2,
                                     className: "point"
                                 }))
                             })),
                             b = [1, 2, 3].map((t => {
                                 const n = x.quartile(e.times, t),
                                     s = c(n),
                                     i = 100 - l / 2;
-                                return d().createElement("g", null, d().createElement("title", null, X(t), " quartile: ", x.round(n, 2), " ms"), d().createElement("line", {
+                                return p().createElement("g", null, p().createElement("title", null, X(t), " quartile: ", x.round(n, 2), " ms"), p().createElement("line", {
                                     x1: s,
                                     y1: i,
                                     x2: s,
                                     y2: i + l,
                                     className: "box-line"
                                 }))
                             }));
-                        return d().createElement("svg", {
+                        return p().createElement("svg", {
                             viewBox: "0 0 755 200",
                             className: "up-BoxPlot"
-                        }, y, d().createElement("g", null, d().createElement("title", null, "Lower whisker, max(lowest value, q1 - 1.5 * IQR) =", " ", x.round(a, 2), " ms"), d().createElement("line", {
+                        }, y, p().createElement("g", null, p().createElement("title", null, "Lower whisker, max(lowest value, q1 - 1.5 * IQR) =", " ", x.round(a, 2), " ms"), p().createElement("line", {
                             x1: c(a),
                             y1: 100,
                             x2: c(s),
                             y2: 100,
                             className: "whisker"
-                        })), d().createElement("g", null, d().createElement("title", null, "Upper whisker, min(higher value, q3 + 1.5 * IQR) =", " ", x.round(o, 2), " ms"), d().createElement("line", {
+                        })), p().createElement("g", null, p().createElement("title", null, "Upper whisker, min(higher value, q3 + 1.5 * IQR) =", " ", x.round(o, 2), " ms"), p().createElement("line", {
                             x1: c(i),
                             y1: 100,
                             x2: c(o),
                             y2: 100,
                             className: "whisker"
-                        })), d().createElement("rect", {
+                        })), p().createElement("rect", {
                             x: c(s),
                             y: 100 - l / 2,
                             width: c(i - s),
                             height: l,
                             className: "box"
-                        }), b, d().createElement("line", {
+                        }), b, p().createElement("line", {
                             x1: "0",
                             x2: 750,
                             y1: 185,
                             y2: 185,
                             className: "timeline"
-                        }), d().createElement("text", {
+                        }), p().createElement("text", {
                             x: "0",
                             y: 200,
                             className: "tickLabel"
-                        }, "0ms"), d().createElement("text", {
+                        }, "0ms"), p().createElement("text", {
                             x: 750,
                             y: 200,
                             style: {
                                 textAnchor: "end"
                             },
                             className: "tickLabel"
                         }, Math.round(t), "ms"))
                     }));
-                    return d().createElement(d().Fragment, null, t)
+                    return p().createElement(p().Fragment, null, t)
                 }
             };
 
             function* q(e) {
                 let t = new Map;
                 for (const n of e.samples) {
                     const s = n.timestamp;
@@ -541,16 +541,16 @@
                             totalTime: Date.now() - a,
                             type: "profile",
                             interrupted: i
                         }
                     },
                     isAvailable: () => void 0 !== window.Profiler,
                     render: function(e) {
-                        const t = d().useRef(null),
-                            [n, s] = d().useState(0);
+                        const t = p().useRef(null),
+                            [n, s] = p().useState(0);
                         if (null === t.current || t.current.stateSource !== e.outcome) {
                             const n = {};
                             for (const t of e.outcome.results)
                                 for (const e of t.traces)
                                     for (const t of L(e)) {
                                         const e = [t.name, t.resource, t.column, t.line].join("-");
                                         if (e in n) n[e].times.push(t.time), n[e].totalTime += t.time, n[e].calls += 1;
@@ -575,82 +575,82 @@
                             0 !== s.length ? t.current = new V({
                                 measurements: s,
                                 stateSource: e.outcome,
                                 sortColumn: "totalTime",
                                 lowerIsBetter: !0
                             }) : t.current = null
                         }
-                        return n > e.outcome.results[0].traces.length ? (s(0), d().createElement(d().Fragment, null)) : d().createElement(d().Fragment, null, d().createElement("select", {
+                        return n > e.outcome.results[0].traces.length ? (s(0), p().createElement(p().Fragment, null)) : p().createElement(p().Fragment, null, p().createElement("select", {
                             value: n,
                             onChange: e => {
                                 s(Number(e.target.value))
                             },
                             className: "up-trace-selector"
-                        }, e.outcome.results[0].traces.map(((e, t) => d().createElement("option", {
+                        }, e.outcome.results[0].traces.map(((e, t) => p().createElement("option", {
                             value: t,
                             key: "trace-" + t
-                        }, "Trace ", t, " (", e.samples.length, " samples)")))), d().createElement(Y, {
+                        }, "Trace ", t, " (", e.samples.length, " samples)")))), p().createElement(Y, {
                             trace: e.outcome.results[0].traces[n],
                             itemHeight: 20
-                        }), t.current ? d().createElement(K, {
+                        }), t.current ? p().createElement(K, {
                             widget: t.current
                         }) : "No results available. Reduce sampling interval, use macro mode, and/or increase the number of repeats.")
                     }
                 },
                 $ = e => {
                     const t = e.load("jupyterlab"),
-                        n = e => d().createElement("div", {
+                        n = e => p().createElement("div", {
                             className: e.className
-                        }, d().createElement(e.TitleField, {
+                        }, p().createElement(e.TitleField, {
                             title: e.title,
                             required: e.required,
                             id: `${e.idSchema.$id}-title`
-                        }), d().createElement(e.DescriptionField, {
+                        }), p().createElement(e.DescriptionField, {
                             id: `${e.idSchema.$id}-description`,
                             description: e.schema.description ?? ""
-                        }), e.items.map((e => d().createElement("div", {
+                        }), e.items.map((e => p().createElement("div", {
                             key: e.key,
                             className: e.className
-                        }, e.children, d().createElement("div", {
+                        }, e.children, p().createElement("div", {
                             className: "jp-ArrayOperations"
-                        }, d().createElement("button", {
+                        }, p().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onReorderClick(e.index, e.index - 1),
                             disabled: !e.hasMoveUp
-                        }, t.__("Move Up")), d().createElement("button", {
+                        }, t.__("Move Up")), p().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onReorderClick(e.index, e.index + 1),
                             disabled: !e.hasMoveDown
-                        }, t.__("Move Down")), d().createElement("button", {
+                        }, t.__("Move Down")), p().createElement("button", {
                             className: "jp-mod-styled jp-mod-warn",
                             onClick: e.onDropIndexClick(e.index),
                             disabled: !e.hasRemove
-                        }, t.__("Remove")))))), e.canAdd && d().createElement("button", {
+                        }, t.__("Remove")))))), e.canAdd && p().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onAddClick
                         }, t.__("Add")));
                     return n.displayName = "JupyterLabArrayTemplate", n
                 },
                 z = e => {
                     const t = e.load("jupyterlab"),
                         n = e => {
                             const {
                                 TitleField: n,
                                 DescriptionField: s
                             } = e;
-                            return d().createElement("fieldset", {
+                            return p().createElement("fieldset", {
                                 id: e.idSchema.$id
-                            }, (e.uiSchema["ui:title"] || e.title) && d().createElement(n, {
+                            }, (e.uiSchema["ui:title"] || e.title) && p().createElement(n, {
                                 id: `${e.idSchema.$id}__title`,
                                 title: e.title || e.uiSchema["ui:title"],
                                 required: e.required
-                            }), e.description && d().createElement(s, {
+                            }), e.description && p().createElement(s, {
                                 id: `${e.idSchema.$id}__description`,
                                 description: e.description
-                            }), e.properties.map((e => e.content)), u.P6.canExpand(e.schema, e.uiSchema, e.formData) && d().createElement("button", {
+                            }), e.properties.map((e => e.content)), u.P6.canExpand(e.schema, e.uiSchema, e.formData) && p().createElement("button", {
                                 className: "jp-mod-styled jp-mod-reject",
                                 onClick: e.onAddClick(e.schema),
                                 disabled: e.disabled || e.readonly
                             }, t.__("Add")))
                         };
                     return n.displayName = "JupyterLabObjectTemplate", n
                 },
@@ -662,41 +662,41 @@
                                 label: s,
                                 displayLabel: i,
                                 id: r,
                                 errors: o,
                                 rawErrors: a,
                                 children: l,
                                 onKeyChange: c,
-                                onDropPropertyClick: p
+                                onDropPropertyClick: d
                             } = e, m = r.split("_");
                             m.shift();
                             const h = "" === m.join("."),
                                 f = !h && "object" !== n.type,
                                 g = Object.prototype.hasOwnProperty.call(n, u.P6.ADDITIONAL_PROPERTY_FLAG);
-                            return d().createElement("div", {
+                            return p().createElement("div", {
                                 className: "form-group " + (i || "boolean" === n.type ? "small-field" : "")
-                            }, a && d().createElement("div", {
+                            }, a && p().createElement("div", {
                                 className: "jp-modifiedIndicator jp-errorIndicator"
-                            }), d().createElement("div", {
+                            }), p().createElement("div", {
                                 className: "jp-FormGroup-content"
-                            }, i && !h && s && !g && d().createElement("h3", {
+                            }, i && !h && s && !g && p().createElement("h3", {
                                 className: "jp-FormGroup-fieldLabel jp-FormGroup-contentItem"
-                            }, s), g && d().createElement("input", {
+                            }, s), g && p().createElement("input", {
                                 className: "jp-FormGroup-contentItem jp-mod-styled",
                                 type: "text",
                                 onBlur: e => c(e.target.value),
                                 defaultValue: s
-                            }), d().createElement("div", {
+                            }), p().createElement("div", {
                                 className: h ? "jp-root" : "object" === n.type ? "jp-objectFieldWrapper" : "jp-inputFieldWrapper jp-FormGroup-contentItem"
-                            }, l), g && d().createElement("button", {
+                            }, l), g && p().createElement("button", {
                                 className: "jp-FormGroup-contentItem jp-mod-styled jp-mod-warn jp-FormGroup-removeButton",
-                                onClick: p(s)
-                            }, t.__("Remove")), n.description && f && d().createElement("div", {
+                                onClick: d(s)
+                            }, t.__("Remove")), n.description && f && p().createElement("div", {
                                 className: "jp-FormGroup-description"
-                            }, n.description), d().createElement("div", {
+                            }, n.description), p().createElement("div", {
                                 className: "validationErrors"
                             }, o)))
                         };
                     return n.displayName = "JupyterLabFieldTemplate", n
                 };
             var U = n(5414);
             class J extends U.BasicMouseHandler {
@@ -830,43 +830,43 @@
                         const t = this.dataModel.data(e.region, e.row, e.column);
                         t === this.sortColumn ? this.sortOrder = "ascending" === this.sortOrder ? "descending" : "ascending" : this.sortColumn = t, this._setupDataModel(!0), this.update()
                     }
                 }
             }
             var G = n(8832);
             const K = e => {
-                const t = d().useRef(null);
-                return d().useEffect((() => {
+                const t = p().useRef(null);
+                return p().useEffect((() => {
                     const n = e.widget;
                     G.Widget.attach(n, t.current);
                     const s = new ResizeObserver((t => {
                         e.widget.fit()
                     }));
                     return s.observe(t.current), () => {
                         G.Widget.detach(n), s.disconnect()
                     }
-                }), [e.widget]), d().createElement("div", {
+                }), [e.widget]), p().createElement("div", {
                     className: "up-LuminoWidgetWrapper",
                     ref: t
                 })
             };
-            class Y extends d().Component {
+            class Y extends p().Component {
                 constructor(e) {
                     super(e), this.deepest = 0, this.contentWidth = 100, this.contentHeight = 100, this.initialWidth = 100, this.state = {
                         scale: {
                             x: 1,
                             y: 1
                         },
                         position: {
                             x: 0,
                             y: 0
                         },
                         dimensions: null,
                         inDrag: !1
-                    }, this.handleMouseUp = this.handleMouseUp.bind(this), this.handleMouseDown = this.handleMouseDown.bind(this), this.handleMouseMove = this.handleMouseMove.bind(this), this.handleWheel = this.handleWheel.bind(this), this.container = d().createRef(), this.resizeObserver = new ResizeObserver(this.updateSizeInfo.bind(this))
+                    }, this.handleMouseUp = this.handleMouseUp.bind(this), this.handleMouseDown = this.handleMouseDown.bind(this), this.handleMouseMove = this.handleMouseMove.bind(this), this.handleWheel = this.handleWheel.bind(this), this.container = p().createRef(), this.resizeObserver = new ResizeObserver(this.updateSizeInfo.bind(this))
                 }
                 componentDidMount() {
                     const e = this.props.trace,
                         t = e.samples[0].timestamp,
                         n = Math.max(...e.samples.map((e => e.timestamp - t))),
                         s = {
                             width: this.container.current.offsetWidth,
@@ -924,25 +924,25 @@
                     }), document.addEventListener("mousemove", this.handleMouseMove), document.addEventListener("mouseup", this.handleMouseUp)
                 }
                 renderContent() {
                     const {
                         trace: e,
                         itemHeight: t
                     } = this.props;
-                    if (!e.samples) return d().createElement("div", null, "No samples in trace");
+                    if (!e.samples) return p().createElement("div", null, "No samples in trace");
                     const n = e.samples[0].timestamp,
                         s = [...q(e)];
                     this.deepest = Math.max(...s.map((e => e.stackDepth)));
                     const i = this.state.scale,
                         r = e.samples.map(((t, s) => {
                             const r = {
                                 width: (e.samples[s + 1]?.timestamp - t.timestamp) * i.x,
                                 left: (t.timestamp - n) * i.x
                             };
-                            return d().createElement("div", {
+                            return p().createElement("div", {
                                 className: "up-ProfileTrace-sample",
                                 key: "sample-" + s,
                                 style: r
                             })
                         }));
                     let o = 0;
                     const a = s.map(((s, r) => {
@@ -952,32 +952,32 @@
                         o = Math.max(o, l + c);
                         const u = {
                             width: c,
                             top: (s.stackDepth - 1) * t * i.y,
                             left: l,
                             height: t
                         };
-                        return d().createElement("div", {
+                        return p().createElement("div", {
                             className: "up-ProfileTrace-frame " + (void 0 === a.resourceId ? "up-ProfileTrace-frame-native" : ""),
                             key: "frame-" + r,
                             style: u,
                             title: [a.name, x.round(s.duration, 1) + "ms"].join("\n")
                         }, a.name)
                     }));
-                    return this.contentWidth = o, this.contentHeight = (2 + this.deepest) * this.props.itemHeight * i.y, d().createElement("div", {
+                    return this.contentWidth = o, this.contentHeight = (2 + this.deepest) * this.props.itemHeight * i.y, p().createElement("div", {
                         className: "up-ProfileTrace-content",
                         style: {
                             transform: `translate(${this.state.position.x}px, ${this.state.position.y}px)`,
                             width: o + "px",
                             height: this.contentHeight + "px"
                         }
                     }, a, r)
                 }
                 render() {
-                    return d().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-ProfileTrace",
                         onWheel: this.handleWheel,
                         onMouseDown: this.handleMouseDown,
                         ref: this.container
                     }, this.state.dimensions ? this.renderContent() : "Loading")
                 }
             }
@@ -1009,33 +1009,33 @@
                     const t = JSON.parse(e.content);
                     t.result && (t.outcome = t.result), this.handleResult(t)
                 }
                 async upload(e) {
                     return await this.ensureResultsDirectory(), this.props.upload(e)
                 }
                 render() {
-                    return d().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-UIProfiler"
-                    }, d().createElement(re, Object.assign({
+                    }, p().createElement(re, Object.assign({
                         onResult: this.handleResult,
                         progress: this.progress
                     }, this.props, {
                         upload: this.upload
-                    })), d().createElement(ee, Object.assign({
+                    })), p().createElement(ee, Object.assign({
                         resultAdded: this.resultAdded,
                         manager: this.manager,
                         onSelect: this.loadResult
-                    }, this.props)), d().createElement(te, {
+                    }, this.props)), p().createElement(te, {
                         result: this.result,
                         scenarios: this.props.profiler.scenarios,
                         benchmarks: this.props.profiler.benchmarks.filter((e => e.id === this.result?.benchmark))
                     }))
                 }
             }
-            class ee extends d().Component {
+            class ee extends p().Component {
                 constructor(e) {
                     super(e), this._handle = null, this.state = {
                         files: [],
                         current: null
                     }, this.update(), this.update = this.update.bind(this), this.props.resultAdded.connect((async (e, t) => {
                         await this.update(), this.setState({
                             current: se(t)
@@ -1051,112 +1051,112 @@
                 componentDidMount() {
                     this._handle = window.setInterval(this.update, 2e3)
                 }
                 componentWillUnmount() {
                     null !== this._handle && window.clearInterval(this._handle)
                 }
                 render() {
-                    let e = this.state.files.map((e => d().createElement("li", {
+                    let e = this.state.files.map((e => p().createElement("li", {
                         className: this.state.current === e.name ? "up-BenchmarkHistory-file up-BenchmarkHistory-file-active" : "up-BenchmarkHistory-file",
                         key: e.name,
                         onClick: () => {
                             this.props.onSelect(e), this.setState({
                                 current: e.path
                             })
                         }
                     }, e.name.replace(".profile.json", ""))));
-                    return this.state.files.length || (e = [d().createElement("li", {
+                    return this.state.files.length || (e = [p().createElement("li", {
                         className: "up-BenchmarkHistory-entry"
-                    }, "(No previous results found)")]), d().createElement("div", {
+                    }, "(No previous results found)")]), p().createElement("div", {
                         className: "up-BenchmarkHistory"
-                    }, d().createElement("h3", {
+                    }, p().createElement("h3", {
                         className: "up-widget-heading"
-                    }, "History"), d().createElement("ul", {
+                    }, "History"), p().createElement("ul", {
                         className: "up-BenchmarkHistory-files"
                     }, e))
                 }
             }
-            class te extends d().Component {
+            class te extends p().Component {
                 constructor() {
                     super(...arguments), this._table = null, this._previousResult = null
                 }
                 render() {
                     const {
                         result: e,
                         benchmarks: t,
                         scenarios: n
-                    } = this.props, s = e => d().createElement("div", {
+                    } = this.props, s = e => p().createElement("div", {
                         className: "up-BenchmarkResult"
                     }, e);
-                    if (!e) return s(d().createElement("div", null, "Choose a result from the panel, or run a new benchmark."));
+                    if (!e) return s(p().createElement("div", null, "Choose a result from the panel, or run a new benchmark."));
                     const i = n.find((t => t.id === e.scenario)),
                         r = t.find((t => t.id === e.benchmark));
-                    if (!i) return s(d().createElement("div", null, "Unknown scenario: ", e.scenario));
-                    if (!r) return s(d().createElement("div", null, "Unknown benchmark: ", e.benchmark));
+                    if (!i) return s(p().createElement("div", null, "Unknown scenario: ", e.scenario));
+                    if (!r) return s(p().createElement("div", null, "Unknown benchmark: ", e.benchmark));
                     r.render || this._previousResult === e.id || ("time" === e.outcome.type ? this._table = new V({
                         measurements: e.outcome.results,
                         reference: e.outcome.reference,
                         sortColumn: r.sortColumn,
                         stateSource: null,
                         lowerIsBetter: !1
                     }) : this._table = null);
                     const o = [...Object.entries(e.outcome.tags)].map((([e, t]) => `${e}:  ${t}`)).join("\n"),
                         a = x.sum([...Object.values(e.outcome.tags)]);
-                    return s(d().createElement(d().Fragment, null, d().createElement("div", {
+                    return s(p().createElement(p().Fragment, null, p().createElement("div", {
                         className: "up-BenchmarkResult-summary"
-                    }, d().createElement("div", {
+                    }, p().createElement("div", {
                         className: "up-BenchmarkResult-benchmarkInfo"
-                    }, d().createElement("div", null, r.name, " ", i.name), "time" === e.outcome.type ? (l = e.outcome, d().createElement(d().Fragment, null, d().createElement("div", {
+                    }, p().createElement("div", null, r.name, " ", i.name), "time" === e.outcome.type ? (l = e.outcome, p().createElement(p().Fragment, null, p().createElement("div", {
                         title: [...l.reference].sort().map(x.round).join(" ms\n") + " ms"
-                    }, "Reference: IQM:", " ", x.round(x.interQuartileMean(l.reference), 1), " [", x.round(x.quartile(l.reference, 1), 1), " –", " ", x.round(x.quartile(l.reference, 3), 1), "] ms, mean:", " ", x.round(x.mean(l.reference), 1), " ms, min:", " ", x.round(x.min(l.reference), 1), " ms"), d().createElement("div", null, "Total time: ", k(l.totalTime)))) : function(e) {
+                    }, "Reference: IQM:", " ", x.round(x.interQuartileMean(l.reference), 1), " [", x.round(x.quartile(l.reference, 1), 1), " –", " ", x.round(x.quartile(l.reference, 3), 1), "] ms, mean:", " ", x.round(x.mean(l.reference), 1), " ms, min:", " ", x.round(x.min(l.reference), 1), " ms"), p().createElement("div", null, "Total time: ", v(l.totalTime)))) : function(e) {
                         const t = e.results[0];
-                        return d().createElement(d().Fragment, null, d().createElement("div", null, "Traces: ", t.traces.length, ". Average number of samples:", " ", x.round(x.mean(t.traces.map((e => e.samples.length))), 1), ", frames:", " ", x.round(x.mean(t.traces.map((e => e.frames.length))), 1), ".", " ", d().createElement("span", {
+                        return p().createElement(p().Fragment, null, p().createElement("div", null, "Traces: ", t.traces.length, ". Average number of samples:", " ", x.round(x.mean(t.traces.map((e => e.samples.length))), 1), ", frames:", " ", x.round(x.mean(t.traces.map((e => e.frames.length))), 1), ".", " ", p().createElement("span", {
                             title: "Average recorderd: " + x.round(t.averageSampleInterval, 1)
-                        }, "Sampling interval: ", x.round(t.samplingInterval, 1), " ms")), d().createElement("div", null, "Total time: ", k(e.totalTime)))
-                    }(e.outcome)), d().createElement("div", {
+                        }, "Sampling interval: ", x.round(t.samplingInterval, 1), " ms")), p().createElement("div", null, "Total time: ", v(e.totalTime)))
+                    }(e.outcome)), p().createElement("div", {
                         className: "up-BenchmarkResult-environmentInfo"
-                    }, d().createElement("div", null, "Application: ", e.jupyter.client, " ", e.jupyter.version, " ", e.jupyter.devMode ? "dev mode" : null, " ", e.jupyter.mode), d().createElement("div", null, d().createElement("span", {
+                    }, p().createElement("div", null, "Application: ", e.jupyter.client, " ", e.jupyter.version, " ", e.jupyter.devMode ? "dev mode" : null, " ", e.jupyter.mode), p().createElement("div", null, p().createElement("span", {
                         title: e.userAgent
                     }, "Browser: ", function(e) {
                         const t = [/Firefox\/\d+/, /OPR\/\d+/, /Edg\/\d+/, /Mobile\/.* Safari\/\d+/, /Chrome\/\d+/];
                         for (const n of t) {
                             const t = e.match(n);
                             if (t) return t[0]
                         }
                         return "Unknown browser"
-                    }(e.userAgent)), ", ", d().createElement("span", {
+                    }(e.userAgent)), ", ", p().createElement("span", {
                         title: o
-                    }, "DOM Elements: ", a)), d().createElement("div", null, "CPU cores: ", e.hardwareConcurrency))), d().createElement("div", {
+                    }, "DOM Elements: ", a)), p().createElement("div", null, "CPU cores: ", e.hardwareConcurrency))), p().createElement("div", {
                         className: "up-BenchmarkResult-options"
-                    }, d().createElement("details", null, d().createElement("summary", null, "Options"), d().createElement("div", {
+                    }, p().createElement("details", null, p().createElement("summary", null, "Options"), p().createElement("div", {
                         className: "up-BenchmarkResult-options-benchmark"
-                    }, d().createElement("b", null, "Benchmark"), d().createElement(y.w, {
+                    }, p().createElement("b", null, "Benchmark"), p().createElement(y.w, {
                         data: e.options.benchmark
-                    })), d().createElement("div", {
+                    })), p().createElement("div", {
                         className: "up-BenchmarkResult-options-scenario"
-                    }, d().createElement("b", null, "Scenario"), void 0 === e.options.scenario ? d().createElement("div", null, "No options") : d().createElement(y.w, {
+                    }, p().createElement("b", null, "Scenario"), void 0 === e.options.scenario ? p().createElement("div", null, "No options") : p().createElement(y.w, {
                         data: e.options.scenario
-                    })))), d().createElement("div", {
+                    })))), p().createElement("div", {
                         className: "up-BenchmarkResult-details"
-                    }, r.interpretation ? d().createElement("details", null, d().createElement("summary", null, "Interpretation"), r.interpretation) : null, r.render ? d().createElement(r.render, {
+                    }, r.interpretation ? p().createElement("details", null, p().createElement("summary", null, "Interpretation"), r.interpretation) : null, r.render ? p().createElement(r.render, {
                         outcome: e.outcome
-                    }) : this._table ? d().createElement(K, {
+                    }) : this._table ? p().createElement(K, {
                         widget: this._table
                     }) : null)));
                     var l
                 }
             }
-            class ne extends d().Component {
+            class ne extends p().Component {
                 constructor() {
                     super(...arguments), this.start = null, this.end = null
                 }
                 render() {
-                    return d().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-BenchmarkMonitor"
-                    }, d().createElement(i.UseSignal, {
+                    }, p().createElement(i.UseSignal, {
                         signal: this.props.progress,
                         initialArgs: {
                             percentage: -1
                         }
                     }, ((e, t) => {
                         t || (t = {
                             percentage: -1
@@ -1164,35 +1164,35 @@
                         let n = NaN,
                             s = NaN,
                             i = "up-mod-waiting";
                         if (t.interrupted && (i = "up-mod-interrupted"), t.errored && (i += " up-mod-errored"), this.start) {
                             const e = (100 === t.percentage || t.interrupted || t.errored) && this.end ? this.end : new Date;
                             this.end = e, n = e.getTime() - this.start.getTime(), t.interrupted || t.errored || (s = (100 - t.percentage) * n / t.percentage, i = 100 === t.percentage ? "up-mod-completed" : "")
                         }
-                        return d().createElement("div", {
+                        return p().createElement("div", {
                             className: i + " up-BenchmarkMonitor-content"
-                        }, d().createElement("div", null, "Elapsed: ", k(n), ". Remaining:", " ", k(s)), d().createElement(h.ProgressBar, {
+                        }, p().createElement("div", null, "Elapsed: ", v(n), ". Remaining:", " ", v(s)), p().createElement(h.ProgressBar, {
                             percentage: t.percentage
                         }))
                     })))
                 }
             }
 
             function se(e) {
                 return e.id + ".profile.json"
             }
 
             function ie(e) {
-                return d().createElement("div", {
+                return p().createElement("div", {
                     className: "rjsf"
-                }, d().createElement("div", {
+                }, p().createElement("div", {
                     className: "jp-root"
-                }, d().createElement("fieldset", null, d().createElement("legend", null, e.name, " configuration"), "No options available for ", e.name, ".")))
+                }, p().createElement("fieldset", null, p().createElement("legend", null, e.name, " configuration"), "No options available for ", e.name, ".")))
             }
-            class re extends d().Component {
+            class re extends p().Component {
                 constructor(e) {
                     super(e), this._config = {
                         scenarios: {},
                         benchmarks: {}
                     }, this._stop = new w.Signal(this);
                     const {
                         profiler: t
@@ -1278,103 +1278,103 @@
                     this._stop.emit(), this.props.profiler.abortBenchmark()
                 }
                 render() {
                     const {
                         profiler: e
                     } = this.props, t = e.benchmarks.map((e => {
                         const t = !!e.isAvailable && !e.isAvailable();
-                        return d().createElement("label", {
+                        return p().createElement("label", {
                             key: e.id,
                             className: t ? "up-label-disabled" : "",
                             title: t ? "This benchmark is not available on this browser" : ""
-                        }, d().createElement("input", {
+                        }, p().createElement("input", {
                             type: "checkbox",
                             defaultChecked: this.state.benchmarks.includes(e),
                             className: "up-BenchmarkLauncher-choice-input",
                             disabled: t,
                             value: e.id
                         }), e.name)
-                    })), n = e.scenarios.map((e => d().createElement("label", {
+                    })), n = e.scenarios.map((e => p().createElement("label", {
                         key: e.id
-                    }, d().createElement("input", {
+                    }, p().createElement("input", {
                         type: "checkbox",
                         defaultChecked: this.state.scenarios.includes(e),
                         className: "up-BenchmarkLauncher-choice-input",
                         value: e.id
                     }), e.name)));
-                    return d().createElement("div", {
+                    return p().createElement("div", {
                         className: "up-BenchmarkLauncher",
                         style: {
                             height: "450px"
                         }
-                    }, d().createElement("h3", {
+                    }, p().createElement("h3", {
                         className: "up-widget-heading"
-                    }, "Launch"), d().createElement("div", {
+                    }, "Launch"), p().createElement("div", {
                         className: "up-BenchmarkLauncher-cards"
-                    }, d().createElement("div", {
+                    }, p().createElement("div", {
                         className: "up-BenchmarkLauncher-card"
-                    }, d().createElement("h4", {
+                    }, p().createElement("h4", {
                         className: "up-card-heading"
-                    }, "Benchmark"), d().createElement("div", {
+                    }, "Benchmark"), p().createElement("div", {
                         className: "up-BenchmarkLauncher-choices",
                         onChange: this.onBenchmarkChanged.bind(this)
-                    }, t), d().createElement("div", {
+                    }, t), p().createElement("div", {
                         className: "up-BenchmarkLauncher-forms"
                     }, this.state.benchmarks.map((e => {
                         const t = e.configSchema.properties;
-                        return t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", d().createElement(u.ZP, {
+                        return t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", p().createElement(u.ZP, {
                             key: "up-profiler-benchmark-" + e.id,
                             schema: e.configSchema,
                             idPrefix: "up-profiler-benchmark",
                             onChange: t => {
                                 this._config.benchmarks[e.id] = t.formData
                             },
                             formData: this._config.benchmarks[e.id],
                             FieldTemplate: this.state.fieldTemplate,
                             ArrayFieldTemplate: this.state.arrayFieldTemplate,
                             ObjectFieldTemplate: this.state.objectFieldTemplate,
                             liveValidate: !0
-                        })) : d().createElement(ie, {
+                        })) : p().createElement(ie, {
                             name: e.name
                         })
-                    })))), d().createElement("div", {
+                    })))), p().createElement("div", {
                         className: "up-BenchmarkLauncher-card"
-                    }, d().createElement("h4", {
+                    }, p().createElement("h4", {
                         className: "up-card-heading"
-                    }, "Scenario"), d().createElement("div", {
+                    }, "Scenario"), p().createElement("div", {
                         className: "up-BenchmarkLauncher-choices",
                         onChange: this.onScenarioChanged.bind(this)
-                    }, n), d().createElement("div", {
+                    }, n), p().createElement("div", {
                         className: "up-BenchmarkLauncher-forms"
                     }, this.state.scenarios.map((e => {
                         const t = e.configSchema?.properties;
-                        return e.configSchema && t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", d().createElement(u.ZP, {
+                        return e.configSchema && t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", p().createElement(u.ZP, {
                             key: "up-profiler-scenario-" + e.id,
                             schema: e.configSchema,
                             idPrefix: "up-profiler-scenario-" + e.id,
                             onChange: t => {
                                 this._config.scenarios[e.id] = t.formData
                             },
                             formData: this._config.scenarios[e.id],
                             FieldTemplate: this.state.fieldTemplate,
                             ArrayFieldTemplate: this.state.arrayFieldTemplate,
                             ObjectFieldTemplate: this.state.objectFieldTemplate,
                             liveValidate: !0
-                        })) : d().createElement(ie, {
+                        })) : p().createElement(ie, {
                             name: e.name
                         })
-                    }))))), d().createElement("div", {
+                    }))))), p().createElement("div", {
                         className: "up-BenchmarkLauncher-launchbar"
-                    }, d().createElement(ne, Object.assign({}, this.props)), d().createElement("div", {
+                    }, p().createElement(ne, Object.assign({}, this.props)), p().createElement("div", {
                         className: "up-BenchmarkLauncher-launchbar-buttons"
-                    }, d().createElement("button", {
+                    }, p().createElement("button", {
                         onClick: this.runSelected,
                         className: "jp-mod-styled jp-mod-accept" + (this.state.isRunning ? " jp-mod-hidden" : ""),
                         disabled: 0 === this.state.scenarios.length || 0 === this.state.benchmarks.length || this.state.isRunning
-                    }, "Start"), d().createElement("button", {
+                    }, "Start"), p().createElement("button", {
                         onClick: this.stopCurrent,
                         className: "jp-mod-styled jp-mod-warn" + (this.state.isRunning ? "" : " jp-mod-hidden"),
                         disabled: !this.state.isRunning
                     }, "Stop"))))
                 }
             }
             async function oe(e) {
@@ -1397,177 +1397,186 @@
                     if (!e) continue;
                     const r = await oe(i.textContent),
                         o = r ? r.sources[0] : null;
                     n++;
                     const a = e.rules;
                     for (let i = 0; i < a.length; i++) {
                         const r = a[i];
-                        r instanceof CSSStyleRule && (t.skipPattern && null != r.selectorText.match(t.skipPattern) || s.push({
+                        r instanceof CSSStyleRule && (t.skipPattern && null != r.selectorText.match(t.skipPattern) || t.includePattern && null == r.selectorText.match(t.includePattern) || s.push({
                             rule: r,
                             selector: r.selectorText,
                             sheet: e,
                             source: o,
                             ruleIndex: i,
                             stylesheetIndex: n
                         }))
                     }
                 }
                 return s
             }
-            const le = JSON.parse('{"title":"Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5}}}'),
-                ce = JSON.parse('{"title":"Style Rule Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":3},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"}}}'),
-                ue = JSON.parse('{"title":"Style Rule Group Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"},"minBlocks":{"title":"Block size to start with","type":"integer","minimum":1,"default":3},"maxBlocks":{"title":"Maximal block size","type":"integer","minimum":1,"default":5},"sheetRandomizations":{"title":"Number of sheet randomizations","type":"integer","minimum":0,"default":5}}}'),
-                pe = JSON.parse('{"title":"Style Rule Usage Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"::"},"excludeMatchPattern":{"title":"Regular expression to filter out classes used for rule discovery","type":"string","default":"(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)"}}}');
-            class de extends Map {
+            const le = JSON.parse('{"title":"Style Rule Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":3},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"},"includePattern":{"title":"Regular expression to filter rules to include","type":"string","default":""}}}'),
+                ce = JSON.parse('{"title":"Style Rule Group Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"},"minBlocks":{"title":"Block size to start with","type":"integer","minimum":1,"default":3},"maxBlocks":{"title":"Maximal block size","type":"integer","minimum":1,"default":5},"sheetRandomizations":{"title":"Number of sheet randomizations","type":"integer","minimum":0,"default":5},"includePattern":{"title":"Regular expression to filter rules to include","type":"string","default":""}}}'),
+                ue = JSON.parse('{"title":"Style Rule Usage Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"::"},"excludeMatchPattern":{"title":"Regular expression to filter out classes used for rule discovery","type":"string","default":"(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)"},"includePattern":{"title":"Regular expression to filter rules to include","type":"string","default":""}}}'),
+                de = JSON.parse('{"title":"Style Sheet Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"includePattern":{"title":"Regular expression to filter sheets to benchmark","type":"string","default":""}}}');
+            class pe extends Map {
                 add(e, t) {
                     let n = this.get(e);
                     n || (n = new Set, this.set(e, n)), n.add(t)
                 }
                 countRulesUsage() {
                     const e = new Map;
                     for (const t of this.values())
                         for (const n of t.values()) e.set(n, (e.get(n) || 0) + 1);
                     return e
                 }
             }
             const me = {
                     id: "rule-usage",
                     name: "Style Rule Usage",
-                    configSchema: pe,
+                    configSchema: ue,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
                             a = Date.now(),
                             l = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
-                            c = t.excludeMatchPattern ? new RegExp(t.excludeMatchPattern, "g") : void 0;
+                            c = t.includePattern ? new RegExp(t.includePattern, "g") : void 0,
+                            u = t.excludeMatchPattern ? new RegExp(t.excludeMatchPattern, "g") : void 0;
                         e.setupSuite && await e.setupSuite();
-                        const u = await D(e, 2 * o, !0);
-                        console.log("Reference for", e.name, "is:", u);
+                        const d = await D(e, 2 * o, !0);
+                        console.log("Reference for", e.name, "is:", d);
                         const p = {
                                 subtree: !0,
                                 childList: !0,
                                 attributes: !0
                             },
-                            d = new Set,
-                            m = e => {
-                                for (const t of S(e)) d.add(t)
+                            m = new Set,
+                            h = e => {
+                                for (const t of S(e)) m.add(t)
                             },
-                            h = new MutationObserver(m);
-                        await M(), h.observe(document.body, p), await D(e, o, !0), await M(), m(h.takeRecords()), h.disconnect();
-                        const f = [...d].filter((e => e instanceof Element)).filter((e => "body" !== e.tagName.toLocaleLowerCase()));
-                        console.log("Relevant nodes:", d);
-                        const g = new Set([...f.map((e => [...e.classList.values()])).flat().filter((e => !c || !e.match(c)))]),
-                            w = f.filter((e => e.id)).map((e => e.id));
-                        console.log("Relevant class names:", g), console.log("Relevant IDs:", w);
-                        const y = [],
+                            f = new MutationObserver(h);
+                        await M(), f.observe(document.body, p), await D(e, o, !0), await M(), h(f.takeRecords()), f.disconnect();
+                        const g = [...m].filter((e => e instanceof Element)).filter((e => "body" !== e.tagName.toLocaleLowerCase()));
+                        console.log("Relevant nodes:", m);
+                        const w = new Set([...g.map((e => [...e.classList.values()])).flat().filter((e => !u || !e.match(u)))]),
+                            y = g.filter((e => e.id)).map((e => e.id));
+                        console.log("Relevant class names:", w), console.log("Relevant IDs:", y);
+                        const v = [],
                             k = [...document.querySelectorAll("style")],
-                            v = await ae(k, {
-                                skipPattern: l
+                            E = await ae(k, {
+                                skipPattern: l,
+                                includePattern: c
                             }),
-                            E = new Set;
-                        for (const e of v) {
-                            for (const t of g)
+                            x = new Set;
+                        for (const e of E) {
+                            for (const t of w)
                                 if (e.selector.includes("." + t)) {
-                                    E.add(e);
+                                    x.add(e);
                                     break
-                                } for (const t of w)
+                                } for (const t of y)
                                 if (e.selector.includes("#" + t)) {
-                                    E.add(e);
+                                    x.add(e);
                                     break
                                 }
                         }
-                        const x = [...E];
+                        const j = [...x];
                         n?.emit({
-                            percentage: 50 / x.length
+                            percentage: 50 / j.length
                         });
-                        const j = new Map,
-                            N = new de,
-                            C = new de,
-                            O = e => {
+                        const N = new Map,
+                            C = new pe,
+                            O = new pe,
+                            I = e => {
                                 const t = new Set;
                                 for (const n of S(e)) t.add(n);
                                 for (const e of t)
                                     if (e instanceof Element)
-                                        for (const t of E) e.matches(t.selector) && (j.set(t.selector, (j.get(t.selector) || 0) + 1), C.add(e, t.selector));
-                                for (const e of E)
-                                    for (const t of document.querySelectorAll(e.selector)) N.add(t, e.selector)
+                                        for (const t of x) e.matches(t.selector) && (N.set(t.selector, (N.get(t.selector) || 0) + 1), O.add(e, t.selector));
+                                for (const e of x)
+                                    for (const t of document.querySelectorAll(e.selector)) C.add(t, e.selector)
                             },
-                            I = new MutationObserver(O);
-                        I.observe(document.body, p), await D(e, o, !0), await M(), O(I.takeRecords()), I.disconnect();
-                        const _ = C.countRulesUsage(),
-                            T = N.countRulesUsage();
-                        for (let t = 0; t < x.length && !i; t++) {
+                            T = new MutationObserver(I);
+                        T.observe(document.body, p), await D(e, o, !0), await M(), I(T.takeRecords()), T.disconnect();
+                        const _ = O.countRulesUsage(),
+                            R = C.countRulesUsage();
+                        for (let t = 0; t < j.length && !i; t++) {
                             n?.emit({
-                                percentage: 100 * (t + .5) / x.length
+                                percentage: 100 * (t + .5) / j.length
                             });
-                            const s = x[t];
+                            const s = j[t];
                             s.sheet.deleteRule(s.ruleIndex), await M();
                             const i = await D(e, o, !0);
-                            y.push({
+                            v.push({
                                 ...i,
                                 selector: s.selector,
                                 source: s.source,
                                 ruleIndex: s.ruleIndex,
                                 stylesheetIndex: s.stylesheetIndex,
-                                touchCount: j.get(s.selector) || 0,
+                                touchCount: N.get(s.selector) || 0,
                                 elementsTouched: _.get(s.selector) || 0,
-                                elementsSeen: T.get(s.selector) || 0
+                                elementsSeen: R.get(s.selector) || 0
                             }), s.sheet.insertRule(s.rule.cssText, s.ruleIndex), await M()
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(r), {
-                            results: y,
-                            reference: u.times,
+                            results: v,
+                            reference: d.times,
                             tags: b(),
                             totalTime: Date.now() - a,
                             type: "time",
                             interrupted: i
                         }
                     },
                     sortColumn: "elementsSeen",
-                    interpretation: d().createElement(d().Fragment, null, d().createElement("ul", null, d().createElement("li", null, d().createElement("code", null, "elementsSeen"), ": how many elements were seen on the entire page when executing the scenario."), d().createElement("li", null, d().createElement("code", null, "elementsTouched"), ": how many elements were modified or in the subtree of a modified element when executing the scenario."), d().createElement("li", null, d().createElement("code", null, "touchCount"), ": upper bound on how many times the rule matched an element (will be high for rules matching many elements, and for rules matching a single element that is repeatedly modified in the chosen scenario).")), d().createElement("div", null, "Low number of ", d().createElement("code", null, "elementsSeen"), " suggest potentially unused rule. Negative ", d().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
+                    interpretation: p().createElement(p().Fragment, null, p().createElement("ul", null, p().createElement("li", null, p().createElement("code", null, "elementsSeen"), ": how many elements were seen on the entire page when executing the scenario."), p().createElement("li", null, p().createElement("code", null, "elementsTouched"), ": how many elements were modified or in the subtree of a modified element when executing the scenario."), p().createElement("li", null, p().createElement("code", null, "touchCount"), ": upper bound on how many times the rule matched an element (will be high for rules matching many elements, and for rules matching a single element that is repeatedly modified in the chosen scenario).")), p().createElement("div", null, "Low number of ", p().createElement("code", null, "elementsSeen"), " suggest potentially unused rule. Negative ", p().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
                 },
                 he = {
                     id: "style-sheet",
                     name: "Style Sheets",
-                    configSchema: le,
+                    configSchema: de,
                     run: async (e, t = {}, n, s) => {
                         const i = t.repeats || 3,
                             r = Date.now();
                         let o = !1;
                         const a = () => {
                             o = !0
                         };
                         s?.connect(a), e.setupSuite && await e.setupSuite();
                         const l = [...document.querySelectorAll("style")],
                             c = await D(e, 2 * i, !0);
                         console.log("Reference for", e.name, "is:", c);
                         const u = [];
-                        let p = 0,
-                            d = 0;
-                        const m = l.filter((e => e.sheet));
-                        m.length !== l.length && console.log("Skipped", l.length - m.length, "style tags without stylesheets (out of", l.length, "total)");
+                        let d = 0,
+                            p = 0;
+                        const m = t.includePattern ? new RegExp(t.includePattern, "g") : void 0,
+                            h = l.filter((e => e.sheet));
+                        h.length !== l.length && console.log("Skipped", l.length - h.length, "style tags without stylesheets (out of", l.length, "total)");
+                        const f = h.length;
                         for (const t of l) {
                             if (o) break;
                             const s = t.sheet;
-                            if (d++, !s) continue;
+                            if (p++, !s) continue;
                             n?.emit({
-                                percentage: 100 * p / m.length
-                            }), p++, s.disabled = !0, await M();
-                            const r = await D(e, i, !0);
-                            await M(), s.disabled = !1;
-                            const a = await oe(t.textContent);
-                            u.push({
-                                ...r,
+                                percentage: 100 * d / f
+                            }), d++;
+                            const r = await oe(t.textContent),
+                                a = null != r ? r.sources[0] : null;
+                            if (m) {
+                                if (null === a) continue;
+                                if (null == a.match(m)) continue
+                            }
+                            s.disabled = !0, await M();
+                            const l = await D(e, i, !0);
+                            await M(), s.disabled = !1, u.push({
+                                ...l,
                                 content: t.textContent,
-                                source: null != a ? a.sources[0] : null,
-                                stylesheetIndex: d
+                                source: a,
+                                stylesheetIndex: p
                             })
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(a), {
                             results: u,
                             reference: c.times,
                             tags: b(),
                             totalTime: Date.now() - r,
@@ -1575,108 +1584,112 @@
                             interrupted: o
                         }
                     }
                 },
                 fe = {
                     id: "style-rule",
                     name: "Style Rules",
-                    configSchema: ce,
+                    configSchema: le,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
                             a = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
-                            l = Date.now();
+                            l = t.includePattern ? new RegExp(t.includePattern, "g") : void 0,
+                            c = Date.now();
                         e.setupSuite && await e.setupSuite();
-                        const c = [...document.querySelectorAll("style")],
-                            u = await D(e, 2 * o, !0);
-                        console.log("Reference for", e.name, "is:", u);
+                        const u = [...document.querySelectorAll("style")],
+                            d = await D(e, 2 * o, !0);
+                        console.log("Reference for", e.name, "is:", d);
                         const p = [],
-                            d = await ae(c, {
-                                skipPattern: a
+                            m = await ae(u, {
+                                skipPattern: a,
+                                includePattern: l
                             });
-                        for (let t = 0; t < d.length && !i; t++) {
+                        for (let t = 0; t < m.length && !i; t++) {
                             n?.emit({
-                                percentage: 100 * t / d.length
+                                percentage: 100 * t / m.length
                             });
-                            const s = d[t];
+                            const s = m[t];
                             s.sheet.deleteRule(s.ruleIndex), await M();
                             const i = await D(e, o, !0);
                             p.push({
                                 ...i,
                                 selector: s.selector,
                                 source: s.source,
                                 ruleIndex: s.ruleIndex,
                                 stylesheetIndex: s.stylesheetIndex,
                                 bgMatches: document.querySelectorAll(s.selector).length
                             }), s.sheet.insertRule(s.rule.cssText, s.ruleIndex), await M()
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(r), {
                             results: p,
-                            reference: u.times,
+                            reference: d.times,
                             tags: b(),
-                            totalTime: Date.now() - l,
+                            totalTime: Date.now() - c,
                             type: "time",
                             interrupted: i
                         }
                     },
-                    interpretation: d().createElement(d().Fragment, null, d().createElement("ul", null, d().createElement("li", null, d().createElement("code", null, "bgMatches"), ": how many elements matched the rule at standby (as compared to during scenario execution); mostly useful to find too broad rules, or potentially unused rules with expensive selectors.")), d().createElement("div", null, "Negative ", d().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
+                    interpretation: p().createElement(p().Fragment, null, p().createElement("ul", null, p().createElement("li", null, p().createElement("code", null, "bgMatches"), ": how many elements matched the rule at standby (as compared to during scenario execution); mostly useful to find too broad rules, or potentially unused rules with expensive selectors.")), p().createElement("div", null, "Negative ", p().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
                 },
                 ge = {
                     id: "style-rule-group",
                     name: "Style Rule Groups",
-                    configSchema: ue,
+                    configSchema: ce,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
                             a = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
-                            l = t.maxBlocks || 5,
-                            c = t.minBlocks || 2,
-                            u = Date.now();
+                            l = t.includePattern ? new RegExp(t.includePattern, "g") : void 0,
+                            c = t.maxBlocks || 5,
+                            u = t.minBlocks || 2,
+                            d = Date.now();
                         e.setupSuite && await e.setupSuite();
                         let p = [...document.querySelectorAll("style")];
-                        const d = await D(e, 2 * o, !0);
-                        console.log("Reference for", e.name, "is:", d);
-                        const m = [],
-                            h = t.sheetRandomizations || 0;
-                        let f = 0;
-                        const g = (l - c + 1) * (h + 1);
-                        for (let t = 0; t < h + 1 && !i; t++) {
+                        const m = await D(e, 2 * o, !0);
+                        console.log("Reference for", e.name, "is:", m);
+                        const h = [],
+                            f = t.sheetRandomizations || 0;
+                        let g = 0;
+                        const w = (c - u + 1) * (f + 1);
+                        for (let t = 0; t < f + 1 && !i; t++) {
                             0 !== t && (p = p.map((e => ({
                                 value: e,
                                 sort: Math.random()
                             }))).sort(((e, t) => e.sort - t.sort)).map((({
                                 value: e
                             }) => e)));
                             const s = await ae(p, {
-                                skipPattern: a
+                                skipPattern: a,
+                                includePattern: l
                             });
                             console.log(`Collected ${s.length} rules, randomization: ${t}`);
-                            for (let r = c; r <= l && !i; r++) {
-                                f += 1, n?.emit({
-                                    percentage: 100 * f / g
+                            for (let r = u; r <= c && !i; r++) {
+                                g += 1, n?.emit({
+                                    percentage: 100 * g / w
                                 });
                                 const i = Math.round(s.length / r);
                                 console.log(`Benchmarking ${r} blocks, each having ${i} rules`);
                                 for (let n = 0; n < r; n++) {
                                     const a = [];
                                     for (let e = i; e >= 0; e--) {
                                         const t = s[n * i + e];
                                         void 0 !== t && (a.push(t), t.sheet.deleteRule(t.ruleIndex))
                                     }
                                     await M();
                                     const l = await D(e, o, !0);
-                                    m.push({
+                                    h.push({
                                         ...l,
                                         rulesInBlock: a,
                                         block: n,
                                         divisions: r,
                                         randomization: t
                                     });
                                     for (let e = a.length - 1; e >= 0; e--) {
@@ -1684,33 +1697,33 @@
                                         t.sheet.insertRule(t.rule.cssText, t.ruleIndex)
                                     }
                                     await M()
                                 }
                             }
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(r), {
-                            results: m,
-                            reference: d.times,
+                            results: h,
+                            reference: m.times,
                             tags: b(),
-                            totalTime: Date.now() - u,
+                            totalTime: Date.now() - d,
                             type: "time",
                             interrupted: i
                         }
                     },
                     render: function(e) {
                         const t = e.outcome.results,
-                            [n, s] = d().useState("block"),
-                            i = d().useRef(null);
+                            [n, s] = p().useState("block"),
+                            i = p().useRef(null);
                         null !== i.current && i.current.stateSource === e.outcome || (i.current = new V({
                             measurements: t,
                             reference: e.outcome.reference,
                             stateSource: e.outcome,
                             lowerIsBetter: !1
                         }));
-                        const r = d().useRef(null);
+                        const r = p().useRef(null);
                         if (null === r.current || r.current.stateSource !== e.outcome) {
                             const n = {};
                             for (const e of t)
                                 for (const t of e.rulesInBlock)
                                     if (t.selector in n) n[t.selector].times.push(...e.times);
                                     else {
                                         const s = {
@@ -1722,29 +1735,29 @@
                                     } r.current = new V({
                                 measurements: [...Object.values(n)],
                                 reference: e.outcome.reference,
                                 stateSource: e.outcome,
                                 lowerIsBetter: !1
                             })
                         }
-                        return d().createElement(d().Fragment, null, d().createElement("div", {
+                        return p().createElement(p().Fragment, null, p().createElement("div", {
                             onChange: e => {
                                 s(e.target.value)
                             }
-                        }, d().createElement("label", null, d().createElement("input", {
+                        }, p().createElement("label", null, p().createElement("input", {
                             type: "radio",
                             checked: "block" === n,
                             value: "block"
-                        }), "Blocks"), d().createElement("label", null, d().createElement("input", {
+                        }), "Blocks"), p().createElement("label", null, p().createElement("input", {
                             type: "radio",
                             checked: "rule" === n,
                             value: "rule"
-                        }), "Rules")), "block" === n ? d().createElement(K, {
+                        }), "Rules")), "block" === n ? p().createElement(K, {
                             widget: i.current
-                        }) : d().createElement(K, {
+                        }) : p().createElement(K, {
                             widget: r.current
                         }))
                     }
                 },
                 we = new f.Token("@jupyterlab/ui-profiler:plugin");
 
             function ye(e) {
@@ -1815,90 +1828,90 @@
                         client: e.name,
                         version: e.version,
                         devMode: "true" === (g.PageConfig.getOption("devMode") || "").toLowerCase(),
                         mode: g.PageConfig.getOption("mode")
                     }
                 }
             }
-            const ke = JSON.parse('{"title":"Scenario Options","type":"object","properties":{}}'),
-                ve = JSON.parse('{"title":"Menu Open Scenario Options","type":"object","properties":{"menu":{"title":"The menu to open","type":"string","default":"file","enum":["file","edit","view","run","kernel","settings","help"]}},"required":["menu"]}'),
+            const ve = JSON.parse('{"title":"Scenario Options","type":"object","properties":{}}'),
+                ke = JSON.parse('{"title":"Menu Open Scenario Options","type":"object","properties":{"menu":{"title":"The menu to open","type":"string","default":"file","enum":["file","edit","view","run","kernel","settings","help"]}},"required":["menu"]}'),
                 Se = JSON.parse('{"title":"Tab Scenario Options","type":"object","definitions":{"tab":{"description":"Tab to open","type":"object","properties":{"path":{"title":"Path","description":"Location of file/notebook to open. If empty opens a new launcher.","type":"string"}},"default":{"path":""}}},"properties":{"tabs":{"title":"List of tabs to use in scenario","description":"Series of two or more tabs","type":"array","items":{"$ref":"#/definitions/tab"},"default":[{"path":""},{"path":""}]}},"required":["tabs"]}'),
                 Ee = JSON.parse('{"title":"Completer Scenario Options","type":"object","properties":{"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"File Editor"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"setup":{"title":"Editor setup for completion","description":"How should the editor be populated?","default":{"tokenCount":1000,"tokenSize":50},"anyOf":[{"type":"object","title":"Auto-generate tokens to complete","properties":{"tokenCount":{"title":"Token count","description":"The number of completion items to generate","type":"number","minimum":1,"default":1000},"tokenSize":{"title":"Token size","description":"The number characters in each token","type":"number","minimum":1,"default":50}},"required":["tokenCount","tokenSize"]},{"type":"object","title":"I will provide a custom text","properties":{"setupText":{"title":"Trigger code","description":"Text to enter into the editor. Last line should include a partial token on which the completion will be riggered.","type":"string","default":"np."},"setupCell":{"title":"Code to run (notebook only)","description":"Code to run prior to invoking completer, e.g. `import numpy as np`. Only has an effect in notebook.","type":"string","default":"import numpy as np"}},"required":["setupText","triggerCell"]}]},"widgetPosition":{"title":"Widget position in the layout","description":"Where to attach the editor widget in the layout","type":"string","enum":["split-top","split-left","split-right","split-bottom","tab-before","tab-after"],"default":"split-right"}},"required":["editor","setup"],"additionalProperties":false}'),
                 xe = JSON.parse('{"title":"Debugger Scenario Options","type":"object","properties":{"codeCells":{"title":"Code to execute","description":"Python code cells to execute one-by-one to populate the debugger namespace, e.g. `from numpy import *`","type":"array","items":{"type":"string"},"default":["[globals().__setitem__(f\'x{i}\', \'y\') for i in range(1000)];","z = 1"]},"expectedNumberOfVariables":{"title":"Expected number of variables","description":"The scenario waits until debugger panel is populated with at least as many variables as specified. For accurate timings should have as many members as there are code cells.","type":"array","items":{"type":"integer","min":0},"default":[1000,1001]},"widgetPosition":{"title":"Widget position in the layout","description":"Where to attach the editor widget in the layout","type":"string","enum":["split-top","split-left","split-right","split-bottom","tab-before","tab-after"],"default":"split-right"}},"required":["codeCells","expectedNumberOfVariables"],"additionalProperties":false}'),
                 je = JSON.parse('{"title":"Sidebars Scenario Options","type":"object","properties":{"sidebars":{"title":"The sidebars to open","type":"array","default":["table-of-contents","jp-debugger-sidebar","jp-property-inspector","filebrowser","extensionmanager.main-view","jp-running-sessions"],"items":{"type":"string"}}},"required":["sidebars"]}'),
                 Ne = JSON.parse('{"title":"Scroll Scenario Options","type":"object","properties":{"scrollTop":{"title":"Scroll from top","description":"Number of pixes to scroll by","type":"number","minimum":0,"default":10000},"scrollBehavior":{"title":"Scroll behaviour","description":"Behavior of scroll, either \'smooth\' for smooth scrolling, or \'auto\' for instant scrolling.","type":"string","enum":["smooth","auto"],"default":"smooth"},"cellByCell":{"title":"Traverse cell-by-cell","description":"Instead of scrolling, traverse notebook cell-by-cell (which also combines stepwise scrolling and cell activation/deactivation). Small number of cells (50-100) is recommended for benchmarking such scenario. \'scrollTop\' and \'scrollBehavior\' have no effect if this variant is enabled. Has no effect in file editor.","type":"boolean","default":false},"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"Notebook"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"cells":{"title":"Number of cells/blocks to append","description":"If using a notebook, how many cell should be created? For file editor, how many lines?","type":"number","minimum":0,"default":1000},"editorContent":{"title":"Editor/cell content","description":"Text to populate editors/cells with.","type":"string","default":"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."},"widgetPosition":{"title":"Widget position in the layout","description":"Where to attach the editor widget in the layout","type":"string","enum":["split-top","split-left","split-right","split-bottom","tab-before","tab-after"],"default":"split-right"}},"required":["editor","cells","scrollTop","scrollBehavior"],"additionalProperties":false}');
             async function Me(e, t = "file") {
-                await e.commands.execute(`${t}menu:open`), await P.waitForSelector(`#jp-mainmenu-${t}`, {
+                await e.commands.execute(`${t}menu:open`), await A.waitForSelector(`#jp-mainmenu-${t}`, {
                     state: "attached"
                 }), await M()
             }
             async function Ce() {
-                await P.waitForSelector(".lm-Menu", {
+                await A.waitForSelector(".lm-Menu", {
                     state: "attached"
-                }), await P.press("Escape"), await P.waitForSelector(".lm-Menu", {
+                }), await A.press("Escape"), await A.waitForSelector(".lm-Menu", {
                     state: "detached"
                 }), await M()
             }
             class Oe {
                 constructor(e) {
-                    this.jupyterApp = e, this.cleanup = Ce, this.id = "menuSwitch", this.name = "Switch Menu", this.configSchema = ke
+                    this.jupyterApp = e, this.cleanup = Ce, this.id = "menuSwitch", this.name = "Switch Menu", this.configSchema = ve
                 }
                 async setup() {
                     return Me(this.jupyterApp)
                 }
                 async run() {
                     return async function(e) {
                         for (const t of ["edit", "view", "run", "kernel", "settings", "help"]) await Me(e, t)
                     }(this.jupyterApp)
                 }
             }
             class Ie {
                 constructor(e) {
-                    this.jupyterApp = e, this.cleanup = Ce, this.id = "menuOpen", this.name = "Open Menu", this.configSchema = ve, this._menu = "file"
+                    this.jupyterApp = e, this.cleanup = Ce, this.id = "menuOpen", this.name = "Open Menu", this.configSchema = ke, this._menu = "file"
                 }
                 setOptions(e) {
                     this._menu = e.menu
                 }
                 async run() {
                     return Me(this.jupyterApp, this._menu)
                 }
             }
-            class _e {
+            class Te {
                 constructor(e) {
                     this.jupyterApp = e, this.id = "sidebarOpen", this.name = "Open Sidebar", this.configSchema = je, this._sidebars = ["filebrowser"]
                 }
                 setOptions(e) {
                     this._sidebars = e.sidebars
                 }
                 async setup() {
                     return async function(e) {
                         for (const t of ["left", "right"]) {
                             const n = document.querySelector(`#jp-${t}-stack`);
-                            n && !n.classList.contains("lm-mod-hidden") && (await e.commands.execute(`application:toggle-${t}-area`), await P.waitForSelector(`#jp-${t}-stack`, {
+                            n && !n.classList.contains("lm-mod-hidden") && (await e.commands.execute(`application:toggle-${t}-area`), await A.waitForSelector(`#jp-${t}-stack`, {
                                 state: "hidden"
                             }), await M())
                         }
                     }(this.jupyterApp)
                 }
                 async run() {
-                    for (const e of this._sidebars) this.jupyterApp.shell.activateById(e), await P.waitForSelector(`#${CSS.escape(e)}`, {
+                    for (const e of this._sidebars) this.jupyterApp.shell.activateById(e), await A.waitForSelector(`#${CSS.escape(e)}`, {
                         state: "visible"
                     }), await M()
                 }
             }
 
-            function Te(e, t) {
+            function _e(e, t) {
                 return e.commands.execute("apputils:run-first-enabled", {
                     commands: ["notebook:replace-selection", "console:replace-selection", "fileeditor:replace-selection"],
                     args: {
                         text: t
                     }
                 })
             }
-            class Be {
+            class Re {
                 constructor(e) {
                     this.jupyterApp = e, this.editor = null, this.path = null, this.options = null, this.useNotebook = !0, this.widget = null
                 }
                 setOptions(e) {
                     this.options = e, this.useNotebook = "Notebook" === this.options.editor
                 }
                 async setupSuite() {
@@ -1917,40 +1930,40 @@
                     }
                     const e = await this.jupyterApp.commands.execute("docmanager:open", {
                         path: this.path,
                         factory: this.useNotebook ? "Notebook" : "Editor"
                     });
                     this.widget = e, this.jupyterApp.shell.add(this.widget, "main", {
                         mode: this.options?.widgetPosition || "split-right"
-                    }), await Fe(this.jupyterApp, e), await M(), this.useNotebook && await P.click(".jp-Dialog-button.jp-mod-accept");
+                    }), await Fe(this.jupyterApp, e), await M(), this.useNotebook && await A.click(".jp-Dialog-button.jp-mod-accept");
                     const t = new C(this.widget.node);
                     await t.waitForSelector(".jp-Editor", {
                         state: "attached"
                     }), await M(), await t.waitForSelector(".jp-Editor", {
                         state: "visible"
                     }), await M(), this.editor = this.useNotebook ? this.widget.node.querySelector(".jp-Notebook") : this.widget.node.querySelector(".jp-FileEditorCodeWrapper")
                 }
                 async cleanupSuite() {
                     this.widget && (await this.jupyterApp.commands.execute("docmanager:save"), this.widget.close())
                 }
             }
-            class Re extends Be {
+            class Be extends Re {
                 constructor() {
                     super(...arguments), this.id = "completer", this.name = "Completer", this.configSchema = Ee
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     let e;
                     if (void 0 !== this.options.setup?.setupText) e = this.options.setup.setupText;
                     else {
                         const t = [];
                         for (let e = 0; e < this.options.setup.tokenCount; e++) t.push(("t" + e).padEnd(this.options.setup.tokenSize, "x") + " = " + e);
                         t.push("t"), e = t.join("\n")
                     }
-                    this.useNotebook && this.options.setup.setupCell ? (await Te(this.jupyterApp, this.options.setup.setupCell), await De(this.widget.node, "idle"), await this.jupyterApp.commands.execute("notebook:run-cell-and-insert-below"), await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:enter-edit-mode")) : await Te(this.jupyterApp, e), this.useNotebook || (this.editor.querySelector(".CodeMirror-scroll") || this.editor.querySelector(".cm-scroller")).scrollBy({
+                    this.useNotebook && this.options.setup.setupCell ? (await _e(this.jupyterApp, this.options.setup.setupCell), await De(this.widget.node, "idle"), await this.jupyterApp.commands.execute("notebook:run-cell-and-insert-below"), await _e(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:enter-edit-mode")) : await _e(this.jupyterApp, e), this.useNotebook || (this.editor.querySelector(".CodeMirror-scroll") || this.editor.querySelector(".cm-scroller")).scrollBy({
                         top: 20 * this.options.setup.tokenCount,
                         left: 0,
                         behavior: "smooth"
                     });
                     try {
                         await this.run()
                     } catch (e) {}
@@ -1960,38 +1973,38 @@
                     if (this.useNotebook) {
                         const e = new C(this.widget.node),
                             t = document.querySelector(".cm-content") ? ".cm-content" : "textarea",
                             n = this.options.setup.setupCell ? await e.$(`.jp-Cell:nth-child(2) .jp-Editor ${t}`) : await e.$(`.jp-Editor ${t}`);
                         if (!n) throw Error("Setup failed: cell editor could not be located");
                         await n.focus()
                     }
-                    await M(), await P.press("Tab"), await M(), await P.waitForSelector(".jp-Completer.jp-HoverBox[style]", {
+                    await M(), await A.press("Tab"), await M(), await A.waitForSelector(".jp-Completer.jp-HoverBox[style]", {
                         state: "attached"
-                    }), await P.waitForSelector(".jp-Completer.jp-HoverBox[style]", {
+                    }), await A.waitForSelector(".jp-Completer.jp-HoverBox[style]", {
                         state: "visible"
                     }), await M()
                 }
                 async cleanup() {
-                    await P.press("Escape"), await M(), await P.waitForSelector(".jp-Completer[style]", {
+                    await A.press("Escape"), await M(), await A.waitForSelector(".jp-Completer[style]", {
                         state: "hidden"
                     }), await M()
                 }
             }
-            async function Ae() {
+            async function Pe() {
                 const e = ".jp-Toolbar-responsive-popup",
-                    t = await P.$('.jp-Toolbar-responsive-opener > button[title="More commands"]');
+                    t = await A.$('.jp-Toolbar-responsive-opener > button[title="More commands"]');
                 if (t && await t.isVisible()) {
-                    const n = await P.$(e);
+                    const n = await A.$(e);
                     if (n && await n.isVisible()) return;
-                    await t.click(), await P.waitForSelector(e, {
+                    await t.click(), await A.waitForSelector(e, {
                         state: "visible"
                     })
                 }
             }
-            class Pe extends Be {
+            class Ae extends Re {
                 constructor() {
                     super(...arguments), this.id = "debugger", this.name = "Debugger", this.configSchema = xe
                 }
                 setOptions(e) {
                     super.setOptions({
                         ...e,
                         editor: "Notebook",
@@ -2000,37 +2013,37 @@
                 }
                 async _goToTop() {
                     if (!this.options) throw new Error("Setup failure");
                     for (let e = 0; e < this.options.codeCells.length + 1; e++) await this.jupyterApp.commands.execute("notebook:move-cursor-up")
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
-                    for (const e of this.options.codeCells) await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:insert-cell-below"), await M(), await M(), await this.jupyterApp.commands.execute("notebook:enter-edit-mode"), await M(), await M();
-                    await Te(this.jupyterApp, "%reset -f"), await this._goToTop(), await De(this.widget.node, "idle");
+                    for (const e of this.options.codeCells) await _e(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:insert-cell-below"), await M(), await M(), await this.jupyterApp.commands.execute("notebook:enter-edit-mode"), await M(), await M();
+                    await _e(this.jupyterApp, "%reset -f"), await this._goToTop(), await De(this.widget.node, "idle");
                     const e = new C(this.widget.node);
-                    await Ae();
+                    await Pe();
                     const t = await e.waitForSelector('button[aria-disabled="false"][title="Enable Debugger"]', {
                         state: "attached"
                     });
-                    await t.click(), await P.waitForSelector(`#${CSS.escape("jp-debugger-sidebar")}`, {
+                    await t.click(), await A.waitForSelector(`#${CSS.escape("jp-debugger-sidebar")}`, {
                         state: "visible"
-                    }), await Ae(), await e.waitForSelector('button[aria-disabled="false"][title="Disable Debugger"]', {
+                    }), await Pe(), await e.waitForSelector('button[aria-disabled="false"][title="Disable Debugger"]', {
                         state: "attached"
-                    }), await M(), await P.waitForSelector(".jp-DebuggerVariables-body", {
+                    }), await M(), await A.waitForSelector(".jp-DebuggerVariables-body", {
                         state: "attached"
-                    }), await P.waitForSelector(".jp-DebuggerVariables-body", {
+                    }), await A.waitForSelector(".jp-DebuggerVariables-body", {
                         state: "visible"
                     })
                 }
                 async run() {
                     if (!this.widget || !this.options) throw new Error("Setup failure");
                     for (let e = 0; e < this.options.codeCells.length; e++) {
                         await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await De(this.widget.node, "idle");
                         const t = this.options.expectedNumberOfVariables[e];
-                        void 0 !== t && await P.waitForSelector(`.jp-DebuggerVariables-body li:nth-child(${t+2})`, {
+                        void 0 !== t && await A.waitForSelector(`.jp-DebuggerVariables-body li:nth-child(${t+2})`, {
                             state: "attached"
                         }), await M()
                     }
                 }
                 async cleanup() {
                     if (!this.widget || !this.options) throw new Error("Setup failure");
                     await M();
@@ -2047,26 +2060,26 @@
                 await new C(e).waitForSelector(`.jp-Notebook-ExecutionIndicator[data-status="${t}"]`, {
                     state: "attached"
                 })
             }
             async function Fe(e, t) {
                 await e.commands.execute("tabsmenu:activate-by-id", {
                     id: t.id
-                }), await M(), await P.waitForSelector(`li.lm-mod-current[data-id="${t.id}"]`, {
+                }), await M(), await A.waitForSelector(`li.lm-mod-current[data-id="${t.id}"]`, {
                     state: "attached"
                 }), await M()
             }
-            class qe extends Be {
+            class qe extends Re {
                 constructor() {
                     super(...arguments), this.id = "scroll", this.name = "Scroll", this.configSchema = Ne
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     const e = this.options.cells < 100 ? 20 : 50;
-                    for (let t = 0; t < this.options.cells; t++) this.useNotebook && await this.jupyterApp.commands.execute("notebook:insert-cell-below"), this.options.editorContent && await Te(this.jupyterApp, this.useNotebook ? this.options.editorContent : this.options.editorContent + "\n"), (t < 5 || t % e == 0) && await M();
+                    for (let t = 0; t < this.options.cells; t++) this.useNotebook && await this.jupyterApp.commands.execute("notebook:insert-cell-below"), this.options.editorContent && await _e(this.jupyterApp, this.useNotebook ? this.options.editorContent : this.options.editorContent + "\n"), (t < 5 || t % e == 0) && await M();
                     this.editor.scrollTop = 0, await M()
                 }
                 async run() {
                     if (!this.widget || !this.options) throw new Error("Scrol scenario setup failure");
                     if (this.options.cellByCell && this.useNotebook) {
                         for (let e = 0; e < this.options.cells; e++) await this.jupyterApp.commands.execute("notebook:move-cursor-down"), await M();
                         await M()
@@ -2106,23 +2119,23 @@
                 }
                 async setupSuite() {
                     this._widgets = [];
                     for (const e of this._tabs) {
                         let t;
                         t = e.path ? await this.jupyterApp.commands.execute("docmanager:open", {
                             path: e.path
-                        }) : await this.jupyterApp.commands.execute("launcher:create"), await P.waitForSelector("#" + t.id, {
+                        }) : await this.jupyterApp.commands.execute("launcher:create"), await A.waitForSelector("#" + t.id, {
                             state: "attached"
                         }), ("first" === this.split && 0 === this._widgets.length || "all" === this.split) && this.jupyterApp.shell.add(t, "main", {
                             mode: "split-right"
                         }), await Fe(this.jupyterApp, t), this._widgets.push(t)
                     }
                 }
                 async cleanupSuite() {
-                    for (const e of this._widgets) e.close(), await P.waitForSelector(`.lm-Widget[data-id="${e.id}"]`, {
+                    for (const e of this._widgets) e.close(), await A.waitForSelector(`.lm-Widget[data-id="${e.id}"]`, {
                         state: "detached"
                     })
                 }
                 async run() {
                     if (!this._widgets.length) throw new Error("Suite not set up");
                     for (const e of this._widgets) await Fe(this.jupyterApp, e)
                 }
@@ -2133,15 +2146,15 @@
                 }
             }
             const $e = {
                 id: "@jupyterlab/ui-profiler:default-scenarios",
                 autoStart: !0,
                 requires: [we],
                 activate: (e, t) => {
-                    [new Ie(e), new Oe(e), new Le(e), new We(e), new _e(e), new Re(e), new qe(e), new Pe(e)].map((e => t.addScenario(e)))
+                    [new Ie(e), new Oe(e), new Le(e), new We(e), new Te(e), new Be(e), new qe(e), new Ae(e)].map((e => t.addScenario(e)))
                 }
             };
             var ze;
             ! function(e) {
                 e.openProfiler = "ui-profiler:open"
             }(ze || (ze = {}));
             const He = [{
@@ -2163,33 +2176,33 @@
                         }),
                         u = {
                             translator: l.nullTranslator,
                             profiler: t,
                             upload: e => a.upload(e),
                             resultLocation: "/ui-profiler-results/"
                         };
-                    let p = null;
-                    const d = new i.WidgetTracker({
+                    let d = null;
+                    const p = new i.WidgetTracker({
                         namespace: "ui-profiler"
                     });
                     e.commands.addCommand(ze.openProfiler, {
                         execute: async () => {
                             let t;
-                            t = !p || p.isDisposed ? (() => {
+                            t = !d || d.isDisposed ? (() => {
                                 const e = new Z(u),
                                     t = new i.MainAreaWidget({
                                         content: e
                                     });
                                 return t.id = "ui-profiler-centre", t.title.label = "UI Profiler", t.title.closable = !0, t.title.icon = c.offlineBoltIcon, t
-                            })() : p, p = t, t.isAttached || e.shell.add(t, "main"), e.shell.activateById(t.id), d.add(t)
+                            })() : d, d = t, t.isAttached || e.shell.add(t, "main"), e.shell.activateById(t.id), p.add(t)
                         },
                         label: "UI Profiler",
                         icon: c.offlineBoltIcon,
                         caption: "Open JupyterLab UI Profiler"
-                    }), r && r.restore(d, {
+                    }), r && r.restore(p, {
                         command: ze.openProfiler,
                         name: e => e.title.label
                     }), s && s.add({
                         command: ze.openProfiler,
                         category: "Other",
                         rank: 1
                     })
```

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/remoteEntry.b7edad4eeff456a5f798.js` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/remoteEntry.edbfe3921863735c974c.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, v = {
+    var e, r, t, a, n, o, i, l, u, f, s, d, p, c, h, v = {
             4299: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(511), t.e(148)]).then((() => () => t(8148))),
-                        "./extension": () => Promise.all([t.e(511), t.e(148)]).then((() => () => t(8148))),
+                        "./index": () => Promise.all([t.e(511), t.e(894)]).then((() => () => t(4894))),
+                        "./extension": () => Promise.all([t.e(511), t.e(894)]).then((() => () => t(4894))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -44,51 +44,51 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        148: "386a0716eefd6e346348",
         511: "91d18779f0d0a64a6570",
-        747: "cddb110f7b8c43b31d07"
+        747: "cddb110f7b8c43b31d07",
+        894: "c1224529783339629936"
     } [e] + ".js?v=" + {
-        148: "386a0716eefd6e346348",
         511: "91d18779f0d0a64a6570",
-        747: "cddb110f7b8c43b31d07"
+        747: "cddb110f7b8c43b31d07",
+        894: "c1224529783339629936"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/ui-profiler:", m.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var d = u[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var s = (r, a) => {
+            var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -105,19 +105,19 @@
                 var o = m.S[t],
                     i = "@jupyterlab/ui-profiler",
                     l = [];
                 return "default" === t && ((e, r, t, a) => {
                     var n = o[e] = o[e] || {},
                         l = n[r];
                     (!l || !l.loaded && (1 != !l.eager ? a : i > l.from)) && (n[r] = {
-                        get: () => Promise.all([m.e(511), m.e(148)]).then((() => () => m(8148))),
+                        get: () => Promise.all([m.e(511), m.e(894)]).then((() => () => m(4894))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab/ui-profiler", "0.2.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@jupyterlab/ui-profiler", "0.2.2"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -166,33 +166,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
-                if ("u" == d) {
-                    if (!u || "u" != s) return !1
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
+                if ("u" == s) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (s == d)
+                    if (d == s)
                         if (l <= a) {
                             if (f != e[l]) return !1
                         } else {
                             if (n ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || d < s != n) return !1;
+                    if (l <= a || s < d != n) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -203,36 +203,36 @@
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = l(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, a)), d(e[t][n])
-    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, a, n) {
+        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, a)), s(e[t][n])
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, a, n) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, a, n)) : e(r, m.S[r], t, a)
     })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), p = {}, c = {
-        1467: () => s("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
-        1526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        1840: () => s("default", "@lumino/signaling", [1, 1, 10, 0]),
-        2502: () => s("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        2583: () => s("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
-        3033: () => s("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        3169: () => s("default", "@jupyterlab/translation", [1, 3, 6, 3]),
-        5414: () => s("default", "@lumino/datagrid", [2, 0, 36, 4]),
-        5687: () => s("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        6271: () => s("default", "react", [1, 17, 0, 1]),
-        7280: () => s("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
-        7986: () => s("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
-        8142: () => s("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        8820: () => s("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        8832: () => s("default", "@lumino/widgets", [1, 1, 37, 2])
+        1467: () => d("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
+        1526: () => d("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        1840: () => d("default", "@lumino/signaling", [1, 1, 10, 0]),
+        2502: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        2583: () => d("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
+        3033: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        3169: () => d("default", "@jupyterlab/translation", [1, 3, 6, 3]),
+        5414: () => d("default", "@lumino/datagrid", [2, 0, 36, 4]),
+        5687: () => d("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        6271: () => d("default", "react", [1, 17, 0, 1]),
+        7280: () => d("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        7986: () => d("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
+        8142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        8820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        8832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
     }, h = {
-        148: [1467, 1526, 1840, 2502, 2583, 3033, 3169, 5414, 5687, 6271, 7280, 7986, 8142, 8820, 8832]
+        894: [1467, 1526, 1840, 2502, 2583, 3033, 3169, 5414, 5687, 6271, 7280, 7986, 8142, 8820, 8832]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
             if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json` & `jupyterlab_ui_profiler-0.2.2/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/benchmark.ts` & `jupyterlab_ui_profiler-0.2.2/src/benchmark.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/browserProfiler.d.ts` & `jupyterlab_ui_profiler-0.2.2/src/browserProfiler.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/css.ts` & `jupyterlab_ui_profiler-0.2.2/src/css.ts`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   }
   const response = await fetch(url);
   return response.json();
 }
 
 export async function collectRules(
   styles: HTMLStyleElement[],
-  options: { skipPattern?: RegExp }
+  options: { skipPattern?: RegExp; includePattern?: RegExp }
 ): Promise<IRuleData[]> {
   let j = 0;
   const allRules: IRuleData[] = [];
   for (const style of styles) {
     const sheet = style.sheet;
     if (!sheet) {
       continue;
@@ -84,14 +84,20 @@
       }
       if (
         options.skipPattern &&
         rule.selectorText.match(options.skipPattern) != null
       ) {
         continue;
       }
+      if (
+        options.includePattern &&
+        rule.selectorText.match(options.includePattern) == null
+      ) {
+        continue;
+      }
       allRules.push({
         rule: rule,
         selector: rule.selectorText,
         sheet: sheet,
         source: sourceName,
         ruleIndex: i,
         stylesheetIndex: j
```

### Comparing `jupyterlab_ui_profiler-0.2.1/src/dramaturg.ts` & `jupyterlab_ui_profiler-0.2.2/src/dramaturg.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/index.ts` & `jupyterlab_ui_profiler-0.2.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/jsBenchmarks.ts` & `jupyterlab_ui_profiler-0.2.2/src/jsBenchmarks.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/lumino.tsx` & `jupyterlab_ui_profiler-0.2.2/src/lumino.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/profiler.ts` & `jupyterlab_ui_profiler-0.2.2/src/profiler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/scenarios.ts` & `jupyterlab_ui_profiler-0.2.2/src/scenarios.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/statistics.ts` & `jupyterlab_ui_profiler-0.2.2/src/statistics.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/styleBenchmarks.tsx` & `jupyterlab_ui_profiler-0.2.2/src/styleBenchmarks.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,31 @@
   IRuleDescription,
   extractSourceMap,
   collectRules
 } from './css';
 import { renderBlockResult } from './ui';
 import { IBenchmark, IScenario } from './tokens';
 
-import benchmarkOptionsSchema from './schema/benchmark-base.json';
 import benchmarkRuleOptionsSchema from './schema/benchmark-rule.json';
 import benchmarkRuleGroupOptionsSchema from './schema/benchmark-rule-group.json';
 import benchmarkRuleUsageOptionsSchema from './schema/benchmark-rule-usage.json';
+import benchmarkSheetOptionsSchema from './schema/benchmark-sheet.json';
 
-import type { BenchmarkOptions } from './types';
 import type { StyleRuleBenchmarkOptions } from './types';
 import type { StyleRuleGroupBenchmarkOptions } from './types';
 import type { StyleRuleUsageOptions } from './types';
+import type { StyleSheetBenchmarkOptions } from './types';
 
-interface IStylesheetResult extends ITimeMeasurement {
+export interface IStylesheetResult extends ITimeMeasurement {
   content: string | null;
   source: string | null;
   stylesheetIndex: number;
 }
 
-interface IRuleResult extends ITimeMeasurement, IRuleDescription {
+export interface IRuleResult extends ITimeMeasurement, IRuleDescription {
   // no-op
 }
 
 export interface IRuleBlockResult extends ITimeMeasurement {
   /**
    * What rules landed in this block?
    */
@@ -92,14 +92,17 @@
       };
       stopSignal?.connect(stopListener);
       const n = options.repeats || 3;
       const start = Date.now();
       const skipPattern = options.skipPattern
         ? new RegExp(options.skipPattern, 'g')
         : undefined;
+      const includePattern = options.includePattern
+        ? new RegExp(options.includePattern, 'g')
+        : undefined;
       const excludePattern = options.excludeMatchPattern
         ? new RegExp(options.excludeMatchPattern, 'g')
         : undefined;
 
       if (scenario.setupSuite) {
         await scenario.setupSuite();
       }
@@ -147,15 +150,18 @@
         .map(element => element.id);
       console.log('Relevant class names:', relevantClassNames);
       console.log('Relevant IDs:', relevantIds);
 
       // Find relevant style rules.
       const results: IRuleResult[] = [];
       const styles = [...document.querySelectorAll('style')];
-      const allRules = await collectRules(styles, { skipPattern });
+      const allRules = await collectRules(styles, {
+        skipPattern,
+        includePattern
+      });
       const relevantRules = new Set<IRuleData>();
       for (const rule of allRules) {
         for (const className of relevantClassNames) {
           if (rule.selector.includes('.' + className)) {
             relevantRules.add(rule);
             break;
           }
@@ -277,18 +283,18 @@
   };
 
 export const styleSheetsBenchmark: IBenchmark<
   ITimingOutcome<IStylesheetResult>
 > = {
   id: 'style-sheet',
   name: 'Style Sheets',
-  configSchema: benchmarkOptionsSchema as JSONSchema7,
+  configSchema: benchmarkSheetOptionsSchema as JSONSchema7,
   run: async (
     scenario: IScenario,
-    options: BenchmarkOptions = {},
+    options: StyleSheetBenchmarkOptions = {},
     progress,
     stopSignal
   ): Promise<ITimingOutcome<IStylesheetResult>> => {
     const n = options.repeats || 3;
     const start = Date.now();
     let stop = false;
     const stopListener = () => {
@@ -300,55 +306,71 @@
     }
     const styles = [...document.querySelectorAll('style')];
     const reference = await benchmark(scenario, n * 2, true);
     console.log('Reference for', scenario.name, 'is:', reference);
     const results: IStylesheetResult[] = [];
     let j = 0;
     let sheetIndex = 0;
+    const includePattern = options.includePattern
+      ? new RegExp(options.includePattern, 'g')
+      : undefined;
     const stylesWithSheets = styles.filter(style => style.sheet);
     if (stylesWithSheets.length !== styles.length) {
       console.log(
         'Skipped',
         styles.length - stylesWithSheets.length,
         'style tags without stylesheets (out of',
         styles.length,
         'total)'
       );
     }
+    const total = stylesWithSheets.length;
+
     for (const style of styles) {
       if (stop) {
         break;
       }
 
       const sheet = style.sheet;
       // Always increment the sheet index.
       sheetIndex++;
+
       if (!sheet) {
         continue;
       }
 
       // Only increment the loop control variable if style included in denominator.
-      progress?.emit({ percentage: (100 * j) / stylesWithSheets.length });
+      progress?.emit({ percentage: (100 * j) / total });
       j++;
 
+      // Extract CSS map
+      const cssMap = await extractSourceMap(style.textContent);
+      const source = cssMap != null ? cssMap.sources[0] : null;
+
+      if (includePattern) {
+        if (source === null) {
+          continue;
+        }
+        if (source.match(includePattern) == null) {
+          continue;
+        }
+      }
+
       // Benchmark the style.
       sheet.disabled = true;
       await layoutReady();
       const measurements = await benchmark(scenario, n, true);
       await layoutReady();
       sheet.disabled = false;
 
-      // Extract CSS map
-      const cssMap = await extractSourceMap(style.textContent);
-
       // Store result.
       results.push({
         ...measurements,
         content: style.textContent,
-        source: cssMap != null ? cssMap.sources[0] : null,
+        source: source,
         stylesheetIndex: sheetIndex
       });
     }
     if (scenario.cleanupSuite) {
       await scenario.cleanupSuite();
     }
     stopSignal?.disconnect(stopListener);
@@ -378,23 +400,26 @@
       stop = true;
     };
     stopSignal?.connect(stopListener);
     const n = options.repeats || 3;
     const skipPattern = options.skipPattern
       ? new RegExp(options.skipPattern, 'g')
       : undefined;
+    const includePattern = options.includePattern
+      ? new RegExp(options.includePattern, 'g')
+      : undefined;
     const start = Date.now();
     if (scenario.setupSuite) {
       await scenario.setupSuite();
     }
     const styles = [...document.querySelectorAll('style')];
     const reference = await benchmark(scenario, n * 2, true);
     console.log('Reference for', scenario.name, 'is:', reference);
     const results: IRuleResult[] = [];
-    const rules = await collectRules(styles, { skipPattern });
+    const rules = await collectRules(styles, { skipPattern, includePattern });
     for (let i = 0; i < rules.length; i++) {
       if (stop) {
         break;
       }
       progress?.emit({ percentage: (100 * i) / rules.length });
       const rule = rules[i];
       // benchmark without the rule
@@ -460,14 +485,17 @@
       stop = true;
     };
     stopSignal?.connect(stopListener);
     const n = options.repeats || 3;
     const skipPattern = options.skipPattern
       ? new RegExp(options.skipPattern, 'g')
       : undefined;
+    const includePattern = options.includePattern
+      ? new RegExp(options.includePattern, 'g')
+      : undefined;
     const maxBlocks = options.maxBlocks || 5;
     const minBlocks = options.minBlocks || 2;
     const start = Date.now();
     if (scenario.setupSuite) {
       await scenario.setupSuite();
     }
     let styles = [...document.querySelectorAll('style')];
@@ -484,15 +512,18 @@
     ) {
       if (stop) {
         break;
       }
       if (randomization !== 0) {
         styles = shuffled(styles);
       }
-      const allRules = await collectRules(styles, { skipPattern });
+      const allRules = await collectRules(styles, {
+        skipPattern,
+        includePattern
+      });
       console.log(
         `Collected ${allRules.length} rules, randomization: ${randomization}`
       );
 
       for (let blocks = minBlocks; blocks <= maxBlocks; blocks++) {
         if (stop) {
           break;
```

### Comparing `jupyterlab_ui_profiler-0.2.1/src/table.ts` & `jupyterlab_ui_profiler-0.2.2/src/table.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/templates.tsx` & `jupyterlab_ui_profiler-0.2.2/src/templates.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/tokens.ts` & `jupyterlab_ui_profiler-0.2.2/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/ui.tsx` & `jupyterlab_ui_profiler-0.2.2/src/ui.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/utils.ts` & `jupyterlab_ui_profiler-0.2.2/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/__tests__/statistics.spec.ts` & `jupyterlab_ui_profiler-0.2.2/src/__tests__/statistics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-profile.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-profile.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-group.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-rule-group.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'properties'": "{'includePattern': OrderedDict([('title', 'Regular expression to filter rules to "*

 * *                 "include'), ('type', 'string'), ('default', '')])}"}*

```diff
@@ -1,9 +1,14 @@
 {
     "properties": {
+        "includePattern": {
+            "default": "",
+            "title": "Regular expression to filter rules to include",
+            "type": "string"
+        },
         "maxBlocks": {
             "default": 5,
             "minimum": 1,
             "title": "Maximal block size",
             "type": "integer"
         },
         "minBlocks": {
```

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-usage.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/benchmark-rule-usage.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'properties'": "{'includePattern': OrderedDict([('title', 'Regular expression to filter rules to "*

 * *                 "include'), ('type', 'string'), ('default', '')])}"}*

```diff
@@ -1,14 +1,19 @@
 {
     "properties": {
         "excludeMatchPattern": {
             "default": "(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)",
             "title": "Regular expression to filter out classes used for rule discovery",
             "type": "string"
         },
+        "includePattern": {
+            "default": "",
+            "title": "Regular expression to filter rules to include",
+            "type": "string"
+        },
         "repeats": {
             "default": 5,
             "minimum": 1,
             "title": "Number of repeats",
             "type": "integer"
         },
         "skipPattern": {
```

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-completer.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/scenario-completer.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-debugger.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/scenario-debugger.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-scroll.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/scenario-scroll.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-tabs.json` & `jupyterlab_ui_profiler-0.2.2/src/schema/scenario-tabs.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-profile.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-profile.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-group.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-rule-group.ts`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,18 @@
  */
 
 export type NumberOfRepeats = number;
 export type RegularExpressionToFilterOutRules = string;
 export type BlockSizeToStartWith = number;
 export type MaximalBlockSize = number;
 export type NumberOfSheetRandomizations = number;
+export type RegularExpressionToFilterRulesToInclude = string;
 
 export interface StyleRuleGroupBenchmarkOptions {
   repeats?: NumberOfRepeats;
   skipPattern?: RegularExpressionToFilterOutRules;
   minBlocks?: BlockSizeToStartWith;
   maxBlocks?: MaximalBlockSize;
   sheetRandomizations?: NumberOfSheetRandomizations;
+  includePattern?: RegularExpressionToFilterRulesToInclude;
   [k: string]: any;
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-usage.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_benchmark-rule.ts`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  * This file was automatically generated by json-schema-to-typescript.
  * DO NOT MODIFY IT BY HAND. Instead, modify the source JSONSchema file,
  * and run json-schema-to-typescript to regenerate this file.
  */
 
 export type NumberOfRepeats = number;
 export type RegularExpressionToFilterOutRules = string;
-export type RegularExpressionToFilterOutClassesUsedForRuleDiscovery = string;
+export type RegularExpressionToFilterRulesToInclude = string;
 
-export interface StyleRuleUsageOptions {
+export interface StyleRuleBenchmarkOptions {
   repeats?: NumberOfRepeats;
   skipPattern?: RegularExpressionToFilterOutRules;
-  excludeMatchPattern?: RegularExpressionToFilterOutClassesUsedForRuleDiscovery;
+  includePattern?: RegularExpressionToFilterRulesToInclude;
   [k: string]: any;
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-completer.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_scenario-completer.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-debugger.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_scenario-debugger.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-scroll.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_scenario-scroll.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-tabs.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/_scenario-tabs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/src/types/index.ts` & `jupyterlab_ui_profiler-0.2.2/src/types/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 export type { BenchmarkOptions } from './_benchmark-base';
 export type { StyleRuleBenchmarkOptions } from './_benchmark-rule';
 export type { StyleRuleGroupBenchmarkOptions } from './_benchmark-rule-group';
 export type { StyleRuleUsageOptions } from './_benchmark-rule-usage';
+export type { StyleSheetBenchmarkOptions } from './_benchmark-sheet';
 export type { ProfileBenchmarkOptions } from './_benchmark-profile';
 export type { ExecutionTimeBenchmarkOptions } from './_benchmark-execution';
 
 export type { TabScenarioOptions } from './_scenario-tabs';
 export type { MenuOpenScenarioOptions } from './_scenario-menu-open';
 export type { CompleterScenarioOptions } from './_scenario-completer';
 export type { SidebarsScenarioOptions } from './_scenario-sidebars';
```

### Comparing `jupyterlab_ui_profiler-0.2.1/style/base.css` & `jupyterlab_ui_profiler-0.2.2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/README.md` & `jupyterlab_ui_profiler-0.2.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/jupyter_server_test_config.py` & `jupyterlab_ui_profiler-0.2.2/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/yarn.lock` & `jupyterlab_ui_profiler-0.2.2/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/profiler.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png` & `jupyterlab_ui_profiler-0.2.2/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/.gitignore` & `jupyterlab_ui_profiler-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/LICENSE` & `jupyterlab_ui_profiler-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/README.md` & `jupyterlab_ui_profiler-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/pyproject.toml` & `jupyterlab_ui_profiler-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.1/PKG-INFO` & `jupyterlab_ui_profiler-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-ui-profiler
-Version: 0.2.1
+Version: 0.2.2
 Summary: JupyterLab extension for profiling UI performance
 Project-URL: Homepage, https://github.com/jupyterlab/ui-profiler
 Project-URL: Bug Tracker, https://github.com/jupyterlab/ui-profiler/issues
 Project-URL: Repository, https://github.com/jupyterlab/ui-profiler.git
 Author: Project Jupyter Contributors
 License: BSD 3-Clause License
```

