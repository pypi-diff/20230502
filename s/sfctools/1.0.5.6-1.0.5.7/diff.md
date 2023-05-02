# Comparing `tmp/sfctools-1.0.5.6.tar.gz` & `tmp/sfctools-1.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.5.6.tar", max compression
+gzip compressed data, was "sfctools-1.0.5.7.tar", max compression
```

## Comparing `sfctools-1.0.5.6.tar` & `sfctools-1.0.5.7.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1157 2022-07-11 05:48:16.488771 sfctools-1.0.5.6/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-02 09:49:33.869373 sfctools-1.0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-20 13:09:06.583059 sfctools-1.0.5.6/README.md
--rw-r--r--   0        0        0     1938 2022-09-30 18:37:37.788985 sfctools-1.0.5.6/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-03-20 13:09:02.730363 sfctools-1.0.5.6/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-07-11 05:48:24.669104 sfctools-1.0.5.6/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-20 13:09:06.605805 sfctools-1.0.5.6/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-20 13:09:06.606808 sfctools-1.0.5.6/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-09-30 16:39:54.806932 sfctools-1.0.5.6/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-07-11 05:48:24.973114 sfctools-1.0.5.6/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-03-20 13:09:02.731669 sfctools-1.0.5.6/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-20 13:09:06.607816 sfctools-1.0.5.6/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-07-11 05:48:25.096539 sfctools-1.0.5.6/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-07-11 05:48:25.136548 sfctools-1.0.5.6/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-09-30 17:46:40.211773 sfctools-1.0.5.6/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-09-30 18:03:18.887479 sfctools-1.0.5.6/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-10-06 06:50:49.792046 sfctools-1.0.5.6/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-20 13:09:06.608843 sfctools-1.0.5.6/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15032 2023-03-20 13:09:06.609847 sfctools-1.0.5.6/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-20 13:09:06.609847 sfctools-1.0.5.6/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-10-06 06:49:21.703590 sfctools-1.0.5.6/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-03-20 13:09:02.733973 sfctools-1.0.5.6/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-07-11 05:48:26.022730 sfctools-1.0.5.6/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-20 13:09:06.610850 sfctools-1.0.5.6/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-03-20 13:09:02.735065 sfctools-1.0.5.6/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-20 13:09:06.611852 sfctools-1.0.5.6/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-07-11 05:48:26.175050 sfctools-1.0.5.6/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-12-30 14:49:34.085439 sfctools-1.0.5.6/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-07-11 05:48:26.251065 sfctools-1.0.5.6/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-07-11 05:48:26.289074 sfctools-1.0.5.6/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-07-11 05:48:26.401099 sfctools-1.0.5.6/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-10-05 17:45:14.259714 sfctools-1.0.5.6/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-20 13:09:06.612897 sfctools-1.0.5.6/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-20 13:09:06.614389 sfctools-1.0.5.6/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-20 13:09:06.615392 sfctools-1.0.5.6/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-20 13:09:06.615392 sfctools-1.0.5.6/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-20 13:09:06.616409 sfctools-1.0.5.6/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-20 13:09:06.616409 sfctools-1.0.5.6/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-20 13:09:06.616409 sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-20 13:09:06.617415 sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-20 13:09:06.617415 sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-20 13:09:06.618422 sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-20 13:09:06.618422 sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-20 13:09:06.618422 sfctools-1.0.5.6/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-20 13:09:06.619427 sfctools-1.0.5.6/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-20 13:09:06.619427 sfctools-1.0.5.6/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-20 13:09:06.621437 sfctools-1.0.5.6/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-20 13:09:06.622441 sfctools-1.0.5.6/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-20 13:09:06.623445 sfctools-1.0.5.6/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-20 13:09:06.623445 sfctools-1.0.5.6/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-20 13:09:06.624450 sfctools-1.0.5.6/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-20 13:09:06.624450 sfctools-1.0.5.6/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-20 13:09:06.625458 sfctools-1.0.5.6/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-20 13:09:06.625458 sfctools-1.0.5.6/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-20 13:09:06.626464 sfctools-1.0.5.6/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-20 13:09:06.626464 sfctools-1.0.5.6/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-20 13:09:06.627470 sfctools-1.0.5.6/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-20 13:09:06.628492 sfctools-1.0.5.6/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-02 14:41:04.722520 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      415 2023-05-02 14:41:04.789151 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      417 2023-05-02 14:41:04.848249 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      413 2023-05-02 14:41:04.910757 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      413 2023-05-02 14:41:04.969838 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      410 2023-05-02 14:41:05.033208 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      415 2023-05-02 14:41:05.092742 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      413 2023-05-02 14:41:05.152384 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      416 2023-05-02 14:41:05.213119 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      413 2023-05-02 14:41:05.272879 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      412 2023-05-02 14:41:05.333495 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-05-02 14:41:05.333495 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-02 14:41:05.333495 sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-20 13:09:06.634587 sfctools-1.0.5.6/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-20 13:09:06.635591 sfctools-1.0.5.6/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-20 13:09:06.635591 sfctools-1.0.5.6/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-20 13:09:06.636593 sfctools-1.0.5.6/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34561 2023-03-20 13:09:06.637593 sfctools-1.0.5.6/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-04-27 13:29:45.411196 sfctools-1.0.5.6/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    72954 2023-05-02 14:26:08.393007 sfctools-1.0.5.6/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-03-20 13:09:02.740428 sfctools-1.0.5.6/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-02 06:24:19.629663 sfctools-1.0.5.6/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-03-20 13:09:02.741615 sfctools-1.0.5.6/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-20 13:09:06.640594 sfctools-1.0.5.6/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-20 13:09:06.641594 sfctools-1.0.5.6/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-08-09 15:11:37.968071 sfctools-1.0.5.6/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-27 08:43:06.249807 sfctools-1.0.5.6/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-02 14:36:23.559376 sfctools-1.0.5.6/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-08-09 15:11:37.968071 sfctools-1.0.5.6/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-08-09 15:11:37.968071 sfctools-1.0.5.6/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-04-27 13:07:33.967008 sfctools-1.0.5.6/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-20 13:09:06.643594 sfctools-1.0.5.6/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-20 13:09:06.644595 sfctools-1.0.5.6/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-03-20 13:09:02.744421 sfctools-1.0.5.6/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-20 13:09:06.645595 sfctools-1.0.5.6/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-03-20 13:09:02.745871 sfctools-1.0.5.6/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-03-20 13:09:02.746872 sfctools-1.0.5.6/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-20 13:09:06.646595 sfctools-1.0.5.6/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-03-20 13:09:02.748074 sfctools-1.0.5.6/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-04-27 16:25:31.372347 sfctools-1.0.5.6/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-02 14:41:53.609577 sfctools-1.0.5.6/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-02 06:27:52.607491 sfctools-1.0.5.6/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-20 13:09:06.647595 sfctools-1.0.5.6/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-20 13:09:06.648596 sfctools-1.0.5.6/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-08-09 15:11:37.952444 sfctools-1.0.5.6/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-03-20 13:09:02.736482 sfctools-1.0.5.6/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2023-03-20 12:39:06.880624 sfctools-1.0.5.6/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-04-27 11:35:47.715548 sfctools-1.0.5.6/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-07-11 05:48:26.867204 sfctools-1.0.5.6/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    18645 2023-03-20 13:09:06.649596 sfctools-1.0.5.6/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-20 13:09:06.650596 sfctools-1.0.5.6/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-07-11 05:48:26.971227 sfctools-1.0.5.6/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.5.6/setup.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 sfctools-1.0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-07-11 05:48:16.488771 sfctools-1.0.5.7/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-02 14:48:01.301162 sfctools-1.0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-20 13:09:06.583059 sfctools-1.0.5.7/README.md
+-rw-r--r--   0        0        0     1938 2022-09-30 18:37:37.788985 sfctools-1.0.5.7/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-03-20 13:09:02.730363 sfctools-1.0.5.7/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-07-11 05:48:24.669104 sfctools-1.0.5.7/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-03-20 13:09:06.605805 sfctools-1.0.5.7/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-20 13:09:06.606808 sfctools-1.0.5.7/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-09-30 16:39:54.806932 sfctools-1.0.5.7/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-07-11 05:48:24.973114 sfctools-1.0.5.7/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-03-20 13:09:02.731669 sfctools-1.0.5.7/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-20 13:09:06.607816 sfctools-1.0.5.7/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-07-11 05:48:25.096539 sfctools-1.0.5.7/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-07-11 05:48:25.136548 sfctools-1.0.5.7/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-09-30 17:46:40.211773 sfctools-1.0.5.7/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2022-09-30 18:03:18.887479 sfctools-1.0.5.7/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-10-06 06:50:49.792046 sfctools-1.0.5.7/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-20 13:09:06.608843 sfctools-1.0.5.7/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15032 2023-03-20 13:09:06.609847 sfctools-1.0.5.7/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-20 13:09:06.609847 sfctools-1.0.5.7/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-10-06 06:49:21.703590 sfctools-1.0.5.7/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-03-20 13:09:02.733973 sfctools-1.0.5.7/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-07-11 05:48:26.022730 sfctools-1.0.5.7/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-03-20 13:09:06.610850 sfctools-1.0.5.7/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-03-20 13:09:02.735065 sfctools-1.0.5.7/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-20 13:09:06.611852 sfctools-1.0.5.7/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-07-11 05:48:26.175050 sfctools-1.0.5.7/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-12-30 14:49:34.085439 sfctools-1.0.5.7/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-07-11 05:48:26.251065 sfctools-1.0.5.7/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-07-11 05:48:26.289074 sfctools-1.0.5.7/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-07-11 05:48:26.401099 sfctools-1.0.5.7/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-10-05 17:45:14.259714 sfctools-1.0.5.7/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-20 13:09:06.612897 sfctools-1.0.5.7/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-20 13:09:06.614389 sfctools-1.0.5.7/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-20 13:09:06.615392 sfctools-1.0.5.7/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-20 13:09:06.615392 sfctools-1.0.5.7/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-20 13:09:06.616409 sfctools-1.0.5.7/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-20 13:09:06.616409 sfctools-1.0.5.7/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-20 13:09:06.616409 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-20 13:09:06.617415 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-20 13:09:06.617415 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-20 13:09:06.618422 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-20 13:09:06.618422 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-20 13:09:06.618422 sfctools-1.0.5.7/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-20 13:09:06.619427 sfctools-1.0.5.7/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-20 13:09:06.619427 sfctools-1.0.5.7/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-20 13:09:06.621437 sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-20 13:09:06.622441 sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-20 13:09:06.623445 sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-20 13:09:06.623445 sfctools-1.0.5.7/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-20 13:09:06.624450 sfctools-1.0.5.7/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-20 13:09:06.624450 sfctools-1.0.5.7/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-20 13:09:06.625458 sfctools-1.0.5.7/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-20 13:09:06.625458 sfctools-1.0.5.7/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-20 13:09:06.626464 sfctools-1.0.5.7/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-20 13:09:06.626464 sfctools-1.0.5.7/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-20 13:09:06.627470 sfctools-1.0.5.7/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-20 13:09:06.628492 sfctools-1.0.5.7/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-02 14:41:04.722520 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      415 2023-05-02 14:41:04.789151 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      417 2023-05-02 14:41:04.848249 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      413 2023-05-02 14:41:04.910757 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      413 2023-05-02 14:41:04.969838 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      410 2023-05-02 14:41:05.033208 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      415 2023-05-02 14:41:05.092742 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      413 2023-05-02 14:41:05.152384 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      416 2023-05-02 14:41:05.213119 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      413 2023-05-02 14:41:05.272879 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      412 2023-05-02 14:41:05.333495 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-05-02 14:41:05.333495 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-02 14:41:05.333495 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-20 13:09:06.634587 sfctools-1.0.5.7/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-20 13:09:06.635591 sfctools-1.0.5.7/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-20 13:09:06.635591 sfctools-1.0.5.7/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-20 13:09:06.636593 sfctools-1.0.5.7/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34561 2023-03-20 13:09:06.637593 sfctools-1.0.5.7/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-04-27 13:29:45.411196 sfctools-1.0.5.7/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    72949 2023-05-02 14:50:59.910575 sfctools-1.0.5.7/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-03-20 13:09:02.740428 sfctools-1.0.5.7/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-02 06:24:19.629663 sfctools-1.0.5.7/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-03-20 13:09:02.741615 sfctools-1.0.5.7/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-20 13:09:06.640594 sfctools-1.0.5.7/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-20 13:09:06.641594 sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-08-09 15:11:37.968071 sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-27 08:43:06.249807 sfctools-1.0.5.7/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136567 2023-05-02 14:36:23.559376 sfctools-1.0.5.7/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-08-09 15:11:37.968071 sfctools-1.0.5.7/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-08-09 15:11:37.968071 sfctools-1.0.5.7/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-04-27 13:07:33.967008 sfctools-1.0.5.7/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-20 13:09:06.643594 sfctools-1.0.5.7/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-20 13:09:06.644595 sfctools-1.0.5.7/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-03-20 13:09:02.744421 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-20 13:09:06.645595 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-03-20 13:09:02.745871 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-03-20 13:09:02.746872 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-20 13:09:06.646595 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-03-20 13:09:02.748074 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-04-27 16:25:31.372347 sfctools-1.0.5.7/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-02 14:49:34.488744 sfctools-1.0.5.7/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-02 06:27:52.607491 sfctools-1.0.5.7/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-20 13:09:06.647595 sfctools-1.0.5.7/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-20 13:09:06.648596 sfctools-1.0.5.7/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-03-20 13:09:02.736482 sfctools-1.0.5.7/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2023-03-20 12:39:06.880624 sfctools-1.0.5.7/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-04-27 11:35:47.715548 sfctools-1.0.5.7/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2022-07-11 05:48:26.867204 sfctools-1.0.5.7/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    18645 2023-03-20 13:09:06.649596 sfctools-1.0.5.7/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-20 13:09:06.650596 sfctools-1.0.5.7/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-07-11 05:48:26.971227 sfctools-1.0.5.7/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.5.7/setup.py
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 sfctools-1.0.5.7/PKG-INFO
```

### Comparing `sfctools-1.0.5.6/LICENSE` & `sfctools-1.0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/pyproject.toml` & `sfctools-1.0.5.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.5.6"
+version = "1.0.5.7"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.5.6/README.md` & `sfctools-1.0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/__init__.py` & `sfctools-1.0.5.7/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/__main__.py` & `sfctools-1.0.5.7/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/automation/calibration.py` & `sfctools-1.0.5.7/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/automation/cgesolver.py` & `sfctools-1.0.5.7/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/automation/runner.py` & `sfctools-1.0.5.7/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/bottomup/matching.py` & `sfctools-1.0.5.7/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/bottomup/productiontree.py` & `sfctools-1.0.5.7/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.5.7/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/bottomup/treestruct.py` & `sfctools-1.0.5.7/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/core/agent.py` & `sfctools-1.0.5.7/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/core/clock.py` & `sfctools-1.0.5.7/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/core/flow_matrix.py` & `sfctools-1.0.5.7/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/core/settings.py` & `sfctools-1.0.5.7/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/core/singleton.py` & `sfctools-1.0.5.7/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/core/world.py` & `sfctools-1.0.5.7/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/balance.py` & `sfctools-1.0.5.7/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.5.7/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.5.7/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/collection.py` & `sfctools-1.0.5.7/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/income_statement.py` & `sfctools-1.0.5.7/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/inventory.py` & `sfctools-1.0.5.7/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/market_registry.py` & `sfctools-1.0.5.7/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/signalslot.py` & `sfctools-1.0.5.7/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.5.7/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/__init__.py` & `sfctools-1.0.5.7/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/balance.py` & `sfctools-1.0.5.7/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.5.7/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/clock.py` & `sfctools-1.0.5.7/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/example_wrapper.py` & `sfctools-1.0.5.7/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.5.7/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/flowmatrix.py` & `sfctools-1.0.5.7/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/hello_agent.py` & `sfctools-1.0.5.7/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/inventory.py` & `sfctools-1.0.5.7/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/market_example/market.py` & `sfctools-1.0.5.7/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/market_example/market2.py` & `sfctools-1.0.5.7/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.5.7/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/order_book.py` & `sfctools-1.0.5.7/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/examples/signal_slot.py` & `sfctools-1.0.5.7/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.5.7/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/draw_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -981,20 +981,20 @@
                 ip = interpolator(alpha)
 
                 x0 = points[0][0]
                 y0 = points[0][1]
                 xf = points[-1][0]
                 yf = points[-1][1]
 
-                xc1, yc1 = self.manhattan_lines(x0,y0,xi,yi,60)
-                # xc2, yc2 = self.manhattan_lines(xi,yi,xd,yd,100)
-                xc2, yc2 = self.manhattan_lines(xi,yi,xf,yf,100)
+                xc1, yc1 = self.manhattan_lines(x0,y0,xi,yi,30)
+                xc2, yc2 = self.manhattan_lines(xi,yi,xd,yd,30)
+                xc3, yc3 = self.manhattan_lines(xd,yd,xf,yf,100)
 
-                x_coords = xc1 + xc2 #+ xc3
-                y_coords = yc1 + yc2 #+ yc3
+                x_coords = xc1 + xc2 + xc3
+                y_coords = yc1 + yc2 + yc3
                 interpolated_points = list(zip(x_coords,y_coords))
 
             # draw connector line as path
             n = len(interpolated_points)
 
             interpolated_points = [(self.raster(t[0]), self.raster(t[1])) for t in interpolated_points]
```

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.5.7/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.5.7/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/CLA.pdf` & `sfctools-1.0.5.7/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.5.7/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/LICENSE` & `sfctools-1.0.5.7/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/gui/README.md` & `sfctools-1.0.5.7/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.5.7/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.5.7/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/sfctools/misc/timeseries.py` & `sfctools-1.0.5.7/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.6/setup.py` & `sfctools-1.0.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.5.6',
+    'version': '1.0.5.7',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.5.6/PKG-INFO` & `sfctools-1.0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.5.6
+Version: 1.0.5.7
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

