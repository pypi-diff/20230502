# Comparing `tmp/typer-0.7.0.tar.gz` & `tmp/typer-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer-0.7.0.tar", last modified: Sat Nov  5 19:43:52 2022, max compression
+gzip compressed data, was "typer-0.8.0.tar", last modified: Mon May  1 11:35:13 2023, max compression
```

## Comparing `typer-0.7.0.tar` & `typer-0.8.0.tar`

### file list

```diff
@@ -1,486 +1,493 @@
--rw-r--r--   0        0        0       89 2022-11-05 19:43:29.205783 typer-0.7.0/.coveragerc
--rw-r--r--   0        0        0       19 2022-11-05 19:43:29.205783 typer-0.7.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      145 2022-11-05 19:43:29.205783 typer-0.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     6218 2022-11-05 19:43:29.205783 typer-0.7.0/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     5288 2022-11-05 19:43:29.205783 typer-0.7.0/.github/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0        0        0      115 2022-11-05 19:43:29.205783 typer-0.7.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      394 2022-11-05 19:43:29.205783 typer-0.7.0/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2074 2022-11-05 19:43:29.205783 typer-0.7.0/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      309 2022-11-05 19:43:29.205783 typer-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2778 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      576 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0     1130 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1195 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/preview-docs.yml
--rw-r--r--   0        0        0      567 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      952 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0     2267 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      117 2022-11-05 19:43:29.205783 typer-0.7.0/.gitignore
--rw-r--r--   0        0        0     1475 2022-11-05 19:43:29.205783 typer-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2022-11-05 19:43:29.205783 typer-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1086 2022-11-05 19:43:29.205783 typer-0.7.0/LICENSE
--rw-r--r--   0        0        0    15251 2022-11-05 19:43:29.205783 typer-0.7.0/README.md
--rw-r--r--   0        0        0     1160 2022-11-05 19:43:29.205783 typer-0.7.0/SECURITY.md
--rw-r--r--   0        0        0     4876 2022-11-05 19:43:29.205783 typer-0.7.0/docs/alternatives.md
--rw-r--r--   0        0        0     5980 2022-11-05 19:43:29.205783 typer-0.7.0/docs/contributing.md
--rw-r--r--   0        0        0      451 2022-11-05 19:43:29.205783 typer-0.7.0/docs/css/custom.css
--rw-r--r--   0        0        0     2214 2022-11-05 19:43:29.205783 typer-0.7.0/docs/css/termynal.css
--rw-r--r--   0        0        0     4434 2022-11-05 19:43:29.205783 typer-0.7.0/docs/features.md
--rw-r--r--   0        0        0     4884 2022-11-05 19:43:29.205783 typer-0.7.0/docs/help-typer.md
--rwxr-xr-x   0        0        0      439 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/favicon.png
--rw-r--r--   0        0        0    48377 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/github-social-preview.png
--rw-r--r--   0        0        0     3936 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/github-social-preview.svg
--rw-r--r--   0        0        0      284 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/icon-black.svg
--rw-r--r--   0        0        0     1743 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/icon-white.svg
--rw-r--r--   0        0        0     6768 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/logo-margin/logo-margin-vector.svg
--rw-r--r--   0        0        0     3010 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/logo-margin/logo-margin.svg
--rw-r--r--   0        0        0    13924 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/pycharm-completion.png
--rw-r--r--   0        0        0    22753 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/vscode-completion.png
--rw-r--r--   0        0        0    15251 2022-11-05 19:43:29.205783 typer-0.7.0/docs/index.md
--rw-r--r--   0        0        0     3897 2022-11-05 19:43:29.205783 typer-0.7.0/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2022-11-05 19:43:29.205783 typer-0.7.0/docs/js/termynal.js
--rw-r--r--   0        0        0      912 2022-11-05 19:43:29.205783 typer-0.7.0/docs/overrides/main.html
--rw-r--r--   0        0        0    26874 2022-11-05 19:43:29.205783 typer-0.7.0/docs/release-notes.md
--rw-r--r--   0        0        0     1445 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/app-dir.md
--rw-r--r--   0        0        0     2437 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/default.md
--rw-r--r--   0        0        0     3107 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/envvar.md
--rw-r--r--   0        0        0    11924 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/help.md
--rw-r--r--   0        0        0      173 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/index.md
--rw-r--r--   0        0        0     4815 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/optional.md
--rw-r--r--   0        0        0      163 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/other-uses.md
--rw-r--r--   0        0        0     1084 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/arguments.md
--rw-r--r--   0        0        0     4837 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/callback.md
--rw-r--r--   0        0        0     3549 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/context.md
--rw-r--r--   0        0        0    33029 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/help.md
--rw-r--r--   0        0        0     7323 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/index.md
--rw-r--r--   0        0        0     1380 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/name.md
--rw-r--r--   0        0        0     3454 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/commands/one-or-multiple.md
--rw-r--r--   0        0        0     2044 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/commands/options.md
--rw-r--r--   0        0        0    24660 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/exceptions.md
--rw-r--r--   0        0        0    25417 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2367 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/index.md
--rw-r--r--   0        0        0      974 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/launch.md
--rw-r--r--   0        0        0     1876 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/arguments-with-multiple-values.md
--rw-r--r--   0        0        0      133 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/index.md
--rw-r--r--   0        0        0     1231 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/multiple-options.md
--rw-r--r--   0        0        0     2315 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/options-with-multiple-values.md
--rw-r--r--   0        0        0    12664 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options-autocompletion.md
--rw-r--r--   0        0        0     7112 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/callback-and-context.md
--rw-r--r--   0        0        0     7202 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/help.md
--rw-r--r--   0        0        0      202 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/index.md
--rw-r--r--   0        0        0     8907 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/name.md
--rw-r--r--   0        0        0     1294 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/password.md
--rw-r--r--   0        0        0     1892 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/prompt.md
--rw-r--r--   0        0        0     1604 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/required.md
--rw-r--r--   0        0        0     3437 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/version.md
--rw-r--r--   0        0        0    20773 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/package.md
--rw-r--r--   0        0        0     4048 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/bool.md
--rw-r--r--   0        0        0     2420 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/datetime.md
--rw-r--r--   0        0        0     1791 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/enum.md
--rw-r--r--   0        0        0     7467 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/file.md
--rw-r--r--   0        0        0     2191 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/index.md
--rw-r--r--   0        0        0     3242 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/number.md
--rw-r--r--   0        0        0     3396 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/path.md
--rw-r--r--   0        0        0     1739 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/uuid.md
--rw-r--r--   0        0        0    10363 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/printing.md
--rw-r--r--   0        0        0     6259 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/progressbar.md
--rw-r--r--   0        0        0     1909 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/prompt.md
--rw-r--r--   0        0        0     3795 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/add-typer.md
--rw-r--r--   0        0        0     2984 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/callback-override.md
--rw-r--r--   0        0        0     1201 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/index.md
--rw-r--r--   0        0        0    12517 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/name-and-help.md
--rw-r--r--   0        0        0     6077 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/nested-subcommands.md
--rw-r--r--   0        0        0     2729 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/single-file.md
--rw-r--r--   0        0        0     3013 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/terminating.md
--rw-r--r--   0        0        0     6146 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6229 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/using-click.md
--rw-r--r--   0        0        0     9703 2022-11-05 19:43:29.209783 typer-0.7.0/docs/typer-cli.md
--rw-r--r--   0        0        0      310 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/app_dir/tutorial001.py
--rw-r--r--   0        0        0      144 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/default/tutorial001.py
--rw-r--r--   0        0        0      236 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/default/tutorial002.py
--rw-r--r--   0        0        0      165 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/envvar/tutorial001.py
--rw-r--r--   0        0        0      179 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/envvar/tutorial002.py
--rw-r--r--   0        0        0      184 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/envvar/tutorial003.py
--rw-r--r--   0        0        0      172 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial001.py
--rw-r--r--   0        0        0      231 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial002.py
--rw-r--r--   0        0        0      218 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial003.py
--rw-r--r--   0        0        0      238 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial004.py
--rw-r--r--   0        0        0      231 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial005.py
--rw-r--r--   0        0        0      164 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial006.py
--rw-r--r--   0        0        0      447 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial007.py
--rw-r--r--   0        0        0      210 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial008.py
--rw-r--r--   0        0        0      134 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/optional/tutorial001.py
--rw-r--r--   0        0        0      239 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/optional/tutorial002.py
--rw-r--r--   0        0        0      241 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/arguments/tutorial001.py
--rw-r--r--   0        0        0      721 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial001.py
--rw-r--r--   0        0        0      216 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial002.py
--rw-r--r--   0        0        0      304 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial003.py
--rw-r--r--   0        0        0      315 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial004.py
--rw-r--r--   0        0        0      411 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial001.py
--rw-r--r--   0        0        0      390 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial002.py
--rw-r--r--   0        0        0      451 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial003.py
--rw-r--r--   0        0        0      277 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial004.py
--rw-r--r--   0        0        0     1196 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial001.py
--rw-r--r--   0        0        0      439 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial002.py
--rw-r--r--   0        0        0      386 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial003.py
--rw-r--r--   0        0        0      827 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial004.py
--rw-r--r--   0        0        0      787 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial005.py
--rw-r--r--   0        0        0     1143 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial006.py
--rw-r--r--   0        0        0     1044 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial007.py
--rw-r--r--   0        0        0      293 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial008.py
--rw-r--r--   0        0        0      138 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/index/tutorial001.py
--rw-r--r--   0        0        0      215 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/index/tutorial002.py
--rw-r--r--   0        0        0      275 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/name/tutorial001.py
--rw-r--r--   0        0        0      187 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/one_or_multiple/tutorial001.py
--rw-r--r--   0        0        0      287 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/one_or_multiple/tutorial002.py
--rw-r--r--   0        0        0      693 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/options/tutorial001.py
--rw-r--r--   0        0        0      115 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial001.py
--rw-r--r--   0        0        0      174 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial002.py
--rw-r--r--   0        0        0      170 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial003.py
--rw-r--r--   0        0        0      171 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial004.py
--rw-r--r--   0        0        0      101 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      112 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      138 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      239 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial004.py
--rw-r--r--   0        0        0      244 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial005.py
--rw-r--r--   0        0        0      358 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial006.py
--rw-r--r--   0        0        0      157 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/launch/tutorial001.py
--rw-r--r--   0        0        0      527 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/launch/tutorial002.py
--rw-r--r--   0        0        0      294 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      291 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
--rw-r--r--   0        0        0      295 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/multiple_options/tutorial001.py
--rw-r--r--   0        0        0      178 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/multiple_options/tutorial002.py
--rw-r--r--   0        0        0      403 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      291 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial001.py
--rw-r--r--   0        0        0      320 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial002.py
--rw-r--r--   0        0        0      385 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial003.py
--rw-r--r--   0        0        0      429 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial004.py
--rw-r--r--   0        0        0      464 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/help/tutorial001.py
--rw-r--r--   0        0        0      643 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/help/tutorial002.py
--rw-r--r--   0        0        0      170 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/help/tutorial003.py
--rw-r--r--   0        0        0      152 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial001.py
--rw-r--r--   0        0        0      158 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial002.py
--rw-r--r--   0        0        0      148 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial003.py
--rw-r--r--   0        0        0      163 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial004.py
--rw-r--r--   0        0        0      281 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial005.py
--rw-r--r--   0        0        0      212 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/password/tutorial001.py
--rw-r--r--   0        0        0      341 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/password/tutorial002.py
--rw-r--r--   0        0        0      171 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/prompt/tutorial001.py
--rw-r--r--   0        0        0      204 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/prompt/tutorial002.py
--rw-r--r--   0        0        0      198 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/prompt/tutorial003.py
--rw-r--r--   0        0        0      158 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/required/tutorial001.py
--rw-r--r--   0        0        0      430 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/version/tutorial001.py
--rw-r--r--   0        0        0      566 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/version/tutorial002.py
--rw-r--r--   0        0        0      597 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/version/tutorial003.py
--rw-r--r--   0        0        0      193 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial001.py
--rw-r--r--   0        0        0      312 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial002.py
--rw-r--r--   0        0        0      478 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial003.py
--rw-r--r--   0        0        0      664 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial004.py
--rw-r--r--   0        0        0      563 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial005.py
--rw-r--r--   0        0        0      262 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial006.py
--rw-r--r--   0        0        0      699 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial007.py
--rw-r--r--   0        0        0      735 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial008.py
--rw-r--r--   0        0        0      818 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial009.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/__init__.py
--rw-r--r--   0        0        0      208 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial001.py
--rw-r--r--   0        0        0      323 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial002.py
--rw-r--r--   0        0        0      228 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial003.py
--rw-r--r--   0        0        0      225 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/datetime/__init__.py
--rw-r--r--   0        0        0      211 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/datetime/tutorial001.py
--rw-r--r--   0        0        0      293 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/datetime/tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/enum/__init__.py
--rw-r--r--   0        0        0      299 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/enum/tutorial001.py
--rw-r--r--   0        0        0      341 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/enum/tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/__init__.py
--rw-r--r--   0        0        0      180 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial001.py
--rw-r--r--   0        0        0      202 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial002.py
--rw-r--r--   0        0        0      321 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial003.py
--rw-r--r--   0        0        0      547 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial004.py
--rw-r--r--   0        0        0      205 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial005.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/index/__init__.py
--rw-r--r--   0        0        0      394 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/index/tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/__init__.py
--rw-r--r--   0        0        0      302 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/tutorial001.py
--rw-r--r--   0        0        0      335 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/tutorial002.py
--rw-r--r--   0        0        0      178 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/path/__init__.py
--rw-r--r--   0        0        0      530 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/path/tutorial001.py
--rw-r--r--   0        0        0      371 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/path/tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/uuid/__init__.py
--rw-r--r--   0        0        0      196 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/uuid/tutorial001.py
--rw-r--r--   0        0        0      296 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial001.py
--rw-r--r--   0        0        0      183 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial002.py
--rw-r--r--   0        0        0      296 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial003.py
--rw-r--r--   0        0        0      214 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial004.py
--rw-r--r--   0        0        0      365 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial005.py
--rw-r--r--   0        0        0      150 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial006.py
--rw-r--r--   0        0        0      315 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial001.py
--rw-r--r--   0        0        0      476 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial002.py
--rw-r--r--   0        0        0      313 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial003.py
--rw-r--r--   0        0        0      455 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial004.py
--rw-r--r--   0        0        0      333 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial005.py
--rw-r--r--   0        0        0      336 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial006.py
--rw-r--r--   0        0        0      162 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial001.py
--rw-r--r--   0        0        0      245 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial002.py
--rw-r--r--   0        0        0      180 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial003.py
--rw-r--r--   0        0        0      193 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial004.py
--rw-r--r--   0        0        0      304 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial001.py
--rw-r--r--   0        0        0      306 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial002.py
--rw-r--r--   0        0        0      409 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial003.py
--rw-r--r--   0        0        0      533 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial004.py
--rw-r--r--   0        0        0      254 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial001.py
--rw-r--r--   0        0        0      289 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial002.py
--rw-r--r--   0        0        0      282 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial003.py
--rw-r--r--   0        0        0      372 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial004.py
--rw-r--r--   0        0        0      473 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial005.py
--rw-r--r--   0        0        0      514 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial006.py
--rw-r--r--   0        0        0      564 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial007.py
--rw-r--r--   0        0        0      644 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial008.py
--rw-r--r--   0        0        0      298 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial001/items.py
--rw-r--r--   0        0        0      177 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial001/main.py
--rw-r--r--   0        0        0      245 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial001/users.py
--rw-r--r--   0        0        0      698 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial002/main.py
--rw-r--r--   0        0        0      298 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/items.py
--rw-r--r--   0        0        0      180 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/lands.py
--rw-r--r--   0        0        0      229 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/main.py
--rw-r--r--   0        0        0      233 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/reigns.py
--rw-r--r--   0        0        0      221 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/towns.py
--rw-r--r--   0        0        0      245 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/users.py
--rw-r--r--   0        0        0      598 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/terminating/tutorial001.py
--rw-r--r--   0        0        0      235 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/terminating/tutorial002.py
--rw-r--r--   0        0        0      230 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/terminating/tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app01/__init__.py
--rw-r--r--   0        0        0      256 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app01/main.py
--rw-r--r--   0        0        0      299 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app01/test_main.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app02/__init__.py
--rw-r--r--   0        0        0      207 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app02/main.py
--rw-r--r--   0        0        0      284 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app02/test_main.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app03/__init__.py
--rw-r--r--   0        0        0      122 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app03/main.py
--rw-r--r--   0        0        0      284 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app03/test_main.py
--rw-r--r--   0        0        0      371 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/using_click/tutorial001.py
--rw-r--r--   0        0        0      287 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/using_click/tutorial002.py
--rw-r--r--   0        0        0      626 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/using_click/tutorial003.py
--rw-r--r--   0        0        0      511 2022-11-05 19:43:29.217783 typer-0.7.0/docs_src/using_click/tutorial004.py
--rw-r--r--   0        0        0       51 2022-11-05 19:43:29.217783 typer-0.7.0/mkdocs.insiders.yml
--rw-r--r--   0        0        0     5359 2022-11-05 19:43:29.217783 typer-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0       96 2022-11-05 19:43:29.217783 typer-0.7.0/mypy.ini
--rw-r--r--   0        0        0     2965 2022-11-05 19:43:29.217783 typer-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0       76 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/clean.sh
--rwxr-xr-x   0        0        0       68 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/docs-live.sh
--rwxr-xr-x   0        0        0      167 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      205 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/format.sh
--rw-r--r--   0        0        0      112 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/get-pwsh-activate.sh
--rwxr-xr-x   0        0        0      122 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/lint.sh
--rwxr-xr-x   0        0        0      339 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/netlify-docs.sh
--rwxr-xr-x   0        0        0       42 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/publish.sh
--rwxr-xr-x   0        0        0       80 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      350 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/test-files.sh
--rwxr-xr-x   0        0        0      490 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/test.sh
--rw-r--r--   0        0        0      108 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/zip-docs.sh
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/__init__.py
--rw-r--r--   0        0        0      675 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/compat_click7_8.py
--rw-r--r--   0        0        0      542 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/completion_no_types.py
--rw-r--r--   0        0        0      542 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/completion_no_types_order.py
--rw-r--r--   0        0        0      160 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/prog_name.py
--rw-r--r--   0        0        0      157 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/type_error_no_rich.py
--rw-r--r--   0        0        0      213 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/type_error_no_rich_short_disable.py
--rw-r--r--   0        0        0      306 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/type_error_normal_traceback.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_compat/__init__.py
--rw-r--r--   0        0        0     1585 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_compat/test_option_get_help.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/__init__.py
--rw-r--r--   0        0        0     5152 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion.py
--rw-r--r--   0        0        0     5551 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_complete.py
--rw-r--r--   0        0        0     2110 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_complete_no_help.py
--rw-r--r--   0        0        0     5559 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_install.py
--rw-r--r--   0        0        0     3273 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_show.py
--rw-r--r--   0        0        0      797 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_exit_errors.py
--rw-r--r--   0        0        0     6720 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_others.py
--rw-r--r--   0        0        0      377 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_prog_name.py
--rw-r--r--   0        0        0      849 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_rich_utils.py
--rw-r--r--   0        0        0     2479 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tracebacks.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_default/__init__.py
--rw-r--r--   0        0        0      947 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
--rw-r--r--   0        0        0     1072 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/__init__.py
--rw-r--r--   0        0        0     1621 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
--rw-r--r--   0        0        0     1217 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
--rw-r--r--   0        0        0     1238 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/__init__.py
--rw-r--r--   0        0        0     1310 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
--rw-r--r--   0        0        0      955 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
--rw-r--r--   0        0        0      946 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
--rw-r--r--   0        0        0      950 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
--rw-r--r--   0        0        0      868 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
--rw-r--r--   0        0        0      852 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
--rw-r--r--   0        0        0      842 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
--rw-r--r--   0        0        0     1290 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/__init__.py
--rw-r--r--   0        0        0     1155 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
--rw-r--r--   0        0        0      850 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_arguments/__init__.py
--rw-r--r--   0        0        0     1045 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/__init__.py
--rw-r--r--   0        0        0     2300 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0      591 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
--rw-r--r--   0        0        0      708 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0      831 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/__init__.py
--rw-r--r--   0        0        0      831 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
--rw-r--r--   0        0        0      949 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
--rw-r--r--   0        0        0      957 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
--rw-r--r--   0        0        0      716 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/__init__.py
--rw-r--r--   0        0        0     4190 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1646 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
--rw-r--r--   0        0        0     1105 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
--rw-r--r--   0        0        0     1808 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
--rw-r--r--   0        0        0     1875 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
--rw-r--r--   0        0        0     1577 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
--rw-r--r--   0        0        0     1674 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
--rw-r--r--   0        0        0      710 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_index/__init__.py
--rw-r--r--   0        0        0      662 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
--rw-r--r--   0        0        0      960 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_name/__init__.py
--rw-r--r--   0        0        0      911 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
--rw-r--r--   0        0        0      721 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
--rw-r--r--   0        0        0      865 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_commands/test_options/__init__.py
--rw-r--r--   0        0        0     3019 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/__init__.py
--rw-r--r--   0        0        0     1886 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial001.py
--rw-r--r--   0        0        0     1898 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial002.py
--rw-r--r--   0        0        0     1145 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial003.py
--rw-r--r--   0        0        0     1090 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0      528 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0      698 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial002.py
--rw-r--r--   0        0        0      735 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial003.py
--rw-r--r--   0        0        0     1521 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial004.py
--rw-r--r--   0        0        0     1510 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial005.py
--rw-r--r--   0        0        0     1386 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial006.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
--rw-r--r--   0        0        0      724 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0     1479 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
--rw-r--r--   0        0        0     1093 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
--rw-r--r--   0        0        0      910 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
--rw-r--r--   0        0        0     1433 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/__init__.py
--rw-r--r--   0        0        0      756 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0     1280 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0     1287 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/__init__.py
--rw-r--r--   0        0        0     1301 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1070 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial002.py
--rw-r--r--   0        0        0      785 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/__init__.py
--rw-r--r--   0        0        0      794 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial001.py
--rw-r--r--   0        0        0      977 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial002.py
--rw-r--r--   0        0        0      827 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial003.py
--rw-r--r--   0        0        0      982 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial004.py
--rw-r--r--   0        0        0     1311 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial005.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/__init__.py
--rw-r--r--   0        0        0     1057 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0     1078 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0     1504 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_required/__init__.py
--rw-r--r--   0        0        0     1302 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_required/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_version/__init__.py
--rw-r--r--   0        0        0     1420 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_version/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/__init__.py
--rw-r--r--   0        0        0     1064 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
--rw-r--r--   0        0        0     1075 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
--rw-r--r--   0        0        0     1144 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
--rw-r--r--   0        0        0     1230 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
--rw-r--r--   0        0        0     1334 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
--rw-r--r--   0        0        0     1378 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
--rw-r--r--   0        0        0     1189 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
--rw-r--r--   0        0        0     1712 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
--rw-r--r--   0        0        0      952 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
--rw-r--r--   0        0        0     1014 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
--rw-r--r--   0        0        0     1438 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
--rw-r--r--   0        0        0      791 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
--rw-r--r--   0        0        0     1280 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
--rw-r--r--   0        0        0      782 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/__init__.py
--rw-r--r--   0        0        0      833 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
--rw-r--r--   0        0        0      859 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
--rw-r--r--   0        0        0      778 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
--rw-r--r--   0        0        0      893 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
--rw-r--r--   0        0        0     1047 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_index/__init__.py
--rw-r--r--   0        0        0     1501 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/__init__.py
--rw-r--r--   0        0        0     2783 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
--rw-r--r--   0        0        0     1058 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
--rw-r--r--   0        0        0     1379 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/__init__.py
--rw-r--r--   0        0        0     1462 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
--rw-r--r--   0        0        0     1312 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
--rw-r--r--   0        0        0     1106 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/__init__.py
--rw-r--r--   0        0        0      611 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0      887 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0      844 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
--rw-r--r--   0        0        0      618 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
--rw-r--r--   0        0        0      618 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
--rw-r--r--   0        0        0      747 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
--rw-r--r--   0        0        0      849 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
--rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
--rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
--rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
--rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
--rw-r--r--   0        0        0      996 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
--rw-r--r--   0        0        0      946 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
--rw-r--r--   0        0        0      979 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
--rw-r--r--   0        0        0      992 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
--rw-r--r--   0        0        0     2572 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial001.py
--rw-r--r--   0        0        0     2145 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial002.py
--rw-r--r--   0        0        0     5514 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/__init__.py
--rw-r--r--   0        0        0     1135 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial001.py
--rw-r--r--   0        0        0      723 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial002.py
--rw-r--r--   0        0        0     1240 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      390 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/test_app01.py
--rw-r--r--   0        0        0      390 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/test_app02.py
--rw-r--r--   0        0        0      390 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/test_app03.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_using_click/__init__.py
--rw-r--r--   0        0        0      861 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_using_click/test_tutorial003.py
--rw-r--r--   0        0        0      938 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_using_click/test_tutorial004.py
--rw-r--r--   0        0        0     2433 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_type_conversion.py
--rw-r--r--   0        0        0     1602 2022-11-05 19:43:29.221783 typer-0.7.0/typer/__init__.py
--rw-r--r--   0        0        0       94 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_compat_utils.py
--rw-r--r--   0        0        0     4957 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_completion_click7.py
--rw-r--r--   0        0        0     6688 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_completion_click8.py
--rw-r--r--   0        0        0     8541 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_completion_shared.py
--rw-r--r--   0        0        0      430 2022-11-05 19:43:29.221783 typer-0.7.0/typer/colors.py
--rw-r--r--   0        0        0     4979 2022-11-05 19:43:29.221783 typer-0.7.0/typer/completion.py
--rw-r--r--   0        0        0    26545 2022-11-05 19:43:29.221783 typer-0.7.0/typer/core.py
--rw-r--r--   0        0        0    39111 2022-11-05 19:43:29.221783 typer-0.7.0/typer/main.py
--rw-r--r--   0        0        0    14736 2022-11-05 19:43:29.221783 typer-0.7.0/typer/models.py
--rw-r--r--   0        0        0     5949 2022-11-05 19:43:29.221783 typer-0.7.0/typer/params.py
--rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/typer/py.typed
--rw-r--r--   0        0        0    23656 2022-11-05 19:43:29.225783 typer-0.7.0/typer/rich_utils.py
--rw-r--r--   0        0        0      874 2022-11-05 19:43:29.225783 typer-0.7.0/typer/testing.py
--rw-r--r--   0        0        0      590 2022-11-05 19:43:29.225783 typer-0.7.0/typer/utils.py
--rw-r--r--   0        0        0    17937 1970-01-01 00:00:00.000000 typer-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      281 2023-05-01 11:34:46.163439 typer-0.8.0/.coveragerc
+-rw-r--r--   0        0        0     5303 2023-05-01 11:34:46.163439 typer-0.8.0/.github/DISCUSSION_TEMPLATE/questions.yml
+-rw-r--r--   0        0        0       19 2023-05-01 11:34:46.163439 typer-0.8.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      758 2023-05-01 11:34:46.163439 typer-0.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      885 2023-05-01 11:34:46.163439 typer-0.8.0/.github/ISSUE_TEMPLATE/privileged.yml
+-rw-r--r--   0        0        0      115 2023-05-01 11:34:46.163439 typer-0.8.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      394 2023-05-01 11:34:46.163439 typer-0.8.0/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2074 2023-05-01 11:34:46.163439 typer-0.8.0/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      309 2023-05-01 11:34:46.163439 typer-0.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2783 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      576 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0     1130 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1303 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/preview-docs.yml
+-rw-r--r--   0        0        0      567 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      957 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     2266 2023-05-01 11:34:46.163439 typer-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      117 2023-05-01 11:34:46.163439 typer-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1523 2023-05-01 11:34:46.163439 typer-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2023-05-01 11:34:46.163439 typer-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1086 2023-05-01 11:34:46.163439 typer-0.8.0/LICENSE
+-rw-r--r--   0        0        0    11885 2023-05-01 11:34:46.163439 typer-0.8.0/README.md
+-rw-r--r--   0        0        0     1160 2023-05-01 11:34:46.163439 typer-0.8.0/SECURITY.md
+-rw-r--r--   0        0        0     4876 2023-05-01 11:34:46.163439 typer-0.8.0/docs/alternatives.md
+-rw-r--r--   0        0        0     5980 2023-05-01 11:34:46.163439 typer-0.8.0/docs/contributing.md
+-rw-r--r--   0        0        0      451 2023-05-01 11:34:46.163439 typer-0.8.0/docs/css/custom.css
+-rw-r--r--   0        0        0     2214 2023-05-01 11:34:46.163439 typer-0.8.0/docs/css/termynal.css
+-rw-r--r--   0        0        0     4434 2023-05-01 11:34:46.163439 typer-0.8.0/docs/features.md
+-rw-r--r--   0        0        0    12075 2023-05-01 11:34:46.163439 typer-0.8.0/docs/help-typer.md
+-rwxr-xr-x   0        0        0      439 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/favicon.png
+-rw-r--r--   0        0        0    48377 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/github-social-preview.png
+-rw-r--r--   0        0        0     3936 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/github-social-preview.svg
+-rw-r--r--   0        0        0      284 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/icon-black.svg
+-rw-r--r--   0        0        0     1743 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/icon-white.svg
+-rw-r--r--   0        0        0     6768 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/logo-margin/logo-margin-vector.svg
+-rw-r--r--   0        0        0     3010 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/logo-margin/logo-margin.svg
+-rw-r--r--   0        0        0    13924 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/pycharm-completion.png
+-rw-r--r--   0        0        0    22753 2023-05-01 11:34:46.167439 typer-0.8.0/docs/img/vscode-completion.png
+-rw-r--r--   0        0        0    11885 2023-05-01 11:34:46.167439 typer-0.8.0/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-05-01 11:34:46.167439 typer-0.8.0/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-05-01 11:34:46.167439 typer-0.8.0/docs/js/termynal.js
+-rw-r--r--   0        0        0      912 2023-05-01 11:34:46.167439 typer-0.8.0/docs/overrides/main.html
+-rw-r--r--   0        0        0    31046 2023-05-01 11:34:46.167439 typer-0.8.0/docs/release-notes.md
+-rw-r--r--   0        0        0     1445 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/app-dir.md
+-rw-r--r--   0        0        0     2437 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/arguments/default.md
+-rw-r--r--   0        0        0     3107 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/arguments/envvar.md
+-rw-r--r--   0        0        0    11924 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/arguments/help.md
+-rw-r--r--   0        0        0      173 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/arguments/index.md
+-rw-r--r--   0        0        0     4815 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/arguments/optional.md
+-rw-r--r--   0        0        0      163 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/arguments/other-uses.md
+-rw-r--r--   0        0        0     1084 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/arguments.md
+-rw-r--r--   0        0        0     4837 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/callback.md
+-rw-r--r--   0        0        0     3549 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/context.md
+-rw-r--r--   0        0        0    33027 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/help.md
+-rw-r--r--   0        0        0     7323 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/index.md
+-rw-r--r--   0        0        0     1380 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/name.md
+-rw-r--r--   0        0        0     3454 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/one-or-multiple.md
+-rw-r--r--   0        0        0     2044 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/commands/options.md
+-rw-r--r--   0        0        0    24660 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/exceptions.md
+-rw-r--r--   0        0        0    25417 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2367 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/index.md
+-rw-r--r--   0        0        0      974 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/launch.md
+-rw-r--r--   0        0        0     1876 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/multiple-values/arguments-with-multiple-values.md
+-rw-r--r--   0        0        0      133 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/multiple-values/index.md
+-rw-r--r--   0        0        0     1231 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/multiple-values/multiple-options.md
+-rw-r--r--   0        0        0     2315 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/multiple-values/options-with-multiple-values.md
+-rw-r--r--   0        0        0    12668 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options-autocompletion.md
+-rw-r--r--   0        0        0     7112 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/callback-and-context.md
+-rw-r--r--   0        0        0     7202 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/help.md
+-rw-r--r--   0        0        0      202 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/index.md
+-rw-r--r--   0        0        0     8907 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/name.md
+-rw-r--r--   0        0        0     1294 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/password.md
+-rw-r--r--   0        0        0     1892 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/prompt.md
+-rw-r--r--   0        0        0     1604 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/required.md
+-rw-r--r--   0        0        0     3437 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/options/version.md
+-rw-r--r--   0        0        0    20775 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/package.md
+-rw-r--r--   0        0        0     4048 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/bool.md
+-rw-r--r--   0        0        0     1189 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/custom-types.md
+-rw-r--r--   0        0        0     2421 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/datetime.md
+-rw-r--r--   0        0        0     1791 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/enum.md
+-rw-r--r--   0        0        0     7467 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/file.md
+-rw-r--r--   0        0        0     2191 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/index.md
+-rw-r--r--   0        0        0     3242 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/number.md
+-rw-r--r--   0        0        0     3396 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/path.md
+-rw-r--r--   0        0        0     1739 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/parameter-types/uuid.md
+-rw-r--r--   0        0        0    10363 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/printing.md
+-rw-r--r--   0        0        0     6259 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/progressbar.md
+-rw-r--r--   0        0        0     1909 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/prompt.md
+-rw-r--r--   0        0        0     3795 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/subcommands/add-typer.md
+-rw-r--r--   0        0        0     2984 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/subcommands/callback-override.md
+-rw-r--r--   0        0        0     1201 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/subcommands/index.md
+-rw-r--r--   0        0        0    12517 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/subcommands/name-and-help.md
+-rw-r--r--   0        0        0     6077 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/subcommands/nested-subcommands.md
+-rw-r--r--   0        0        0     2729 2023-05-01 11:34:46.167439 typer-0.8.0/docs/tutorial/subcommands/single-file.md
+-rw-r--r--   0        0        0     3013 2023-05-01 11:34:46.171439 typer-0.8.0/docs/tutorial/terminating.md
+-rw-r--r--   0        0        0     6146 2023-05-01 11:34:46.171439 typer-0.8.0/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6229 2023-05-01 11:34:46.171439 typer-0.8.0/docs/tutorial/using-click.md
+-rw-r--r--   0        0        0     9703 2023-05-01 11:34:46.171439 typer-0.8.0/docs/typer-cli.md
+-rw-r--r--   0        0        0      310 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/app_dir/tutorial001.py
+-rw-r--r--   0        0        0      144 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/default/tutorial001.py
+-rw-r--r--   0        0        0      236 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/default/tutorial002.py
+-rw-r--r--   0        0        0      165 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/envvar/tutorial001.py
+-rw-r--r--   0        0        0      179 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/envvar/tutorial002.py
+-rw-r--r--   0        0        0      184 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/envvar/tutorial003.py
+-rw-r--r--   0        0        0      172 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial001.py
+-rw-r--r--   0        0        0      231 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial002.py
+-rw-r--r--   0        0        0      218 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial003.py
+-rw-r--r--   0        0        0      238 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial004.py
+-rw-r--r--   0        0        0      231 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial005.py
+-rw-r--r--   0        0        0      164 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial006.py
+-rw-r--r--   0        0        0      447 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial007.py
+-rw-r--r--   0        0        0      210 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/help/tutorial008.py
+-rw-r--r--   0        0        0      134 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/optional/tutorial001.py
+-rw-r--r--   0        0        0      239 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/arguments/optional/tutorial002.py
+-rw-r--r--   0        0        0      241 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/arguments/tutorial001.py
+-rw-r--r--   0        0        0      721 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/callback/tutorial001.py
+-rw-r--r--   0        0        0      216 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/callback/tutorial002.py
+-rw-r--r--   0        0        0      304 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/callback/tutorial003.py
+-rw-r--r--   0        0        0      315 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/callback/tutorial004.py
+-rw-r--r--   0        0        0      411 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/context/tutorial001.py
+-rw-r--r--   0        0        0      390 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/context/tutorial002.py
+-rw-r--r--   0        0        0      451 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/context/tutorial003.py
+-rw-r--r--   0        0        0      277 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/context/tutorial004.py
+-rw-r--r--   0        0        0     1196 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial001.py
+-rw-r--r--   0        0        0      439 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial002.py
+-rw-r--r--   0        0        0      386 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial003.py
+-rw-r--r--   0        0        0      826 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial004.py
+-rw-r--r--   0        0        0      786 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial005.py
+-rw-r--r--   0        0        0     1143 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial006.py
+-rw-r--r--   0        0        0     1044 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial007.py
+-rw-r--r--   0        0        0      293 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/help/tutorial008.py
+-rw-r--r--   0        0        0      138 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/index/tutorial001.py
+-rw-r--r--   0        0        0      215 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/index/tutorial002.py
+-rw-r--r--   0        0        0      275 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/name/tutorial001.py
+-rw-r--r--   0        0        0      187 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/one_or_multiple/tutorial001.py
+-rw-r--r--   0        0        0      287 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/one_or_multiple/tutorial002.py
+-rw-r--r--   0        0        0      693 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/commands/options/tutorial001.py
+-rw-r--r--   0        0        0      115 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/exceptions/tutorial001.py
+-rw-r--r--   0        0        0      174 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/exceptions/tutorial002.py
+-rw-r--r--   0        0        0      170 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/exceptions/tutorial003.py
+-rw-r--r--   0        0        0      171 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/exceptions/tutorial004.py
+-rw-r--r--   0        0        0      101 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      112 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      138 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      239 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/first_steps/tutorial004.py
+-rw-r--r--   0        0        0      244 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/first_steps/tutorial005.py
+-rw-r--r--   0        0        0      358 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/first_steps/tutorial006.py
+-rw-r--r--   0        0        0      157 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/launch/tutorial001.py
+-rw-r--r--   0        0        0      527 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/launch/tutorial002.py
+-rw-r--r--   0        0        0      294 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      291 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
+-rw-r--r--   0        0        0      295 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/multiple_values/multiple_options/tutorial001.py
+-rw-r--r--   0        0        0      178 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/multiple_values/multiple_options/tutorial002.py
+-rw-r--r--   0        0        0      403 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      291 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/callback/tutorial001.py
+-rw-r--r--   0        0        0      320 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/callback/tutorial002.py
+-rw-r--r--   0        0        0      385 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/callback/tutorial003.py
+-rw-r--r--   0        0        0      429 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/callback/tutorial004.py
+-rw-r--r--   0        0        0      464 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/help/tutorial001.py
+-rw-r--r--   0        0        0      643 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/help/tutorial002.py
+-rw-r--r--   0        0        0      170 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/help/tutorial003.py
+-rw-r--r--   0        0        0      152 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/name/tutorial001.py
+-rw-r--r--   0        0        0      158 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/name/tutorial002.py
+-rw-r--r--   0        0        0      148 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/name/tutorial003.py
+-rw-r--r--   0        0        0      163 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/name/tutorial004.py
+-rw-r--r--   0        0        0      281 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/name/tutorial005.py
+-rw-r--r--   0        0        0      212 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/password/tutorial001.py
+-rw-r--r--   0        0        0      341 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/password/tutorial002.py
+-rw-r--r--   0        0        0      171 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/prompt/tutorial001.py
+-rw-r--r--   0        0        0      204 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/prompt/tutorial002.py
+-rw-r--r--   0        0        0      198 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/prompt/tutorial003.py
+-rw-r--r--   0        0        0      158 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/required/tutorial001.py
+-rw-r--r--   0        0        0      430 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/version/tutorial001.py
+-rw-r--r--   0        0        0      566 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/version/tutorial002.py
+-rw-r--r--   0        0        0      597 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options/version/tutorial003.py
+-rw-r--r--   0        0        0      193 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial001.py
+-rw-r--r--   0        0        0      312 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial002.py
+-rw-r--r--   0        0        0      478 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial003.py
+-rw-r--r--   0        0        0      664 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial004.py
+-rw-r--r--   0        0        0      563 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial005.py
+-rw-r--r--   0        0        0      262 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial006.py
+-rw-r--r--   0        0        0      699 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial007.py
+-rw-r--r--   0        0        0      735 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial008.py
+-rw-r--r--   0        0        0      818 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/options_autocompletion/tutorial009.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/bool/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/bool/tutorial001.py
+-rw-r--r--   0        0        0      323 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/bool/tutorial002.py
+-rw-r--r--   0        0        0      228 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/bool/tutorial003.py
+-rw-r--r--   0        0        0      225 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/bool/tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/custom_types/__init__.py
+-rw-r--r--   0        0        0      547 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/custom_types/tutorial001.py
+-rw-r--r--   0        0        0      649 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/custom_types/tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/datetime/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/datetime/tutorial001.py
+-rw-r--r--   0        0        0      293 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/datetime/tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/enum/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/enum/tutorial001.py
+-rw-r--r--   0        0        0      341 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/enum/tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/file/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/file/tutorial001.py
+-rw-r--r--   0        0        0      202 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/file/tutorial002.py
+-rw-r--r--   0        0        0      321 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/file/tutorial003.py
+-rw-r--r--   0        0        0      547 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/file/tutorial004.py
+-rw-r--r--   0        0        0      205 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/file/tutorial005.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/index/__init__.py
+-rw-r--r--   0        0        0      394 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/index/tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/number/__init__.py
+-rw-r--r--   0        0        0      302 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/number/tutorial001.py
+-rw-r--r--   0        0        0      335 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/number/tutorial002.py
+-rw-r--r--   0        0        0      178 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/number/tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/path/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/path/tutorial001.py
+-rw-r--r--   0        0        0      371 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/path/tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/uuid/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/parameter_types/uuid/tutorial001.py
+-rw-r--r--   0        0        0      296 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/printing/tutorial001.py
+-rw-r--r--   0        0        0      183 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/printing/tutorial002.py
+-rw-r--r--   0        0        0      296 2023-05-01 11:34:46.171439 typer-0.8.0/docs_src/printing/tutorial003.py
+-rw-r--r--   0        0        0      214 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/printing/tutorial004.py
+-rw-r--r--   0        0        0      365 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/printing/tutorial005.py
+-rw-r--r--   0        0        0      150 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/printing/tutorial006.py
+-rw-r--r--   0        0        0      315 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/progressbar/tutorial001.py
+-rw-r--r--   0        0        0      476 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/progressbar/tutorial002.py
+-rw-r--r--   0        0        0      313 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/progressbar/tutorial003.py
+-rw-r--r--   0        0        0      455 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/progressbar/tutorial004.py
+-rw-r--r--   0        0        0      333 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/progressbar/tutorial005.py
+-rw-r--r--   0        0        0      336 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/progressbar/tutorial006.py
+-rw-r--r--   0        0        0      162 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/prompt/tutorial001.py
+-rw-r--r--   0        0        0      245 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/prompt/tutorial002.py
+-rw-r--r--   0        0        0      180 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/prompt/tutorial003.py
+-rw-r--r--   0        0        0      193 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/prompt/tutorial004.py
+-rw-r--r--   0        0        0      304 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/callback_override/tutorial001.py
+-rw-r--r--   0        0        0      306 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/callback_override/tutorial002.py
+-rw-r--r--   0        0        0      409 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/callback_override/tutorial003.py
+-rw-r--r--   0        0        0      533 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/callback_override/tutorial004.py
+-rw-r--r--   0        0        0      254 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial001.py
+-rw-r--r--   0        0        0      289 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial002.py
+-rw-r--r--   0        0        0      282 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial003.py
+-rw-r--r--   0        0        0      372 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial004.py
+-rw-r--r--   0        0        0      473 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial005.py
+-rw-r--r--   0        0        0      514 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial006.py
+-rw-r--r--   0        0        0      564 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial007.py
+-rw-r--r--   0        0        0      644 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/name_help/tutorial008.py
+-rw-r--r--   0        0        0      298 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial001/items.py
+-rw-r--r--   0        0        0      177 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial001/main.py
+-rw-r--r--   0        0        0      245 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial001/users.py
+-rw-r--r--   0        0        0      698 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial002/main.py
+-rw-r--r--   0        0        0      298 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial003/items.py
+-rw-r--r--   0        0        0      180 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial003/lands.py
+-rw-r--r--   0        0        0      229 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial003/main.py
+-rw-r--r--   0        0        0      233 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial003/reigns.py
+-rw-r--r--   0        0        0      221 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial003/towns.py
+-rw-r--r--   0        0        0      245 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/subcommands/tutorial003/users.py
+-rw-r--r--   0        0        0      598 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/terminating/tutorial001.py
+-rw-r--r--   0        0        0      235 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/terminating/tutorial002.py
+-rw-r--r--   0        0        0      230 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/terminating/tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app01/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app01/main.py
+-rw-r--r--   0        0        0      299 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app01/test_main.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app02/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app02/main.py
+-rw-r--r--   0        0        0      284 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app02/test_main.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app03/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app03/main.py
+-rw-r--r--   0        0        0      284 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/testing/app03/test_main.py
+-rw-r--r--   0        0        0      371 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/using_click/tutorial001.py
+-rw-r--r--   0        0        0      287 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/using_click/tutorial002.py
+-rw-r--r--   0        0        0      626 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/using_click/tutorial003.py
+-rw-r--r--   0        0        0      511 2023-05-01 11:34:46.175439 typer-0.8.0/docs_src/using_click/tutorial004.py
+-rw-r--r--   0        0        0       51 2023-05-01 11:34:46.175439 typer-0.8.0/mkdocs.insiders.yml
+-rw-r--r--   0        0        0     5424 2023-05-01 11:34:46.175439 typer-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0       96 2023-05-01 11:34:46.175439 typer-0.8.0/mypy.ini
+-rw-r--r--   0        0        0     2965 2023-05-01 11:34:46.175439 typer-0.8.0/pyproject.toml
+-rwxr-xr-x   0        0        0       76 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/clean.sh
+-rwxr-xr-x   0        0        0       68 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0      167 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      205 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/format.sh
+-rw-r--r--   0        0        0      112 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/get-pwsh-activate.sh
+-rwxr-xr-x   0        0        0      122 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0      339 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/netlify-docs.sh
+-rwxr-xr-x   0        0        0       42 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       80 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      350 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      490 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/test.sh
+-rw-r--r--   0        0        0      115 2023-05-01 11:34:46.175439 typer-0.8.0/scripts/zip-docs.sh
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/__init__.py
+-rw-r--r--   0        0        0      675 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/compat_click7_8.py
+-rw-r--r--   0        0        0      542 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/completion_no_types.py
+-rw-r--r--   0        0        0      542 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/completion_no_types_order.py
+-rw-r--r--   0        0        0      160 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/prog_name.py
+-rw-r--r--   0        0        0      157 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/type_error_no_rich.py
+-rw-r--r--   0        0        0      213 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/type_error_no_rich_short_disable.py
+-rw-r--r--   0        0        0      306 2023-05-01 11:34:46.175439 typer-0.8.0/tests/assets/type_error_normal_traceback.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_compat/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_compat/test_option_get_help.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_completion/__init__.py
+-rw-r--r--   0        0        0     5328 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_completion/test_completion.py
+-rw-r--r--   0        0        0     5782 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_completion/test_completion_complete.py
+-rw-r--r--   0        0        0     2209 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_completion/test_completion_complete_no_help.py
+-rw-r--r--   0        0        0     5943 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_completion/test_completion_install.py
+-rw-r--r--   0        0        0     3891 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_completion/test_completion_show.py
+-rw-r--r--   0        0        0      797 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_exit_errors.py
+-rw-r--r--   0        0        0     8120 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_others.py
+-rw-r--r--   0        0        0      410 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_prog_name.py
+-rw-r--r--   0        0        0      849 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_rich_utils.py
+-rw-r--r--   0        0        0     2556 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tracebacks.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_default/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
+-rw-r--r--   0        0        0     1105 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/__init__.py
+-rw-r--r--   0        0        0     1654 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
+-rw-r--r--   0        0        0     1250 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
+-rw-r--r--   0        0        0     1271 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/__init__.py
+-rw-r--r--   0        0        0     1343 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0      988 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0      979 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0      983 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0      901 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0      885 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0      875 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0     1323 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_optional/__init__.py
+-rw-r--r--   0        0        0     1188 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
+-rw-r--r--   0        0        0      883 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_arguments/__init__.py
+-rw-r--r--   0        0        0     1078 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_callback/__init__.py
+-rw-r--r--   0        0        0     2333 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0      624 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
+-rw-r--r--   0        0        0      741 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0      864 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_context/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
+-rw-r--r--   0        0        0      982 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
+-rw-r--r--   0        0        0      990 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
+-rw-r--r--   0        0        0      749 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/__init__.py
+-rw-r--r--   0        0        0     4223 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1679 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0     1138 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0     1839 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0     1906 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0     1610 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0     1707 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0      743 2023-05-01 11:34:46.175439 typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_index/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0      993 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_name/__init__.py
+-rw-r--r--   0        0        0      944 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
+-rw-r--r--   0        0        0      754 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
+-rw-r--r--   0        0        0      898 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_options/__init__.py
+-rw-r--r--   0        0        0     3052 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_exceptions/__init__.py
+-rw-r--r--   0        0        0     1963 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial001.py
+-rw-r--r--   0        0        0     1975 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial002.py
+-rw-r--r--   0        0        0     1200 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial003.py
+-rw-r--r--   0        0        0     1145 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      561 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0      731 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial002.py
+-rw-r--r--   0        0        0      768 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial003.py
+-rw-r--r--   0        0        0     1554 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial004.py
+-rw-r--r--   0        0        0     1543 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial005.py
+-rw-r--r--   0        0        0     1419 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0      757 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0     1512 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
+-rw-r--r--   0        0        0      943 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0     1466 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_callback/__init__.py
+-rw-r--r--   0        0        0      789 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0     1335 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0     1342 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_help/__init__.py
+-rw-r--r--   0        0        0     1334 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1103 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0      818 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_name/__init__.py
+-rw-r--r--   0        0        0      827 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0     1010 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial002.py
+-rw-r--r--   0        0        0      860 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial003.py
+-rw-r--r--   0        0        0     1015 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial004.py
+-rw-r--r--   0        0        0     1344 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_prompt/__init__.py
+-rw-r--r--   0        0        0     1090 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0     1111 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0     1537 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_required/__init__.py
+-rw-r--r--   0        0        0     1335 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_required/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_version/__init__.py
+-rw-r--r--   0        0        0     1475 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options/test_version/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/__init__.py
+-rw-r--r--   0        0        0     1119 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
+-rw-r--r--   0        0        0     1130 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
+-rw-r--r--   0        0        0     1199 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
+-rw-r--r--   0        0        0     1285 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
+-rw-r--r--   0        0        0     1389 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
+-rw-r--r--   0        0        0     1433 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
+-rw-r--r--   0        0        0     1745 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
+-rw-r--r--   0        0        0      985 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
+-rw-r--r--   0        0        0     1047 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_custom_types/__init__.py
+-rw-r--r--   0        0        0     1017 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py
+-rw-r--r--   0        0        0     1021 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
+-rw-r--r--   0        0        0      824 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
+-rw-r--r--   0        0        0     1313 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
+-rw-r--r--   0        0        0      815 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/__init__.py
+-rw-r--r--   0        0        0      866 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
+-rw-r--r--   0        0        0      892 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
+-rw-r--r--   0        0        0      811 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
+-rw-r--r--   0        0        0      926 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
+-rw-r--r--   0        0        0     1080 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_index/__init__.py
+-rw-r--r--   0        0        0     1534 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/__init__.py
+-rw-r--r--   0        0        0     2816 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
+-rw-r--r--   0        0        0     1091 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
+-rw-r--r--   0        0        0     1412 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_path/__init__.py
+-rw-r--r--   0        0        0     1495 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
+-rw-r--r--   0        0        0     1345 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_prompt/__init__.py
+-rw-r--r--   0        0        0      644 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0      920 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0      877 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
+-rw-r--r--   0        0        0      651 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
+-rw-r--r--   0        0        0      780 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
+-rw-r--r--   0        0        0      882 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
+-rw-r--r--   0        0        0      987 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
+-rw-r--r--   0        0        0      987 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
+-rw-r--r--   0        0        0      987 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
+-rw-r--r--   0        0        0      987 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
+-rw-r--r--   0        0        0     1029 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
+-rw-r--r--   0        0        0      979 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
+-rw-r--r--   0        0        0     1012 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
+-rw-r--r--   0        0        0     1025 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
+-rw-r--r--   0        0        0     2726 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_tutorial001.py
+-rw-r--r--   0        0        0     2178 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_tutorial002.py
+-rw-r--r--   0        0        0     5668 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_subcommands/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_terminating/__init__.py
+-rw-r--r--   0        0        0     1168 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_terminating/test_tutorial001.py
+-rw-r--r--   0        0        0      756 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_terminating/test_tutorial002.py
+-rw-r--r--   0        0        0     1273 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_terminating/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_testing/test_app01.py
+-rw-r--r--   0        0        0      423 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_testing/test_app02.py
+-rw-r--r--   0        0        0      423 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_testing/test_app03.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_using_click/__init__.py
+-rw-r--r--   0        0        0      894 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_using_click/test_tutorial003.py
+-rw-r--r--   0        0        0      971 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_tutorial/test_using_click/test_tutorial004.py
+-rw-r--r--   0        0        0     3316 2023-05-01 11:34:46.179439 typer-0.8.0/tests/test_type_conversion.py
+-rw-r--r--   0        0        0     1602 2023-05-01 11:34:46.179439 typer-0.8.0/typer/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-01 11:34:46.179439 typer-0.8.0/typer/_compat_utils.py
+-rw-r--r--   0        0        0     4957 2023-05-01 11:34:46.179439 typer-0.8.0/typer/_completion_click7.py
+-rw-r--r--   0        0        0     6688 2023-05-01 11:34:46.179439 typer-0.8.0/typer/_completion_click8.py
+-rw-r--r--   0        0        0     8541 2023-05-01 11:34:46.179439 typer-0.8.0/typer/_completion_shared.py
+-rw-r--r--   0        0        0      430 2023-05-01 11:34:46.179439 typer-0.8.0/typer/colors.py
+-rw-r--r--   0        0        0     4979 2023-05-01 11:34:46.179439 typer-0.8.0/typer/completion.py
+-rw-r--r--   0        0        0    26545 2023-05-01 11:34:46.179439 typer-0.8.0/typer/core.py
+-rw-r--r--   0        0        0    39310 2023-05-01 11:34:46.183439 typer-0.8.0/typer/main.py
+-rw-r--r--   0        0        0    15661 2023-05-01 11:34:46.183439 typer-0.8.0/typer/models.py
+-rw-r--r--   0        0        0    13055 2023-05-01 11:34:46.183439 typer-0.8.0/typer/params.py
+-rw-r--r--   0        0        0        0 2023-05-01 11:34:46.183439 typer-0.8.0/typer/py.typed
+-rw-r--r--   0        0        0    23654 2023-05-01 11:34:46.183439 typer-0.8.0/typer/rich_utils.py
+-rw-r--r--   0        0        0      874 2023-05-01 11:34:46.183439 typer-0.8.0/typer/testing.py
+-rw-r--r--   0        0        0      590 2023-05-01 11:34:46.183439 typer-0.8.0/typer/utils.py
+-rw-r--r--   0        0        0    14571 1970-01-01 00:00:00.000000 typer-0.8.0/PKG-INFO
```

### Comparing `typer-0.7.0/.github/ISSUE_TEMPLATE/feature-request.yml` & `typer-0.8.0/.github/DISCUSSION_TEMPLATE/questions.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-name: Feature Request
-description: Suggest an idea or ask for a feature that you would like to have in Typer
-labels: [enhancement]
+labels: [question]
 body:
   - type: markdown
     attributes:
       value: |
         Thanks for your interest in Typer! 🚀
 
         Please follow these instructions, fill every question, and do every step. 🙏
 
-        I'm asking this because answering questions and solving problems in GitHub issues is what consumes most of the time.
+        I'm asking this because answering questions and solving problems in GitHub is what consumes most of the time.
 
-        I end up not being able to add new features, fix bugs, review pull requests, etc. as fast as I wish because I have to spend too much time handling issues.
+        I end up not being able to add new features, fix bugs, review pull requests, etc. as fast as I wish because I have to spend too much time handling questions.
 
         All that, on top of all the incredible help provided by a bunch of community members that give a lot of their time to come here and help others.
 
         If more Typer users came to help others like them just a little bit more, it would be much less effort for them (and you and me 😅).
 
         By asking questions in a structured way (following this) it will be much easier to help you.
 
         And there's a high chance that you will find the solution along the way and you won't even have to submit it and wait for an answer. 😎
 
-        As there are too many issues with questions, I'll have to close the incomplete ones. That will allow me (and others) to focus on helping people like you that follow the whole process and help us help you. 🤓
+        As there are too many questions, I'll have to discard and close the incomplete ones. That will allow me (and others) to focus on helping people like you that follow the whole process and help us help you. 🤓
   - type: checkboxes
     id: checks
     attributes:
       label: First Check
       description: Please confirm and check all the following options.
       options:
-        - label: I added a very descriptive title to this issue.
+        - label: I added a very descriptive title here.
           required: true
-        - label: I used the GitHub search to find a similar issue and didn't find it.
+        - label: I used the GitHub search to find a similar question and didn't find it.
           required: true
         - label: I searched the Typer documentation, with the integrated search.
           required: true
         - label: I already searched in Google "How to X in Typer" and didn't find any information.
           required: true
         - label: I already read and followed all the tutorial in the docs and didn't find an answer.
           required: true
@@ -45,15 +43,15 @@
     attributes:
       label: Commit to Help
       description: |
         After submitting this, I commit to one of:
 
           * Read open issues with questions until I find 2 issues where I can help someone and add a comment to help there.
           * I already hit the "watch" button in this repository to receive notifications and I commit to help at least 2 people that ask questions in the future.
-          * Implement a Pull Request for a confirmed bug.
+          * Review one Pull Request by downloading the code and following all the review process](https://typer.tiangolo.com/help-typer/#review-pull-requests).
 
       options:
         - label: I commit to help with one of those options 👆
           required: true
   - type: textarea
     id: example
     attributes:
@@ -77,59 +75,25 @@
     validations:
       required: true
   - type: textarea
     id: description
     attributes:
       label: Description
       description: |
-        What is your feature request?
+        What is the problem, question, or error?
 
-        Write a short description telling me what you are trying to solve and what you are currently doing.
+        Write a short description telling me what you are doing, what you expect to happen, and what is currently happening.
       placeholder: |
-        * Create a Typer CLI that says "Hello".
-        * Run it on the command line without a name.
-        * I would like it to use Privacy-Aware Artificial Intelligence based on Block Chain and predict my name without me typing it.
+        * Create a small Typer script.
+        * Open a Terminal with Ninja-Turtle-Shell.
+        * Trigger autocompletion hitting TAB.
+        * I don't see any completion in the terminal using Ninja-Turtle-Shell.
+        * I expected to see autocompletion there.
     validations:
       required: true
-  - type: textarea
-    id: wanted-solution
-    attributes:
-      label: Wanted Solution
-      description: |
-        Tell me what's the solution you would like.
-      placeholder: |
-        I would like it to say my name without me having to type it.
-    validations:
-      required: true
-  - type: textarea
-    id: wanted-code
-    attributes:
-      label: Wanted Code
-      description: Show me an example of how you would want the code to look like.
-      placeholder: |
-        import typer
-
-
-        def main(name: str):
-            typer.guess_name(f"Hello {name}")
-
-
-        if __name__ == "__main__":
-            typer.run(main)
-      render: python
-    validations:
-      required: true
-  - type: textarea
-    id: alternatives
-    attributes:
-      label: Alternatives
-      description: |
-        Tell me about alternatives you've considered.
-      placeholder: |
-        To hardcode my name, so that if I don't type it it will be the default.
   - type: dropdown
     id: os
     attributes:
       label: Operating System
       description: What operating system are you on?
       multiple: true
       options:
```

### Comparing `typer-0.7.0/.github/actions/comment-docs-preview-in-pr/app/main.py` & `typer-0.8.0/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/.github/workflows/build-docs.yml` & `typer-0.8.0/.github/workflows/build-docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -17,55 +17,55 @@
     steps:
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.7"
       # Allow debugging with tmate
       - name: Setup tmate session
         uses: mxschmitt/action-tmate@v3
         if: ${{ github.event_name == 'workflow_dispatch' && github.event.inputs.debug_enabled }}
         with:
           limit-access-to-actor: true
-      - uses: actions/cache@v2
+      - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-docs-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-v01
       - name: Install Flit
         if: steps.cache.outputs.cache-hit != 'true'
         run: python3.7 -m pip install flit
       - name: Install docs extras
         if: steps.cache.outputs.cache-hit != 'true'
         run: python3.7 -m flit install --extras doc
       - name: Install Material for MkDocs Insiders
         if: ( github.event_name != 'pull_request' || github.event.pull_request.head.repo.fork == false ) && steps.cache.outputs.cache-hit != 'true'
         run: python3.7 -m pip install git+https://${{ secrets.ACTIONS_TOKEN }}@github.com/squidfunk/mkdocs-material-insiders.git
-      - uses: actions/cache@v2
+      - uses: actions/cache@v3
         with:
           key: mkdocs-cards-${{ github.ref }}-v1
           path: .cache
       - name: Build Docs
         if: github.event_name == 'pull_request' && github.event.pull_request.head.repo.fork == true
         run: python3.7 -m mkdocs build
       - name: Build Docs with Insiders
         if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.fork == false
         run: python3.7 -m mkdocs build --config-file mkdocs.insiders.yml
       - name: Zip docs
         run: bash ./scripts/zip-docs.sh
       - uses: actions/upload-artifact@v3
         with:
           name: docs-zip
-          path: ./docs.zip
+          path: ./site/docs.zip
       - name: Deploy to Netlify
-        uses: nwtgck/actions-netlify@v1.2.4
+        uses: nwtgck/actions-netlify@v2.0.0
         with:
           publish-dir: './site'
           production-branch: master
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
```

### Comparing `typer-0.7.0/.github/workflows/issue-manager.yml` & `typer-0.8.0/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/.github/workflows/latest-changes.yml` & `typer-0.8.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/.github/workflows/preview-docs.yml` & `typer-0.8.0/.github/workflows/preview-docs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -7,29 +7,34 @@
       - completed
 
 jobs:
   preview-docs:
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
+      - name: Clean site
+        run: |
+          rm -rf ./site
+          mkdir ./site
       - name: Download Artifact Docs
-        uses: dawidd6/action-download-artifact@v2.9.0
+        uses: dawidd6/action-download-artifact@v2.26.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           workflow: build-docs.yml
           run_id: ${{ github.event.workflow_run.id }}
           name: docs-zip
+          path: ./site/
       - name: Unzip docs
         run: |
-          rm -rf ./site
+          cd ./site
           unzip docs.zip
           rm -f docs.zip
       - name: Deploy to Netlify
         id: netlify
-        uses: nwtgck/actions-netlify@v1.2.4
+        uses: nwtgck/actions-netlify@v2.0.0
         with:
           publish-dir: './site'
           production-deploy: false
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
```

### Comparing `typer-0.7.0/.github/workflows/publish.yml` & `typer-0.8.0/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.7"
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
         run: flit install --symlink
       - name: Publish
```

### Comparing `typer-0.7.0/.github/workflows/smokeshow.yml` & `typer-0.8.0/.github/workflows/smokeshow.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     steps:
       - uses: actions/setup-python@v4
         with:
           python-version: '3.9'
 
       - run: pip install smokeshow
 
-      - uses: dawidd6/action-download-artifact@v2
+      - uses: dawidd6/action-download-artifact@v2.26.0
         with:
           workflow: test.yml
           commit: ${{ github.event.workflow_run.head_sha }}
 
       - run: smokeshow upload coverage-html
         env:
           SMOKESHOW_GITHUB_STATUS_DESCRIPTION: Coverage {coverage-percentage}
```

### Comparing `typer-0.7.0/.github/workflows/test.yml` & `typer-0.8.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
     branches:
       - master
   pull_request:
     types: [opened, synchronize]
 
 jobs:
   test:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
         click-7: [true, false]
       fail-fast: false
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
         if: ${{ matrix.python-version != '3.6' }}
         run: python -m flit install --symlink
```

### Comparing `typer-0.7.0/.pre-commit-config.yaml` & `typer-0.8.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
+default_language_version:
+    python: python3.10
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     -   id: check-added-large-files
     -   id: check-toml
     -   id: check-yaml
         args:
         -   --unsafe
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.0
+    rev: v3.3.1
     hooks:
     -   id: pyupgrade
         args:
         - --py3-plus
         - --keep-runtime-typing
         # This file is more readable without yield from
         exclude: ^docs_src/progressbar/tutorial004\.py
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v1.7.7
+    rev: v2.1.1
     hooks:
     -   id: autoflake
         args:
         - --recursive
         - --in-place
         - --remove-all-unused-imports
         - --remove-unused-variables
         - --expand-star-imports
         - --exclude
         - __init__.py
         - --remove-duplicate-keys
 -   repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     -   id: isort
         name: isort (python)
     -   id: isort
         name: isort (cython)
         types: [cython]
     -   id: isort
         name: isort (pyi)
         types: [pyi]
 -   repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
     -   id: black
 ci:
     autofix_commit_msg: 🎨 [pre-commit.ci] Auto format from pre-commit.com hooks
     autoupdate_commit_msg: ⬆ [pre-commit.ci] pre-commit autoupdate
```

### Comparing `typer-0.7.0/LICENSE` & `typer-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/SECURITY.md` & `typer-0.8.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/alternatives.md` & `typer-0.8.0/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/contributing.md` & `typer-0.8.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/css/termynal.css` & `typer-0.8.0/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/features.md` & `typer-0.8.0/docs/features.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/github-social-preview.png` & `typer-0.8.0/docs/img/github-social-preview.png`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/github-social-preview.svg` & `typer-0.8.0/docs/img/github-social-preview.svg`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/icon-white.svg` & `typer-0.8.0/docs/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/logo-margin/logo-margin-vector.svg` & `typer-0.8.0/docs/img/logo-margin/logo-margin-vector.svg`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/logo-margin/logo-margin.svg` & `typer-0.8.0/docs/img/logo-margin/logo-margin.svg`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/pycharm-completion.png` & `typer-0.8.0/docs/img/pycharm-completion.png`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/img/vscode-completion.png` & `typer-0.8.0/docs/img/vscode-completion.png`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/js/custom.js` & `typer-0.8.0/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/js/termynal.js` & `typer-0.8.0/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/overrides/main.html` & `typer-0.8.0/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/release-notes.md` & `typer-0.8.0/docs/release-notes.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,50 @@
 ## Latest Changes
 
 
+
+## 0.8.0
+
+### Features
+
+* ✨ Add support for custom types and parsers. Initial PR [#583](https://github.com/tiangolo/typer/pull/583) by [@jpurviance](https://github.com/jpurviance). Based on original PR [#443](https://github.com/tiangolo/typer/pull/443) by [@paulo-raca](https://github.com/paulo-raca).
+    * New docs: [CLI Parameter Types: Custom Types](https://typer.tiangolo.com/tutorial/parameter-types/custom-types/).
+
+### Upgrades
+
+* ⬆ Upgrade Rich, support 13.x. PR [#524](https://github.com/tiangolo/typer/pull/524) by [@musicinmybrain](https://github.com/musicinmybrain).
+
+### Docs
+
+* 📝 Tweak docs, Custom Types path, main page and READAME colors, broken links. PR [#588](https://github.com/tiangolo/typer/pull/588) by [@tiangolo](https://github.com/tiangolo).
+* ✏ Fix spelling (shinny -> shiny). PR [#586](https://github.com/tiangolo/typer/pull/586) by [@runofthemill](https://github.com/runofthemill).
+* 📝 Update docs about helping Typer. PR [#547](https://github.com/tiangolo/typer/pull/547) by [@tiangolo](https://github.com/tiangolo).
+* ✏️ Fix typo in datetime docs. PR [#495](https://github.com/tiangolo/typer/pull/495) by [@huxuan](https://github.com/huxuan).
+* ✏️ Add quotes to package name that includes brackets in docs. PR [#475](https://github.com/tiangolo/typer/pull/475) by [@gjolga](https://github.com/gjolga).
+
+### Internal
+
+* ⬆ Bump dawidd6/action-download-artifact from 2.24.2 to 2.26.0. PR [#558](https://github.com/tiangolo/typer/pull/558) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#549](https://github.com/tiangolo/typer/pull/549) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+* 🔧 Add `exclude_lines` to coverage configuration. PR [#585](https://github.com/tiangolo/typer/pull/585) by [@dmontagu](https://github.com/dmontagu).
+* ⬆️ Upgrade analytics. PR [#557](https://github.com/tiangolo/typer/pull/557) by [@tiangolo](https://github.com/tiangolo).
+* 🔧 Update new issue chooser to suggest GitHub Discussions. PR [#544](https://github.com/tiangolo/typer/pull/544) by [@tiangolo](https://github.com/tiangolo).
+* 🔧 Add GitHub Discussion templates for questions. PR [#541](https://github.com/tiangolo/typer/pull/541) by [@tiangolo](https://github.com/tiangolo).
+* 🔧 Update pre-commit, Python version, isort version. PR [#542](https://github.com/tiangolo/typer/pull/542) by [@tiangolo](https://github.com/tiangolo).
+* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#512](https://github.com/tiangolo/typer/pull/512) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+* ⬆ Bump nwtgck/actions-netlify from 1.2.4 to 2.0.0. PR [#513](https://github.com/tiangolo/typer/pull/513) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* 👷 Refactor CI artifact upload/download for docs previews. PR [#516](https://github.com/tiangolo/typer/pull/516) by [@tiangolo](https://github.com/tiangolo).
+* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#500](https://github.com/tiangolo/typer/pull/500) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+* ⬆ Bump actions/cache from 2 to 3. PR [#496](https://github.com/tiangolo/typer/pull/496) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump dawidd6/action-download-artifact from 2.24.1 to 2.24.2. PR [#494](https://github.com/tiangolo/typer/pull/494) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump dawidd6/action-download-artifact from 2.9.0 to 2.24.1. PR [#491](https://github.com/tiangolo/typer/pull/491) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump actions/setup-python from 2 to 4. PR [#492](https://github.com/tiangolo/typer/pull/492) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* 👷‍♂️ Consistently use `sys.executable` to run subprocesses, needed by OpenSUSE. PR [#408](https://github.com/tiangolo/typer/pull/408) by [@theMarix](https://github.com/theMarix).
+* 👷‍♂️ Ensure the `PYTHONPATH` is set properly when testing the tutorial scripts. PR [#407](https://github.com/tiangolo/typer/pull/407) by [@theMarix](https://github.com/theMarix).
+
 ## 0.7.0
 
 ### Features
 
 * ✨ Make `typer.run()` not add completion scripts by default, it only makes sense in installed apps. Also update docs for handling [autocompletion in CLI options](https://typer.tiangolo.com/tutorial/options-autocompletion/). PR [#488](https://github.com/tiangolo/typer/pull/488) by [@tiangolo](https://github.com/tiangolo).
 * ✨ Add support for Python 3.11, tests in CI and official marker. PR [#487](https://github.com/tiangolo/typer/pull/487) by [@tiangolo](https://github.com/tiangolo).
 * 👷 Add CI for Python 3.10. PR [#384](https://github.com/tiangolo/typer/pull/384) by [@tiangolo](https://github.com/tiangolo).
```

### Comparing `typer-0.7.0/docs/tutorial/app-dir.md` & `typer-0.8.0/docs/tutorial/app-dir.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/arguments/default.md` & `typer-0.8.0/docs/tutorial/arguments/default.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/arguments/envvar.md` & `typer-0.8.0/docs/tutorial/arguments/envvar.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/arguments/help.md` & `typer-0.8.0/docs/tutorial/arguments/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/arguments/optional.md` & `typer-0.8.0/docs/tutorial/arguments/optional.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/arguments.md` & `typer-0.8.0/docs/tutorial/commands/arguments.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/callback.md` & `typer-0.8.0/docs/tutorial/commands/callback.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/context.md` & `typer-0.8.0/docs/tutorial/commands/context.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/help.md` & `typer-0.8.0/docs/tutorial/commands/help.md`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 <div class="termy">
 
 ```console
 $ python main.py create --help
 
 <b> </b><font color="#F4BF75"><b>Usage: </b></font><b>main.py create [OPTIONS] USERNAME                     </b>
 <b>                                                                     </b>
- <font color="#A6E22E"><b>Create</b></font> a new <i>shinny</i> user. ✨
+ <font color="#A6E22E"><b>Create</b></font> a new <i>shiny</i> user. ✨
  This requires a <font color="#A5A5A1"><u style="text-decoration-style:single">username</u></font><font color="#A5A5A1">.                                           </font>
 
 <font color="#A5A5A1">╭─ Arguments ───────────────────────────────────────────────────────╮</font>
 <font color="#A5A5A1">│ </font><font color="#F92672">*</font>    username      <font color="#F4BF75"><b>TEXT</b></font>  The username to be <font color="#A6E22E">created</font>               │
 <font color="#A5A5A1">│                          [default: None]                          │</font>
 <font color="#A5A5A1">│                          </font><font color="#A6194C">[required]                </font>               │
 <font color="#A5A5A1">╰───────────────────────────────────────────────────────────────────╯</font>
@@ -268,15 +268,15 @@
 <div class="termy">
 
 ```console
 $ python main.py create --help
 
 <b> </b><font color="#F4BF75"><b>Usage: </b></font><b>main.py create [OPTIONS] USERNAME                     </b>
 <b>                                                                     </b>
- <b>Create</b> a new <i>shinny</i> user. ✨
+ <b>Create</b> a new <i>shiny</i> user. ✨
 
  <font color="#F4BF75"><b> • </b></font><font color="#A5A5A1">Create a username                                                </font>
  <font color="#F4BF75"><b> • </b></font><font color="#A5A5A1">Show that the username is created                                </font>
 
  <font color="#F4BF75">───────────────────────────────────────────────────────────────────</font>
  Learn more at the <font color="#44919F">Typer docs website</font>
```

### Comparing `typer-0.7.0/docs/tutorial/commands/index.md` & `typer-0.8.0/docs/tutorial/commands/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/name.md` & `typer-0.8.0/docs/tutorial/commands/name.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/one-or-multiple.md` & `typer-0.8.0/docs/tutorial/commands/one-or-multiple.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/commands/options.md` & `typer-0.8.0/docs/tutorial/commands/options.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/exceptions.md` & `typer-0.8.0/docs/tutorial/exceptions.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/first-steps.md` & `typer-0.8.0/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/index.md` & `typer-0.8.0/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/launch.md` & `typer-0.8.0/docs/tutorial/launch.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/multiple-values/arguments-with-multiple-values.md` & `typer-0.8.0/docs/tutorial/multiple-values/arguments-with-multiple-values.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/multiple-values/multiple-options.md` & `typer-0.8.0/docs/tutorial/multiple-values/multiple-options.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/multiple-values/options-with-multiple-values.md` & `typer-0.8.0/docs/tutorial/multiple-values/options-with-multiple-values.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options-autocompletion.md` & `typer-0.8.0/docs/tutorial/options-autocompletion.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Review completion
 
 Before checking how to provide custom completions, let's check again how it works.
 
 After installing completion (for your own Python package or for **Typer CLI**), when you use your CLI program and start adding a *CLI option* with `--` an then hit <kbd>TAB</kbd>, your shell will show you the available *CLI options* (the same for *CLI arguments*, etc).
 
-To check it quickly without creating a new Python package, install [Typer CLI](../../typer-cli.md){.internal-link target=_blank}.
+To check it quickly without creating a new Python package, install [Typer CLI](../typer-cli.md){.internal-link target=_blank}.
 
 Then let's create small example program:
 
 ```Python
 {!../docs_src/options_autocompletion/tutorial001.py!}
 ```
 
@@ -44,15 +44,15 @@
 
 </div>
 
 ## Custom completion for values
 
 Right now we get completion for the *CLI option* names, but not for the values.
 
-We can provide completion for the values creating an `autocompletion` function, similar to the `callback` functions from [CLI Option Callback and Context](./callback-and-context.md){.internal-link target=_blank}:
+We can provide completion for the values creating an `autocompletion` function, similar to the `callback` functions from [CLI Option Callback and Context](./options/callback-and-context.md){.internal-link target=_blank}:
 
 ```Python hl_lines="4-5  14"
 {!../docs_src/options_autocompletion/tutorial002.py!}
 ```
 
 We return a `list` of strings from the `complete_name()` function.
 
@@ -269,15 +269,15 @@
 As a simple example, let's show it on the screen before completion.
 
 Because completion is based on the output printed by your program (handled internally by **Typer**), during completion we can't just print something else as we normally do.
 
 ### Printing to "standard error"
 
 !!! tip
-    If you need a refresher about what is "standard output" and "standard error" check the section in [Printing and Colors: "Standard Output" and "Standard Error"](../printing.md#standard-output-and-standard-error){.internal-link target=_blank}.
+    If you need a refresher about what is "standard output" and "standard error" check the section in [Printing and Colors: "Standard Output" and "Standard Error"](./printing.md#standard-output-and-standard-error){.internal-link target=_blank}.
 
 The completion system only reads from "standard output", so, printing to "standard error" won't break completion. 🚀
 
 You can print to "standard error" with a **Rich** `Console(stderr=True)`.
 
 Using `stderr=True` tells **Rich** that the output should be shown in "standard error".
```

### Comparing `typer-0.7.0/docs/tutorial/options/callback-and-context.md` & `typer-0.8.0/docs/tutorial/options/callback-and-context.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options/help.md` & `typer-0.8.0/docs/tutorial/options/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options/name.md` & `typer-0.8.0/docs/tutorial/options/name.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options/password.md` & `typer-0.8.0/docs/tutorial/options/password.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options/prompt.md` & `typer-0.8.0/docs/tutorial/options/prompt.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options/required.md` & `typer-0.8.0/docs/tutorial/options/required.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/options/version.md` & `typer-0.8.0/docs/tutorial/options/version.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/package.md` & `typer-0.8.0/docs/tutorial/package.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ## Dependencies and environment
 
 Add `typer[all]` to your dependencies:
 
 <div class="termy">
 
 ```console
-$ poetry add typer[all]
+$ poetry add "typer[all]"
 
 // It creates a virtual environment for your project
 Creating virtualenv rick-portal-gun-w31dJa0b-py3.6 in /home/rick/.cache/pypoetry/virtualenvs
 Using version ^0.1.0 for typer
 
 Updating dependencies
 Resolving dependencies... (1.2s)
```

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/bool.md` & `typer-0.8.0/docs/tutorial/parameter-types/bool.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/datetime.md` & `typer-0.8.0/docs/tutorial/parameter-types/datetime.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {!../docs_src/parameter_types/datetime/tutorial001.py!}
 ```
 
 Typer will accept any string from the following formats:
 
 * `%Y-%m-%d`
 * `%Y-%m-%dT%H:%M:%S`
-* `%Y-%m%d %H:%M:%S`
+* `%Y-%m-%d %H:%M:%S`
 
 Check it:
 
 <div class="termy">
 
 ```console
 $ python main.py --help
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 You can specify a *CLI parameter* as a Python `datetime`. Your function will
 receive a standard Python `datetime` object, and again, your editor will give
 you completion, etc. ```Python hl_lines="1 6 7 8" {!../docs_src/
 parameter_types/datetime/tutorial001.py!} ``` Typer will accept any string from
-the following formats: * `%Y-%m-%d` * `%Y-%m-%dT%H:%M:%S` * `%Y-%m%d %H:%M:%S`
+the following formats: * `%Y-%m-%d` * `%Y-%m-%dT%H:%M:%S` * `%Y-%m-%d %H:%M:%S`
 Check it:
 ```console $ python main.py --help Usage: main.py [OPTIONS] BIRTH:[%Y-%m-%d|%Y-
 %m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S] Arguments: BIRTH:[%Y-%m-%d|%Y-%m-%dT%H:%M:
 %S|%Y-%m-%d %H:%M:%S][required] Options: --install-completion Install
 completion for the current shell. --show-completion Show completion for the
 current shell, to copy it or customize the installation. --help Show this
 message and exit. // Pass a datetime $ python main.py 1956-01-31T10:00:00
```

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/enum.md` & `typer-0.8.0/docs/tutorial/parameter-types/enum.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/file.md` & `typer-0.8.0/docs/tutorial/parameter-types/file.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/index.md` & `typer-0.8.0/docs/tutorial/parameter-types/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/number.md` & `typer-0.8.0/docs/tutorial/parameter-types/number.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/path.md` & `typer-0.8.0/docs/tutorial/parameter-types/path.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/parameter-types/uuid.md` & `typer-0.8.0/docs/tutorial/parameter-types/uuid.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/printing.md` & `typer-0.8.0/docs/tutorial/printing.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/progressbar.md` & `typer-0.8.0/docs/tutorial/progressbar.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/prompt.md` & `typer-0.8.0/docs/tutorial/prompt.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/subcommands/add-typer.md` & `typer-0.8.0/docs/tutorial/subcommands/add-typer.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/subcommands/callback-override.md` & `typer-0.8.0/docs/tutorial/subcommands/callback-override.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/subcommands/index.md` & `typer-0.8.0/docs/tutorial/subcommands/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/subcommands/name-and-help.md` & `typer-0.8.0/docs/tutorial/subcommands/name-and-help.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/subcommands/nested-subcommands.md` & `typer-0.8.0/docs/tutorial/subcommands/nested-subcommands.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/subcommands/single-file.md` & `typer-0.8.0/docs/tutorial/subcommands/single-file.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/terminating.md` & `typer-0.8.0/docs/tutorial/terminating.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/testing.md` & `typer-0.8.0/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/tutorial/using-click.md` & `typer-0.8.0/docs/tutorial/using-click.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs/typer-cli.md` & `typer-0.8.0/docs/typer-cli.md`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/commands/callback/tutorial001.py` & `typer-0.8.0/docs_src/commands/callback/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/commands/help/tutorial001.py` & `typer-0.8.0/docs_src/commands/help/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/commands/help/tutorial004.py` & `typer-0.8.0/docs_src/commands/help/tutorial004.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @app.command()
 def create(
     username: str = typer.Argument(
         ..., help="The username to be [green]created[/green]"
     )
 ):
     """
-    [bold green]Create[/bold green] a new [italic]shinny[/italic] user. :sparkles:
+    [bold green]Create[/bold green] a new [italic]shiny[/italic] user. :sparkles:
 
     This requires a [underline]username[/underline].
     """
     print(f"Creating user: {username}")
 
 
 @app.command(help="[bold red]Delete[/bold red] a user with [italic]USERNAME[/italic].")
```

### Comparing `typer-0.7.0/docs_src/commands/help/tutorial005.py` & `typer-0.8.0/docs_src/commands/help/tutorial005.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 app = typer.Typer(rich_markup_mode="markdown")
 
 
 @app.command()
 def create(username: str = typer.Argument(..., help="The username to be **created**")):
     """
-    **Create** a new *shinny* user. :sparkles:
+    **Create** a new *shiny* user. :sparkles:
 
     * Create a username
 
     * Show that the username is created
 
     ---
```

### Comparing `typer-0.7.0/docs_src/commands/help/tutorial006.py` & `typer-0.8.0/docs_src/commands/help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/commands/help/tutorial007.py` & `typer-0.8.0/docs_src/commands/help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/commands/options/tutorial001.py` & `typer-0.8.0/docs_src/commands/options/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/launch/tutorial002.py` & `typer-0.8.0/docs_src/launch/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options/help/tutorial002.py` & `typer-0.8.0/docs_src/options/help/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options/version/tutorial002.py` & `typer-0.8.0/docs_src/options/version/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options/version/tutorial003.py` & `typer-0.8.0/docs_src/options/version/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options_autocompletion/tutorial004.py` & `typer-0.8.0/docs_src/options_autocompletion/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options_autocompletion/tutorial005.py` & `typer-0.8.0/docs_src/options_autocompletion/tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options_autocompletion/tutorial007.py` & `typer-0.8.0/docs_src/options_autocompletion/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options_autocompletion/tutorial008.py` & `typer-0.8.0/docs_src/options_autocompletion/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/options_autocompletion/tutorial009.py` & `typer-0.8.0/docs_src/options_autocompletion/tutorial009.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/parameter_types/file/tutorial004.py` & `typer-0.8.0/docs_src/parameter_types/file/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/parameter_types/path/tutorial001.py` & `typer-0.8.0/docs_src/parameter_types/path/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/subcommands/callback_override/tutorial004.py` & `typer-0.8.0/docs_src/subcommands/callback_override/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/subcommands/name_help/tutorial006.py` & `typer-0.8.0/docs_src/subcommands/name_help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/subcommands/name_help/tutorial007.py` & `typer-0.8.0/docs_src/subcommands/name_help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/subcommands/name_help/tutorial008.py` & `typer-0.8.0/docs_src/subcommands/name_help/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/subcommands/tutorial002/main.py` & `typer-0.8.0/docs_src/subcommands/tutorial002/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/terminating/tutorial001.py` & `typer-0.8.0/docs_src/terminating/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/docs_src/using_click/tutorial003.py` & `typer-0.8.0/docs_src/using_click/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/mkdocs.yml` & `typer-0.8.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
           - Number: tutorial/parameter-types/number.md
           - Boolean CLI Options: tutorial/parameter-types/bool.md
           - UUID: tutorial/parameter-types/uuid.md
           - DateTime: tutorial/parameter-types/datetime.md
           - Enum - Choices: tutorial/parameter-types/enum.md
           - Path: tutorial/parameter-types/path.md
           - File: tutorial/parameter-types/file.md
+          - Custom Types: tutorial/parameter-types/custom-types.md
       - SubCommands - Command Groups:
           - SubCommands - Command Groups - Intro: tutorial/subcommands/index.md
           - Add Typer: tutorial/subcommands/add-typer.md
           - SubCommands in a Single File: tutorial/subcommands/single-file.md
           - Nested SubCommands: tutorial/subcommands/nested-subcommands.md
           - Sub-Typer Callback Override: tutorial/subcommands/callback-override.md
           - SubCommand Name and Help: tutorial/subcommands/name-and-help.md
@@ -103,15 +104,15 @@
       alternate_style: true
   - mdx_include:
       base_path: docs
 
 extra:
   analytics:
     provider: google
-    property: UA-133183413-1
+    property: G-T78C5GNRXK
   social:
     - icon: fontawesome/brands/github-alt
       link: https://github.com/tiangolo/typer
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/tiangolo
     - icon: fontawesome/brands/linkedin
       link: https://www.linkedin.com/in/tiangolo
```

### Comparing `typer-0.7.0/pyproject.toml` & `typer-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "pytest-cov >=2.10.0,<5.0.0",
     "coverage >=6.2,<7.0",
     "pytest-xdist >=1.32.0,<4.0.0",
     "pytest-sugar >=0.9.4,<0.10.0",
     "mypy ==0.910",
     "black >=22.3.0,<23.0.0",
     "isort >=5.0.6,<6.0.0",
-    "rich >=10.11.0,<13.0.0",
+    "rich >=10.11.0,<14.0.0",
 ]
 doc = [
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=8.1.4,<9.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "pillow >=9.3.0,<10.0.0",
     "cairosvg >=2.5.2,<3.0.0",
@@ -62,15 +62,15 @@
     "autoflake >=1.3.1,<2.0.0",
     "flake8 >=3.8.3,<4.0.0",
     "pre-commit >=2.17.0,<3.0.0",
 ]
 all = [
     "colorama >=0.4.3,<0.5.0",
     "shellingham >=1.3.0,<2.0.0",
-    "rich >=10.11.0,<13.0.0",
+    "rich >=10.11.0,<14.0.0",
 ]
 
 [tool.isort]
 profile = "black"
 known_third_party = ["typer", "click"]
 skip_glob = [
     "docs_src/subcommands/tutorial001/main.py",
```

### Comparing `typer-0.7.0/tests/assets/compat_click7_8.py` & `typer-0.8.0/tests/assets/compat_click7_8.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/tests/assets/completion_no_types.py` & `typer-0.8.0/tests/assets/completion_no_types.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/tests/assets/completion_no_types_order.py` & `typer-0.8.0/tests/assets/completion_no_types_order.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/tests/test_compat/test_option_get_help.py` & `typer-0.8.0/tests/test_compat/test_option_get_help.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+import sys
 
 import typer.core
 from typer.testing import CliRunner
 
 from tests.assets import compat_click7_8 as mod
 
 runner = CliRunner()
@@ -36,15 +37,15 @@
     result = runner.invoke(mod.app)
     assert result.exit_code == 0
     assert "Hello John Doe, it seems you have 42" in result.output
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_COMPAT_CLICK7_8.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "compat_click7_8.py --nickname ",
```

### Comparing `typer-0.7.0/tests/test_completion/test_completion.py` & `typer-0.8.0/tests/test_completion/test_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     assert ".bash_completions/tutorial001.py.sh" in new_text
     assert "completion installed in" in result.stdout
     assert "Completion will take effect once you restart the terminal" in result.stdout
 
 
 def test_completion_invalid_instruction():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "sourcebash",
             "_TYPER_COMPLETE_TESTING": "True",
@@ -59,15 +59,15 @@
     )
     assert result.returncode != 0
     assert "Invalid completion instruction." in result.stderr
 
 
 def test_completion_source_bash():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_bash",
             "_TYPER_COMPLETE_TESTING": "True",
@@ -77,75 +77,75 @@
         "complete -o default -F _tutorial001py_completion tutorial001.py"
         in result.stdout
     )
 
 
 def test_completion_source_invalid_shell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_xxx",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "Shell xxx not supported." in result.stderr
 
 
 def test_completion_source_invalid_instruction():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "explode_bash",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert 'Completion instruction "explode" not supported.' in result.stderr
 
 
 def test_completion_source_zsh():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_zsh",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "compdef _tutorial001py_completion tutorial001.py" in result.stdout
 
 
 def test_completion_source_fish():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_fish",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "complete --command tutorial001.py --no-files" in result.stdout
 
 
 def test_completion_source_powershell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_powershell",
             "_TYPER_COMPLETE_TESTING": "True",
@@ -155,15 +155,15 @@
         "Register-ArgumentCompleter -Native -CommandName tutorial001.py -ScriptBlock $scriptblock"
         in result.stdout
     )
 
 
 def test_completion_source_pwsh():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__],
+        [sys.executable, "-m", "coverage", "run", mod.__file__],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_pwsh",
             "_TYPER_COMPLETE_TESTING": "True",
```

### Comparing `typer-0.7.0/tests/test_completion/test_completion_complete.py` & `typer-0.8.0/tests/test_completion/test_completion_complete.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import subprocess
+import sys
 
 from docs_src.commands.help import tutorial001 as mod
 
 
 def test_completion_complete_subcommand_bash():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial001.py del",
@@ -19,15 +20,15 @@
         },
     )
     assert "delete\ndelete-all" in result.stdout
 
 
 def test_completion_complete_subcommand_bash_invalid():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial001.py del",
@@ -36,15 +37,15 @@
         },
     )
     assert "create\ndelete\ndelete-all\ninit" in result.stdout
 
 
 def test_completion_complete_subcommand_zsh():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
@@ -55,15 +56,15 @@
         """_arguments '*: :(("delete":"Delete a user with USERNAME."\n"""
         """\"delete-all":"Delete ALL users in the database."))'"""
     ) in result.stdout
 
 
 def test_completion_complete_subcommand_zsh_files():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py delete ",
@@ -71,15 +72,15 @@
         },
     )
     assert ("_files") in result.stdout
 
 
 def test_completion_complete_subcommand_fish():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
@@ -91,15 +92,15 @@
         "delete\tDelete a user with USERNAME.\ndelete-all\tDelete ALL users in the database."
         in result.stdout
     )
 
 
 def test_completion_complete_subcommand_fish_should_complete():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
@@ -108,15 +109,15 @@
         },
     )
     assert result.returncode == 0
 
 
 def test_completion_complete_subcommand_fish_should_complete_no():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py delete ",
@@ -125,15 +126,15 @@
         },
     )
     assert result.returncode != 0
 
 
 def test_completion_complete_subcommand_powershell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_powershell",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
@@ -143,15 +144,15 @@
     assert (
         "delete:::Delete a user with USERNAME.\ndelete-all:::Delete ALL users in the database."
     ) in result.stdout
 
 
 def test_completion_complete_subcommand_pwsh():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_pwsh",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
@@ -161,15 +162,15 @@
     assert (
         "delete:::Delete a user with USERNAME.\ndelete-all:::Delete ALL users in the database."
     ) in result.stdout
 
 
 def test_completion_complete_subcommand_noshell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_noshell",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
```

### Comparing `typer-0.7.0/tests/test_completion/test_completion_complete_no_help.py` & `typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,46 @@
 import os
 import subprocess
+import sys
 
-from docs_src.commands.index import tutorial002 as mod
+from typer.testing import CliRunner
 
+from docs_src.options_autocompletion import tutorial008 as mod
 
-def test_completion_complete_subcommand_zsh():
-    result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        encoding="utf-8",
-        env={
-            **os.environ,
-            "_TUTORIAL002.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_TESTING": "True",
-        },
-    )
-    assert "create" in result.stdout
-    assert "delete" in result.stdout
+runner = CliRunner()
 
 
-def test_completion_complete_subcommand_fish():
+def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL002.PY_COMPLETE": "complete_fish",
-            "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_FISH_ACTION": "get-args",
+            "_TUTORIAL008.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial008.py --name ",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
-    assert "create\ndelete" in result.stdout
+    assert '"Camila":"The reader of books."' in result.stdout
+    assert '"Carlos":"The writer of scripts."' in result.stdout
+    assert '"Sebastian":"The type hints guy."' in result.stdout
+    # TODO: when deprecating Click 7, remove second option
+    assert "[]" in result.stderr or "['--name']" in result.stderr
 
 
-def test_completion_complete_subcommand_powershell():
-    result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        encoding="utf-8",
-        env={
-            **os.environ,
-            "_TUTORIAL002.PY_COMPLETE": "complete_powershell",
-            "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_TESTING": "True",
-        },
-    )
-    assert ("create::: \ndelete::: ") in result.stdout
+def test_1():
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
+    assert result.exit_code == 0
+    assert "Hello Camila" in result.output
+    assert "Hello Sebastian" in result.output
 
 
-def test_completion_complete_subcommand_pwsh():
+def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
-        env={
-            **os.environ,
-            "_TUTORIAL002.PY_COMPLETE": "complete_pwsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_TESTING": "True",
-        },
     )
-    assert ("create::: \ndelete::: ") in result.stdout
+    assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_completion/test_completion_install.py` & `typer-0.8.0/tests/test_completion/test_completion_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+import sys
 from pathlib import Path
 from unittest import mock
 
 import shellingham
 import typer
 from typer.testing import CliRunner
 
@@ -12,15 +13,15 @@
 runner = CliRunner()
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_completion_install_no_shell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--install-completion"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--install-completion"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
@@ -35,15 +36,23 @@
 
 def test_completion_install_bash():
     bash_completion_path: Path = Path.home() / ".bashrc"
     text = ""
     if bash_completion_path.is_file():
         text = bash_completion_path.read_text()
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--install-completion", "bash"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--install-completion",
+            "bash",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
@@ -70,15 +79,23 @@
     completion_path: Path = Path.home() / ".zshrc"
     text = ""
     if not completion_path.is_file():  # pragma: nocover
         completion_path.write_text('echo "custom .zshrc"')
     if completion_path.is_file():
         text = completion_path.read_text()
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--install-completion", "zsh"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--install-completion",
+            "zsh",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
@@ -99,15 +116,23 @@
 
 def test_completion_install_fish():
     script_path = Path(mod.__file__)
     completion_path: Path = (
         Path.home() / f".config/fish/completions/{script_path.name}.fish"
     )
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--install-completion", "fish"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--install-completion",
+            "fish",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
```

### Comparing `typer-0.7.0/tests/test_completion/test_completion_show.py` & `typer-0.8.0/tests/test_completion/test_completion_show.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import subprocess
+import sys
 
 from docs_src.commands.index import tutorial001 as mod
 
 
 def test_completion_show_no_shell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--show-completion"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--show-completion"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
@@ -21,15 +22,23 @@
         "Option '--show-completion' requires an argument" in result.stderr
         or "--show-completion option requires an argument" in result.stderr
     )
 
 
 def test_completion_show_bash():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--show-completion", "bash"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--show-completion",
+            "bash",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
@@ -39,45 +48,69 @@
         "complete -o default -F _tutorial001py_completion tutorial001.py"
         in result.stdout
     )
 
 
 def test_completion_source_zsh():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--show-completion", "zsh"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--show-completion",
+            "zsh",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert "compdef _tutorial001py_completion tutorial001.py" in result.stdout
 
 
 def test_completion_source_fish():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--show-completion", "fish"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--show-completion",
+            "fish",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert "complete --command tutorial001.py --no-files" in result.stdout
 
 
 def test_completion_source_powershell():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--show-completion", "powershell"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--show-completion",
+            "powershell",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
@@ -87,15 +120,23 @@
         "Register-ArgumentCompleter -Native -CommandName tutorial001.py -ScriptBlock $scriptblock"
         in result.stdout
     )
 
 
 def test_completion_source_pwsh():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--show-completion", "pwsh"],
+        [
+            sys.executable,
+            "-m",
+            "coverage",
+            "run",
+            mod.__file__,
+            "--show-completion",
+            "pwsh",
+        ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
```

### Comparing `typer-0.7.0/tests/test_exit_errors.py` & `typer-0.8.0/tests/test_exit_errors.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/tests/test_others.py` & `typer-0.8.0/tests/test_others.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 import subprocess
+import sys
+import typing
 from pathlib import Path
 from unittest import mock
 
 import click
 import pytest
 import shellingham
 import typer
 import typer.completion
 from typer.main import solve_typer_info_defaults, solve_typer_info_help
-from typer.models import TyperInfo
+from typer.models import ParameterInfo, TyperInfo
 from typer.testing import CliRunner
 
 runner = CliRunner()
 
 
 def test_help_from_info():
     # Mainly for coverage/completeness
@@ -23,14 +25,58 @@
 
 def test_defaults_from_info():
     # Mainly for coverage/completeness
     value = solve_typer_info_defaults(TyperInfo())
     assert value
 
 
+def test_too_may_parsers():
+    def custom_parser(value: str) -> int:
+        return int(value)  # pragma: no cover
+
+    class CustomClickParser(click.ParamType):
+        name = "custom_parser"
+
+        def convert(
+            self,
+            value: str,
+            param: typing.Optional[click.Parameter],
+            ctx: typing.Optional[click.Context],
+        ) -> typing.Any:
+            return int(value)  # pragma: no cover
+
+    expected_error = (
+        "Multiple custom type parsers provided. "
+        "`parser` and `click_type` may not both be provided."
+    )
+
+    with pytest.raises(ValueError, match=expected_error):
+        ParameterInfo(parser=custom_parser, click_type=CustomClickParser())
+
+
+def test_valid_parser_permutations():
+    def custom_parser(value: str) -> int:
+        return int(value)  # pragma: no cover
+
+    class CustomClickParser(click.ParamType):
+        name = "custom_parser"
+
+        def convert(
+            self,
+            value: str,
+            param: typing.Optional[click.Parameter],
+            ctx: typing.Optional[click.Context],
+        ) -> typing.Any:
+            return int(value)  # pragma: no cover
+
+    ParameterInfo()
+    ParameterInfo(parser=custom_parser)
+    ParameterInfo(click_type=CustomClickParser())
+
+
 def test_install_invalid_shell():
     app = typer.Typer()
 
     @app.command()
     def main():
         print("Hello World")
 
@@ -93,15 +139,15 @@
     assert "param name is: name" in result.stdout
     assert "value is: Camila" in result.stdout
 
 
 def test_completion_untyped_parameters():
     file_path = Path(__file__).parent / "assets/completion_no_types.py"
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_COMPLETION_NO_TYPES.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "completion_no_types.py --name Sebastian --name Ca",
@@ -115,26 +161,26 @@
         or "args is: ['--name', 'Sebastian', '--name']" in result.stderr
     )
     assert "incomplete is: Ca" in result.stderr
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
 
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Hello World" in result.stdout
 
 
 def test_completion_untyped_parameters_different_order_correct_names():
     file_path = Path(__file__).parent / "assets/completion_no_types_order.py"
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_COMPLETION_NO_TYPES_ORDER.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "completion_no_types_order.py --name Sebastian --name Ca",
@@ -148,15 +194,15 @@
         or "args is: ['--name', 'Sebastian', '--name']" in result.stderr
     )
     assert "incomplete is: Ca" in result.stderr
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
 
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Hello World" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_rich_utils.py` & `typer-0.8.0/tests/test_rich_utils.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/tests/test_tracebacks.py` & `typer-0.8.0/tests/test_tracebacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import subprocess
+import sys
 from pathlib import Path
 
 
 def test_traceback_no_rich():
     file_path = Path(__file__).parent / "assets/type_error_no_rich.py"
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
     assert "return get_command(self)(*args, **kwargs)" not in result.stderr
 
@@ -22,15 +23,15 @@
         or "TypeError: must be str, not int" in result.stderr
     )
 
 
 def test_traceback_no_rich_short_disable():
     file_path = Path(__file__).parent / "assets/type_error_no_rich_short_disable.py"
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
     assert "return get_command(self)(*args, **kwargs)" not in result.stderr
 
@@ -42,15 +43,15 @@
         or "TypeError: must be str, not int" in result.stderr
     )
 
 
 def test_unmodified_traceback():
     file_path = Path(__file__).parent / "assets/type_error_normal_traceback.py"
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
     assert "morty" in result.stdout, "the call to the first app should work normally"
     assert "return callback(**use_params)" in result.stderr, (
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.arguments.default import tutorial001 as mod
+from docs_src.arguments.help import tutorial005 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "[OPTIONS] [NAME]" in result.output
     assert "Arguments" in result.output
-    assert "[default: Wade Wilson]" in result.output
-
-
-def test_call_no_arg():
-    result = runner.invoke(app)
-    assert result.exit_code == 0
-    assert "Hello Wade Wilson" in result.output
+    assert "Who to greet" in result.output
+    assert "[default: (Deadpoolio the amazing's name)]" in result.output
 
 
 def test_call_arg():
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.arguments.default import tutorial002 as mod
 
 runner = CliRunner()
@@ -31,13 +32,13 @@
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
 from docs_src.arguments.envvar import tutorial001 as mod
 
@@ -49,13 +50,13 @@
     result = runner.invoke(app, ["Czernobog"], env={"AWESOME_NAME": "Wednesday"})
     assert result.exit_code == 0
     assert "Hello Mr. Czernobog" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.arguments.envvar import tutorial002 as mod
 
 runner = CliRunner()
@@ -36,13 +37,13 @@
     result = runner.invoke(app, env={"GOD_NAME": "Anubis"})
     assert result.exit_code == 0
     assert "Hello Mr. Anubis" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.arguments.envvar import tutorial003 as mod
 
 runner = CliRunner()
@@ -36,13 +37,13 @@
     result = runner.invoke(app, ["Czernobog"], env={"AWESOME_NAME": "Wednesday"})
     assert result.exit_code == 0
     assert "Hello Mr. Czernobog" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
 from docs_src.arguments.help import tutorial001 as mod
 
@@ -39,13 +40,13 @@
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_index/test_tutorial002.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import subprocess
+import sys
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.arguments.help import tutorial002 as mod
+from docs_src.commands.index import tutorial002 as mod
 
-runner = CliRunner()
+app = mod.app
 
-app = typer.Typer()
-app.command()(mod.main)
+runner = CliRunner()
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "[OPTIONS] NAME" in result.output
-    assert "Say hi to NAME very gently, like Dirk." in result.output
-    assert "Arguments" in result.output
-    assert "NAME" in result.output
-    assert "The name of the user to greet" in result.output
-    assert "[required]" in result.output
+    assert "[OPTIONS] COMMAND [ARGS]..." in result.output
+    assert "Commands" in result.output
+    assert "create" in result.output
+    assert "delete" in result.output
+
+
+def test_create():
+    result = runner.invoke(app, ["create"])
+    assert result.exit_code == 0
+    assert "Creating user: Hiro Hamada" in result.output
 
 
-def test_call_arg():
-    result = runner.invoke(app, ["Camila"])
+def test_delete():
+    result = runner.invoke(app, ["delete"])
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
+    assert "Deleting user: Hiro Hamada" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.arguments.help import tutorial003 as mod
 
 runner = CliRunner()
@@ -26,13 +27,13 @@
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.arguments.help import tutorial004 as mod
 
 runner = CliRunner()
@@ -26,13 +27,13 @@
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial002.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.arguments.help import tutorial005 as mod
+from docs_src.options.name import tutorial002 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_help():
+def test_option_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "[OPTIONS] [NAME]" in result.output
-    assert "Arguments" in result.output
-    assert "Who to greet" in result.output
-    assert "[default: (Deadpoolio the amazing's name)]" in result.output
+    assert "-n" in result.output
+    assert "--name" in result.output
+    assert "TEXT" in result.output
+    assert "--user-name" not in result.output
 
 
-def test_call_arg():
-    result = runner.invoke(app, ["Camila"])
+def test_call():
+    result = runner.invoke(app, ["-n", "Camila"])
+    assert result.exit_code == 0
+    assert "Hello Camila" in result.output
+
+
+def test_call_long():
+    result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.arguments.help import tutorial006 as mod
+from docs_src.parameter_types.bool import tutorial003 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "[OPTIONS] ✨username✨" in result.output
-    assert "Arguments" in result.output
-    assert "✨username✨" in result.output
-    assert "[default: World]" in result.output
+    assert "-f" in result.output
+    assert "--force" in result.output
+    assert "-F" in result.output
+    assert "--no-force" in result.output
 
 
-def test_call_arg():
-    result = runner.invoke(app, ["Camila"])
+def test_force():
+    result = runner.invoke(app, ["-f"])
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
+    assert "Forcing operation" in result.output
+
+
+def test_no_force():
+    result = runner.invoke(app, ["-F"])
+    assert result.exit_code == 0
+    assert "Not forcing" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import subprocess
+import sys
 
-import typer
-import typer.core
 from typer.testing import CliRunner
 
-from docs_src.arguments.help import tutorial007 as mod
+from docs_src.commands.callback import tutorial004 as mod
 
-runner = CliRunner()
+app = mod.app
 
-app = typer.Typer()
-app.command()(mod.main)
+runner = CliRunner()
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "Say hi to NAME very gently, like Dirk." in result.output
-    assert "Arguments" in result.output
-    assert "Secondary Arguments" in result.output
+    assert "Manage users CLI app." in result.output
+    assert "Use it with the create command." in result.output
+    assert "A new user with the given NAME will be created." in result.output
 
 
-def test_call_arg():
-    result = runner.invoke(app, ["Camila"])
+def test_app():
+    result = runner.invoke(app, ["create", "Camila"])
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
+    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
 from docs_src.arguments.help import tutorial008 as mod
 
@@ -37,13 +38,13 @@
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_terminating/test_tutorial003.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
-from docs_src.arguments.optional import tutorial001 as mod
+from docs_src.terminating import tutorial003 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_call_no_arg():
-    result = runner.invoke(app)
-    assert result.exit_code != 0
-    assert "Missing argument 'NAME'." in result.output
+def test_cli():
+    result = runner.invoke(app, ["Camila"])
+    assert result.exit_code == 0
+    assert "New user created: Camila" in result.output
+
+
+def test_root():
+    result = runner.invoke(app, ["root"])
+    assert result.exit_code == 1
+    assert "The root user is reserved" in result.output
+    assert "Aborted" in result.output
 
 
-def test_call_no_arg_standalone():
+def test_root_no_standalone():
     # Mainly for coverage
-    result = runner.invoke(app, standalone_mode=False)
-    assert result.exit_code != 0
+    result = runner.invoke(app, ["root"], standalone_mode=False)
+    assert result.exit_code == 1
 
 
-def test_call_no_arg_no_rich():
+def test_root_no_rich():
     # Mainly for coverage
     rich = typer.core.rich
     typer.core.rich = None
-    result = runner.invoke(app)
-    assert result.exit_code != 0
-    assert "Error: Missing argument 'NAME'" in result.stdout
+    result = runner.invoke(app, ["root"])
+    assert result.exit_code == 1
+    assert "The root user is reserved" in result.stdout
+    assert "Aborted!" in result.stdout
     typer.core.rich = rich
 
 
-def test_call_arg():
-    result = runner.invoke(app, ["Camila"])
-    assert result.exit_code == 0
-    assert "Hello Camila" in result.output
-
-
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.arguments.optional import tutorial002 as mod
+from docs_src.arguments.default import tutorial001 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "[OPTIONS] [NAME]" in result.output
+    assert "Arguments" in result.output
+    assert "[default: Wade Wilson]" in result.output
 
 
 def test_call_no_arg():
     result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "Hello World!" in result.output
+    assert "Hello Wade Wilson" in result.output
 
 
 def test_call_arg():
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 import subprocess
+import sys
 
+import typer
 from typer.testing import CliRunner
 
-from docs_src.commands.arguments import tutorial001 as mod
-
-app = mod.app
+from docs_src.parameter_types.bool import tutorial004 as mod
 
 runner = CliRunner()
 
+app = typer.Typer()
+app.command()(mod.main)
+
 
-def test_help_create():
-    result = runner.invoke(app, ["create", "--help"])
+def test_help():
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "create [OPTIONS] USERNAME" in result.output
+    assert "-d" in result.output
+    assert "--demo" in result.output
 
 
-def test_help_delete():
-    result = runner.invoke(app, ["delete", "--help"])
+def test_main():
+    result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "delete [OPTIONS] USERNAME" in result.output
+    assert "Running in production" in result.output
 
 
-def test_create():
-    result = runner.invoke(app, ["create", "Camila"])
+def test_demo():
+    result = runner.invoke(app, ["--demo"])
     assert result.exit_code == 0
-    assert "Creating user: Camila" in result.output
+    assert "Running demo" in result.output
 
 
-def test_delete():
-    result = runner.invoke(app, ["delete", "Camila"])
+def test_short_demo():
+    result = runner.invoke(app, ["-d"])
     assert result.exit_code == 0
-    assert "Deleting user: Camila" in result.output
+    assert "Running demo" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer.core
 from typer.testing import CliRunner
 
 from docs_src.commands.callback import tutorial001 as mod
 
 app = mod.app
@@ -67,13 +68,13 @@
         "No such option: --verbose" in result.output
         or "no such option: --verbose" in result.output
     )
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.callback import tutorial002 as mod
 
 app = mod.app
 
@@ -14,13 +15,13 @@
     assert result.exit_code == 0
     assert "Running a command" in result.output
     assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.callback import tutorial003 as mod
 
 app = mod.app
 
@@ -19,13 +20,13 @@
 
 def test_for_coverage():
     mod.callback()
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.callback import tutorial004 as mod
-
-app = mod.app
+from docs_src.subcommands.name_help import tutorial006 as mod
 
 runner = CliRunner()
 
+app = mod.app
+
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "Manage users CLI app." in result.output
-    assert "Use it with the create command." in result.output
-    assert "A new user with the given NAME will be created." in result.output
+    assert "Commands" in result.output
+    assert "exp-users" in result.output
+    assert "Explicit help." in result.output
+
+
+def test_command_help():
+    result = runner.invoke(app, ["exp-users", "--help"])
+    assert result.exit_code == 0
+    assert "Explicit help." in result.output
 
 
-def test_app():
-    result = runner.invoke(app, ["create", "Camila"])
+def test_command():
+    result = runner.invoke(app, ["exp-users", "create", "Camila"])
     assert result.exit_code == 0
     assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.context import tutorial001 as mod
+from docs_src.commands.arguments import tutorial001 as mod
 
 app = mod.app
 
 runner = CliRunner()
 
 
+def test_help_create():
+    result = runner.invoke(app, ["create", "--help"])
+    assert result.exit_code == 0
+    assert "create [OPTIONS] USERNAME" in result.output
+
+
+def test_help_delete():
+    result = runner.invoke(app, ["delete", "--help"])
+    assert result.exit_code == 0
+    assert "delete [OPTIONS] USERNAME" in result.output
+
+
 def test_create():
     result = runner.invoke(app, ["create", "Camila"])
     assert result.exit_code == 0
-    assert "About to execute command: create" in result.output
     assert "Creating user: Camila" in result.output
 
 
 def test_delete():
     result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
-    assert "About to execute command: delete" in result.output
     assert "Deleting user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import subprocess
+import sys
 
+import typer
 from typer.testing import CliRunner
 
-from docs_src.commands.context import tutorial002 as mod
-
-app = mod.app
+from docs_src.multiple_values.multiple_options import tutorial002 as mod
 
 runner = CliRunner()
+app = typer.Typer()
+app.command()(mod.main)
 
 
-def test_create():
-    result = runner.invoke(app, ["create", "Camila"])
+def test_main():
+    result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "Initializing database" in result.output
-    assert "Creating user: Camila" in result.output
+    assert "The sum is 0" in result.output
 
 
-def test_delete():
-    result = runner.invoke(app, ["delete", "Camila"])
+def test_1_number():
+    result = runner.invoke(app, ["--number", "2"])
     assert result.exit_code == 0
-    assert "Initializing database" in result.output
-    assert "Deleting user: Camila" in result.output
+    assert "The sum is 2.0" in result.output
 
 
-def test_callback():
-    result = runner.invoke(app)
+def test_2_number():
+    result = runner.invoke(app, ["--number", "2", "--number", "3", "--number", "4.5"])
     assert result.exit_code == 0
-    assert "Initializing database" in result.output
+    assert "The sum is 9.5" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.context import tutorial003 as mod
-
-app = mod.app
+from docs_src.subcommands.name_help import tutorial002 as mod
 
 runner = CliRunner()
 
+app = mod.app
+
 
-def test_create():
-    result = runner.invoke(app, ["create", "Camila"])
+def test_help():
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "Initializing database" not in result.output
-    assert "Creating user: Camila" in result.output
+    assert "Commands" in result.output
+    assert "users" in result.output
+    assert "Manage users in the app." in result.output
 
 
-def test_delete():
-    result = runner.invoke(app, ["delete", "Camila"])
+def test_command_help():
+    result = runner.invoke(app, ["users", "--help"])
     assert result.exit_code == 0
-    assert "Initializing database" not in result.output
-    assert "Deleting user: Camila" in result.output
+    assert "Manage users in the app." in result.output
 
 
-def test_callback():
-    result = runner.invoke(app)
+def test_command():
+    result = runner.invoke(app, ["users", "create", "Camila"])
     assert result.exit_code == 0
-    assert "Initializing database" in result.output
+    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.context import tutorial004 as mod
+from docs_src.commands.one_or_multiple import tutorial002 as mod
 
 app = mod.app
 
 runner = CliRunner()
 
 
-def test_1():
-    result = runner.invoke(app, ["--name", "Camila", "--city", "Berlin"])
+def test_help():
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "Got extra arg: --name" in result.output
-    assert "Got extra arg: Camila" in result.output
-    assert "Got extra arg: --city" in result.output
-    assert "Got extra arg: Berlin" in result.output
+    assert "Creates a single user Hiro Hamada." in result.output
+    assert "In the next version it will create 5 users more." in result.output
+    assert "Commands" in result.output
+    assert "create" in result.output
+
+
+def test_command():
+    result = runner.invoke(app, ["create"])
+    assert result.exit_code == 0
+    assert "Creating user: Hiro Hamada" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial001.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial001 as mod
 
 app = mod.app
 
@@ -113,13 +114,13 @@
     result = runner.invoke(app, ["init"])
     assert result.exit_code == 0
     assert "Initializing user database" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial002.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial002 as mod
 
 app = mod.app
 
@@ -44,13 +45,13 @@
     result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
     assert "Deleting user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial003.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial003 as mod
 
 app = mod.app
 
@@ -32,13 +33,13 @@
     assert result.exit_code == 0
     result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial004.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial004 as mod
 
 app = mod.app
 
 runner = CliRunner()
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "create" in result.output
-    assert "Create a new shinny user. ✨" in result.output
+    assert "Create a new shiny user. ✨" in result.output
     assert "delete" in result.output
     assert "Delete a user with USERNAME." in result.output
     assert "Some internal utility function to create." not in result.output
     assert "Some internal utility function to delete." not in result.output
 
 
 def test_help_create():
     result = runner.invoke(app, ["create", "--help"])
     assert result.exit_code == 0
-    assert "Create a new shinny user. ✨" in result.output
+    assert "Create a new shiny user. ✨" in result.output
     assert "The username to be created" in result.output
     assert "Some internal utility function to create." not in result.output
 
 
 def test_help_delete():
     result = runner.invoke(app, ["delete", "--help"])
     assert result.exit_code == 0
@@ -47,13 +48,13 @@
     result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
     assert "Deleting user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial005.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial005.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial005 as mod
 
 app = mod.app
 
 runner = CliRunner()
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "create" in result.output
-    assert "Create a new shinny user. ✨" in result.output
+    assert "Create a new shiny user. ✨" in result.output
     assert "delete" in result.output
     assert "Delete a user with USERNAME." in result.output
     assert "Some internal utility function to create." not in result.output
     assert "Some internal utility function to delete." not in result.output
 
 
 def test_help_create():
     result = runner.invoke(app, ["create", "--help"])
     assert result.exit_code == 0
-    assert "Create a new shinny user. ✨" in result.output
+    assert "Create a new shiny user. ✨" in result.output
     assert "The username to be created" in result.output
     assert "Learn more at the Typer docs website" in result.output
     assert "Some internal utility function to create." not in result.output
 
 
 def test_help_delete():
     result = runner.invoke(app, ["delete", "--help"])
@@ -48,13 +49,13 @@
     result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
     assert "Deleting user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial006.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial006.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial006 as mod
 
 app = mod.app
 
@@ -39,13 +40,13 @@
     assert result.exit_code == 0
     result = runner.invoke(app, ["report"])
     assert result.exit_code == 0
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial007.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial007.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.help import tutorial007 as mod
 
 app = mod.app
 
@@ -43,13 +44,13 @@
     assert result.exit_code == 0
     result = runner.invoke(app, ["config", "Morty"])
     assert result.exit_code == 0
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial008.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.help import tutorial008 as mod
-
-app = mod.app
+from docs_src.subcommands.callback_override import tutorial003 as mod
 
 runner = CliRunner()
 
+app = mod.app
 
-def test_main_help():
-    result = runner.invoke(app, ["--help"])
+
+def test_cli():
+    result = runner.invoke(app, ["users", "create", "Camila"])
     assert result.exit_code == 0
-    assert "Create a new user. ✨" in result.output
-    assert "Made with ❤ in Venus" in result.output
+    assert "Running a users command" not in result.output
+    assert "Callback override, running users command" in result.output
+    assert "Creating user: Camila" in result.output
 
 
-def test_call():
-    # Mainly for coverage
-    result = runner.invoke(app, ["Morty"])
-    assert result.exit_code == 0
+def test_for_coverage():
+    mod.default_callback()
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.index import tutorial001 as mod
+from docs_src.subcommands.name_help import tutorial005 as mod
+
+runner = CliRunner()
 
 app = mod.app
 
-runner = CliRunner()
+
+def test_help():
+    result = runner.invoke(app, ["--help"])
+    assert result.exit_code == 0
+    assert "Commands" in result.output
+    assert "new-users" in result.output
+    assert "I have the highland! Create some users." in result.output
 
 
-def test_no_arg():
-    result = runner.invoke(app)
-    assert result.exit_code != 0
-    assert "Missing argument 'NAME'." in result.output
+def test_command_help():
+    result = runner.invoke(app, ["new-users", "--help"])
+    assert result.exit_code == 0
+    assert "I have the highland! Create some users." in result.output
 
 
-def test_arg():
-    result = runner.invoke(app, ["Camila"])
+def test_command():
+    result = runner.invoke(app, ["new-users", "create", "Camila"])
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
+    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_terminating/test_tutorial002.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import subprocess
+import sys
 
+import typer
 from typer.testing import CliRunner
 
-from docs_src.commands.index import tutorial002 as mod
-
-app = mod.app
+from docs_src.terminating import tutorial002 as mod
 
 runner = CliRunner()
 
-
-def test_help():
-    result = runner.invoke(app, ["--help"])
-    assert result.exit_code == 0
-    assert "[OPTIONS] COMMAND [ARGS]..." in result.output
-    assert "Commands" in result.output
-    assert "create" in result.output
-    assert "delete" in result.output
+app = typer.Typer()
+app.command()(mod.main)
 
 
-def test_create():
-    result = runner.invoke(app, ["create"])
+def test_cli():
+    result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
-    assert "Creating user: Hiro Hamada" in result.output
+    assert "New user created: Camila" in result.output
 
 
-def test_delete():
-    result = runner.invoke(app, ["delete"])
-    assert result.exit_code == 0
-    assert "Deleting user: Hiro Hamada" in result.output
+def test_root():
+    result = runner.invoke(app, ["root"])
+    assert result.exit_code == 1
+    assert "The root user is reserved" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_name/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.name import tutorial001 as mod
+from docs_src.commands.one_or_multiple import tutorial001 as mod
 
 app = mod.app
 
 runner = CliRunner()
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "Commands" in result.output
     assert "create" in result.output
-    assert "delete" in result.output
 
 
-def test_create():
-    result = runner.invoke(app, ["create", "Camila"])
+def test_command():
+    result = runner.invoke(app, ["create"])
     assert result.exit_code == 0
-    assert "Creating user: Camila" in result.output
-
-
-def test_delete():
-    result = runner.invoke(app, ["delete", "Camila"])
-    assert result.exit_code == 0
-    assert "Deleting user: Camila" in result.output
+    assert "Creating user: Hiro Hamada" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.one_or_multiple import tutorial001 as mod
-
-app = mod.app
+from docs_src.subcommands.name_help import tutorial001 as mod
 
 runner = CliRunner()
 
+app = mod.app
+
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "Commands" in result.output
-    assert "create" in result.output
+    assert "users" in result.output
+    assert "Manage users in the app." in result.output
+
+
+def test_command_help():
+    result = runner.invoke(app, ["users", "--help"])
+    assert result.exit_code == 0
+    assert "Manage users in the app." in result.output
 
 
 def test_command():
-    result = runner.invoke(app, ["create"])
+    result = runner.invoke(app, ["users", "create", "Camila"])
     assert result.exit_code == 0
-    assert "Creating user: Hiro Hamada" in result.output
+    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_name/test_tutorial001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.commands.one_or_multiple import tutorial002 as mod
+from docs_src.commands.name import tutorial001 as mod
 
 app = mod.app
 
 runner = CliRunner()
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "Creates a single user Hiro Hamada." in result.output
-    assert "In the next version it will create 5 users more." in result.output
     assert "Commands" in result.output
     assert "create" in result.output
+    assert "delete" in result.output
 
 
-def test_command():
-    result = runner.invoke(app, ["create"])
+def test_create():
+    result = runner.invoke(app, ["create", "Camila"])
     assert result.exit_code == 0
-    assert "Creating user: Hiro Hamada" in result.output
+    assert "Creating user: Camila" in result.output
+
+
+def test_delete():
+    result = runner.invoke(app, ["delete", "Camila"])
+    assert result.exit_code == 0
+    assert "Deleting user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_commands/test_options/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_options/test_tutorial001.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.commands.options import tutorial001 as mod
 
 app = mod.app
 
@@ -84,13 +85,13 @@
     result = runner.invoke(app, ["init"])
     assert result.exit_code == 0
     assert "Initializing user database" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial001.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 import subprocess
+import sys
 from pathlib import Path
 
 from typer.testing import CliRunner
 
 from docs_src.exceptions import tutorial001 as mod
 
 runner = CliRunner()
 
 
 def test_traceback_rich():
     file_path = Path(mod.__file__)
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
     assert "return get_command(self)(*args, **kwargs)" not in result.stderr
 
@@ -30,15 +31,15 @@
     )
     assert "name = 'morty'" in result.stderr
 
 
 def test_standard_traceback_env_var():
     file_path = Path(mod.__file__)
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": "1"},
     )
     assert "return get_command(self)(*args, **kwargs)" in result.stderr
 
@@ -51,13 +52,13 @@
         or "TypeError: must be str, not int" in result.stderr
     )
     assert "name = 'morty'" not in result.stderr
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial002.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 import subprocess
+import sys
 from pathlib import Path
 
 from typer.testing import CliRunner
 
 from docs_src.exceptions import tutorial002 as mod
 
 runner = CliRunner()
 
 
 def test_traceback_rich():
     file_path = Path(mod.__file__)
     result = subprocess.run(
-        ["coverage", "run", str(file_path), "secret"],
+        [sys.executable, "-m", "coverage", "run", str(file_path), "secret"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
     assert "return get_command(self)(*args, **kwargs)" not in result.stderr
 
@@ -30,15 +31,15 @@
     )
     assert "name = 'morty'" not in result.stderr
 
 
 def test_standard_traceback_env_var():
     file_path = Path(mod.__file__)
     result = subprocess.run(
-        ["coverage", "run", str(file_path), "secret"],
+        [sys.executable, "-m", "coverage", "run", str(file_path), "secret"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": "1"},
     )
     assert "return get_command(self)(*args, **kwargs)" in result.stderr
 
@@ -51,13 +52,13 @@
         or "TypeError: must be str, not int" in result.stderr
     )
     assert "name = 'morty'" not in result.stderr
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial004.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import os
 import subprocess
+import sys
 from pathlib import Path
 
 from typer.testing import CliRunner
 
-from docs_src.exceptions import tutorial003 as mod
+from docs_src.exceptions import tutorial004 as mod
 
 runner = CliRunner()
 
 
-def test_traceback_rich_pretty_short_disable():
+def test_rich_pretty_exceptions_disable():
     file_path = Path(mod.__file__)
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
-    assert "return get_command(self)(*args, **kwargs)" not in result.stderr
+    assert "return get_command(self)(*args, **kwargs)" in result.stderr
 
     assert "app()" in result.stderr
     assert "print(name + 3)" in result.stderr
-
     # TODO: when deprecating Python 3.6, remove second option
     assert (
         'TypeError: can only concatenate str (not "int") to str' in result.stderr
         or "TypeError: must be str, not int" in result.stderr
     )
-    assert "name = 'morty'" in result.stderr
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_exceptions/test_tutorial003.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import os
 import subprocess
+import sys
 from pathlib import Path
 
 from typer.testing import CliRunner
 
-from docs_src.exceptions import tutorial004 as mod
+from docs_src.exceptions import tutorial003 as mod
 
 runner = CliRunner()
 
 
-def test_rich_pretty_exceptions_disable():
+def test_traceback_rich_pretty_short_disable():
     file_path = Path(mod.__file__)
     result = subprocess.run(
-        ["coverage", "run", str(file_path)],
+        [sys.executable, "-m", "coverage", "run", str(file_path)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={**os.environ, "_TYPER_STANDARD_TRACEBACK": ""},
     )
-    assert "return get_command(self)(*args, **kwargs)" in result.stderr
+    assert "return get_command(self)(*args, **kwargs)" not in result.stderr
 
     assert "app()" in result.stderr
     assert "print(name + 3)" in result.stderr
+
     # TODO: when deprecating Python 3.6, remove second option
     assert (
         'TypeError: can only concatenate str (not "int") to str' in result.stderr
         or "TypeError: must be str, not int" in result.stderr
     )
+    assert "name = 'morty'" in result.stderr
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.first_steps import tutorial001 as mod
 
 runner = CliRunner()
@@ -13,13 +14,13 @@
     app.command()(mod.main)
     result = runner.invoke(app, [])
     assert result.output == "Hello World\n"
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial002.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.first_steps import tutorial002 as mod
 
 runner = CliRunner()
@@ -21,13 +22,13 @@
     result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial003.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.first_steps import tutorial003 as mod
 
 runner = CliRunner()
@@ -21,13 +22,13 @@
     result = runner.invoke(app, ["Camila", "Gutiérrez"])
     assert result.exit_code == 0
     assert "Hello Camila Gutiérrez" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial004.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.first_steps import tutorial004 as mod
 
 runner = CliRunner()
@@ -45,13 +46,13 @@
     result = runner.invoke(app, ["--formal", "Camila", "Gutiérrez"])
     assert result.exit_code == 0
     assert "Good day Ms. Camila Gutiérrez." in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial005.py` & `typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial005.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.first_steps import tutorial005 as mod
 
 runner = CliRunner()
@@ -45,13 +46,13 @@
     result = runner.invoke(app, ["Camila", "--lastname", "Gutiérrez", "--formal"])
     assert result.exit_code == 0
     assert "Good day Ms. Camila Gutiérrez." in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial006.py` & `typer-0.8.0/tests/test_tutorial/test_first_steps/test_tutorial006.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.first_steps import tutorial006 as mod
 
 runner = CliRunner()
@@ -40,13 +41,13 @@
     result = runner.invoke(app, ["Camila", "--lastname", "Gutiérrez", "--formal"])
     assert result.exit_code == 0
     assert "Good day Ms. Camila Gutiérrez." in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.multiple_values.arguments_with_multiple_values import tutorial001 as mod
 
 runner = CliRunner()
@@ -15,13 +16,13 @@
     assert result.exit_code == 0
     assert "This file exists: README.md\nwoohoo!" in result.output
     assert "This file exists: pyproject.toml\nwoohoo!" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.multiple_values.arguments_with_multiple_values import tutorial002 as mod
 
 runner = CliRunner()
@@ -43,13 +44,13 @@
     assert "Hello Draco" in result.stdout
     assert "Hello Hagrid" in result.stdout
     assert "Hello Dobby" in result.stdout
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.multiple_values.multiple_options import tutorial001 as mod
 
 runner = CliRunner()
@@ -31,13 +32,13 @@
     assert "Processing user: Camila" in result.output
     assert "Processing user: Rick" in result.output
     assert "Processing user: Morty" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_required/test_tutorial002.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 import subprocess
+import sys
 
 import typer
+import typer.core
 from typer.testing import CliRunner
 
-from docs_src.multiple_values.multiple_options import tutorial002 as mod
+from docs_src.options.required import tutorial001 as mod
 
 runner = CliRunner()
+
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_main():
-    result = runner.invoke(app)
+def test_1():
+    result = runner.invoke(app, ["Camila"])
+    assert result.exit_code != 0
+    assert "Missing option '--lastname'." in result.output
+
+
+def test_option_lastname():
+    result = runner.invoke(app, ["Camila", "--lastname", "Gutiérrez"])
     assert result.exit_code == 0
-    assert "The sum is 0" in result.output
+    assert "Hello Camila Gutiérrez" in result.output
 
 
-def test_1_number():
-    result = runner.invoke(app, ["--number", "2"])
+def test_help():
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "The sum is 2.0" in result.output
+    assert "--lastname" in result.output
+    assert "TEXT" in result.output
+    assert "[required]" in result.output
 
 
-def test_2_number():
-    result = runner.invoke(app, ["--number", "2", "--number", "3", "--number", "4.5"])
+def test_help_no_rich():
+    rich = typer.core.rich
+    typer.core.rich = None
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "The sum is 9.5" in result.output
+    assert "--lastname" in result.output
+    assert "TEXT" in result.output
+    assert "[required]" in result.output
+    typer.core.rich = rich
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.multiple_values.options_with_multiple_values import tutorial001 as mod
 
 runner = CliRunner()
@@ -40,13 +41,13 @@
         "Option '--user' requires 3 arguments" in result.output
         or "--user option requires 3 arguments" in result.output
     )
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_prompt/test_tutorial001.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.callback import tutorial001 as mod
+from docs_src.prompt import tutorial001 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_1():
-    result = runner.invoke(app, ["--name", "Camila"])
+def test_cli():
+    result = runner.invoke(app, input="Camila\n")
     assert result.exit_code == 0
+    assert "What's your name?:" in result.output
     assert "Hello Camila" in result.output
 
 
-def test_2():
-    result = runner.invoke(app, ["--name", "rick"])
-    assert result.exit_code != 0
-    assert "Invalid value for '--name': Only Camila is allowed" in result.output
-
-
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_callback/test_tutorial003.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.callback import tutorial003 as mod
 
 runner = CliRunner()
@@ -23,25 +24,25 @@
     result = runner.invoke(app, ["--name", "rick"])
     assert result.exit_code != 0
     assert "Invalid value for '--name': Only Camila is allowed" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL003.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial003.py --",
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_callback/test_tutorial004.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.callback import tutorial004 as mod
 
 runner = CliRunner()
@@ -23,25 +24,25 @@
     result = runner.invoke(app, ["--name", "rick"])
     assert result.exit_code != 0
     assert "Invalid value for '--name': Only Camila is allowed" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL004.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial004.py --",
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_help/test_tutorial001.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.help import tutorial001 as mod
 
 runner = CliRunner()
@@ -36,13 +37,13 @@
     result = runner.invoke(app, ["Camila", "--lastname", "Gutiérrez", "--formal"])
     assert result.exit_code == 0
     assert "Good day Ms. Camila Gutiérrez." in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_help/test_tutorial002.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.help import tutorial002 as mod
 
 runner = CliRunner()
@@ -32,13 +33,13 @@
     assert "--no-formal" in result.output
     assert "--debug" in result.output
     assert "--no-debug" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_help/test_tutorial003.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.help import tutorial003 as mod
 
 runner = CliRunner()
@@ -23,13 +24,13 @@
     assert "--fullname" in result.output
     assert "TEXT" in result.output
     assert "[default: Wade Wilson]" not in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial001.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.name import tutorial001 as mod
 
 runner = CliRunner()
@@ -23,13 +24,13 @@
     result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial004.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.name import tutorial002 as mod
+from docs_src.options.name import tutorial004 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_option_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "-n" in result.output
-    assert "--name" in result.output
+    assert "--user-name" in result.output
     assert "TEXT" in result.output
-    assert "--user-name" not in result.output
+    assert "--name" not in result.output
 
 
 def test_call():
     result = runner.invoke(app, ["-n", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_call_long():
-    result = runner.invoke(app, ["--name", "Camila"])
+    result = runner.invoke(app, ["--user-name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial003.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.name import tutorial003 as mod
 
 runner = CliRunner()
@@ -24,13 +25,13 @@
     result = runner.invoke(app, ["-n", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_name/test_tutorial005.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.name import tutorial004 as mod
+from docs_src.options.name import tutorial005 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_option_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
     assert "-n" in result.output
-    assert "--user-name" in result.output
+    assert "--name" in result.output
     assert "TEXT" in result.output
-    assert "--name" not in result.output
+    assert "-f" in result.output
+    assert "--formal" in result.output
 
 
 def test_call():
     result = runner.invoke(app, ["-n", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
-def test_call_long():
-    result = runner.invoke(app, ["--user-name", "Camila"])
+def test_call_formal():
+    result = runner.invoke(app, ["-n", "Camila", "-f"])
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
+    assert "Good day Ms. Camila." in result.output
+
+
+def test_call_formal_condensed():
+    result = runner.invoke(app, ["-fn", "Camila"])
+    assert result.exit_code == 0
+    assert "Good day Ms. Camila." in result.output
+
+
+def test_call_condensed_wrong_order():
+    result = runner.invoke(app, ["-nf", "Camila"])
+    assert result.exit_code != 0
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial005.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,40 @@
 import subprocess
+import sys
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.name import tutorial005 as mod
+from docs_src.subcommands.name_help import tutorial003 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
+app = mod.app
 
 
-def test_option_help():
+def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "-n" in result.output
-    assert "--name" in result.output
-    assert "TEXT" in result.output
-    assert "-f" in result.output
-    assert "--formal" in result.output
+    assert "Commands" in result.output
+    assert "users" in result.output
+    assert "Manage users in the app." in result.output
 
 
-def test_call():
-    result = runner.invoke(app, ["-n", "Camila"])
+def test_command_help():
+    result = runner.invoke(app, ["users", "--help"])
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
+    assert "Manage users in the app." in result.output
 
 
-def test_call_formal():
-    result = runner.invoke(app, ["-n", "Camila", "-f"])
+def test_command():
+    result = runner.invoke(app, ["users", "create", "Camila"])
     assert result.exit_code == 0
-    assert "Good day Ms. Camila." in result.output
-
-
-def test_call_formal_condensed():
-    result = runner.invoke(app, ["-fn", "Camila"])
-    assert result.exit_code == 0
-    assert "Good day Ms. Camila." in result.output
-
-
-def test_call_condensed_wrong_order():
-    result = runner.invoke(app, ["-nf", "Camila"])
-    assert result.exit_code != 0
+    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.prompt import tutorial001 as mod
 
 runner = CliRunner()
@@ -30,13 +31,13 @@
     assert "--lastname" in result.output
     assert "TEXT" in result.output
     assert "[required]" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.prompt import tutorial002 as mod
 
 runner = CliRunner()
@@ -30,13 +31,13 @@
     assert "--lastname" in result.output
     assert "TEXT" in result.output
     assert "[required]" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.prompt import tutorial003 as mod
 
 runner = CliRunner()
@@ -44,13 +45,13 @@
     assert "--project-name" in result.output
     assert "TEXT" in result.output
     assert "[required]" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_required/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_context/test_tutorial003.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 import subprocess
+import sys
 
-import typer
-import typer.core
 from typer.testing import CliRunner
 
-from docs_src.options.required import tutorial001 as mod
+from docs_src.commands.context import tutorial003 as mod
 
-runner = CliRunner()
-
-app = typer.Typer()
-app.command()(mod.main)
+app = mod.app
 
-
-def test_1():
-    result = runner.invoke(app, ["Camila"])
-    assert result.exit_code != 0
-    assert "Missing option '--lastname'." in result.output
+runner = CliRunner()
 
 
-def test_option_lastname():
-    result = runner.invoke(app, ["Camila", "--lastname", "Gutiérrez"])
+def test_create():
+    result = runner.invoke(app, ["create", "Camila"])
     assert result.exit_code == 0
-    assert "Hello Camila Gutiérrez" in result.output
+    assert "Initializing database" not in result.output
+    assert "Creating user: Camila" in result.output
 
 
-def test_help():
-    result = runner.invoke(app, ["--help"])
+def test_delete():
+    result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
-    assert "--lastname" in result.output
-    assert "TEXT" in result.output
-    assert "[required]" in result.output
+    assert "Initializing database" not in result.output
+    assert "Deleting user: Camila" in result.output
 
 
-def test_help_no_rich():
-    rich = typer.core.rich
-    typer.core.rich = None
-    result = runner.invoke(app, ["--help"])
+def test_callback():
+    result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "--lastname" in result.output
-    assert "TEXT" in result.output
-    assert "[required]" in result.output
-    typer.core.rich = rich
+    assert "Initializing database" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options/test_version/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_version/test_tutorial003.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.options.version import tutorial003 as mod
 
 runner = CliRunner()
@@ -28,25 +29,25 @@
     result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL003.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial003.py --name Rick --v",
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.options_autocompletion import tutorial002 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial002.py --name ",
@@ -30,13 +31,13 @@
     result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.options_autocompletion import tutorial003 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL003.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial003.py --name Seb",
@@ -30,13 +31,13 @@
     result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.options_autocompletion import tutorial004 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL004.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial004_aux.py --name ",
@@ -30,13 +31,13 @@
     result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py` & `typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import os
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial007 as mod
+from docs_src.options_autocompletion import tutorial009 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL007.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial007.py --name Sebastian --name ",
+            "_TUTORIAL009.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial009.py --name Sebastian --name ",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
+    # TODO: when deprecating Click 7, remove second option
+    assert "[]" in result.stderr or "['--name', 'Sebastian', '--name']" in result.stderr
 
 
 def test_1():
     result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py` & `typer-0.8.0/tests/test_tutorial/test_prompt/test_tutorial002.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-import os
 import subprocess
+import sys
 
+import typer
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial008 as mod
+from docs_src.prompt import tutorial002 as mod
 
 runner = CliRunner()
 
-
-def test_completion():
-    result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        encoding="utf-8",
-        env={
-            **os.environ,
-            "_TUTORIAL008.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial008.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
-        },
-    )
-    assert '"Camila":"The reader of books."' in result.stdout
-    assert '"Carlos":"The writer of scripts."' in result.stdout
-    assert '"Sebastian":"The type hints guy."' in result.stdout
-    # TODO: when deprecating Click 7, remove second option
-    assert "[]" in result.stderr or "['--name']" in result.stderr
+app = typer.Typer()
+app.command()(mod.main)
 
 
-def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
+def test_cli():
+    result = runner.invoke(app, input="y\n")
     assert result.exit_code == 0
-    assert "Hello Camila" in result.output
-    assert "Hello Sebastian" in result.output
+    assert "Are you sure you want to delete it? [y/N]:" in result.output
+    assert "Deleting it!" in result.output
+
+
+def test_no_confirm():
+    result = runner.invoke(app, input="n\n")
+    assert result.exit_code == 1
+    assert "Are you sure you want to delete it? [y/N]:" in result.output
+    assert "Not deleting" in result.output
+    assert "Aborted" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py` & `typer-0.8.0/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import os
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial009 as mod
+from docs_src.options_autocompletion import tutorial007 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL009.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial009.py --name Sebastian --name ",
+            "_TUTORIAL007.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial007.py --name Sebastian --name ",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
-    # TODO: when deprecating Click 7, remove second option
-    assert "[]" in result.stderr or "['--name', 'Sebastian', '--name']" in result.stderr
 
 
 def test_1():
     result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.bool import tutorial001 as mod
 
 runner = CliRunner()
@@ -39,13 +40,13 @@
         "No such option: --no-force" in result.output
         or "no such option: --no-force" in result.output
     )
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.bool import tutorial002 as mod
 
@@ -58,13 +59,13 @@
         "No such option: --no-accept" in result.output
         or "no such option: --no-accept" in result.output
     )
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.parameter_types.bool import tutorial003 as mod
+from docs_src.arguments.optional import tutorial002 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_help():
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "-f" in result.output
-    assert "--force" in result.output
-    assert "-F" in result.output
-    assert "--no-force" in result.output
+    assert "[OPTIONS] [NAME]" in result.output
 
 
-def test_force():
-    result = runner.invoke(app, ["-f"])
+def test_call_no_arg():
+    result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "Forcing operation" in result.output
+    assert "Hello World!" in result.output
 
 
-def test_no_force():
-    result = runner.invoke(app, ["-F"])
+def test_call_arg():
+    result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
-    assert "Not forcing" in result.output
+    assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.parameter_types.bool import tutorial004 as mod
+from docs_src.parameter_types.number import tutorial003 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_help():
-    result = runner.invoke(app, ["--help"])
+def test_main():
+    result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "-d" in result.output
-    assert "--demo" in result.output
+    assert "Verbose level is 0" in result.output
 
 
-def test_main():
-    result = runner.invoke(app)
+def test_verbose_1():
+    result = runner.invoke(app, ["--verbose"])
+    assert result.exit_code == 0
+    assert "Verbose level is 1" in result.output
+
+
+def test_verbose_3():
+    result = runner.invoke(app, ["--verbose", "--verbose", "--verbose"])
+    assert result.exit_code == 0
+    assert "Verbose level is 3" in result.output
+
+
+def test_verbose_short_1():
+    result = runner.invoke(app, ["-v"])
     assert result.exit_code == 0
-    assert "Running in production" in result.output
+    assert "Verbose level is 1" in result.output
 
 
-def test_demo():
-    result = runner.invoke(app, ["--demo"])
+def test_verbose_short_3():
+    result = runner.invoke(app, ["-v", "-v", "-v"])
     assert result.exit_code == 0
-    assert "Running demo" in result.output
+    assert "Verbose level is 3" in result.output
 
 
-def test_short_demo():
-    result = runner.invoke(app, ["-d"])
+def test_verbose_short_3_condensed():
+    result = runner.invoke(app, ["-vvv"])
     assert result.exit_code == 0
-    assert "Running demo" in result.output
+    assert "Verbose level is 3" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.datetime import tutorial001 as mod
 
 runner = CliRunner()
@@ -39,13 +40,13 @@
     assert "%Y-%m-%d" in result.output
     assert "%Y-%m-%dT%H:%M:%S" in result.output
     assert "%Y-%m-%d %H:%M:%S" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.datetime import tutorial002 as mod
 
 runner = CliRunner()
@@ -21,13 +22,13 @@
     result = runner.invoke(app, ["10/29/1969"])
     assert result.exit_code == 0
     assert "Launch will be at: 1969-10-29 00:00:00" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.enum import tutorial001 as mod
 
 runner = CliRunner()
@@ -37,13 +38,13 @@
     assert "simple" in result.output
     assert "conv" in result.output
     assert "lstm" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.enum import tutorial002 as mod
 
 runner = CliRunner()
@@ -21,13 +22,13 @@
     result = runner.invoke(app, ["--network", "LsTm"])
     assert result.exit_code == 0
     assert "Training neural network of type: lstm" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.file import tutorial001 as mod
 
@@ -20,13 +21,13 @@
     assert result.exit_code == 0
     assert "Config line: some settings" in result.output
     assert "Config line: some more settings" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.parameter_types.file import tutorial002 as mod
+from docs_src.parameter_types.file import tutorial005 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_main(tmpdir):
     config_file = Path(tmpdir) / "config.txt"
     if config_file.exists():  # pragma no cover
         config_file.unlink()
+        config_file.write_text("")
+    result = runner.invoke(app, ["--config", f"{config_file}"])
+    result = runner.invoke(app, ["--config", f"{config_file}"])
     result = runner.invoke(app, ["--config", f"{config_file}"])
     text = config_file.read_text()
     config_file.unlink()
     assert result.exit_code == 0
-    assert "Config written" in result.output
-    assert "Some config written by the app" in text
+    assert "Config line written"
+    assert "This is a single line\nThis is a single line\nThis is a single line" in text
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.file import tutorial003 as mod
 
@@ -19,13 +20,13 @@
     binary_file.unlink()
     assert result.exit_code == 0
     assert "Processed bytes total:" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.file import tutorial004 as mod
 
@@ -23,13 +24,13 @@
     assert "Binary file written" in result.output
     assert "some settings" in text
     assert "la cigüeña trae al niño" in text
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.parameter_types.file import tutorial005 as mod
+from docs_src.parameter_types.path import tutorial002 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_main(tmpdir):
+def test_not_exists(tmpdir):
     config_file = Path(tmpdir) / "config.txt"
     if config_file.exists():  # pragma no cover
         config_file.unlink()
-        config_file.write_text("")
-    result = runner.invoke(app, ["--config", f"{config_file}"])
     result = runner.invoke(app, ["--config", f"{config_file}"])
+    assert result.exit_code != 0
+    assert "Invalid value for '--config': File" in result.output
+    assert "does not exist" in result.output
+
+
+def test_exists(tmpdir):
+    config_file = Path(tmpdir) / "config.txt"
+    config_file.write_text("some settings")
     result = runner.invoke(app, ["--config", f"{config_file}"])
-    text = config_file.read_text()
     config_file.unlink()
     assert result.exit_code == 0
-    assert "Config line written"
-    assert "This is a single line\nThis is a single line\nThis is a single line" in text
+    assert "Config file contents: some settings" in result.output
+
+
+def test_dir():
+    result = runner.invoke(app, ["--config", "./"])
+    assert result.exit_code != 0
+    assert "Invalid value for '--config': File './' is a directory." in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.index import tutorial001 as mod
 
 runner = CliRunner()
@@ -40,13 +41,13 @@
         "Invalid value for '--age': '15.3' is not a valid integer" in result.output
         or "Invalid value for '--age': 15.3 is not a valid integer" in result.output
     )
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.number import tutorial001 as mod
 
@@ -86,13 +87,13 @@
     assert "ID is 5" in result.output
     assert "--age is 20" in result.output
     assert "--score is -5.0" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.number import tutorial002 as mod
 
 runner = CliRunner()
@@ -29,13 +30,13 @@
     assert "ID is 5" in result.output
     assert "--rank is 10" in result.output
     assert "--score is 0" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.path import tutorial001 as mod
 
@@ -42,13 +43,13 @@
     result = runner.invoke(app, ["--config", "./"])
     assert result.exit_code == 0
     assert "Config is a directory, will use all its config files" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.parameter_types.path import tutorial002 as mod
+from docs_src.parameter_types.file import tutorial002 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_not_exists(tmpdir):
+def test_main(tmpdir):
     config_file = Path(tmpdir) / "config.txt"
     if config_file.exists():  # pragma no cover
         config_file.unlink()
     result = runner.invoke(app, ["--config", f"{config_file}"])
-    assert result.exit_code != 0
-    assert "Invalid value for '--config': File" in result.output
-    assert "does not exist" in result.output
-
-
-def test_exists(tmpdir):
-    config_file = Path(tmpdir) / "config.txt"
-    config_file.write_text("some settings")
-    result = runner.invoke(app, ["--config", f"{config_file}"])
+    text = config_file.read_text()
     config_file.unlink()
     assert result.exit_code == 0
-    assert "Config file contents: some settings" in result.output
-
-
-def test_dir():
-    result = runner.invoke(app, ["--config", "./"])
-    assert result.exit_code != 0
-    assert "Invalid value for '--config': File './' is a directory." in result.output
+    assert "Config written" in result.output
+    assert "Some config written by the app" in text
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
 from docs_src.parameter_types.uuid import tutorial001 as mod
 
 runner = CliRunner()
@@ -29,13 +30,13 @@
         or "Invalid value for 'USER_ID': 7479706572-72756c6573 is not a valid UUID value"
         in result.output
     )
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_index/test_tutorial001.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import subprocess
+import sys
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.prompt import tutorial001 as mod
+from docs_src.commands.index import tutorial001 as mod
+
+app = mod.app
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
+
+def test_no_arg():
+    result = runner.invoke(app)
+    assert result.exit_code != 0
+    assert "Missing argument 'NAME'." in result.output
 
 
-def test_cli():
-    result = runner.invoke(app, input="Camila\n")
+def test_arg():
+    result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
-    assert "What's your name?:" in result.output
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_prompt/test_tutorial003.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.prompt import tutorial002 as mod
+from docs_src.prompt import tutorial003 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
@@ -18,19 +19,18 @@
     assert "Deleting it!" in result.output
 
 
 def test_no_confirm():
     result = runner.invoke(app, input="n\n")
     assert result.exit_code == 1
     assert "Are you sure you want to delete it? [y/N]:" in result.output
-    assert "Not deleting" in result.output
     assert "Aborted" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_options/test_callback/test_tutorial001.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import subprocess
+import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.prompt import tutorial003 as mod
+from docs_src.options.callback import tutorial001 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_cli():
-    result = runner.invoke(app, input="y\n")
+def test_1():
+    result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
-    assert "Are you sure you want to delete it? [y/N]:" in result.output
-    assert "Deleting it!" in result.output
+    assert "Hello Camila" in result.output
 
 
-def test_no_confirm():
-    result = runner.invoke(app, input="n\n")
-    assert result.exit_code == 1
-    assert "Are you sure you want to delete it? [y/N]:" in result.output
-    assert "Aborted" in result.output
+def test_2():
+    result = runner.invoke(app, ["--name", "rick"])
+    assert result.exit_code != 0
+    assert "Invalid value for '--name': Only Camila is allowed" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.subcommands.callback_override import tutorial001 as mod
 
 runner = CliRunner()
 
@@ -14,13 +15,13 @@
     assert result.exit_code == 0
     assert "Running a users command" in result.output
     assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.subcommands.callback_override import tutorial002 as mod
 
 runner = CliRunner()
 
@@ -14,13 +15,13 @@
     assert result.exit_code == 0
     assert "Running a users command" in result.output
     assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.subcommands.callback_override import tutorial003 as mod
+from docs_src.subcommands.name_help import tutorial008 as mod
 
 runner = CliRunner()
 
 app = mod.app
 
 
-def test_cli():
-    result = runner.invoke(app, ["users", "create", "Camila"])
+def test_help():
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "Running a users command" not in result.output
-    assert "Callback override, running users command" in result.output
-    assert "Creating user: Camila" in result.output
+    assert "Commands" in result.output
+    assert "cake-sith-users" in result.output
+    assert "Unlimited powder! Eh, users." in result.output
+
+
+def test_command_help():
+    result = runner.invoke(app, ["cake-sith-users", "--help"])
+    assert result.exit_code == 0
+    assert "Unlimited powder! Eh, users." in result.output
 
 
-def test_for_coverage():
-    mod.default_callback()
+def test_command():
+    result = runner.invoke(app, ["cake-sith-users", "create", "Camila"])
+    assert result.exit_code == 0
+    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.subcommands.callback_override import tutorial004 as mod
 
 runner = CliRunner()
 
@@ -21,13 +22,13 @@
 def test_for_coverage():
     mod.default_callback()
     mod.user_callback()
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.subcommands.name_help import tutorial001 as mod
+from docs_src.subcommands.name_help import tutorial004 as mod
 
 runner = CliRunner()
 
 app = mod.app
 
 
 def test_help():
@@ -27,13 +28,13 @@
     result = runner.invoke(app, ["users", "create", "Camila"])
     assert result.exit_code == 0
     assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_terminating/test_tutorial001.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import subprocess
+import sys
 
+import typer
 from typer.testing import CliRunner
 
-from docs_src.subcommands.name_help import tutorial002 as mod
+from docs_src.terminating import tutorial001 as mod
 
 runner = CliRunner()
 
-app = mod.app
+app = typer.Typer()
+app.command()(mod.main)
 
 
-def test_help():
-    result = runner.invoke(app, ["--help"])
+def test_cli():
+    result = runner.invoke(app, ["Camila"])
     assert result.exit_code == 0
-    assert "Commands" in result.output
-    assert "users" in result.output
-    assert "Manage users in the app." in result.output
+    assert "User created: Camila" in result.output
+    assert "Notification sent for new user: Camila" in result.output
 
 
-def test_command_help():
-    result = runner.invoke(app, ["users", "--help"])
+def test_existing():
+    result = runner.invoke(app, ["rick"])
     assert result.exit_code == 0
-    assert "Manage users in the app." in result.output
+    assert "The user already exists" in result.output
+    assert "Notification sent for new user" not in result.output
 
 
-def test_command():
-    result = runner.invoke(app, ["users", "create", "Camila"])
+def test_existing_no_standalone():
+    # Mainly for coverage
+    result = runner.invoke(app, ["rick"], standalone_mode=False)
     assert result.exit_code == 0
-    assert "Creating user: Camila" in result.output
+    assert "The user already exists" in result.output
+    assert "Notification sent for new user" not in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_help/test_tutorial008.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
-from docs_src.subcommands.name_help import tutorial005 as mod
-
-runner = CliRunner()
+from docs_src.commands.help import tutorial008 as mod
 
 app = mod.app
 
-
-def test_help():
-    result = runner.invoke(app, ["--help"])
-    assert result.exit_code == 0
-    assert "Commands" in result.output
-    assert "new-users" in result.output
-    assert "I have the highland! Create some users." in result.output
+runner = CliRunner()
 
 
-def test_command_help():
-    result = runner.invoke(app, ["new-users", "--help"])
+def test_main_help():
+    result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
-    assert "I have the highland! Create some users." in result.output
+    assert "Create a new user. ✨" in result.output
+    assert "Made with ❤ in Venus" in result.output
 
 
-def test_command():
-    result = runner.invoke(app, ["new-users", "create", "Camila"])
+def test_call():
+    # Mainly for coverage
+    result = runner.invoke(app, ["Morty"])
     assert result.exit_code == 0
-    assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py` & `typer-0.8.0/tests/test_tutorial/test_using_click/test_tutorial003.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import subprocess
+import sys
 
-from typer.testing import CliRunner
+from click.testing import CliRunner
 
-from docs_src.subcommands.name_help import tutorial006 as mod
+from docs_src.using_click import tutorial003 as mod
 
 runner = CliRunner()
 
-app = mod.app
 
+def test_cli():
+    result = runner.invoke(mod.typer_click_object, [])
+    # TODO: when deprecating Click 7, remove second option
+    assert "Missing command" in result.stdout or "Usage" in result.stdout
 
-def test_help():
-    result = runner.invoke(app, ["--help"])
-    assert result.exit_code == 0
-    assert "Commands" in result.output
-    assert "exp-users" in result.output
-    assert "Explicit help." in result.output
 
+def test_typer():
+    result = runner.invoke(mod.typer_click_object, ["top"])
+    assert "The Typer app is at the top level" in result.stdout
 
-def test_command_help():
-    result = runner.invoke(app, ["exp-users", "--help"])
-    assert result.exit_code == 0
-    assert "Explicit help." in result.output
 
-
-def test_command():
-    result = runner.invoke(app, ["exp-users", "create", "Camila"])
-    assert result.exit_code == 0
-    assert "Creating user: Camila" in result.output
+def test_click():
+    result = runner.invoke(mod.typer_click_object, ["hello", "--name", "Camila"])
+    assert "Hello Camila!" in result.stdout
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.subcommands.name_help import tutorial007 as mod
 
 runner = CliRunner()
 
@@ -27,13 +28,13 @@
     result = runner.invoke(app, ["call-users", "create", "Camila"])
     assert result.exit_code == 0
     assert "Creating user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_tutorial001.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import subprocess
+import sys
 
 import pytest
 from typer.testing import CliRunner
 
 from docs_src.subcommands import tutorial001
 
 runner = CliRunner()
@@ -80,15 +82,19 @@
     assert result.exit_code == 0
     assert "Deleting user: Camila" in result.output
 
 
 def test_scripts(mod):
     from docs_src.subcommands.tutorial001 import items, users
 
+    env = os.environ.copy()
+    env["PYTHONPATH"] = ":".join(list(tutorial001.__path__))
+
     for module in [mod, items, users]:
         result = subprocess.run(
-            ["coverage", "run", module.__file__, "--help"],
+            [sys.executable, "-m", "coverage", "run", module.__file__, "--help"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             encoding="utf-8",
+            env=env,
         )
         assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_tutorial002.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import subprocess
+import sys
 
 from typer.testing import CliRunner
 
 from docs_src.subcommands.tutorial002 import main as mod
 
 app = mod.app
 runner = CliRunner()
@@ -65,13 +66,13 @@
     result = runner.invoke(app, ["users", "delete", "Camila"])
     assert result.exit_code == 0
     assert "Deleting user: Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_subcommands/test_tutorial003.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import subprocess
+import sys
 
 import pytest
 from typer.testing import CliRunner
 
 from docs_src.subcommands import tutorial003
 from docs_src.subcommands.tutorial003 import items, users
 
@@ -153,15 +155,19 @@
     assert result.exit_code == 0
     assert "Burning town: New Asgard" in result.output
 
 
 def test_scripts(mod):
     from docs_src.subcommands.tutorial003 import items, lands, reigns, towns, users
 
+    env = os.environ.copy()
+    env["PYTHONPATH"] = ":".join(list(tutorial003.__path__))
+
     for module in [mod, items, lands, reigns, towns, users]:
         result = subprocess.run(
-            ["coverage", "run", module.__file__, "--help"],
+            [sys.executable, "-m", "coverage", "run", module.__file__, "--help"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             encoding="utf-8",
+            env=env,
         )
         assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial001.py` & `typer-0.8.0/tests/test_tutorial/test_commands/test_context/test_tutorial002.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import subprocess
+import sys
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.terminating import tutorial001 as mod
+from docs_src.commands.context import tutorial002 as mod
 
-runner = CliRunner()
+app = mod.app
 
-app = typer.Typer()
-app.command()(mod.main)
+runner = CliRunner()
 
 
-def test_cli():
-    result = runner.invoke(app, ["Camila"])
+def test_create():
+    result = runner.invoke(app, ["create", "Camila"])
     assert result.exit_code == 0
-    assert "User created: Camila" in result.output
-    assert "Notification sent for new user: Camila" in result.output
+    assert "Initializing database" in result.output
+    assert "Creating user: Camila" in result.output
 
 
-def test_existing():
-    result = runner.invoke(app, ["rick"])
+def test_delete():
+    result = runner.invoke(app, ["delete", "Camila"])
     assert result.exit_code == 0
-    assert "The user already exists" in result.output
-    assert "Notification sent for new user" not in result.output
+    assert "Initializing database" in result.output
+    assert "Deleting user: Camila" in result.output
 
 
-def test_existing_no_standalone():
-    # Mainly for coverage
-    result = runner.invoke(app, ["rick"], standalone_mode=False)
+def test_callback():
+    result = runner.invoke(app)
     assert result.exit_code == 0
-    assert "The user already exists" in result.output
-    assert "Notification sent for new user" not in result.output
+    assert "Initializing database" in result.output
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial002.py` & `typer-0.8.0/tests/test_tutorial/test_using_click/test_tutorial004.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import subprocess
+import sys
 
-import typer
-from typer.testing import CliRunner
+from click.testing import CliRunner
 
-from docs_src.terminating import tutorial002 as mod
+from docs_src.using_click import tutorial004 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
-
 
 def test_cli():
-    result = runner.invoke(app, ["Camila"])
-    assert result.exit_code == 0
-    assert "New user created: Camila" in result.output
+    result = runner.invoke(mod.cli, [])
+    assert "Usage" in result.stdout
+    assert "dropdb" in result.stdout
+    assert "sub" in result.stdout
+
+
+def test_typer():
+    result = runner.invoke(mod.cli, ["sub"])
+    assert "Typer is now below Click, the Click app is the top level" in result.stdout
+
+
+def test_click_initdb():
+    result = runner.invoke(mod.cli, ["initdb"])
+    assert "Initialized the database" in result.stdout
 
 
-def test_root():
-    result = runner.invoke(app, ["root"])
-    assert result.exit_code == 1
-    assert "The root user is reserved" in result.output
+def test_click_dropdb():
+    result = runner.invoke(mod.cli, ["dropdb"])
+    assert "Dropped the database" in result.stdout
 
 
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial003.py` & `typer-0.8.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 import subprocess
+import sys
 
 import typer
 import typer.core
 from typer.testing import CliRunner
 
-from docs_src.terminating import tutorial003 as mod
+from docs_src.arguments.optional import tutorial001 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_cli():
-    result = runner.invoke(app, ["Camila"])
-    assert result.exit_code == 0
-    assert "New user created: Camila" in result.output
-
-
-def test_root():
-    result = runner.invoke(app, ["root"])
-    assert result.exit_code == 1
-    assert "The root user is reserved" in result.output
-    assert "Aborted" in result.output
+def test_call_no_arg():
+    result = runner.invoke(app)
+    assert result.exit_code != 0
+    assert "Missing argument 'NAME'." in result.output
 
 
-def test_root_no_standalone():
+def test_call_no_arg_standalone():
     # Mainly for coverage
-    result = runner.invoke(app, ["root"], standalone_mode=False)
-    assert result.exit_code == 1
+    result = runner.invoke(app, standalone_mode=False)
+    assert result.exit_code != 0
 
 
-def test_root_no_rich():
+def test_call_no_arg_no_rich():
     # Mainly for coverage
     rich = typer.core.rich
     typer.core.rich = None
-    result = runner.invoke(app, ["root"])
-    assert result.exit_code == 1
-    assert "The root user is reserved" in result.stdout
-    assert "Aborted!" in result.stdout
+    result = runner.invoke(app)
+    assert result.exit_code != 0
+    assert "Error: Missing argument 'NAME'" in result.stdout
     typer.core.rich = rich
 
 
+def test_call_arg():
+    result = runner.invoke(app, ["Camila"])
+    assert result.exit_code == 0
+    assert "Hello Camila" in result.output
+
+
 def test_script():
     result = subprocess.run(
-        ["coverage", "run", mod.__file__, "--help"],
+        [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
```

### Comparing `typer-0.7.0/typer/__init__.py` & `typer-0.8.0/typer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Typer, build great CLIs. Easy to code. Based on Python type hints."""
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 from shutil import get_terminal_size as get_terminal_size
 
 from click.exceptions import Abort as Abort
 from click.exceptions import BadParameter as BadParameter
 from click.exceptions import Exit as Exit
 from click.termui import clear as clear
```

### Comparing `typer-0.7.0/typer/_completion_click7.py` & `typer-0.8.0/typer/_completion_click7.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/typer/_completion_click8.py` & `typer-0.8.0/typer/_completion_click8.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/typer/_completion_shared.py` & `typer-0.8.0/typer/_completion_shared.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/typer/completion.py` & `typer-0.8.0/typer/completion.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/typer/core.py` & `typer-0.8.0/typer/core.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/typer/main.py` & `typer-0.8.0/typer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -685,15 +685,21 @@
     update_wrapper(wrapper, callback)
     return wrapper
 
 
 def get_click_type(
     *, annotation: Any, parameter_info: ParameterInfo
 ) -> click.ParamType:
-    if annotation == str:
+    if parameter_info.click_type is not None:
+        return parameter_info.click_type
+
+    elif parameter_info.parser is not None:
+        return click.types.FuncParamType(parameter_info.parser)
+
+    elif annotation == str:
         return click.STRING
     elif annotation == int:
         if parameter_info.min is not None or parameter_info.max is not None:
             min_ = None
             max_ = None
             if parameter_info.min is not None:
                 min_ = int(parameter_info.min)
```

### Comparing `typer-0.7.0/typer/models.py` & `typer-0.8.0/typer/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -180,14 +180,17 @@
         shell_complete: Optional[
             Callable[
                 [click.Context, click.Parameter, str],
                 Union[List["click.shell_completion.CompletionItem"], List[str]],
             ]
         ] = None,
         autocompletion: Optional[Callable[..., Any]] = None,
+        # Custom type
+        parser: Optional[Callable[[str], Any]] = None,
+        click_type: Optional[click.ParamType] = None,
         # TyperArgument
         show_default: Union[bool, str] = True,
         show_choices: bool = True,
         show_envvar: bool = True,
         help: Optional[str] = None,
         hidden: bool = False,
         # Choice
@@ -212,23 +215,33 @@
         readable: bool = True,
         resolve_path: bool = False,
         allow_dash: bool = False,
         path_type: Union[None, Type[str], Type[bytes]] = None,
         # Rich settings
         rich_help_panel: Union[str, None] = None,
     ):
+        # Check if user has provided multiple custom parsers
+        if parser and click_type:
+            raise ValueError(
+                "Multiple custom type parsers provided. "
+                "`parser` and `click_type` may not both be provided."
+            )
+
         self.default = default
         self.param_decls = param_decls
         self.callback = callback
         self.metavar = metavar
         self.expose_value = expose_value
         self.is_eager = is_eager
         self.envvar = envvar
         self.shell_complete = shell_complete
         self.autocompletion = autocompletion
+        # Custom type
+        self.parser = parser
+        self.click_type = click_type
         # TyperArgument
         self.show_default = show_default
         self.show_choices = show_choices
         self.show_envvar = show_envvar
         self.help = help
         self.hidden = hidden
         # Choice
@@ -273,14 +286,17 @@
         shell_complete: Optional[
             Callable[
                 [click.Context, click.Parameter, str],
                 Union[List["click.shell_completion.CompletionItem"], List[str]],
             ]
         ] = None,
         autocompletion: Optional[Callable[..., Any]] = None,
+        # Custom type
+        parser: Optional[Callable[[str], Any]] = None,
+        click_type: Optional[click.ParamType] = None,
         # Option
         show_default: bool = True,
         prompt: Union[bool, str] = False,
         confirmation_prompt: bool = False,
         prompt_required: bool = True,
         hide_input: bool = False,
         is_flag: Optional[bool] = None,
@@ -323,14 +339,17 @@
             callback=callback,
             metavar=metavar,
             expose_value=expose_value,
             is_eager=is_eager,
             envvar=envvar,
             shell_complete=shell_complete,
             autocompletion=autocompletion,
+            # Custom type
+            parser=parser,
+            click_type=click_type,
             # TyperArgument
             show_default=show_default,
             show_choices=show_choices,
             show_envvar=show_envvar,
             help=help,
             hidden=hidden,
             # Choice
@@ -384,14 +403,17 @@
         shell_complete: Optional[
             Callable[
                 [click.Context, click.Parameter, str],
                 Union[List["click.shell_completion.CompletionItem"], List[str]],
             ]
         ] = None,
         autocompletion: Optional[Callable[..., Any]] = None,
+        # Custom type
+        parser: Optional[Callable[[str], Any]] = None,
+        click_type: Optional[click.ParamType] = None,
         # TyperArgument
         show_default: Union[bool, str] = True,
         show_choices: bool = True,
         show_envvar: bool = True,
         help: Optional[str] = None,
         hidden: bool = False,
         # Choice
@@ -426,14 +448,17 @@
             callback=callback,
             metavar=metavar,
             expose_value=expose_value,
             is_eager=is_eager,
             envvar=envvar,
             shell_complete=shell_complete,
             autocompletion=autocompletion,
+            # Custom type
+            parser=parser,
+            click_type=click_type,
             # TyperArgument
             show_default=show_default,
             show_choices=show_choices,
             show_envvar=show_envvar,
             help=help,
             hidden=hidden,
             # Choice
```

### Comparing `typer-0.7.0/typer/rich_utils.py` & `typer-0.8.0/typer/rich_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,14 @@
     # Print usage
     console.print(
         Padding(highlighter(obj.get_usage(ctx)), 1), style=STYLE_USAGE_COMMAND
     )
 
     # Print command / group help if we have some
     if obj.help:
-
         # Print with some padding
         console.print(
             Padding(
                 Align(
                     _get_help_text(
                         obj=obj,
                         markup_mode=markup_mode,
@@ -565,15 +564,14 @@
                 ),
                 (0, 1, 1, 1),
             )
         )
     panel_to_arguments: DefaultDict[str, List[click.Argument]] = defaultdict(list)
     panel_to_options: DefaultDict[str, List[click.Option]] = defaultdict(list)
     for param in obj.get_params(ctx):
-
         # Skip if option is hidden
         if getattr(param, "hidden", False):
             continue
         if isinstance(param, click.Argument):
             panel_name = (
                 getattr(param, _RICH_HELP_PANEL_NAME, None) or ARGUMENTS_PANEL_TITLE
             )
```

### Comparing `typer-0.7.0/typer/testing.py` & `typer-0.8.0/typer/testing.py`

 * *Files identical despite different names*

### Comparing `typer-0.7.0/typer/utils.py` & `typer-0.8.0/typer/utils.py`

 * *Files identical despite different names*

