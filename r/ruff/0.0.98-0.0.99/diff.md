# Comparing `tmp/ruff-0.0.98.tar.gz` & `tmp/ruff-0.0.99.tar.gz`

## Comparing `ruff-0.0.98.tar` & `ruff-0.0.99.tar`

### file list

```diff
@@ -1,448 +1,448 @@
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 ruff-0.0.98/Cargo.toml
--rw-r--r--   0      501       20      278 2022-11-03 14:21:02.000000 ruff-0.0.98/.editorconfig
--rw-r--r--   0      501       20     3712 2022-11-03 14:21:02.000000 ruff-0.0.98/.github/workflows/ci.yaml
--rw-r--r--   0      501       20     8911 2022-11-03 14:21:02.000000 ruff-0.0.98/.github/workflows/flake8-to-ruff.yaml
--rw-r--r--   0      501       20     8618 2022-11-03 14:21:02.000000 ruff-0.0.98/.github/workflows/ruff.yaml
--rw-r--r--   0      501       20     3407 2022-11-03 14:21:02.000000 ruff-0.0.98/.gitignore
--rw-r--r--   0      501       20      231 2022-11-03 14:21:02.000000 ruff-0.0.98/.pre-commit-config.yaml
--rw-r--r--   0      501       20     5227 2022-11-03 14:21:02.000000 ruff-0.0.98/CODE_OF_CONDUCT.md
--rw-r--r--   0      501       20     4582 2022-11-03 14:21:02.000000 ruff-0.0.98/CONTRIBUTING.md
--rw-r--r--   0      501       20    82250 2022-11-03 14:21:02.000000 ruff-0.0.98/Cargo.lock
--rw-r--r--   0      501       20     1070 2022-11-03 14:21:02.000000 ruff-0.0.98/LICENSE
--rw-r--r--   0      501       20    35349 2022-11-03 14:21:02.000000 ruff-0.0.98/README.md
--rw-r--r--   0      501       20      475 2022-11-03 14:21:02.000000 ruff-0.0.98/benches/source_code_locator.rs
--rw-r--r--   0      501       20     3261 2022-11-03 14:21:02.000000 ruff-0.0.98/examples/generate_check_code_prefix.rs
--rw-r--r--   0      501       20      942 2022-11-03 14:21:02.000000 ruff-0.0.98/examples/generate_rules_table.rs
--rw-r--r--   0      501       20      568 2022-11-03 14:21:02.000000 ruff-0.0.98/examples/generate_source_code.rs
--rw-r--r--   0      501       20      477 2022-11-03 14:21:02.000000 ruff-0.0.98/examples/print_ast.rs
--rw-r--r--   0      501       20      470 2022-11-03 14:21:02.000000 ruff-0.0.98/examples/print_tokens.rs
--rw-r--r--   0      501       20     1100 2022-11-03 14:21:02.000000 ruff-0.0.98/pyproject.toml
--rw-r--r--   0      501       20      368 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/A001.py
--rw-r--r--   0      501       20      130 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/A002.py
--rw-r--r--   0      501       20      127 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/A003.py
--rw-r--r--   0      501       20      223 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B002.py
--rw-r--r--   0      501       20     3342 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B006_B008.py
--rw-r--r--   0      501       20      716 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B007.py
--rw-r--r--   0      501       20      133 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B011.py
--rw-r--r--   0      501       20      119 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B013.py
--rw-r--r--   0      501       20     1364 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B014.py
--rw-r--r--   0      501       20      829 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B017.py
--rw-r--r--   0      501       20      446 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/B025.py
--rw-r--r--   0      501       20       66 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C400.py
--rw-r--r--   0      501       20       64 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C401.py
--rw-r--r--   0      501       20      106 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C402.py
--rw-r--r--   0      501       20       68 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C403.py
--rw-r--r--   0      501       20       71 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C404.py
--rw-r--r--   0      501       20       71 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C405.py
--rw-r--r--   0      501       20       81 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C406.py
--rw-r--r--   0      501       20       66 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C408.py
--rw-r--r--   0      501       20      107 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C409.py
--rw-r--r--   0      501       20       64 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C410.py
--rw-r--r--   0      501       20       35 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C411.py
--rw-r--r--   0      501       20       84 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C413.py
--rw-r--r--   0      501       20      216 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C414.py
--rw-r--r--   0      501       20      193 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C415.py
--rw-r--r--   0      501       20       95 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C416.py
--rw-r--r--   0      501       20      179 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/C417.py
--rw-r--r--   0      501       20    12157 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/D.py
--rw-r--r--   0      501       20      294 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E402.py
--rw-r--r--   0      501       20      786 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E501.py
--rw-r--r--   0      501       20      648 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E711.py
--rw-r--r--   0      501       20      653 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E712.py
--rw-r--r--   0      501       20      540 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E713.py
--rw-r--r--   0      501       20      508 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E714.py
--rw-r--r--   0      501       20      907 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E721.py
--rw-r--r--   0      501       20      327 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E722.py
--rw-r--r--   0      501       20      252 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E731.py
--rw-r--r--   0      501       20      676 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E741.py
--rw-r--r--   0      501       20       78 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E742.py
--rw-r--r--   0      501       20       99 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E743.py
--rw-r--r--   0      501       20       10 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/E999.py
--rw-r--r--   0      501       20     1549 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F401_0.py
--rw-r--r--   0      501       20      121 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F401_1.py
--rw-r--r--   0      501       20      242 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F401_2.py
--rw-r--r--   0      501       20      302 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F401_3.py
--rw-r--r--   0      501       20      315 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F401_4.py
--rw-r--r--   0      501       20      126 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F401_5.py
--rw-r--r--   0      501       20       96 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F402.py
--rw-r--r--   0      501       20      152 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F403.py
--rw-r--r--   0      501       20      130 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F404.py
--rw-r--r--   0      501       20      116 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F405.py
--rw-r--r--   0      501       20       87 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F406.py
--rw-r--r--   0      501       20       82 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F407.py
--rw-r--r--   0      501       20      112 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F541.py
--rw-r--r--   0      501       20      144 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F601.py
--rw-r--r--   0      501       20       50 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F602.py
--rw-r--r--   0      501       20       64 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F622.py
--rw-r--r--   0      501       20       58 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F631.py
--rw-r--r--   0      501       20       51 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F632.py
--rw-r--r--   0      501       20       79 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F633.py
--rw-r--r--   0      501       20      122 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F634.py
--rw-r--r--   0      501       20      179 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F701.py
--rw-r--r--   0      501       20      200 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F702.py
--rw-r--r--   0      501       20       76 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F704.py
--rw-r--r--   0      501       20       66 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F706.py
--rw-r--r--   0      501       20      380 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F707.py
--rw-r--r--   0      501       20       74 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F722.py
--rw-r--r--   0      501       20     2196 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F821_0.py
--rw-r--r--   0      501       20      395 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F821_1.py
--rw-r--r--   0      501       20      259 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F821_2.py
--rw-r--r--   0      501       20       28 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F822.py
--rw-r--r--   0      501       20      245 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F823.py
--rw-r--r--   0      501       20      159 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F831.py
--rw-r--r--   0      501       20      343 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F841.py
--rw-r--r--   0      501       20       88 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/F901.py
--rw-r--r--   0      501       20     1762 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/M001.py
--rw-r--r--   0      501       20      225 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N801.py
--rw-r--r--   0      501       20      354 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N802.py
--rw-r--r--   0      501       20       95 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N803.py
--rw-r--r--   0      501       20      264 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N804.py
--rw-r--r--   0      501       20      345 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N805.py
--rw-r--r--   0      501       20       64 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N806.py
--rw-r--r--   0      501       20      126 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N807.py
--rw-r--r--   0      501       20      116 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N811.py
--rw-r--r--   0      501       20      124 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N812.py
--rw-r--r--   0      501       20      119 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N813.py
--rw-r--r--   0      501       20      119 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N814.py
--rw-r--r--   0      501       20       96 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N815.py
--rw-r--r--   0      501       20       67 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N816.py
--rw-r--r--   0      501       20       55 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N817.py
--rw-r--r--   0      501       20      106 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/N818.py
--rw-r--r--   0      501       20       31 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/T201.py
--rw-r--r--   0      501       20      148 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/T203.py
--rw-r--r--   0      501       20      152 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U001.py
--rw-r--r--   0      501       20      146 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U002.py
--rw-r--r--   0      501       20       45 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U003.py
--rw-r--r--   0      501       20      883 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U004.py
--rw-r--r--   0      501       20      263 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U005.py
--rw-r--r--   0      501       20      125 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U006.py
--rw-r--r--   0      501       20      463 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U007.py
--rw-r--r--   0      501       20     1483 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/U008.py
--rw-r--r--   0      501       20       26 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/W292_0.py
--rw-r--r--   0      501       20       40 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/W292_1.py
--rw-r--r--   0      501       20       27 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/W292_2.py
--rw-r--r--   0      501       20      316 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/W605.py
--rw-r--r--   0      501       20       54 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/__init__.py
--rw-r--r--   0      501       20        0 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/bar/__init__.py
--rw-r--r--   0      501       20        0 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/bar/migrations/__init__.py
--rw-r--r--   0      501       20       90 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/bar/migrations/migration.py
--rw-r--r--   0      501       20     4176 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/canonical_google_examples.py
--rw-r--r--   0      501       20     5315 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/canonical_numpy_examples.py
--rw-r--r--   0      501       20       90 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/directory/also_excluded.py
--rw-r--r--   0      501       20       90 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/excluded.py
--rw-r--r--   0      501       20      716 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_doubles.py
--rw-r--r--   0      501       20      290 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_doubles_class.py
--rw-r--r--   0      501       20      406 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_doubles_function.py
--rw-r--r--   0      501       20      133 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_doubles_module_multiline.py
--rw-r--r--   0      501       20      135 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_doubles_module_singleline.py
--rw-r--r--   0      501       20      772 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_singles.py
--rw-r--r--   0      501       20      290 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_singles_class.py
--rw-r--r--   0      501       20      408 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_singles_function.py
--rw-r--r--   0      501       20      133 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_singles_module_multiline.py
--rw-r--r--   0      501       20      135 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_singles_module_singleline.py
--rw-r--r--   0      501       20       93 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/doubles.py
--rw-r--r--   0      501       20      203 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/doubles_escaped.py
--rw-r--r--   0      501       20      165 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/doubles_multiline_string.py
--rw-r--r--   0      501       20       58 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/doubles_noqa.py
--rw-r--r--   0      501       20      106 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/doubles_wrapped.py
--rw-r--r--   0      501       20       93 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/singles.py
--rw-r--r--   0      501       20      203 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/singles_escaped.py
--rw-r--r--   0      501       20      165 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/singles_multiline_string.py
--rw-r--r--   0      501       20       58 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/singles_noqa.py
--rw-r--r--   0      501       20      106 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/flake8_quotes/singles_wrapped.py
--rw-r--r--   0      501       20        0 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/foo/__init__.py
--rw-r--r--   0      501       20        0 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/foo/migrations/__init__.py
--rw-r--r--   0      501       20       90 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/foo/migrations/migration.py
--rw-r--r--   0      501       20      444 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/future_annotations.py
--rw-r--r--   0      501       20      632 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/pyproject.toml
--rw-r--r--   0      501       20    12260 2022-11-03 14:21:02.000000 ruff-0.0.98/resources/test/fixtures/sections.py
--rw-r--r--   0      501       20        7 2022-11-03 14:21:02.000000 ruff-0.0.98/rust-toolchain
--rw-r--r--   0      501       20      390 2022-11-03 14:21:02.000000 ruff-0.0.98/rustfmt.toml
--rw-r--r--   0      501       20      302 2022-11-03 14:21:02.000000 ruff-0.0.98/scripts/.flake8
--rw-r--r--   0      501       20    37365 2022-11-03 14:21:02.000000 ruff-0.0.98/scripts/poetry.lock
--rw-r--r--   0      501       20      454 2022-11-03 14:21:02.000000 ruff-0.0.98/scripts/pyproject.toml
--rwxr-xr-x   0      501       20     1035 2022-11-03 14:21:02.000000 ruff-0.0.98/scripts/run_flake8.py
--rw-r--r--   0      501       20      565 2022-11-03 14:21:02.000000 ruff-0.0.98/setup.py
--rw-r--r--   0      501       20     4422 2022-11-03 14:21:02.000000 ruff-0.0.98/src/ast/helpers.rs
--rw-r--r--   0      501       20       87 2022-11-03 14:21:02.000000 ruff-0.0.98/src/ast/mod.rs
--rw-r--r--   0      501       20     3881 2022-11-03 14:21:02.000000 ruff-0.0.98/src/ast/operations.rs
--rw-r--r--   0      501       20     4574 2022-11-03 14:21:02.000000 ruff-0.0.98/src/ast/relocate.rs
--rw-r--r--   0      501       20     2211 2022-11-03 14:21:02.000000 ruff-0.0.98/src/ast/types.rs
--rw-r--r--   0      501       20    18283 2022-11-03 14:21:02.000000 ruff-0.0.98/src/ast/visitor.rs
--rw-r--r--   0      501       20     6495 2022-11-03 14:21:02.000000 ruff-0.0.98/src/autofix/fixer.rs
--rw-r--r--   0      501       20     3383 2022-11-03 14:21:02.000000 ruff-0.0.98/src/autofix/helpers.rs
--rw-r--r--   0      501       20     1217 2022-11-03 14:21:02.000000 ruff-0.0.98/src/autofix/mod.rs
--rw-r--r--   0      501       20     4136 2022-11-03 14:21:02.000000 ruff-0.0.98/src/cache.rs
--rw-r--r--   0      501       20   100050 2022-11-03 14:21:02.000000 ruff-0.0.98/src/check_ast.rs
--rw-r--r--   0      501       20     9787 2022-11-03 14:21:02.000000 ruff-0.0.98/src/check_lines.rs
--rw-r--r--   0      501       20     1740 2022-11-03 14:21:02.000000 ruff-0.0.98/src/check_tokens.rs
--rw-r--r--   0      501       20    69698 2022-11-03 14:21:02.000000 ruff-0.0.98/src/checks.rs
--rw-r--r--   0      501       20    43059 2022-11-03 14:21:02.000000 ruff-0.0.98/src/checks_gen.rs
--rw-r--r--   0      501       20     6185 2022-11-03 14:21:02.000000 ruff-0.0.98/src/cli.rs
--rw-r--r--   0      501       20    36461 2022-11-03 14:21:02.000000 ruff-0.0.98/src/code_gen.rs
--rw-r--r--   0      501       20     1201 2022-11-03 14:21:02.000000 ruff-0.0.98/src/cst/helpers.rs
--rw-r--r--   0      501       20      536 2022-11-03 14:21:02.000000 ruff-0.0.98/src/cst/matchers.rs
--rw-r--r--   0      501       20       35 2022-11-03 14:21:02.000000 ruff-0.0.98/src/cst/mod.rs
--rw-r--r--   0      501       20      404 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/definition.rs
--rw-r--r--   0      501       20     2428 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/extraction.rs
--rw-r--r--   0      501       20     1423 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/google.rs
--rw-r--r--   0      501       20     1363 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/helpers.rs
--rw-r--r--   0      501       20      122 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/mod.rs
--rw-r--r--   0      501       20      908 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/numpy.rs
--rw-r--r--   0      501       20     3140 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/sections.rs
--rw-r--r--   0      501       20      797 2022-11-03 14:21:02.000000 ruff-0.0.98/src/docstrings/styles.rs
--rw-r--r--   0      501       20       17 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/mod.rs
--rw-r--r--   0      501       20     2046 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/assert_false.rs
--rw-r--r--   0      501       20      918 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/assert_raises_exception.rs
--rw-r--r--   0      501       20     4108 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/duplicate_exceptions.rs
--rw-r--r--   0      501       20      654 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/mod.rs
--rw-r--r--   0      501       20     2255 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/mutable_argument_default.rs
--rw-r--r--   0      501       20      822 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs
--rw-r--r--   0      501       20      635 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/unary_prefix_increment.rs
--rw-r--r--   0      501       20     2046 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_bugbear/plugins/unused_loop_control_variable.rs
--rw-r--r--   0      501       20      759 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_builtins/checks.rs
--rw-r--r--   0      501       20       31 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_builtins/mod.rs
--rw-r--r--   0      501       20       70 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_builtins/types.rs
--rw-r--r--   0      501       20    15040 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_comprehensions/checks.rs
--rw-r--r--   0      501       20    14688 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_comprehensions/fixes.rs
--rw-r--r--   0      501       20       27 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_comprehensions/mod.rs
--rw-r--r--   0      501       20      949 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_print/checks.rs
--rw-r--r--   0      501       20       29 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_print/mod.rs
--rw-r--r--   0      501       20       49 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_print/plugins/mod.rs
--rw-r--r--   0      501       20     1657 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_print/plugins/print_call.rs
--rw-r--r--   0      501       20    10466 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/checks.rs
--rw-r--r--   0      501       20     3662 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/docstring_detection.rs
--rw-r--r--   0      501       20       63 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/mod.rs
--rw-r--r--   0      501       20     1382 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/settings.rs
--rw-r--r--   0      501       20      737 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap
--rw-r--r--   0      501       20      331 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_class.py.snap
--rw-r--r--   0      501       20      737 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap
--rw-r--r--   0      501       20      329 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_multiline.py.snap
--rw-r--r--   0      501       20      330 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_singleline.py.snap
--rw-r--r--   0      501       20      447 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles.py.snap
--rw-r--r--   0      501       20      446 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_class.py.snap
--rw-r--r--   0      501       20      318 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_function.py.snap
--rw-r--r--   0      501       20      190 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_multiline.py.snap
--rw-r--r--   0      501       20      191 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_singleline.py.snap
--rw-r--r--   0      501       20      326 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles.py.snap
--rw-r--r--   0      501       20      178 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_escaped.py.snap
--rw-r--r--   0      501       20      197 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_multiline_string.py.snap
--rw-r--r--   0      501       20       67 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_noqa.py.snap
--rw-r--r--   0      501       20       67 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_wrapped.py.snap
--rw-r--r--   0      501       20      447 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles.py.snap
--rw-r--r--   0      501       20      446 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_class.py.snap
--rw-r--r--   0      501       20      318 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_function.py.snap
--rw-r--r--   0      501       20      190 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_multiline.py.snap
--rw-r--r--   0      501       20      191 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_singleline.py.snap
--rw-r--r--   0      501       20      872 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap
--rw-r--r--   0      501       20      331 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_class.py.snap
--rw-r--r--   0      501       20      737 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap
--rw-r--r--   0      501       20      329 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_multiline.py.snap
--rw-r--r--   0      501       20      330 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_singleline.py.snap
--rw-r--r--   0      501       20      326 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles.py.snap
--rw-r--r--   0      501       20      178 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_escaped.py.snap
--rw-r--r--   0      501       20      197 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_multiline_string.py.snap
--rw-r--r--   0      501       20       67 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_noqa.py.snap
--rw-r--r--   0      501       20       67 2022-11-03 14:21:02.000000 ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_wrapped.py.snap
--rw-r--r--   0      501       20     9122 2022-11-03 14:21:02.000000 ruff-0.0.98/src/fs.rs
--rw-r--r--   0      501       20     2144 2022-11-03 14:21:02.000000 ruff-0.0.98/src/lib.rs
--rw-r--r--   0      501       20    19321 2022-11-03 14:21:02.000000 ruff-0.0.98/src/linter.rs
--rw-r--r--   0      501       20     1989 2022-11-03 14:21:02.000000 ruff-0.0.98/src/logging.rs
--rw-r--r--   0      501       20    13963 2022-11-03 14:21:02.000000 ruff-0.0.98/src/main.rs
--rw-r--r--   0      501       20     1733 2022-11-03 14:21:02.000000 ruff-0.0.98/src/message.rs
--rw-r--r--   0      501       20     8990 2022-11-03 14:21:02.000000 ruff-0.0.98/src/noqa.rs
--rw-r--r--   0      501       20     9580 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pep8_naming/checks.rs
--rw-r--r--   0      501       20       34 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pep8_naming/mod.rs
--rw-r--r--   0      501       20     1859 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pep8_naming/settings.rs
--rw-r--r--   0      501       20     3935 2022-11-03 14:21:02.000000 ruff-0.0.98/src/printer.rs
--rw-r--r--   0      501       20    10683 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pycodestyle/checks.rs
--rw-r--r--   0      501       20       16 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pycodestyle/mod.rs
--rw-r--r--   0      501       20       17 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pydocstyle/mod.rs
--rw-r--r--   0      501       20    60594 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pydocstyle/plugins.rs
--rw-r--r--   0      501       20     9625 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/checks.rs
--rw-r--r--   0      501       20     4224 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/fixes.rs
--rw-r--r--   0      501       20       48 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/mod.rs
--rw-r--r--   0      501       20      362 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/plugins/assert_tuple.rs
--rw-r--r--   0      501       20      350 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/plugins/if_tuple.rs
--rw-r--r--   0      501       20      708 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/plugins/invalid_print_syntax.rs
--rw-r--r--   0      501       20      175 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyflakes/plugins/mod.rs
--rw-r--r--   0      501       20     2925 2022-11-03 14:21:02.000000 ruff-0.0.98/src/python/builtins.rs
--rw-r--r--   0      501       20      300 2022-11-03 14:21:02.000000 ruff-0.0.98/src/python/future.rs
--rw-r--r--   0      501       20       50 2022-11-03 14:21:02.000000 ruff-0.0.98/src/python/mod.rs
--rw-r--r--   0      501       20     9789 2022-11-03 14:21:02.000000 ruff-0.0.98/src/python/typing.rs
--rw-r--r--   0      501       20     5229 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/checks.rs
--rw-r--r--   0      501       20     4454 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/fixes.rs
--rw-r--r--   0      501       20       59 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/mod.rs
--rw-r--r--   0      501       20     1970 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/deprecated_unittest_alias.rs
--rw-r--r--   0      501       20      676 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/mod.rs
--rw-r--r--   0      501       20     1025 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/super_call_with_parameters.rs
--rw-r--r--   0      501       20      769 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/type_of_primitive.rs
--rw-r--r--   0      501       20      639 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/unnecessary_abspath.rs
--rw-r--r--   0      501       20      571 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/use_pep585_annotation.rs
--rw-r--r--   0      501       20     3378 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/use_pep604_annotation.rs
--rw-r--r--   0      501       20     1315 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/useless_metaclass_type.rs
--rw-r--r--   0      501       20      763 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/plugins/useless_object_inheritance.rs
--rw-r--r--   0      501       20     1092 2022-11-03 14:21:02.000000 ruff-0.0.98/src/pyupgrade/types.rs
--rw-r--r--   0      501       20     4057 2022-11-03 14:21:02.000000 ruff-0.0.98/src/settings/configuration.rs
--rw-r--r--   0      501       20     5970 2022-11-03 14:21:02.000000 ruff-0.0.98/src/settings/mod.rs
--rw-r--r--   0      501       20     1023 2022-11-03 14:21:02.000000 ruff-0.0.98/src/settings/options.rs
--rw-r--r--   0      501       20    11361 2022-11-03 14:21:02.000000 ruff-0.0.98/src/settings/pyproject.rs
--rw-r--r--   0      501       20     3714 2022-11-03 14:21:02.000000 ruff-0.0.98/src/settings/types.rs
--rw-r--r--   0      501       20     2856 2022-11-03 14:21:02.000000 ruff-0.0.98/src/settings/user.rs
--rw-r--r--   0      501       20     2445 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__A001_A001.py.snap
--rw-r--r--   0      501       20      986 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__A002_A002.py.snap
--rw-r--r--   0      501       20      319 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__A003_A003.py.snap
--rw-r--r--   0      501       20      289 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B002_B002.py.snap
--rw-r--r--   0      501       20     1394 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap
--rw-r--r--   0      501       20     1174 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B007_B007.py.snap
--rw-r--r--   0      501       20      629 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B011_B011.py.snap
--rw-r--r--   0      501       20      195 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B013_B013.py.snap
--rw-r--r--   0      501       20      964 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B014_B014.py.snap
--rw-r--r--   0      501       20      171 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B017_B017.py.snap
--rw-r--r--   0      501       20      617 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__B025_B025.py.snap
--rw-r--r--   0      501       20      638 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C400_C400.py.snap
--rw-r--r--   0      501       20      636 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C401_C401.py.snap
--rw-r--r--   0      501       20      644 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C402_C402.py.snap
--rw-r--r--   0      501       20      652 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C403_C403.py.snap
--rw-r--r--   0      501       20      179 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C404_C404.py.snap
--rw-r--r--   0      501       20     1178 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C405_C405.py.snap
--rw-r--r--   0      501       20      568 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C406_C406.py.snap
--rw-r--r--   0      501       20     1030 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C408_C408.py.snap
--rw-r--r--   0      501       20     1532 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C409_C409.py.snap
--rw-r--r--   0      501       20     1220 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C410_C410.py.snap
--rw-r--r--   0      501       20      329 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C411_C411.py.snap
--rw-r--r--   0      501       20      460 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C413_C413.py.snap
--rw-r--r--   0      501       20     2134 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C414_C414.py.snap
--rw-r--r--   0      501       20      597 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C415_C415.py.snap
--rw-r--r--   0      501       20      311 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C416_C416.py.snap
--rw-r--r--   0      501       20     1042 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__C417_C417.py.snap
--rw-r--r--   0      501       20      158 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D100_D.py.snap
--rw-r--r--   0      501       20      159 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D101_D.py.snap
--rw-r--r--   0      501       20      380 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D102_D.py.snap
--rw-r--r--   0      501       20      164 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D103_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D104_D.py.snap
--rw-r--r--   0      501       20      159 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D105_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D106_D.py.snap
--rw-r--r--   0      501       20      268 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D107_D.py.snap
--rw-r--r--   0      501       20      620 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D201_D.py.snap
--rw-r--r--   0      501       20      618 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D202_D.py.snap
--rw-r--r--   0      501       20      904 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D203_D.py.snap
--rw-r--r--   0      501       20      618 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D204_D.py.snap
--rw-r--r--   0      501       20      600 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D205_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D206_D.py.snap
--rw-r--r--   0      501       20      630 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D207_D.py.snap
--rw-r--r--   0      501       20      869 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D208_D.py.snap
--rw-r--r--   0      501       20      336 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D209_D.py.snap
--rw-r--r--   0      501       20      949 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D210_D.py.snap
--rw-r--r--   0      501       20      614 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D211_D.py.snap
--rw-r--r--   0      501       20      175 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D212_D.py.snap
--rw-r--r--   0      501       20     2069 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D213_D.py.snap
--rw-r--r--   0      501       20      341 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D214_sections.py.snap
--rw-r--r--   0      501       20      650 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D215_sections.py.snap
--rw-r--r--   0      501       20      635 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D300_D.py.snap
--rw-r--r--   0      501       20     1860 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D400_D.py.snap
--rw-r--r--   0      501       20      162 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D402_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D403_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D404_D.py.snap
--rw-r--r--   0      501       20      642 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D405_sections.py.snap
--rw-r--r--   0      501       20     1204 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D406_sections.py.snap
--rw-r--r--   0      501       20     4593 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D407_sections.py.snap
--rw-r--r--   0      501       20      336 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D408_sections.py.snap
--rw-r--r--   0      501       20      677 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D409_sections.py.snap
--rw-r--r--   0      501       20      622 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D410_sections.py.snap
--rw-r--r--   0      501       20      911 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D411_sections.py.snap
--rw-r--r--   0      501       20      356 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D412_sections.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D413_sections.py.snap
--rw-r--r--   0      501       20      683 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D414_sections.py.snap
--rw-r--r--   0      501       20     1822 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D415_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D416_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D417_canonical_google_examples.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D417_canonical_numpy_examples.py.snap
--rw-r--r--   0      501       20     1667 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D417_sections.py.snap
--rw-r--r--   0      501       20      385 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D418_D.py.snap
--rw-r--r--   0      501       20      371 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__D419_D.py.snap
--rw-r--r--   0      501       20      174 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E402_E402.py.snap
--rw-r--r--   0      501       20      187 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E501_E501.py.snap
--rw-r--r--   0      501       20     1024 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E711_E711.py.snap
--rw-r--r--   0      501       20     1383 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E712_E712.py.snap
--rw-r--r--   0      501       20      587 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E713_E713.py.snap
--rw-r--r--   0      501       20      369 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E714_E714.py.snap
--rw-r--r--   0      501       20     1868 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E721_E721.py.snap
--rw-r--r--   0      501       20      396 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E722_E722.py.snap
--rw-r--r--   0      501       20      624 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E731_E731.py.snap
--rw-r--r--   0      501       20     3201 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E741_E741.py.snap
--rw-r--r--   0      501       20      414 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E742_E742.py.snap
--rw-r--r--   0      501       20      424 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E743_E743.py.snap
--rw-r--r--   0      501       20      181 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__E999_E999.py.snap
--rw-r--r--   0      501       20     2224 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_1.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_2.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_3.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_4.py.snap
--rw-r--r--   0      501       20     1214 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap
--rw-r--r--   0      501       20      342 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F402_F402.py.snap
--rw-r--r--   0      501       20      292 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F403_F403.py.snap
--rw-r--r--   0      501       20      163 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F404_F404.py.snap
--rw-r--r--   0      501       20      347 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F405_F405.py.snap
--rw-r--r--   0      501       20      308 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F406_F406.py.snap
--rw-r--r--   0      501       20      196 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F407_F407.py.snap
--rw-r--r--   0      501       20      419 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F541_F541.py.snap
--rw-r--r--   0      501       20      425 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F601_F601.py.snap
--rw-r--r--   0      501       20      182 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F602_F602.py.snap
--rw-r--r--   0      501       20      167 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F622_F622.py.snap
--rw-r--r--   0      501       20      266 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F631_F631.py.snap
--rw-r--r--   0      501       20      262 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F632_F632.py.snap
--rw-r--r--   0      501       20      164 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F633_F633.py.snap
--rw-r--r--   0      501       20      256 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F634_F634.py.snap
--rw-r--r--   0      501       20      504 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F701_F701.py.snap
--rw-r--r--   0      501       20      519 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F702_F702.py.snap
--rw-r--r--   0      501       20      402 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F704_F704.py.snap
--rw-r--r--   0      501       20      285 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F706_F706.py.snap
--rw-r--r--   0      501       20      402 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F707_F707.py.snap
--rw-r--r--   0      501       20      185 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F722_F722.py.snap
--rw-r--r--   0      501       20     1410 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap
--rw-r--r--   0      501       20      545 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap
--rw-r--r--   0      501       20      172 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F821_F821_2.py.snap
--rw-r--r--   0      501       20      168 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F822_F822.py.snap
--rw-r--r--   0      501       20      173 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F823_F823.py.snap
--rw-r--r--   0      501       20      407 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F831_F831.py.snap
--rw-r--r--   0      501       20      645 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F841_F841.py.snap
--rw-r--r--   0      501       20      284 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__F901_F901.py.snap
--rw-r--r--   0      501       20      679 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N801_N801.py.snap
--rw-r--r--   0      501       20      688 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N802_N802.py.snap
--rw-r--r--   0      501       20      298 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N803_N803.py.snap
--rw-r--r--   0      501       20      186 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N804_N804.py.snap
--rw-r--r--   0      501       20      314 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N805_N805.py.snap
--rw-r--r--   0      501       20      328 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N806_N806.py.snap
--rw-r--r--   0      501       20      164 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N807_N807.py.snap
--rw-r--r--   0      501       20      555 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N811_N811.py.snap
--rw-r--r--   0      501       20      568 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N812_N812.py.snap
--rw-r--r--   0      501       20      555 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N813_N813.py.snap
--rw-r--r--   0      501       20      552 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N814_N814.py.snap
--rw-r--r--   0      501       20      475 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N815_N815.py.snap
--rw-r--r--   0      501       20      477 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N816_N816.py.snap
--rw-r--r--   0      501       20      360 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N817_N817.py.snap
--rw-r--r--   0      501       20      180 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__N818_N818.py.snap
--rw-r--r--   0      501       20      305 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__T201_T201.py.snap
--rw-r--r--   0      501       20      562 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__T203_T203.py.snap
--rw-r--r--   0      501       20      583 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U001_U001.py.snap
--rw-r--r--   0      501       20      864 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U002_U002.py.snap
--rw-r--r--   0      501       20     1411 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U003_U003.py.snap
--rw-r--r--   0      501       20     5675 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U004_U004.py.snap
--rw-r--r--   0      501       20     1407 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U005_U005.py.snap
--rw-r--r--   0      501       20      608 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U006_U006.py.snap
--rw-r--r--   0      501       20     2314 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U007_U007.py.snap
--rw-r--r--   0      501       20     1442 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__U008_U008.py.snap
--rw-r--r--   0      501       20      166 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__W292_W292_0.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__W292_W292_1.py.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__W292_W292_2.py.snap
--rw-r--r--   0      501       20      555 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__W605_W605.py.snap
--rw-r--r--   0      501       20      894 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap
--rw-r--r--   0      501       20      503 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__future_annotations.snap
--rw-r--r--   0      501       20       53 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__init.snap
--rw-r--r--   0      501       20     2011 2022-11-03 14:21:02.000000 ruff-0.0.98/src/snapshots/ruff__linter__tests__m001.snap
--rw-r--r--   0      501       20     3960 2022-11-03 14:21:02.000000 ruff-0.0.98/src/source_code_locator.rs
--rw-r--r--   0      501       20     5340 2022-11-03 14:21:02.000000 ruff-0.0.98/src/visibility.rs
--rw-r--r--   0      501       20     2220 2022-11-03 14:21:02.000000 ruff-0.0.98/tests/integration_test.rs
--rw-r--r--   0      501       20    82250 2022-11-03 14:21:02.000000 ruff-0.0.98/Cargo.lock
--rw-r--r--   0        0        0    36355 1970-01-01 00:00:00.000000 ruff-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 ruff-0.0.99/Cargo.toml
+-rw-r--r--   0      501       20      278 2022-11-03 15:48:01.000000 ruff-0.0.99/.editorconfig
+-rw-r--r--   0      501       20     3712 2022-11-03 15:48:01.000000 ruff-0.0.99/.github/workflows/ci.yaml
+-rw-r--r--   0      501       20     8911 2022-11-03 15:48:01.000000 ruff-0.0.99/.github/workflows/flake8-to-ruff.yaml
+-rw-r--r--   0      501       20     8618 2022-11-03 15:48:01.000000 ruff-0.0.99/.github/workflows/ruff.yaml
+-rw-r--r--   0      501       20     3407 2022-11-03 15:48:01.000000 ruff-0.0.99/.gitignore
+-rw-r--r--   0      501       20      231 2022-11-03 15:48:01.000000 ruff-0.0.99/.pre-commit-config.yaml
+-rw-r--r--   0      501       20     5227 2022-11-03 15:48:01.000000 ruff-0.0.99/CODE_OF_CONDUCT.md
+-rw-r--r--   0      501       20     4582 2022-11-03 15:48:01.000000 ruff-0.0.99/CONTRIBUTING.md
+-rw-r--r--   0      501       20    82250 2022-11-03 15:48:01.000000 ruff-0.0.99/Cargo.lock
+-rw-r--r--   0      501       20     1070 2022-11-03 15:48:01.000000 ruff-0.0.99/LICENSE
+-rw-r--r--   0      501       20    35357 2022-11-03 15:48:01.000000 ruff-0.0.99/README.md
+-rw-r--r--   0      501       20      475 2022-11-03 15:48:01.000000 ruff-0.0.99/benches/source_code_locator.rs
+-rw-r--r--   0      501       20     3261 2022-11-03 15:48:01.000000 ruff-0.0.99/examples/generate_check_code_prefix.rs
+-rw-r--r--   0      501       20      942 2022-11-03 15:48:01.000000 ruff-0.0.99/examples/generate_rules_table.rs
+-rw-r--r--   0      501       20      568 2022-11-03 15:48:01.000000 ruff-0.0.99/examples/generate_source_code.rs
+-rw-r--r--   0      501       20      477 2022-11-03 15:48:01.000000 ruff-0.0.99/examples/print_ast.rs
+-rw-r--r--   0      501       20      470 2022-11-03 15:48:01.000000 ruff-0.0.99/examples/print_tokens.rs
+-rw-r--r--   0      501       20     1100 2022-11-03 15:48:01.000000 ruff-0.0.99/pyproject.toml
+-rw-r--r--   0      501       20      368 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/A001.py
+-rw-r--r--   0      501       20      130 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/A002.py
+-rw-r--r--   0      501       20      127 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/A003.py
+-rw-r--r--   0      501       20      223 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B002.py
+-rw-r--r--   0      501       20     3342 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B006_B008.py
+-rw-r--r--   0      501       20      716 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B007.py
+-rw-r--r--   0      501       20      133 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B011.py
+-rw-r--r--   0      501       20      119 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B013.py
+-rw-r--r--   0      501       20     1364 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B014.py
+-rw-r--r--   0      501       20      829 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B017.py
+-rw-r--r--   0      501       20      446 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/B025.py
+-rw-r--r--   0      501       20       66 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C400.py
+-rw-r--r--   0      501       20       64 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C401.py
+-rw-r--r--   0      501       20      106 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C402.py
+-rw-r--r--   0      501       20       68 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C403.py
+-rw-r--r--   0      501       20       71 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C404.py
+-rw-r--r--   0      501       20       71 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C405.py
+-rw-r--r--   0      501       20       81 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C406.py
+-rw-r--r--   0      501       20       66 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C408.py
+-rw-r--r--   0      501       20      107 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C409.py
+-rw-r--r--   0      501       20       64 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C410.py
+-rw-r--r--   0      501       20       35 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C411.py
+-rw-r--r--   0      501       20       84 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C413.py
+-rw-r--r--   0      501       20      216 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C414.py
+-rw-r--r--   0      501       20      193 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C415.py
+-rw-r--r--   0      501       20       95 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C416.py
+-rw-r--r--   0      501       20      179 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/C417.py
+-rw-r--r--   0      501       20    12157 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/D.py
+-rw-r--r--   0      501       20      294 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E402.py
+-rw-r--r--   0      501       20      786 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E501.py
+-rw-r--r--   0      501       20      648 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E711.py
+-rw-r--r--   0      501       20      653 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E712.py
+-rw-r--r--   0      501       20      540 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E713.py
+-rw-r--r--   0      501       20      508 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E714.py
+-rw-r--r--   0      501       20      907 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E721.py
+-rw-r--r--   0      501       20      327 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E722.py
+-rw-r--r--   0      501       20      252 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E731.py
+-rw-r--r--   0      501       20      676 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E741.py
+-rw-r--r--   0      501       20       78 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E742.py
+-rw-r--r--   0      501       20       99 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E743.py
+-rw-r--r--   0      501       20       10 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/E999.py
+-rw-r--r--   0      501       20     1549 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/F401_0.py
+-rw-r--r--   0      501       20      121 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/F401_1.py
+-rw-r--r--   0      501       20      242 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/F401_2.py
+-rw-r--r--   0      501       20      302 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/F401_3.py
+-rw-r--r--   0      501       20      315 2022-11-03 15:48:01.000000 ruff-0.0.99/resources/test/fixtures/F401_4.py
+-rw-r--r--   0      501       20      126 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F401_5.py
+-rw-r--r--   0      501       20       96 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F402.py
+-rw-r--r--   0      501       20      152 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F403.py
+-rw-r--r--   0      501       20      130 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F404.py
+-rw-r--r--   0      501       20      116 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F405.py
+-rw-r--r--   0      501       20       87 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F406.py
+-rw-r--r--   0      501       20       82 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F407.py
+-rw-r--r--   0      501       20      112 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F541.py
+-rw-r--r--   0      501       20      144 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F601.py
+-rw-r--r--   0      501       20       50 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F602.py
+-rw-r--r--   0      501       20       64 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F622.py
+-rw-r--r--   0      501       20       58 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F631.py
+-rw-r--r--   0      501       20       51 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F632.py
+-rw-r--r--   0      501       20       79 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F633.py
+-rw-r--r--   0      501       20      122 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F634.py
+-rw-r--r--   0      501       20      179 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F701.py
+-rw-r--r--   0      501       20      200 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F702.py
+-rw-r--r--   0      501       20       76 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F704.py
+-rw-r--r--   0      501       20       66 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F706.py
+-rw-r--r--   0      501       20      380 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F707.py
+-rw-r--r--   0      501       20       74 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F722.py
+-rw-r--r--   0      501       20     2196 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F821_0.py
+-rw-r--r--   0      501       20      395 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F821_1.py
+-rw-r--r--   0      501       20      259 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F821_2.py
+-rw-r--r--   0      501       20       28 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F822.py
+-rw-r--r--   0      501       20      245 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F823.py
+-rw-r--r--   0      501       20      159 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F831.py
+-rw-r--r--   0      501       20      343 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F841.py
+-rw-r--r--   0      501       20       88 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/F901.py
+-rw-r--r--   0      501       20     1762 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/M001.py
+-rw-r--r--   0      501       20      225 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N801.py
+-rw-r--r--   0      501       20      354 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N802.py
+-rw-r--r--   0      501       20       95 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N803.py
+-rw-r--r--   0      501       20      264 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N804.py
+-rw-r--r--   0      501       20      345 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N805.py
+-rw-r--r--   0      501       20       64 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N806.py
+-rw-r--r--   0      501       20      126 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N807.py
+-rw-r--r--   0      501       20      116 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N811.py
+-rw-r--r--   0      501       20      124 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N812.py
+-rw-r--r--   0      501       20      119 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N813.py
+-rw-r--r--   0      501       20      119 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N814.py
+-rw-r--r--   0      501       20       96 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N815.py
+-rw-r--r--   0      501       20       67 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N816.py
+-rw-r--r--   0      501       20       55 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N817.py
+-rw-r--r--   0      501       20      106 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/N818.py
+-rw-r--r--   0      501       20       31 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/T201.py
+-rw-r--r--   0      501       20      148 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/T203.py
+-rw-r--r--   0      501       20      152 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U001.py
+-rw-r--r--   0      501       20      146 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U002.py
+-rw-r--r--   0      501       20       45 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U003.py
+-rw-r--r--   0      501       20      883 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U004.py
+-rw-r--r--   0      501       20      263 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U005.py
+-rw-r--r--   0      501       20      125 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U006.py
+-rw-r--r--   0      501       20      463 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U007.py
+-rw-r--r--   0      501       20     1483 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/U008.py
+-rw-r--r--   0      501       20       26 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/W292_0.py
+-rw-r--r--   0      501       20       40 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/W292_1.py
+-rw-r--r--   0      501       20       27 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/W292_2.py
+-rw-r--r--   0      501       20      316 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/W605.py
+-rw-r--r--   0      501       20       54 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/__init__.py
+-rw-r--r--   0      501       20        0 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/bar/__init__.py
+-rw-r--r--   0      501       20        0 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/bar/migrations/__init__.py
+-rw-r--r--   0      501       20       90 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/bar/migrations/migration.py
+-rw-r--r--   0      501       20     4176 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/canonical_google_examples.py
+-rw-r--r--   0      501       20     5315 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/canonical_numpy_examples.py
+-rw-r--r--   0      501       20       90 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/directory/also_excluded.py
+-rw-r--r--   0      501       20       90 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/excluded.py
+-rw-r--r--   0      501       20      716 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_doubles.py
+-rw-r--r--   0      501       20      290 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_doubles_class.py
+-rw-r--r--   0      501       20      406 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_doubles_function.py
+-rw-r--r--   0      501       20      133 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_doubles_module_multiline.py
+-rw-r--r--   0      501       20      135 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_doubles_module_singleline.py
+-rw-r--r--   0      501       20      772 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_singles.py
+-rw-r--r--   0      501       20      290 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_singles_class.py
+-rw-r--r--   0      501       20      408 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_singles_function.py
+-rw-r--r--   0      501       20      133 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_singles_module_multiline.py
+-rw-r--r--   0      501       20      135 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_singles_module_singleline.py
+-rw-r--r--   0      501       20       93 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/doubles.py
+-rw-r--r--   0      501       20      203 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/doubles_escaped.py
+-rw-r--r--   0      501       20      165 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/doubles_multiline_string.py
+-rw-r--r--   0      501       20       58 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/doubles_noqa.py
+-rw-r--r--   0      501       20      106 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/doubles_wrapped.py
+-rw-r--r--   0      501       20       93 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/singles.py
+-rw-r--r--   0      501       20      203 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/singles_escaped.py
+-rw-r--r--   0      501       20      165 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/singles_multiline_string.py
+-rw-r--r--   0      501       20       58 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/singles_noqa.py
+-rw-r--r--   0      501       20      106 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/flake8_quotes/singles_wrapped.py
+-rw-r--r--   0      501       20        0 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/foo/__init__.py
+-rw-r--r--   0      501       20        0 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/foo/migrations/__init__.py
+-rw-r--r--   0      501       20       90 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/foo/migrations/migration.py
+-rw-r--r--   0      501       20      444 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/future_annotations.py
+-rw-r--r--   0      501       20      632 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/pyproject.toml
+-rw-r--r--   0      501       20    12260 2022-11-03 15:48:02.000000 ruff-0.0.99/resources/test/fixtures/sections.py
+-rw-r--r--   0      501       20        7 2022-11-03 15:48:02.000000 ruff-0.0.99/rust-toolchain
+-rw-r--r--   0      501       20      390 2022-11-03 15:48:02.000000 ruff-0.0.99/rustfmt.toml
+-rw-r--r--   0      501       20      302 2022-11-03 15:48:02.000000 ruff-0.0.99/scripts/.flake8
+-rw-r--r--   0      501       20    37365 2022-11-03 15:48:02.000000 ruff-0.0.99/scripts/poetry.lock
+-rw-r--r--   0      501       20      454 2022-11-03 15:48:02.000000 ruff-0.0.99/scripts/pyproject.toml
+-rwxr-xr-x   0      501       20     1035 2022-11-03 15:48:02.000000 ruff-0.0.99/scripts/run_flake8.py
+-rw-r--r--   0      501       20      565 2022-11-03 15:48:02.000000 ruff-0.0.99/setup.py
+-rw-r--r--   0      501       20     4422 2022-11-03 15:48:02.000000 ruff-0.0.99/src/ast/helpers.rs
+-rw-r--r--   0      501       20       87 2022-11-03 15:48:02.000000 ruff-0.0.99/src/ast/mod.rs
+-rw-r--r--   0      501       20     3881 2022-11-03 15:48:02.000000 ruff-0.0.99/src/ast/operations.rs
+-rw-r--r--   0      501       20     4574 2022-11-03 15:48:02.000000 ruff-0.0.99/src/ast/relocate.rs
+-rw-r--r--   0      501       20     2211 2022-11-03 15:48:02.000000 ruff-0.0.99/src/ast/types.rs
+-rw-r--r--   0      501       20    18283 2022-11-03 15:48:02.000000 ruff-0.0.99/src/ast/visitor.rs
+-rw-r--r--   0      501       20     6495 2022-11-03 15:48:02.000000 ruff-0.0.99/src/autofix/fixer.rs
+-rw-r--r--   0      501       20     3383 2022-11-03 15:48:02.000000 ruff-0.0.99/src/autofix/helpers.rs
+-rw-r--r--   0      501       20     1217 2022-11-03 15:48:02.000000 ruff-0.0.99/src/autofix/mod.rs
+-rw-r--r--   0      501       20     4136 2022-11-03 15:48:02.000000 ruff-0.0.99/src/cache.rs
+-rw-r--r--   0      501       20   100232 2022-11-03 15:48:02.000000 ruff-0.0.99/src/check_ast.rs
+-rw-r--r--   0      501       20     9787 2022-11-03 15:48:02.000000 ruff-0.0.99/src/check_lines.rs
+-rw-r--r--   0      501       20     1740 2022-11-03 15:48:02.000000 ruff-0.0.99/src/check_tokens.rs
+-rw-r--r--   0      501       20    69810 2022-11-03 15:48:02.000000 ruff-0.0.99/src/checks.rs
+-rw-r--r--   0      501       20    43059 2022-11-03 15:48:02.000000 ruff-0.0.99/src/checks_gen.rs
+-rw-r--r--   0      501       20     6185 2022-11-03 15:48:02.000000 ruff-0.0.99/src/cli.rs
+-rw-r--r--   0      501       20    36461 2022-11-03 15:48:02.000000 ruff-0.0.99/src/code_gen.rs
+-rw-r--r--   0      501       20     1201 2022-11-03 15:48:02.000000 ruff-0.0.99/src/cst/helpers.rs
+-rw-r--r--   0      501       20      536 2022-11-03 15:48:02.000000 ruff-0.0.99/src/cst/matchers.rs
+-rw-r--r--   0      501       20       35 2022-11-03 15:48:02.000000 ruff-0.0.99/src/cst/mod.rs
+-rw-r--r--   0      501       20      404 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/definition.rs
+-rw-r--r--   0      501       20     2428 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/extraction.rs
+-rw-r--r--   0      501       20     1423 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/google.rs
+-rw-r--r--   0      501       20     1363 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/helpers.rs
+-rw-r--r--   0      501       20      122 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/mod.rs
+-rw-r--r--   0      501       20      908 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/numpy.rs
+-rw-r--r--   0      501       20     3140 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/sections.rs
+-rw-r--r--   0      501       20      797 2022-11-03 15:48:02.000000 ruff-0.0.99/src/docstrings/styles.rs
+-rw-r--r--   0      501       20       17 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/mod.rs
+-rw-r--r--   0      501       20     2046 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/assert_false.rs
+-rw-r--r--   0      501       20      918 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/assert_raises_exception.rs
+-rw-r--r--   0      501       20     4108 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/duplicate_exceptions.rs
+-rw-r--r--   0      501       20      654 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/mod.rs
+-rw-r--r--   0      501       20     2255 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/mutable_argument_default.rs
+-rw-r--r--   0      501       20      822 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs
+-rw-r--r--   0      501       20      635 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/unary_prefix_increment.rs
+-rw-r--r--   0      501       20     2046 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_bugbear/plugins/unused_loop_control_variable.rs
+-rw-r--r--   0      501       20      759 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_builtins/checks.rs
+-rw-r--r--   0      501       20       31 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_builtins/mod.rs
+-rw-r--r--   0      501       20       70 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_builtins/types.rs
+-rw-r--r--   0      501       20    15487 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_comprehensions/checks.rs
+-rw-r--r--   0      501       20    21798 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_comprehensions/fixes.rs
+-rw-r--r--   0      501       20       27 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_comprehensions/mod.rs
+-rw-r--r--   0      501       20      949 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_print/checks.rs
+-rw-r--r--   0      501       20       29 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_print/mod.rs
+-rw-r--r--   0      501       20       49 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_print/plugins/mod.rs
+-rw-r--r--   0      501       20     1657 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_print/plugins/print_call.rs
+-rw-r--r--   0      501       20    10466 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/checks.rs
+-rw-r--r--   0      501       20     3662 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/docstring_detection.rs
+-rw-r--r--   0      501       20       63 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/mod.rs
+-rw-r--r--   0      501       20     1382 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/settings.rs
+-rw-r--r--   0      501       20      737 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap
+-rw-r--r--   0      501       20      331 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_class.py.snap
+-rw-r--r--   0      501       20      737 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap
+-rw-r--r--   0      501       20      329 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_multiline.py.snap
+-rw-r--r--   0      501       20      330 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_singleline.py.snap
+-rw-r--r--   0      501       20      447 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles.py.snap
+-rw-r--r--   0      501       20      446 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_class.py.snap
+-rw-r--r--   0      501       20      318 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_function.py.snap
+-rw-r--r--   0      501       20      190 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_multiline.py.snap
+-rw-r--r--   0      501       20      191 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_singleline.py.snap
+-rw-r--r--   0      501       20      326 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles.py.snap
+-rw-r--r--   0      501       20      178 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_escaped.py.snap
+-rw-r--r--   0      501       20      197 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_multiline_string.py.snap
+-rw-r--r--   0      501       20       67 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_noqa.py.snap
+-rw-r--r--   0      501       20       67 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_wrapped.py.snap
+-rw-r--r--   0      501       20      447 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles.py.snap
+-rw-r--r--   0      501       20      446 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_class.py.snap
+-rw-r--r--   0      501       20      318 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_function.py.snap
+-rw-r--r--   0      501       20      190 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_multiline.py.snap
+-rw-r--r--   0      501       20      191 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_singleline.py.snap
+-rw-r--r--   0      501       20      872 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap
+-rw-r--r--   0      501       20      331 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_class.py.snap
+-rw-r--r--   0      501       20      737 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap
+-rw-r--r--   0      501       20      329 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_multiline.py.snap
+-rw-r--r--   0      501       20      330 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_singleline.py.snap
+-rw-r--r--   0      501       20      326 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles.py.snap
+-rw-r--r--   0      501       20      178 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_escaped.py.snap
+-rw-r--r--   0      501       20      197 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_multiline_string.py.snap
+-rw-r--r--   0      501       20       67 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_noqa.py.snap
+-rw-r--r--   0      501       20       67 2022-11-03 15:48:02.000000 ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_wrapped.py.snap
+-rw-r--r--   0      501       20     9122 2022-11-03 15:48:02.000000 ruff-0.0.99/src/fs.rs
+-rw-r--r--   0      501       20     2144 2022-11-03 15:48:02.000000 ruff-0.0.99/src/lib.rs
+-rw-r--r--   0      501       20    19321 2022-11-03 15:48:02.000000 ruff-0.0.99/src/linter.rs
+-rw-r--r--   0      501       20     1989 2022-11-03 15:48:02.000000 ruff-0.0.99/src/logging.rs
+-rw-r--r--   0      501       20    13963 2022-11-03 15:48:02.000000 ruff-0.0.99/src/main.rs
+-rw-r--r--   0      501       20     1733 2022-11-03 15:48:02.000000 ruff-0.0.99/src/message.rs
+-rw-r--r--   0      501       20     8990 2022-11-03 15:48:02.000000 ruff-0.0.99/src/noqa.rs
+-rw-r--r--   0      501       20     9580 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pep8_naming/checks.rs
+-rw-r--r--   0      501       20       34 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pep8_naming/mod.rs
+-rw-r--r--   0      501       20     1859 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pep8_naming/settings.rs
+-rw-r--r--   0      501       20     3935 2022-11-03 15:48:02.000000 ruff-0.0.99/src/printer.rs
+-rw-r--r--   0      501       20    10683 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pycodestyle/checks.rs
+-rw-r--r--   0      501       20       16 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pycodestyle/mod.rs
+-rw-r--r--   0      501       20       17 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pydocstyle/mod.rs
+-rw-r--r--   0      501       20    60594 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pydocstyle/plugins.rs
+-rw-r--r--   0      501       20     9625 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/checks.rs
+-rw-r--r--   0      501       20     4219 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/fixes.rs
+-rw-r--r--   0      501       20       48 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/mod.rs
+-rw-r--r--   0      501       20      362 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/plugins/assert_tuple.rs
+-rw-r--r--   0      501       20      350 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/plugins/if_tuple.rs
+-rw-r--r--   0      501       20      708 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/plugins/invalid_print_syntax.rs
+-rw-r--r--   0      501       20      175 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyflakes/plugins/mod.rs
+-rw-r--r--   0      501       20     2925 2022-11-03 15:48:02.000000 ruff-0.0.99/src/python/builtins.rs
+-rw-r--r--   0      501       20      300 2022-11-03 15:48:02.000000 ruff-0.0.99/src/python/future.rs
+-rw-r--r--   0      501       20       50 2022-11-03 15:48:02.000000 ruff-0.0.99/src/python/mod.rs
+-rw-r--r--   0      501       20     9789 2022-11-03 15:48:02.000000 ruff-0.0.99/src/python/typing.rs
+-rw-r--r--   0      501       20     5229 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/checks.rs
+-rw-r--r--   0      501       20     4454 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/fixes.rs
+-rw-r--r--   0      501       20       59 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/mod.rs
+-rw-r--r--   0      501       20     1970 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/deprecated_unittest_alias.rs
+-rw-r--r--   0      501       20      676 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/mod.rs
+-rw-r--r--   0      501       20     1025 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/super_call_with_parameters.rs
+-rw-r--r--   0      501       20      769 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/type_of_primitive.rs
+-rw-r--r--   0      501       20      639 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/unnecessary_abspath.rs
+-rw-r--r--   0      501       20      571 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/use_pep585_annotation.rs
+-rw-r--r--   0      501       20     3378 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/use_pep604_annotation.rs
+-rw-r--r--   0      501       20     1315 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/useless_metaclass_type.rs
+-rw-r--r--   0      501       20      763 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/plugins/useless_object_inheritance.rs
+-rw-r--r--   0      501       20     1092 2022-11-03 15:48:02.000000 ruff-0.0.99/src/pyupgrade/types.rs
+-rw-r--r--   0      501       20     4057 2022-11-03 15:48:02.000000 ruff-0.0.99/src/settings/configuration.rs
+-rw-r--r--   0      501       20     5970 2022-11-03 15:48:02.000000 ruff-0.0.99/src/settings/mod.rs
+-rw-r--r--   0      501       20     1023 2022-11-03 15:48:02.000000 ruff-0.0.99/src/settings/options.rs
+-rw-r--r--   0      501       20    11361 2022-11-03 15:48:02.000000 ruff-0.0.99/src/settings/pyproject.rs
+-rw-r--r--   0      501       20     3714 2022-11-03 15:48:02.000000 ruff-0.0.99/src/settings/types.rs
+-rw-r--r--   0      501       20     2856 2022-11-03 15:48:02.000000 ruff-0.0.99/src/settings/user.rs
+-rw-r--r--   0      501       20     2445 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__A001_A001.py.snap
+-rw-r--r--   0      501       20      986 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__A002_A002.py.snap
+-rw-r--r--   0      501       20      319 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__A003_A003.py.snap
+-rw-r--r--   0      501       20      289 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B002_B002.py.snap
+-rw-r--r--   0      501       20     1394 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap
+-rw-r--r--   0      501       20     1174 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B007_B007.py.snap
+-rw-r--r--   0      501       20      629 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B011_B011.py.snap
+-rw-r--r--   0      501       20      195 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B013_B013.py.snap
+-rw-r--r--   0      501       20      964 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B014_B014.py.snap
+-rw-r--r--   0      501       20      171 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B017_B017.py.snap
+-rw-r--r--   0      501       20      617 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__B025_B025.py.snap
+-rw-r--r--   0      501       20      638 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C400_C400.py.snap
+-rw-r--r--   0      501       20      636 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C401_C401.py.snap
+-rw-r--r--   0      501       20      644 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C402_C402.py.snap
+-rw-r--r--   0      501       20      652 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C403_C403.py.snap
+-rw-r--r--   0      501       20      179 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C404_C404.py.snap
+-rw-r--r--   0      501       20     1178 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C405_C405.py.snap
+-rw-r--r--   0      501       20     1181 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C406_C406.py.snap
+-rw-r--r--   0      501       20     1189 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C408_C408.py.snap
+-rw-r--r--   0      501       20     1532 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C409_C409.py.snap
+-rw-r--r--   0      501       20     1220 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C410_C410.py.snap
+-rw-r--r--   0      501       20      329 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C411_C411.py.snap
+-rw-r--r--   0      501       20      460 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C413_C413.py.snap
+-rw-r--r--   0      501       20     2134 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C414_C414.py.snap
+-rw-r--r--   0      501       20      597 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C415_C415.py.snap
+-rw-r--r--   0      501       20      618 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C416_C416.py.snap
+-rw-r--r--   0      501       20     1042 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__C417_C417.py.snap
+-rw-r--r--   0      501       20      158 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D100_D.py.snap
+-rw-r--r--   0      501       20      159 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D101_D.py.snap
+-rw-r--r--   0      501       20      380 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D102_D.py.snap
+-rw-r--r--   0      501       20      164 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D103_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D104_D.py.snap
+-rw-r--r--   0      501       20      159 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D105_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D106_D.py.snap
+-rw-r--r--   0      501       20      268 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D107_D.py.snap
+-rw-r--r--   0      501       20      620 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D201_D.py.snap
+-rw-r--r--   0      501       20      618 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D202_D.py.snap
+-rw-r--r--   0      501       20      904 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D203_D.py.snap
+-rw-r--r--   0      501       20      618 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D204_D.py.snap
+-rw-r--r--   0      501       20      600 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D205_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D206_D.py.snap
+-rw-r--r--   0      501       20      630 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D207_D.py.snap
+-rw-r--r--   0      501       20      869 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D208_D.py.snap
+-rw-r--r--   0      501       20      336 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D209_D.py.snap
+-rw-r--r--   0      501       20      949 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D210_D.py.snap
+-rw-r--r--   0      501       20      614 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D211_D.py.snap
+-rw-r--r--   0      501       20      175 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D212_D.py.snap
+-rw-r--r--   0      501       20     2069 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D213_D.py.snap
+-rw-r--r--   0      501       20      341 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D214_sections.py.snap
+-rw-r--r--   0      501       20      650 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D215_sections.py.snap
+-rw-r--r--   0      501       20      635 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D300_D.py.snap
+-rw-r--r--   0      501       20     1860 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D400_D.py.snap
+-rw-r--r--   0      501       20      162 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D402_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D403_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D404_D.py.snap
+-rw-r--r--   0      501       20      642 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D405_sections.py.snap
+-rw-r--r--   0      501       20     1204 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D406_sections.py.snap
+-rw-r--r--   0      501       20     4593 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D407_sections.py.snap
+-rw-r--r--   0      501       20      336 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D408_sections.py.snap
+-rw-r--r--   0      501       20      677 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D409_sections.py.snap
+-rw-r--r--   0      501       20      622 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D410_sections.py.snap
+-rw-r--r--   0      501       20      911 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D411_sections.py.snap
+-rw-r--r--   0      501       20      356 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D412_sections.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D413_sections.py.snap
+-rw-r--r--   0      501       20      683 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D414_sections.py.snap
+-rw-r--r--   0      501       20     1822 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D415_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D416_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D417_canonical_google_examples.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D417_canonical_numpy_examples.py.snap
+-rw-r--r--   0      501       20     1667 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D417_sections.py.snap
+-rw-r--r--   0      501       20      385 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D418_D.py.snap
+-rw-r--r--   0      501       20      371 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__D419_D.py.snap
+-rw-r--r--   0      501       20      174 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E402_E402.py.snap
+-rw-r--r--   0      501       20      187 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E501_E501.py.snap
+-rw-r--r--   0      501       20     1024 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E711_E711.py.snap
+-rw-r--r--   0      501       20     1383 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E712_E712.py.snap
+-rw-r--r--   0      501       20      587 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E713_E713.py.snap
+-rw-r--r--   0      501       20      369 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E714_E714.py.snap
+-rw-r--r--   0      501       20     1868 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E721_E721.py.snap
+-rw-r--r--   0      501       20      396 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E722_E722.py.snap
+-rw-r--r--   0      501       20      624 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E731_E731.py.snap
+-rw-r--r--   0      501       20     3201 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E741_E741.py.snap
+-rw-r--r--   0      501       20      414 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E742_E742.py.snap
+-rw-r--r--   0      501       20      424 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E743_E743.py.snap
+-rw-r--r--   0      501       20      181 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__E999_E999.py.snap
+-rw-r--r--   0      501       20     2224 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_1.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_2.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_3.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_4.py.snap
+-rw-r--r--   0      501       20     1214 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap
+-rw-r--r--   0      501       20      342 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F402_F402.py.snap
+-rw-r--r--   0      501       20      292 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F403_F403.py.snap
+-rw-r--r--   0      501       20      163 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F404_F404.py.snap
+-rw-r--r--   0      501       20      347 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F405_F405.py.snap
+-rw-r--r--   0      501       20      308 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F406_F406.py.snap
+-rw-r--r--   0      501       20      196 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F407_F407.py.snap
+-rw-r--r--   0      501       20      419 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F541_F541.py.snap
+-rw-r--r--   0      501       20      425 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F601_F601.py.snap
+-rw-r--r--   0      501       20      182 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F602_F602.py.snap
+-rw-r--r--   0      501       20      167 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F622_F622.py.snap
+-rw-r--r--   0      501       20      266 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F631_F631.py.snap
+-rw-r--r--   0      501       20      262 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F632_F632.py.snap
+-rw-r--r--   0      501       20      164 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F633_F633.py.snap
+-rw-r--r--   0      501       20      256 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F634_F634.py.snap
+-rw-r--r--   0      501       20      504 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F701_F701.py.snap
+-rw-r--r--   0      501       20      519 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F702_F702.py.snap
+-rw-r--r--   0      501       20      402 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F704_F704.py.snap
+-rw-r--r--   0      501       20      285 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F706_F706.py.snap
+-rw-r--r--   0      501       20      402 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F707_F707.py.snap
+-rw-r--r--   0      501       20      185 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F722_F722.py.snap
+-rw-r--r--   0      501       20     1410 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap
+-rw-r--r--   0      501       20      545 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap
+-rw-r--r--   0      501       20      172 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F821_F821_2.py.snap
+-rw-r--r--   0      501       20      168 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F822_F822.py.snap
+-rw-r--r--   0      501       20      173 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F823_F823.py.snap
+-rw-r--r--   0      501       20      407 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F831_F831.py.snap
+-rw-r--r--   0      501       20      645 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F841_F841.py.snap
+-rw-r--r--   0      501       20      284 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__F901_F901.py.snap
+-rw-r--r--   0      501       20      679 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N801_N801.py.snap
+-rw-r--r--   0      501       20      688 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N802_N802.py.snap
+-rw-r--r--   0      501       20      298 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N803_N803.py.snap
+-rw-r--r--   0      501       20      186 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N804_N804.py.snap
+-rw-r--r--   0      501       20      314 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N805_N805.py.snap
+-rw-r--r--   0      501       20      328 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N806_N806.py.snap
+-rw-r--r--   0      501       20      164 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N807_N807.py.snap
+-rw-r--r--   0      501       20      555 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N811_N811.py.snap
+-rw-r--r--   0      501       20      568 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N812_N812.py.snap
+-rw-r--r--   0      501       20      555 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N813_N813.py.snap
+-rw-r--r--   0      501       20      552 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N814_N814.py.snap
+-rw-r--r--   0      501       20      475 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N815_N815.py.snap
+-rw-r--r--   0      501       20      477 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N816_N816.py.snap
+-rw-r--r--   0      501       20      360 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N817_N817.py.snap
+-rw-r--r--   0      501       20      180 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__N818_N818.py.snap
+-rw-r--r--   0      501       20      305 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__T201_T201.py.snap
+-rw-r--r--   0      501       20      562 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__T203_T203.py.snap
+-rw-r--r--   0      501       20      583 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U001_U001.py.snap
+-rw-r--r--   0      501       20      864 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U002_U002.py.snap
+-rw-r--r--   0      501       20     1411 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U003_U003.py.snap
+-rw-r--r--   0      501       20     5675 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U004_U004.py.snap
+-rw-r--r--   0      501       20     1407 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U005_U005.py.snap
+-rw-r--r--   0      501       20      608 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U006_U006.py.snap
+-rw-r--r--   0      501       20     2314 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U007_U007.py.snap
+-rw-r--r--   0      501       20     1442 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__U008_U008.py.snap
+-rw-r--r--   0      501       20      166 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__W292_W292_0.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__W292_W292_1.py.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__W292_W292_2.py.snap
+-rw-r--r--   0      501       20      555 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__W605_W605.py.snap
+-rw-r--r--   0      501       20      894 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap
+-rw-r--r--   0      501       20      503 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__future_annotations.snap
+-rw-r--r--   0      501       20       53 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__init.snap
+-rw-r--r--   0      501       20     2011 2022-11-03 15:48:02.000000 ruff-0.0.99/src/snapshots/ruff__linter__tests__m001.snap
+-rw-r--r--   0      501       20     3960 2022-11-03 15:48:02.000000 ruff-0.0.99/src/source_code_locator.rs
+-rw-r--r--   0      501       20     5340 2022-11-03 15:48:02.000000 ruff-0.0.99/src/visibility.rs
+-rw-r--r--   0      501       20     2220 2022-11-03 15:48:02.000000 ruff-0.0.99/tests/integration_test.rs
+-rw-r--r--   0      501       20    82250 2022-11-03 15:48:01.000000 ruff-0.0.99/Cargo.lock
+-rw-r--r--   0        0        0    36363 1970-01-01 00:00:00.000000 ruff-0.0.99/PKG-INFO
```

### Comparing `ruff-0.0.98/Cargo.toml` & `ruff-0.0.99/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [workspace]
 members = [
     "flake8_to_ruff",
 ]
 
 [package]
 name = "ruff"
-version = "0.0.98"
+version = "0.0.99"
 edition = "2021"
 
 [lib]
 name = "ruff"
 
 [dependencies]
 anyhow = { version = "1.0.60" }
```

### Comparing `ruff-0.0.98/.github/workflows/ci.yaml` & `ruff-0.0.99/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/.github/workflows/flake8-to-ruff.yaml` & `ruff-0.0.99/.github/workflows/flake8-to-ruff.yaml`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/.github/workflows/ruff.yaml` & `ruff-0.0.99/.github/workflows/ruff.yaml`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/.gitignore` & `ruff-0.0.99/.gitignore`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/CODE_OF_CONDUCT.md` & `ruff-0.0.99/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/CONTRIBUTING.md` & `ruff-0.0.99/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/Cargo.lock` & `ruff-0.0.99/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -916,15 +916,15 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flake8-to-ruff"
-version = "0.0.98-dev.0"
+version = "0.0.99-dev.0"
 dependencies = [
  "anyhow",
  "clap 4.0.15",
  "configparser",
  "once_cell",
  "regex",
  "ruff",
@@ -2207,15 +2207,15 @@
  "untrusted",
  "web-sys",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.98"
+version = "0.0.99"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "bincode",
  "cacache",
  "chrono",
  "clap 4.0.15",
```

### Comparing `ruff-0.0.98/LICENSE` & `ruff-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/README.md` & `ruff-0.0.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 ```
 
 Ruff also works with [pre-commit](https://pre-commit.com):
 
 ```yaml
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.98
+    rev: v0.0.99
     hooks:
       - id: ruff
 ```
 
 <!-- TODO(charlie): Remove this message a few versions after v0.0.86. -->
 _Note: prior to `v0.0.86`, `ruff-pre-commit` used `lint` (rather than `ruff`) as the hook ID._
 
@@ -441,23 +441,23 @@
 | ---- | ---- | ------- | --- |
 | C400 | UnnecessaryGeneratorList | Unnecessary generator (rewrite as a `list` comprehension) | 🛠 |
 | C401 | UnnecessaryGeneratorSet | Unnecessary generator (rewrite as a `set` comprehension) | 🛠 |
 | C402 | UnnecessaryGeneratorDict | Unnecessary generator (rewrite as a `dict` comprehension) | 🛠 |
 | C403 | UnnecessaryListComprehensionSet | Unnecessary `list` comprehension (rewrite as a `set` comprehension) | 🛠 |
 | C404 | UnnecessaryListComprehensionDict | Unnecessary `list` comprehension (rewrite as a `dict` comprehension) |  |
 | C405 | UnnecessaryLiteralSet | Unnecessary `(list\|tuple)` literal (rewrite as a `set` literal) | 🛠 |
-| C406 | UnnecessaryLiteralDict | Unnecessary `(list\|tuple)` literal (rewrite as a `dict` literal) |  |
+| C406 | UnnecessaryLiteralDict | Unnecessary `(list\|tuple)` literal (rewrite as a `dict` literal) | 🛠 |
 | C408 | UnnecessaryCollectionCall | Unnecessary `(dict\|list\|tuple)` call (rewrite as a literal) | 🛠 |
 | C409 | UnnecessaryLiteralWithinTupleCall | Unnecessary `(list\|tuple)` literal passed to `tuple()` (remove the outer call to `tuple()`) | 🛠 |
 | C410 | UnnecessaryLiteralWithinListCall | Unnecessary `(list\|tuple)` literal passed to `list()` (rewrite as a `list` literal) | 🛠 |
 | C411 | UnnecessaryListCall | Unnecessary `list` call (remove the outer call to `list()`) | 🛠 |
 | C413 | UnnecessaryCallAroundSorted | Unnecessary `(list\|reversed)` call around `sorted()` |  |
 | C414 | UnnecessaryDoubleCastOrProcess | Unnecessary `(list\|reversed\|set\|sorted\|tuple)` call within `(list\|set\|sorted\|tuple)()` |  |
 | C415 | UnnecessarySubscriptReversal | Unnecessary subscript reversal of iterable within `(reversed\|set\|sorted)()` |  |
-| C416 | UnnecessaryComprehension | Unnecessary `(list\|set)` comprehension (rewrite using `(list\|set)()`) |  |
+| C416 | UnnecessaryComprehension | Unnecessary `(list\|set)` comprehension (rewrite using `(list\|set)()`) | 🛠 |
 | C417 | UnnecessaryMap | Unnecessary `map` usage (rewrite using a `(list\|set\|dict)` comprehension) |  |
 
 ### flake8-bugbear
 
 | Code | Name | Message | Fix |
 | ---- | ---- | ------- | --- |
 | B002 | UnaryPrefixIncrement | Python does not support the unary prefix increment. |  |
```

### Comparing `ruff-0.0.98/examples/generate_check_code_prefix.rs` & `ruff-0.0.99/examples/generate_check_code_prefix.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/examples/generate_rules_table.rs` & `ruff-0.0.99/examples/generate_rules_table.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/examples/generate_source_code.rs` & `ruff-0.0.99/examples/generate_source_code.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/pyproject.toml` & `ruff-0.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/B006_B008.py` & `ruff-0.0.99/resources/test/fixtures/B006_B008.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/B007.py` & `ruff-0.0.99/resources/test/fixtures/B007.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/B014.py` & `ruff-0.0.99/resources/test/fixtures/B014.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/B017.py` & `ruff-0.0.99/resources/test/fixtures/B017.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/D.py` & `ruff-0.0.99/resources/test/fixtures/D.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/E501.py` & `ruff-0.0.99/resources/test/fixtures/E501.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/E711.py` & `ruff-0.0.99/resources/test/fixtures/E711.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/E712.py` & `ruff-0.0.99/resources/test/fixtures/E712.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/E713.py` & `ruff-0.0.99/resources/test/fixtures/E713.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/E721.py` & `ruff-0.0.99/resources/test/fixtures/E721.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/E741.py` & `ruff-0.0.99/resources/test/fixtures/E741.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/F401_0.py` & `ruff-0.0.99/resources/test/fixtures/F401_0.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/F821_0.py` & `ruff-0.0.99/resources/test/fixtures/F821_0.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/M001.py` & `ruff-0.0.99/resources/test/fixtures/M001.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/U004.py` & `ruff-0.0.99/resources/test/fixtures/U004.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/U008.py` & `ruff-0.0.99/resources/test/fixtures/U008.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/canonical_google_examples.py` & `ruff-0.0.99/resources/test/fixtures/canonical_google_examples.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/canonical_numpy_examples.py` & `ruff-0.0.99/resources/test/fixtures/canonical_numpy_examples.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_doubles.py` & `ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_doubles.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/flake8_quotes/docstring_singles.py` & `ruff-0.0.99/resources/test/fixtures/flake8_quotes/docstring_singles.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/pyproject.toml` & `ruff-0.0.99/resources/test/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/resources/test/fixtures/sections.py` & `ruff-0.0.99/resources/test/fixtures/sections.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/scripts/poetry.lock` & `ruff-0.0.99/scripts/poetry.lock`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/scripts/run_flake8.py` & `ruff-0.0.99/scripts/run_flake8.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/setup.py` & `ruff-0.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/ast/helpers.rs` & `ruff-0.0.99/src/ast/helpers.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/ast/operations.rs` & `ruff-0.0.99/src/ast/operations.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/ast/relocate.rs` & `ruff-0.0.99/src/ast/relocate.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/ast/types.rs` & `ruff-0.0.99/src/ast/types.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/ast/visitor.rs` & `ruff-0.0.99/src/ast/visitor.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/autofix/fixer.rs` & `ruff-0.0.99/src/autofix/fixer.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/autofix/helpers.rs` & `ruff-0.0.99/src/autofix/helpers.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/autofix/mod.rs` & `ruff-0.0.99/src/autofix/mod.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/cache.rs` & `ruff-0.0.99/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/check_ast.rs` & `ruff-0.0.99/src/check_ast.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1072,17 +1072,20 @@
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C406) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_literal_dict(
+                        expr,
                         func,
                         args,
                         keywords,
+                        self.locator,
+                        self.patch(),
                         self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C408) {
@@ -1359,14 +1362,16 @@
 
             ExprKind::ListComp { elt, generators } | ExprKind::SetComp { elt, generators } => {
                 if self.settings.enabled.contains(&CheckCode::C416) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_comprehension(
                         expr,
                         elt,
                         generators,
+                        self.locator,
+                        self.patch(),
                         self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
                 self.push_scope(Scope::new(ScopeKind::Generator))
             }
```

### Comparing `ruff-0.0.98/src/check_lines.rs` & `ruff-0.0.99/src/check_lines.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/check_tokens.rs` & `ruff-0.0.99/src/check_tokens.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/checks.rs` & `ruff-0.0.99/src/checks.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1466,19 +1466,21 @@
                 | CheckKind::SectionUnderlineAfterName(_)
                 | CheckKind::SectionUnderlineMatchesSectionLength(_)
                 | CheckKind::SectionUnderlineNotOverIndented(_)
                 | CheckKind::SuperCallWithParameters
                 | CheckKind::TypeOfPrimitive(_)
                 | CheckKind::UnnecessaryAbspath
                 | CheckKind::UnnecessaryCollectionCall(_)
+                | CheckKind::UnnecessaryComprehension(_)
                 | CheckKind::UnnecessaryGeneratorDict
                 | CheckKind::UnnecessaryGeneratorList
                 | CheckKind::UnnecessaryGeneratorSet
                 | CheckKind::UnnecessaryListCall
                 | CheckKind::UnnecessaryListComprehensionSet
+                | CheckKind::UnnecessaryLiteralDict(_)
                 | CheckKind::UnnecessaryLiteralSet(_)
                 | CheckKind::UnnecessaryLiteralWithinListCall(_)
                 | CheckKind::UnnecessaryLiteralWithinTupleCall(_)
                 | CheckKind::UnusedImport(_, false)
                 | CheckKind::UnusedLoopControlVariable(_)
                 | CheckKind::UnusedNOQA(_)
                 | CheckKind::UsePEP585Annotation(_)
```

### Comparing `ruff-0.0.98/src/checks_gen.rs` & `ruff-0.0.99/src/checks_gen.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/cli.rs` & `ruff-0.0.99/src/cli.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/code_gen.rs` & `ruff-0.0.99/src/code_gen.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/cst/helpers.rs` & `ruff-0.0.99/src/cst/helpers.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/cst/matchers.rs` & `ruff-0.0.99/src/cst/matchers.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/docstrings/extraction.rs` & `ruff-0.0.99/src/docstrings/extraction.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/docstrings/google.rs` & `ruff-0.0.99/src/docstrings/google.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/docstrings/helpers.rs` & `ruff-0.0.99/src/docstrings/helpers.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/docstrings/numpy.rs` & `ruff-0.0.99/src/docstrings/numpy.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/docstrings/sections.rs` & `ruff-0.0.99/src/docstrings/sections.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/docstrings/styles.rs` & `ruff-0.0.99/src/docstrings/styles.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/assert_false.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/assert_false.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/assert_raises_exception.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/assert_raises_exception.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/duplicate_exceptions.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/duplicate_exceptions.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/mod.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/mod.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/mutable_argument_default.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/mutable_argument_default.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/unary_prefix_increment.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/unary_prefix_increment.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_bugbear/plugins/unused_loop_control_variable.rs` & `ruff-0.0.99/src/flake8_bugbear/plugins/unused_loop_control_variable.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_builtins/checks.rs` & `ruff-0.0.99/src/flake8_builtins/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_comprehensions/checks.rs` & `ruff-0.0.99/src/flake8_comprehensions/checks.rs`

 * *Files 5% similar despite different names*

```diff
@@ -193,37 +193,46 @@
         }
     }
     Some(check)
 }
 
 /// C406 (`dict([(1, 2)])`)
 pub fn unnecessary_literal_dict(
+    expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
     location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("dict", func, args, keywords)?;
     let (kind, elts) = match argument {
         ExprKind::Tuple { elts, .. } => ("tuple", elts),
         ExprKind::List { elts, .. } => ("list", elts),
         _ => return None,
     };
-
-    if let Some(elt) = elts.first() {
-        // dict((1, 2), ...)) or dict([(1, 2), ...])
-        if !matches!(&elt.node, ExprKind::Tuple { elts, .. } if elts.len() == 2) {
-            return None;
-        }
+    // Accept `dict((1, 2), ...))` `dict([(1, 2), ...])`.
+    if !elts
+        .iter()
+        .all(|elt| matches!(&elt.node, ExprKind::Tuple { elts, .. } if elts.len() == 2))
+    {
+        return None;
     }
-
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryLiteralDict(kind.to_string()),
         location,
-    ))
+    );
+    if fix {
+        match fixes::fix_unnecessary_literal_dict(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C408
 pub fn unnecessary_collection_call(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
@@ -246,20 +255,17 @@
         _ => return None,
     };
     let mut check = Check::new(
         CheckKind::UnnecessaryCollectionCall(id.to_string()),
         location,
     );
     if fix {
-        // TODO(charlie): Support fixing `dict(a=1)`.
-        if keywords.is_empty() {
-            match fixes::fix_unnecessary_collection_call(locator, expr) {
-                Ok(fix) => check.amend(fix),
-                Err(e) => error!("Failed to generate fix: {}", e),
-            }
+        match fixes::fix_unnecessary_collection_call(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
         }
     }
     Some(check)
 }
 
 /// C409
 pub fn unnecessary_literal_within_tuple_call(
@@ -442,14 +448,16 @@
 }
 
 /// C416
 pub fn unnecessary_comprehension(
     expr: &Expr,
     elt: &Expr,
     generators: &[Comprehension],
+    locator: &SourceCodeLocator,
+    fix: bool,
     location: Range,
 ) -> Option<Check> {
     if generators.len() != 1 {
         return None;
     }
     let generator = &generators[0];
     if !(generator.ifs.is_empty() && generator.is_async == 0) {
@@ -461,18 +469,25 @@
         return None;
     }
     let expr_kind = match &expr.node {
         ExprKind::ListComp { .. } => "list",
         ExprKind::SetComp { .. } => "set",
         _ => return None,
     };
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryComprehension(expr_kind.to_string()),
         location,
-    ))
+    );
+    if fix {
+        match fixes::fix_unnecessary_comprehension(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C417
 pub fn unnecessary_map(func: &Expr, args: &[Expr], location: Range) -> Option<Check> {
     fn new_check(kind: &str, location: Range) -> Check {
         Check::new(CheckKind::UnnecessaryMap(kind.to_string()), location)
     }
```

### Comparing `ruff-0.0.98/src/flake8_comprehensions/fixes.rs` & `ruff-0.0.99/src/flake8_comprehensions/fixes.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 use anyhow::Result;
 use libcst_native::{
-    Arg, Call, Codegen, Dict, DictComp, Element, Expr, Expression, LeftCurlyBrace, LeftParen,
-    LeftSquareBracket, List, ListComp, Module, ParenthesizableWhitespace, RightCurlyBrace,
-    RightParen, RightSquareBracket, Set, SetComp, SimpleWhitespace, SmallStatement, Statement,
-    Tuple,
+    Arg, Call, Codegen, Dict, DictComp, DictElement, Element, Expr, Expression, LeftCurlyBrace,
+    LeftParen, LeftSquareBracket, List, ListComp, Module, Name, ParenthesizableWhitespace,
+    RightCurlyBrace, RightParen, RightSquareBracket, Set, SetComp, SimpleString, SimpleWhitespace,
+    SmallStatement, Statement, Tuple,
 };
 
 use crate::autofix::Fix;
 use crate::cst::matchers::match_tree;
 use crate::source_code_locator::SourceCodeLocator;
 
 fn match_expr<'a, 'b>(module: &'a mut Module<'b>) -> Result<&'a mut Expr<'b>> {
     if let Some(Statement::Simple(expr)) = module.body.first_mut() {
         if let Some(SmallStatement::Expr(expr)) = expr.body.first_mut() {
             Ok(expr)
         } else {
-            Err(anyhow::anyhow!(
-                "Expected node to be: SmallStatement::Expr."
-            ))
+            Err(anyhow::anyhow!("Expected node to be: SmallStatement::Expr"))
         }
     } else {
-        Err(anyhow::anyhow!("Expected node to be: Statement::Simple."))
+        Err(anyhow::anyhow!("Expected node to be: Statement::Simple"))
     }
 }
 
 fn match_call<'a, 'b>(expr: &'a mut Expr<'b>) -> Result<&'a mut Call<'b>> {
     if let Expression::Call(call) = &mut expr.value {
         Ok(call)
     } else {
-        Err(anyhow::anyhow!("Expected node to be: Expression::Call."))
+        Err(anyhow::anyhow!("Expected node to be: Expression::Call"))
     }
 }
 
 fn match_arg<'a, 'b>(call: &'a Call<'b>) -> Result<&'a Arg<'b>> {
     if let Some(arg) = call.args.first() {
         Ok(arg)
     } else {
-        Err(anyhow::anyhow!("Expected node to be: Arg."))
+        Err(anyhow::anyhow!("Expected node to be: Arg"))
     }
 }
 
 /// (C400) Convert `list(x for x in y)` to `[x for x in y]`.
 pub fn fix_unnecessary_generator_list(
     locator: &SourceCodeLocator,
     expr: &rustpython_ast::Expr,
@@ -51,15 +49,15 @@
     let call = match_call(body)?;
     let arg = match_arg(call)?;
 
     let generator_exp = if let Expression::GeneratorExp(generator_exp) = &arg.value {
         generator_exp
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: Expression::GeneratorExp."
+            "Expected node to be: Expression::GeneratorExp"
         ));
     };
 
     body.value = Expression::ListComp(Box::new(ListComp {
         elt: generator_exp.elt.clone(),
         for_in: generator_exp.for_in.clone(),
         lbracket: LeftSquareBracket {
@@ -93,15 +91,15 @@
     let call = match_call(body)?;
     let arg = match_arg(call)?;
 
     let generator_exp = if let Expression::GeneratorExp(generator_exp) = &arg.value {
         generator_exp
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: Expression::GeneratorExp."
+            "Expected node to be: Expression::GeneratorExp"
         ));
     };
 
     body.value = Expression::SetComp(Box::new(SetComp {
         elt: generator_exp.elt.clone(),
         for_in: generator_exp.for_in.clone(),
         lbrace: LeftCurlyBrace {
@@ -136,34 +134,34 @@
     let arg = match_arg(call)?;
 
     // Extract the (k, v) from `(k, v) for ...`.
     let generator_exp = if let Expression::GeneratorExp(generator_exp) = &arg.value {
         generator_exp
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: Expression::GeneratorExp."
+            "Expected node to be: Expression::GeneratorExp"
         ));
     };
     let tuple = if let Expression::Tuple(tuple) = &generator_exp.elt.as_ref() {
         tuple
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Expression::Tuple."));
+        return Err(anyhow::anyhow!("Expected node to be: Expression::Tuple"));
     };
     let key = if let Some(Element::Simple { value, .. }) = &tuple.elements.get(0) {
         value
     } else {
         return Err(anyhow::anyhow!(
-            "Expected tuple to contain a key as the first element."
+            "Expected tuple to contain a key as the first element"
         ));
     };
     let value = if let Some(Element::Simple { value, .. }) = &tuple.elements.get(1) {
         value
     } else {
         return Err(anyhow::anyhow!(
-            "Expected tuple to contain a key as the second element."
+            "Expected tuple to contain a key as the second element"
         ));
     };
 
     body.value = Expression::DictComp(Box::new(DictComp {
         key: Box::new(key.clone()),
         value: Box::new(value.clone()),
         for_in: generator_exp.for_in.clone(),
@@ -200,17 +198,15 @@
     let mut body = match_expr(&mut tree)?;
     let call = match_call(body)?;
     let arg = match_arg(call)?;
 
     let list_comp = if let Expression::ListComp(list_comp) = &arg.value {
         list_comp
     } else {
-        return Err(anyhow::anyhow!(
-            "Expected node to be: Expression::ListComp."
-        ));
+        return Err(anyhow::anyhow!("Expected node to be: Expression::ListComp"));
     };
 
     body.value = Expression::SetComp(Box::new(SetComp {
         elt: list_comp.elt.clone(),
         for_in: list_comp.for_in.clone(),
         lbrace: LeftCurlyBrace {
             whitespace_after: call.whitespace_before_args.clone(),
@@ -244,15 +240,15 @@
     let arg = match_arg(call)?;
 
     let elements = match &arg.value {
         Expression::Tuple(inner) => &inner.elements,
         Expression::List(inner) => &inner.elements,
         _ => {
             return Err(anyhow::anyhow!(
-                "Expected node to be: Expression::Tuple | Expression::List."
+                "Expected node to be: Expression::Tuple | Expression::List"
             ))
         }
     };
 
     if elements.is_empty() {
         call.args = vec![];
     } else {
@@ -275,29 +271,104 @@
     Ok(Fix::replacement(
         state.to_string(),
         expr.location,
         expr.end_location.unwrap(),
     ))
 }
 
+/// (C406) Convert `dict([(1, 2)])` to `{1: 2}`.
+pub fn fix_unnecessary_literal_dict(
+    locator: &SourceCodeLocator,
+    expr: &rustpython_ast::Expr,
+) -> Result<Fix> {
+    // Expr(Call(List|Tuple)))) -> Expr(Dict)))
+    let mut tree = match_tree(locator, expr)?;
+    let mut body = match_expr(&mut tree)?;
+    let call = match_call(body)?;
+    let arg = match_arg(call)?;
+
+    let elements = match &arg.value {
+        Expression::Tuple(inner) => &inner.elements,
+        Expression::List(inner) => &inner.elements,
+        _ => {
+            return Err(anyhow::anyhow!(
+                "Expected node to be: Expression::Tuple | Expression::List"
+            ))
+        }
+    };
+
+    let elements: Vec<DictElement> = elements
+        .iter()
+        .map(|element| {
+            if let Element::Simple {
+                value: Expression::Tuple(tuple),
+                comma,
+            } = element
+            {
+                if let Some(Element::Simple { value: key, .. }) = tuple.elements.get(0) {
+                    if let Some(Element::Simple { value, .. }) = tuple.elements.get(1) {
+                        return Ok(DictElement::Simple {
+                            key: key.clone(),
+                            value: value.clone(),
+                            comma: comma.clone(),
+                            whitespace_before_colon: Default::default(),
+                            whitespace_after_colon: ParenthesizableWhitespace::SimpleWhitespace(
+                                SimpleWhitespace(" "),
+                            ),
+                        });
+                    }
+                }
+            }
+            Err(anyhow::anyhow!(
+                "Expected each argument to be a tuple of length two"
+            ))
+        })
+        .collect::<Result<Vec<DictElement>>>()?;
+
+    body.value = Expression::Dict(Box::new(Dict {
+        elements,
+        lbrace: LeftCurlyBrace {
+            whitespace_after: call.whitespace_before_args.clone(),
+        },
+        rbrace: RightCurlyBrace {
+            whitespace_before: arg.whitespace_after_arg.clone(),
+        },
+        lpar: Default::default(),
+        rpar: Default::default(),
+    }));
+
+    let mut state = Default::default();
+    tree.codegen(&mut state);
+
+    Ok(Fix::replacement(
+        state.to_string(),
+        expr.location,
+        expr.end_location.unwrap(),
+    ))
+}
+
 /// (C408)
 pub fn fix_unnecessary_collection_call(
     locator: &SourceCodeLocator,
     expr: &rustpython_ast::Expr,
 ) -> Result<Fix> {
     // Expr(Call("list" | "tuple" | "dict")))) -> Expr(List|Tuple|Dict)))
     let mut tree = match_tree(locator, expr)?;
     let mut body = match_expr(&mut tree)?;
     let call = match_call(body)?;
     let name = if let Expression::Name(name) = &call.func.as_ref() {
         name
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Expression::Name."));
+        return Err(anyhow::anyhow!("Expected node to be: Expression::Name"));
     };
 
+    // Arena allocator used to create formatted strings of sufficient lifetime,
+    // below.
+    let mut arena: Vec<String> = vec![];
+
     match name.value {
         "tuple" => {
             body.value = Expression::Tuple(Box::new(Tuple {
                 elements: Default::default(),
                 lpar: vec![Default::default()],
                 rpar: vec![Default::default()],
             }));
@@ -308,25 +379,75 @@
                 lbracket: Default::default(),
                 rbracket: Default::default(),
                 lpar: Default::default(),
                 rpar: Default::default(),
             }));
         }
         "dict" => {
-            body.value = Expression::Dict(Box::new(Dict {
-                elements: Default::default(),
-                lbrace: Default::default(),
-                rbrace: Default::default(),
-                lpar: Default::default(),
-                rpar: Default::default(),
-            }));
+            if call.args.is_empty() {
+                body.value = Expression::Dict(Box::new(Dict {
+                    elements: Default::default(),
+                    lbrace: Default::default(),
+                    rbrace: Default::default(),
+                    lpar: Default::default(),
+                    rpar: Default::default(),
+                }));
+            } else {
+                // Quote each argument.
+                for arg in &call.args {
+                    let quoted = format!(
+                        "\"{}\"",
+                        arg.keyword
+                            .as_ref()
+                            .expect("Expected dictionary argument to be kwarg")
+                            .value
+                    );
+                    arena.push(quoted);
+                }
+
+                let elements = call
+                    .args
+                    .iter()
+                    .enumerate()
+                    .map(|(i, arg)| DictElement::Simple {
+                        key: Expression::SimpleString(Box::new(SimpleString {
+                            value: &arena[i],
+                            lpar: Default::default(),
+                            rpar: Default::default(),
+                        })),
+                        value: arg.value.clone(),
+                        comma: arg.comma.clone(),
+                        whitespace_before_colon: Default::default(),
+                        whitespace_after_colon: ParenthesizableWhitespace::SimpleWhitespace(
+                            SimpleWhitespace(" "),
+                        ),
+                    })
+                    .collect();
+
+                body.value = Expression::Dict(Box::new(Dict {
+                    elements,
+                    lbrace: LeftCurlyBrace {
+                        whitespace_after: call.whitespace_before_args.clone(),
+                    },
+                    rbrace: RightCurlyBrace {
+                        whitespace_before: call
+                            .args
+                            .last()
+                            .expect("Arguments should be non-empty")
+                            .whitespace_after_arg
+                            .clone(),
+                    },
+                    lpar: Default::default(),
+                    rpar: Default::default(),
+                }));
+            }
         }
         _ => {
             return Err(anyhow::anyhow!("Expected function name to be one of: \
-                                        'tuple', 'list', 'dict'."
+                                        'tuple', 'list', 'dict'"
                 .to_string()));
         }
     };
 
     let mut state = Default::default();
     tree.codegen(&mut state);
 
@@ -348,30 +469,30 @@
     let arg = match_arg(call)?;
     let (elements, whitespace_after, whitespace_before) = match &arg.value {
         Expression::Tuple(inner) => (
             &inner.elements,
             &inner
                 .lpar
                 .first()
-                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses."))?
+                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses"))?
                 .whitespace_after,
             &inner
                 .rpar
                 .first()
-                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses."))?
+                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses"))?
                 .whitespace_before,
         ),
         Expression::List(inner) => (
             &inner.elements,
             &inner.lbracket.whitespace_after,
             &inner.rbracket.whitespace_before,
         ),
         _ => {
             return Err(anyhow::anyhow!(
-                "Expected node to be: Expression::Tuple | Expression::List."
+                "Expected node to be: Expression::Tuple | Expression::List"
             ))
         }
     };
 
     body.value = Expression::Tuple(Box::new(Tuple {
         elements: elements.clone(),
         lpar: vec![LeftParen {
@@ -403,30 +524,30 @@
     let arg = match_arg(call)?;
     let (elements, whitespace_after, whitespace_before) = match &arg.value {
         Expression::Tuple(inner) => (
             &inner.elements,
             &inner
                 .lpar
                 .first()
-                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses."))?
+                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses"))?
                 .whitespace_after,
             &inner
                 .rpar
                 .first()
-                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses."))?
+                .ok_or_else(|| anyhow::anyhow!("Expected at least one set of parentheses"))?
                 .whitespace_before,
         ),
         Expression::List(inner) => (
             &inner.elements,
             &inner.lbracket.whitespace_after,
             &inner.rbracket.whitespace_before,
         ),
         _ => {
             return Err(anyhow::anyhow!(
-                "Expected node to be: Expression::Tuple | Expression::List."
+                "Expected node to be: Expression::Tuple | Expression::List"
             ))
         }
     };
 
     body.value = Expression::List(Box::new(List {
         elements: elements.clone(),
         lbracket: LeftSquareBracket {
@@ -445,15 +566,15 @@
     Ok(Fix::replacement(
         state.to_string(),
         expr.location,
         expr.end_location.unwrap(),
     ))
 }
 
-/// (C411) Convert `list([i for i in x])` to `[i for i in x]`.
+/// (C411) Convert `list([i * i for i in x])` to `[i * i for i in x]`.
 pub fn fix_unnecessary_list_call(
     locator: &SourceCodeLocator,
     expr: &rustpython_ast::Expr,
 ) -> Result<Fix> {
     // Expr(Call(List|Tuple)))) -> Expr(List|Tuple)))
     let mut tree = match_tree(locator, expr)?;
     let mut body = match_expr(&mut tree)?;
@@ -464,10 +585,80 @@
 
     let mut state = Default::default();
     tree.codegen(&mut state);
 
     Ok(Fix::replacement(
         state.to_string(),
         expr.location,
+        expr.end_location.unwrap(),
+    ))
+}
+
+/// (C416) Convert `[i for i in x]` to `list(x)`.
+pub fn fix_unnecessary_comprehension(
+    locator: &SourceCodeLocator,
+    expr: &rustpython_ast::Expr,
+) -> Result<Fix> {
+    let mut tree = match_tree(locator, expr)?;
+    let mut body = match_expr(&mut tree)?;
+
+    match &body.value {
+        Expression::ListComp(inner) => {
+            body.value = Expression::Call(Box::new(Call {
+                func: Box::new(Expression::Name(Box::new(Name {
+                    value: "list",
+                    lpar: Default::default(),
+                    rpar: Default::default(),
+                }))),
+                args: vec![Arg {
+                    value: inner.for_in.iter.clone(),
+                    keyword: Default::default(),
+                    equal: Default::default(),
+                    comma: Default::default(),
+                    star: Default::default(),
+                    whitespace_after_star: Default::default(),
+                    whitespace_after_arg: Default::default(),
+                }],
+                lpar: Default::default(),
+                rpar: Default::default(),
+                whitespace_after_func: Default::default(),
+                whitespace_before_args: Default::default(),
+            }))
+        }
+        Expression::SetComp(inner) => {
+            body.value = Expression::Call(Box::new(Call {
+                func: Box::new(Expression::Name(Box::new(Name {
+                    value: "set",
+                    lpar: Default::default(),
+                    rpar: Default::default(),
+                }))),
+                args: vec![Arg {
+                    value: inner.for_in.iter.clone(),
+                    keyword: Default::default(),
+                    equal: Default::default(),
+                    comma: Default::default(),
+                    star: Default::default(),
+                    whitespace_after_star: Default::default(),
+                    whitespace_after_arg: Default::default(),
+                }],
+                lpar: Default::default(),
+                rpar: Default::default(),
+                whitespace_after_func: Default::default(),
+                whitespace_before_args: Default::default(),
+            }))
+        }
+        _ => {
+            return Err(anyhow::anyhow!(
+                "Expected node to be: Expression::ListComp | Expression:SetComp"
+            ))
+        }
+    }
+
+    let mut state = Default::default();
+    tree.codegen(&mut state);
+
+    Ok(Fix::replacement(
+        state.to_string(),
+        expr.location,
         expr.end_location.unwrap(),
     ))
 }
```

### Comparing `ruff-0.0.98/src/flake8_print/checks.rs` & `ruff-0.0.99/src/flake8_print/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_print/plugins/print_call.rs` & `ruff-0.0.99/src/flake8_print/plugins/print_call.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/checks.rs` & `ruff-0.0.99/src/flake8_quotes/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/docstring_detection.rs` & `ruff-0.0.99/src/flake8_quotes/docstring_detection.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/settings.rs` & `ruff-0.0.99/src/flake8_quotes/settings.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap` & `ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap` & `ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap` & `ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap` & `ruff-0.0.99/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/fs.rs` & `ruff-0.0.99/src/fs.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/lib.rs` & `ruff-0.0.99/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/linter.rs` & `ruff-0.0.99/src/linter.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/logging.rs` & `ruff-0.0.99/src/logging.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/main.rs` & `ruff-0.0.99/src/main.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/message.rs` & `ruff-0.0.99/src/message.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/noqa.rs` & `ruff-0.0.99/src/noqa.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pep8_naming/checks.rs` & `ruff-0.0.99/src/pep8_naming/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pep8_naming/settings.rs` & `ruff-0.0.99/src/pep8_naming/settings.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/printer.rs` & `ruff-0.0.99/src/printer.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pycodestyle/checks.rs` & `ruff-0.0.99/src/pycodestyle/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pydocstyle/plugins.rs` & `ruff-0.0.99/src/pydocstyle/plugins.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyflakes/checks.rs` & `ruff-0.0.99/src/pyflakes/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyflakes/fixes.rs` & `ruff-0.0.99/src/pyflakes/fixes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     deleted: &[&Stmt],
 ) -> Result<Fix> {
     let mut tree = match_tree(locator, stmt)?;
 
     let body = if let Some(Statement::Simple(body)) = tree.body.first_mut() {
         body
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple."));
+        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple"));
     };
     let body = if let Some(SmallStatement::Import(body)) = body.body.first_mut() {
         body
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: SmallStatement::ImportFrom."
+            "Expected node to be: SmallStatement::ImportFrom"
         ));
     };
     let aliases = &mut body.names;
 
     // Preserve the trailing comma (or not) from the last entry.
     let trailing_comma = aliases.last().and_then(|alias| alias.comma.clone());
 
@@ -73,28 +73,28 @@
     deleted: &[&Stmt],
 ) -> Result<Fix> {
     let mut tree = match_tree(locator, stmt)?;
 
     let body = if let Some(Statement::Simple(body)) = tree.body.first_mut() {
         body
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple."));
+        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple"));
     };
     let body = if let Some(SmallStatement::ImportFrom(body)) = body.body.first_mut() {
         body
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: SmallStatement::ImportFrom."
+            "Expected node to be: SmallStatement::ImportFrom"
         ));
     };
 
     let aliases = if let ImportNames::Aliases(aliases) = &mut body.names {
         aliases
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Aliases."));
+        return Err(anyhow::anyhow!("Expected node to be: Aliases"));
     };
 
     // Preserve the trailing comma (or not) from the last entry.
     let trailing_comma = aliases.last().and_then(|alias| alias.comma.clone());
 
     // Identify unused imports from within the `import from`.
     let mut removable = vec![];
```

### Comparing `ruff-0.0.98/src/pyflakes/plugins/invalid_print_syntax.rs` & `ruff-0.0.99/src/pyflakes/plugins/invalid_print_syntax.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/python/builtins.rs` & `ruff-0.0.99/src/python/builtins.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/python/typing.rs` & `ruff-0.0.99/src/python/typing.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/checks.rs` & `ruff-0.0.99/src/pyupgrade/checks.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/fixes.rs` & `ruff-0.0.99/src/pyupgrade/fixes.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/deprecated_unittest_alias.rs` & `ruff-0.0.99/src/pyupgrade/plugins/deprecated_unittest_alias.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/mod.rs` & `ruff-0.0.99/src/pyupgrade/plugins/mod.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/super_call_with_parameters.rs` & `ruff-0.0.99/src/pyupgrade/plugins/super_call_with_parameters.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/type_of_primitive.rs` & `ruff-0.0.99/src/pyupgrade/plugins/type_of_primitive.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/unnecessary_abspath.rs` & `ruff-0.0.99/src/pyupgrade/plugins/unnecessary_abspath.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/use_pep585_annotation.rs` & `ruff-0.0.99/src/pyupgrade/plugins/use_pep585_annotation.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/use_pep604_annotation.rs` & `ruff-0.0.99/src/pyupgrade/plugins/use_pep604_annotation.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/useless_metaclass_type.rs` & `ruff-0.0.99/src/pyupgrade/plugins/useless_metaclass_type.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/plugins/useless_object_inheritance.rs` & `ruff-0.0.99/src/pyupgrade/plugins/useless_object_inheritance.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/pyupgrade/types.rs` & `ruff-0.0.99/src/pyupgrade/types.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/settings/configuration.rs` & `ruff-0.0.99/src/settings/configuration.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/settings/mod.rs` & `ruff-0.0.99/src/settings/mod.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/settings/options.rs` & `ruff-0.0.99/src/settings/options.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/settings/pyproject.rs` & `ruff-0.0.99/src/settings/pyproject.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/settings/types.rs` & `ruff-0.0.99/src/settings/types.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/settings/user.rs` & `ruff-0.0.99/src/settings/user.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__A001_A001.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__A001_A001.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__A002_A002.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__A002_A002.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__B007_B007.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__B007_B007.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__B011_B011.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__B011_B011.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__B014_B014.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__B014_B014.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__B025_B025.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__B025_B025.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C400_C400.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C400_C400.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C401_C401.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C401_C401.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C402_C402.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C402_C402.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C403_C403.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C403_C403.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C405_C405.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C405_C405.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C406_C406.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__F841_F841.py.snap`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
 - kind:
-    UnnecessaryLiteralDict: list
+    UnusedVariable: e
   location:
-    row: 1
-    column: 5
+    row: 3
+    column: 0
   end_location:
-    row: 1
-    column: 19
+    row: 7
+    column: 0
   fix: ~
 - kind:
-    UnnecessaryLiteralDict: tuple
+    UnusedVariable: z
   location:
-    row: 2
+    row: 16
+    column: 4
+  end_location:
+    row: 16
     column: 5
+  fix: ~
+- kind:
+    UnusedVariable: foo
+  location:
+    row: 20
+    column: 4
   end_location:
-    row: 2
-    column: 20
+    row: 20
+    column: 7
   fix: ~
 - kind:
-    UnnecessaryLiteralDict: list
+    UnusedVariable: a
   location:
-    row: 3
+    row: 21
     column: 5
   end_location:
-    row: 3
-    column: 13
+    row: 21
+    column: 6
   fix: ~
 - kind:
-    UnnecessaryLiteralDict: tuple
+    UnusedVariable: b
   location:
-    row: 4
-    column: 5
+    row: 21
+    column: 8
   end_location:
-    row: 4
-    column: 13
+    row: 21
+    column: 9
   fix: ~
```

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C408_C408.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C408_C408.py.snap`

 * *Files 5% similar despite different names*

```diff
@@ -60,9 +60,18 @@
     UnnecessaryCollectionCall: dict
   location:
     row: 4
     column: 5
   end_location:
     row: 4
     column: 14
-  fix: ~
+  fix:
+    patch:
+      content: "{\"a\": 1}"
+      location:
+        row: 4
+        column: 5
+      end_location:
+        row: 4
+        column: 14
+    applied: false
```

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C409_C409.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C409_C409.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C410_C410.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C410_C410.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C414_C414.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C414_C414.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C415_C415.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C415_C415.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__C417_C417.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C417_C417.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D201_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D201_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D202_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D202_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D203_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D203_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D204_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D204_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D205_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D205_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D207_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D207_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D208_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D208_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D210_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D210_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D211_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D211_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D213_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D213_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D215_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D215_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D300_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D300_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D400_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D400_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D405_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D405_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D406_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D406_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D407_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D407_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D409_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D409_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D410_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D410_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D411_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D411_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D414_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D414_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D415_D.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D415_D.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__D417_sections.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__D417_sections.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__E711_E711.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__E711_E711.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__E712_E712.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__E712_E712.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__E713_E713.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__E713_E713.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__E721_E721.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__E721_E721.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__E731_E731.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__E731_E731.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__E741_E741.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__E741_E741.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__F702_F702.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__F702_F702.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__F841_F841.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U001_U001.py.snap`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind:
-    UnusedVariable: e
+- kind: UselessMetaclassType
   location:
-    row: 3
-    column: 0
-  end_location:
-    row: 7
-    column: 0
-  fix: ~
-- kind:
-    UnusedVariable: z
-  location:
-    row: 16
+    row: 2
     column: 4
   end_location:
-    row: 16
-    column: 5
-  fix: ~
-- kind:
-    UnusedVariable: foo
+    row: 2
+    column: 24
+  fix:
+    patch:
+      content: pass
+      location:
+        row: 2
+        column: 4
+      end_location:
+        row: 2
+        column: 24
+    applied: false
+- kind: UselessMetaclassType
   location:
-    row: 20
+    row: 6
     column: 4
   end_location:
-    row: 20
-    column: 7
-  fix: ~
-- kind:
-    UnusedVariable: a
-  location:
-    row: 21
-    column: 5
-  end_location:
-    row: 21
-    column: 6
-  fix: ~
-- kind:
-    UnusedVariable: b
-  location:
-    row: 21
-    column: 8
-  end_location:
-    row: 21
-    column: 9
-  fix: ~
+    row: 6
+    column: 24
+  fix:
+    patch:
+      content: ""
+      location:
+        row: 6
+        column: 0
+      end_location:
+        row: 7
+        column: 0
+    applied: false
```

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__N801_N801.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__N801_N801.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__N802_N802.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__N802_N802.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__N811_N811.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__N811_N811.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__N812_N812.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__N812_N812.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__N813_N813.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__N813_N813.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__N814_N814.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__N814_N814.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__T203_T203.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__T203_T203.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U001_U001.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__C416_C416.py.snap`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind: UselessMetaclassType
+- kind:
+    UnnecessaryComprehension: list
   location:
     row: 2
-    column: 4
+    column: 0
   end_location:
     row: 2
-    column: 24
+    column: 14
   fix:
     patch:
-      content: pass
+      content: list(x)
       location:
         row: 2
-        column: 4
+        column: 0
       end_location:
         row: 2
-        column: 24
+        column: 14
     applied: false
-- kind: UselessMetaclassType
+- kind:
+    UnnecessaryComprehension: set
   location:
-    row: 6
-    column: 4
+    row: 3
+    column: 0
   end_location:
-    row: 6
-    column: 24
+    row: 3
+    column: 14
   fix:
     patch:
-      content: ""
+      content: set(x)
       location:
-        row: 6
+        row: 3
         column: 0
       end_location:
-        row: 7
-        column: 0
+        row: 3
+        column: 14
     applied: false
```

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U002_U002.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U002_U002.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U003_U003.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U003_U003.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U004_U004.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U004_U004.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U005_U005.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U005_U005.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U006_U006.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U006_U006.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U007_U007.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U007_U007.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__U008_U008.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__U008_U008.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__W605_W605.py.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__W605_W605.py.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/snapshots/ruff__linter__tests__m001.snap` & `ruff-0.0.99/src/snapshots/ruff__linter__tests__m001.snap`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/source_code_locator.rs` & `ruff-0.0.99/src/source_code_locator.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/src/visibility.rs` & `ruff-0.0.99/src/visibility.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/tests/integration_test.rs` & `ruff-0.0.99/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `ruff-0.0.98/PKG-INFO` & `ruff-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruff
-Version: 0.0.98
+Version: 0.0.99
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -108,15 +108,15 @@
 ```
 
 Ruff also works with [pre-commit](https://pre-commit.com):
 
 ```yaml
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.98
+    rev: v0.0.99
     hooks:
       - id: ruff
 ```
 
 <!-- TODO(charlie): Remove this message a few versions after v0.0.86. -->
 _Note: prior to `v0.0.86`, `ruff-pre-commit` used `lint` (rather than `ruff`) as the hook ID._
 
@@ -464,23 +464,23 @@
 | ---- | ---- | ------- | --- |
 | C400 | UnnecessaryGeneratorList | Unnecessary generator (rewrite as a `list` comprehension) | 🛠 |
 | C401 | UnnecessaryGeneratorSet | Unnecessary generator (rewrite as a `set` comprehension) | 🛠 |
 | C402 | UnnecessaryGeneratorDict | Unnecessary generator (rewrite as a `dict` comprehension) | 🛠 |
 | C403 | UnnecessaryListComprehensionSet | Unnecessary `list` comprehension (rewrite as a `set` comprehension) | 🛠 |
 | C404 | UnnecessaryListComprehensionDict | Unnecessary `list` comprehension (rewrite as a `dict` comprehension) |  |
 | C405 | UnnecessaryLiteralSet | Unnecessary `(list\|tuple)` literal (rewrite as a `set` literal) | 🛠 |
-| C406 | UnnecessaryLiteralDict | Unnecessary `(list\|tuple)` literal (rewrite as a `dict` literal) |  |
+| C406 | UnnecessaryLiteralDict | Unnecessary `(list\|tuple)` literal (rewrite as a `dict` literal) | 🛠 |
 | C408 | UnnecessaryCollectionCall | Unnecessary `(dict\|list\|tuple)` call (rewrite as a literal) | 🛠 |
 | C409 | UnnecessaryLiteralWithinTupleCall | Unnecessary `(list\|tuple)` literal passed to `tuple()` (remove the outer call to `tuple()`) | 🛠 |
 | C410 | UnnecessaryLiteralWithinListCall | Unnecessary `(list\|tuple)` literal passed to `list()` (rewrite as a `list` literal) | 🛠 |
 | C411 | UnnecessaryListCall | Unnecessary `list` call (remove the outer call to `list()`) | 🛠 |
 | C413 | UnnecessaryCallAroundSorted | Unnecessary `(list\|reversed)` call around `sorted()` |  |
 | C414 | UnnecessaryDoubleCastOrProcess | Unnecessary `(list\|reversed\|set\|sorted\|tuple)` call within `(list\|set\|sorted\|tuple)()` |  |
 | C415 | UnnecessarySubscriptReversal | Unnecessary subscript reversal of iterable within `(reversed\|set\|sorted)()` |  |
-| C416 | UnnecessaryComprehension | Unnecessary `(list\|set)` comprehension (rewrite using `(list\|set)()`) |  |
+| C416 | UnnecessaryComprehension | Unnecessary `(list\|set)` comprehension (rewrite using `(list\|set)()`) | 🛠 |
 | C417 | UnnecessaryMap | Unnecessary `map` usage (rewrite using a `(list\|set\|dict)` comprehension) |  |
 
 ### flake8-bugbear
 
 | Code | Name | Message | Fix |
 | ---- | ---- | ------- | --- |
 | B002 | UnaryPrefixIncrement | Python does not support the unary prefix increment. |  |
```

