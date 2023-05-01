# Comparing `tmp/pre_commit-3.2.2.tar.gz` & `tmp/pre_commit-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit-3.2.2.tar", last modified: Mon Apr  3 20:31:16 2023, max compression
+gzip compressed data, was "pre_commit-3.3.0.tar", last modified: Mon May  1 22:23:57 2023, max compression
```

## Comparing `pre_commit-3.2.2.tar` & `pre_commit-3.3.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.528295 pre_commit-3.2.2/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:40.000000 pre_commit-3.2.2/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-04-03 20:31:16.528295 pre_commit-3.2.2/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      480 2022-12-31 16:55:07.000000 pre_commit-3.2.2/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.508295 pre_commit-3.2.2/pre_commit/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      127 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1357 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/all_languages.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12139 2023-03-17 16:29:01.000000 pre_commit-3.2.2/pre_commit/clientlib.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3219 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/color.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.512295 pre_commit-3.2.2/pre_commit/commands/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6217 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/autoupdate.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/clean.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2804 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/gc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9391 2023-03-17 16:29:01.000000 pre_commit-3.2.2/pre_commit/commands/hook_impl.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/init_templatedir.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5408 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/install_uninstall.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2099 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/migrate_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14102 2023-03-17 16:29:01.000000 pre_commit-3.2.2/pre_commit/commands/run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      453 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/sample_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2578 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/try_repo.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      362 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/validate_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      368 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/commands/validate_manifest.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      282 2023-03-17 16:29:01.000000 pre_commit-3.2.2/pre_commit/constants.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1612 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/envcontext.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2624 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/error_handler.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/errors.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2369 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/file_lock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8509 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/git.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1504 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/hook.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5351 2023-02-21 16:34:35.000000 pre_commit-3.2.2/pre_commit/lang_base.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.520295 pre_commit-3.2.2/pre_commit/languages/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/languages/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2415 2023-03-05 21:04:19.000000 pre_commit-3.2.2/pre_commit/languages/conda.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2502 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/coursier.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3112 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/dart.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4630 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/docker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      827 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/docker_image.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3469 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/dotnet.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      676 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/fail.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4531 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/golang.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2529 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/lua.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3831 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/node.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2023-02-21 16:06:00.000000 pre_commit-3.2.2/pre_commit/languages/perl.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3811 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/pygrep.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6806 2023-03-05 21:04:19.000000 pre_commit-3.2.2/pre_commit/languages/python.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4863 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/r.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4396 2023-02-21 15:20:44.000000 pre_commit-3.2.2/pre_commit/languages/ruby.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5470 2023-03-25 18:01:33.000000 pre_commit-3.2.2/pre_commit/languages/rust.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      777 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/script.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1599 2023-04-03 20:26:07.000000 pre_commit-3.2.2/pre_commit/languages/swift.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2023-02-21 15:20:22.000000 pre_commit-3.2.2/pre_commit/languages/system.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1022 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/logging_handler.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    15276 2023-03-17 16:29:01.000000 pre_commit-3.2.2/pre_commit/main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.520295 pre_commit-3.2.2/pre_commit/meta_hooks/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/meta_hooks/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1193 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/meta_hooks/check_hooks_apply.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2554 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/meta_hooks/check_useless_excludes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      337 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/meta_hooks/identity.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/output.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2472 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/parse_shebang.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      495 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/prefix.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8327 2023-02-23 01:44:08.000000 pre_commit-3.2.2/pre_commit/repository.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.528295 pre_commit-3.2.2/pre_commit/resources/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/resources/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)        2 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_.npmignore
--rw-r--r--   0 asottile  (1000) asottile  (1000)       96 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_Cargo.toml
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1052 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_LICENSE.renv
--rw-r--r--   0 asottile  (1000) asottile  (1000)      104 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_Makefile.PL
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12037 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_activate.R
--rw-r--r--   0 asottile  (1000) asottile  (1000)      302 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_environment.yml
--rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_go.mod
--rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_main.go
--rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_main.rs
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_package.json
--rw-r--r--   0 asottile  (1000) asottile  (1000)      212 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
--rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
--rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_pubspec.yaml
--rw-r--r--   0 asottile  (1000) asottile  (1000)      351 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_renv.lock
--rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/resources/empty_template_setup.py
--rwxr-xr-x   0 asottile  (1000) asottile  (1000)      528 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/hook-tmpl
--rw-r--r--   0 asottile  (1000) asottile  (1000)    32551 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/rbenv.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)    76466 2023-01-24 00:54:44.000000 pre_commit-3.2.2/pre_commit/resources/ruby-build.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2022-04-30 16:59:40.000000 pre_commit-3.2.2/pre_commit/resources/ruby-download.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3922 2023-02-23 01:23:01.000000 pre_commit-3.2.2/pre_commit/staged_files_only.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9257 2023-02-23 01:44:08.000000 pre_commit-3.2.2/pre_commit/store.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6645 2023-03-05 21:04:19.000000 pre_commit-3.2.2/pre_commit/util.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5058 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/xargs.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      499 2023-02-20 22:54:27.000000 pre_commit-3.2.2/pre_commit/yaml.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-03 20:31:16.508295 pre_commit-3.2.2/pre_commit.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-04-03 20:31:16.000000 pre_commit-3.2.2/pre_commit.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2947 2023-04-03 20:31:16.000000 pre_commit-3.2.2/pre_commit.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-04-03 20:31:16.000000 pre_commit-3.2.2/pre_commit.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2023-04-03 20:31:16.000000 pre_commit-3.2.2/pre_commit.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2023-04-03 20:31:16.000000 pre_commit-3.2.2/pre_commit.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-04-03 20:31:16.000000 pre_commit-3.2.2/pre_commit.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1397 2023-04-03 20:31:16.528295 pre_commit-3.2.2/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-02-20 22:54:27.000000 pre_commit-3.2.2/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.773691 pre_commit-3.3.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:40.000000 pre_commit-3.3.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-05-01 22:23:57.773691 pre_commit-3.3.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      480 2022-12-31 16:55:07.000000 pre_commit-3.3.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.761690 pre_commit-3.3.0/pre_commit/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      127 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1357 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/all_languages.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12139 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/clientlib.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3219 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/color.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.765690 pre_commit-3.3.0/pre_commit/commands/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7022 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/commands/autoupdate.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/clean.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2804 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/gc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9391 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/commands/hook_impl.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/init_templatedir.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5408 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/install_uninstall.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2099 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/migrate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14102 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/commands/run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      453 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/sample_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2578 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/try_repo.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      362 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/validate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      368 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/validate_manifest.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      282 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/constants.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1612 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/envcontext.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2624 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/error_handler.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/errors.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2369 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/file_lock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8509 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/git.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1504 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/hook.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5232 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/lang_base.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.769691 pre_commit-3.3.0/pre_commit/languages/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/languages/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2415 2023-03-05 21:04:19.000000 pre_commit-3.3.0/pre_commit/languages/conda.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2502 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/coursier.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3112 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/dart.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4630 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/docker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      827 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/docker_image.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3469 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/dotnet.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      676 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/fail.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4531 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/golang.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2529 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/lua.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3831 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/node.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2023-02-21 16:06:00.000000 pre_commit-3.3.0/pre_commit/languages/perl.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3811 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/pygrep.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6806 2023-03-05 21:04:19.000000 pre_commit-3.3.0/pre_commit/languages/python.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4863 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/r.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4396 2023-02-21 15:20:44.000000 pre_commit-3.3.0/pre_commit/languages/ruby.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5470 2023-03-25 18:01:33.000000 pre_commit-3.3.0/pre_commit/languages/rust.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      777 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/script.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1599 2023-04-03 20:26:07.000000 pre_commit-3.3.0/pre_commit/languages/swift.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/system.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1022 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/logging_handler.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    15466 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.769691 pre_commit-3.3.0/pre_commit/meta_hooks/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1193 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/check_hooks_apply.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2554 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/check_useless_excludes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      337 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/identity.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/output.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2472 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/parse_shebang.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      495 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/prefix.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8327 2023-02-23 01:44:08.000000 pre_commit-3.3.0/pre_commit/repository.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.773691 pre_commit-3.3.0/pre_commit/resources/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/resources/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        2 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_.npmignore
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       96 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_Cargo.toml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1052 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_LICENSE.renv
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      104 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_Makefile.PL
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12037 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_activate.R
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      302 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_environment.yml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_go.mod
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_main.go
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_main.rs
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_package.json
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      212 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_pubspec.yaml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      351 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_renv.lock
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_setup.py
+-rwxr-xr-x   0 asottile  (1000) asottile  (1000)      528 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/hook-tmpl
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    32551 2023-04-29 17:03:06.000000 pre_commit-3.3.0/pre_commit/resources/rbenv.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    75808 2023-04-29 17:07:26.000000 pre_commit-3.3.0/pre_commit/resources/ruby-build.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2023-04-29 17:03:06.000000 pre_commit-3.3.0/pre_commit/resources/ruby-download.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3922 2023-02-23 01:23:01.000000 pre_commit-3.3.0/pre_commit/staged_files_only.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9257 2023-02-23 01:44:08.000000 pre_commit-3.3.0/pre_commit/store.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6645 2023-03-05 21:04:19.000000 pre_commit-3.3.0/pre_commit/util.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5208 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/xargs.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      499 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/yaml.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.761690 pre_commit-3.3.0/pre_commit.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2947 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1397 2023-05-01 22:23:57.773691 pre_commit-3.3.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-02-20 22:54:27.000000 pre_commit-3.3.0/setup.py
```

### Comparing `pre_commit-3.2.2/LICENSE` & `pre_commit-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/PKG-INFO` & `pre_commit-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre_commit
-Version: 3.2.2
+Version: 3.3.0
 Summary: A framework for managing and maintaining multi-language pre-commit hooks.
 Home-page: https://github.com/pre-commit/pre-commit
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit-3.2.2/pre_commit/all_languages.py` & `pre_commit-3.3.0/pre_commit/all_languages.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/clientlib.py` & `pre_commit-3.3.0/pre_commit/clientlib.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/color.py` & `pre_commit-3.3.0/pre_commit/color.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/autoupdate.py` & `pre_commit-3.3.0/pre_commit/commands/autoupdate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,120 @@
 from __future__ import annotations
 
+import concurrent.futures
 import os.path
 import re
 import tempfile
 from typing import Any
 from typing import NamedTuple
 from typing import Sequence
 
 import pre_commit.constants as C
 from pre_commit import git
 from pre_commit import output
+from pre_commit import xargs
 from pre_commit.clientlib import InvalidManifestError
 from pre_commit.clientlib import load_config
 from pre_commit.clientlib import load_manifest
 from pre_commit.clientlib import LOCAL
 from pre_commit.clientlib import META
 from pre_commit.commands.migrate_config import migrate_config
-from pre_commit.store import Store
 from pre_commit.util import CalledProcessError
 from pre_commit.util import cmd_output
 from pre_commit.util import cmd_output_b
 from pre_commit.yaml import yaml_dump
 from pre_commit.yaml import yaml_load
 
 
 class RevInfo(NamedTuple):
     repo: str
     rev: str
-    frozen: str | None
+    frozen: str | None = None
+    hook_ids: frozenset[str] = frozenset()
 
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> RevInfo:
-        return cls(config['repo'], config['rev'], None)
+        return cls(config['repo'], config['rev'])
 
     def update(self, tags_only: bool, freeze: bool) -> RevInfo:
-        git_cmd = ('git', *git.NO_FS_MONITOR)
+        with tempfile.TemporaryDirectory() as tmp:
+            _git = ('git', *git.NO_FS_MONITOR, '-C', tmp)
 
-        if tags_only:
-            tag_cmd = (
-                *git_cmd, 'describe',
-                'FETCH_HEAD', '--tags', '--abbrev=0',
-            )
-        else:
-            tag_cmd = (
-                *git_cmd, 'describe',
-                'FETCH_HEAD', '--tags', '--exact',
-            )
+            if tags_only:
+                tag_opt = '--abbrev=0'
+            else:
+                tag_opt = '--exact'
+            tag_cmd = (*_git, 'describe', 'FETCH_HEAD', '--tags', tag_opt)
 
-        with tempfile.TemporaryDirectory() as tmp:
             git.init_repo(tmp, self.repo)
+            cmd_output_b(*_git, 'config', 'extensions.partialClone', 'true')
             cmd_output_b(
-                *git_cmd, 'fetch', 'origin', 'HEAD', '--tags',
-                cwd=tmp,
+                *_git, 'fetch', 'origin', 'HEAD',
+                '--quiet', '--filter=blob:none', '--tags',
             )
 
             try:
-                rev = cmd_output(*tag_cmd, cwd=tmp)[1].strip()
+                rev = cmd_output(*tag_cmd)[1].strip()
             except CalledProcessError:
-                cmd = (*git_cmd, 'rev-parse', 'FETCH_HEAD')
-                rev = cmd_output(*cmd, cwd=tmp)[1].strip()
+                rev = cmd_output(*_git, 'rev-parse', 'FETCH_HEAD')[1].strip()
             else:
                 if tags_only:
                     rev = git.get_best_candidate_tag(rev, tmp)
 
             frozen = None
             if freeze:
-                exact_rev_cmd = (*git_cmd, 'rev-parse', rev)
-                exact = cmd_output(*exact_rev_cmd, cwd=tmp)[1].strip()
+                exact = cmd_output(*_git, 'rev-parse', rev)[1].strip()
                 if exact != rev:
                     rev, frozen = exact, rev
-        return self._replace(rev=rev, frozen=frozen)
+
+            try:
+                cmd_output(*_git, 'checkout', rev, '--', C.MANIFEST_FILE)
+            except CalledProcessError:
+                pass  # this will be caught by manifest validating code
+            try:
+                manifest = load_manifest(os.path.join(tmp, C.MANIFEST_FILE))
+            except InvalidManifestError as e:
+                raise RepositoryCannotBeUpdatedError(f'[{self.repo}] {e}')
+            else:
+                hook_ids = frozenset(hook['id'] for hook in manifest)
+
+        return self._replace(rev=rev, frozen=frozen, hook_ids=hook_ids)
 
 
 class RepositoryCannotBeUpdatedError(RuntimeError):
     pass
 
 
 def _check_hooks_still_exist_at_rev(
         repo_config: dict[str, Any],
         info: RevInfo,
-        store: Store,
 ) -> None:
-    try:
-        path = store.clone(repo_config['repo'], info.rev)
-        manifest = load_manifest(os.path.join(path, C.MANIFEST_FILE))
-    except InvalidManifestError as e:
-        raise RepositoryCannotBeUpdatedError(str(e))
-
     # See if any of our hooks were deleted with the new commits
     hooks = {hook['id'] for hook in repo_config['hooks']}
-    hooks_missing = hooks - {hook['id'] for hook in manifest}
+    hooks_missing = hooks - info.hook_ids
     if hooks_missing:
         raise RepositoryCannotBeUpdatedError(
-            f'Cannot update because the update target is missing these '
-            f'hooks:\n{", ".join(sorted(hooks_missing))}',
+            f'[{info.repo}] Cannot update because the update target is '
+            f'missing these hooks: {", ".join(sorted(hooks_missing))}',
         )
 
 
+def _update_one(
+        i: int,
+        repo: dict[str, Any],
+        *,
+        tags_only: bool,
+        freeze: bool,
+) -> tuple[int, RevInfo, RevInfo]:
+    old = RevInfo.from_config(repo)
+    new = old.update(tags_only=tags_only, freeze=freeze)
+    _check_hooks_still_exist_at_rev(repo, new)
+    return i, old, new
+
+
 REV_LINE_RE = re.compile(r'^(\s+)rev:(\s*)([\'"]?)([^\s#]+)(.*)(\r?\n)$')
 
 
 def _original_lines(
         path: str,
         rev_infos: list[RevInfo | None],
         retry: bool = False,
@@ -141,55 +155,59 @@
 
     with open(path, 'w', newline='') as f:
         f.write(''.join(lines))
 
 
 def autoupdate(
         config_file: str,
-        store: Store,
         tags_only: bool,
         freeze: bool,
         repos: Sequence[str] = (),
+        jobs: int = 1,
 ) -> int:
     """Auto-update the pre-commit config to the latest versions of repos."""
     migrate_config(config_file, quiet=True)
-    retv = 0
-    rev_infos: list[RevInfo | None] = []
     changed = False
+    retv = 0
 
-    config = load_config(config_file)
-    for repo_config in config['repos']:
-        if repo_config['repo'] in {LOCAL, META}:
-            continue
-
-        info = RevInfo.from_config(repo_config)
-        if repos and info.repo not in repos:
-            rev_infos.append(None)
-            continue
-
-        output.write(f'Updating {info.repo} ... ')
-        new_info = info.update(tags_only=tags_only, freeze=freeze)
-        try:
-            _check_hooks_still_exist_at_rev(repo_config, new_info, store)
-        except RepositoryCannotBeUpdatedError as error:
-            output.write_line(error.args[0])
-            rev_infos.append(None)
-            retv = 1
-            continue
-
-        if new_info.rev != info.rev:
-            changed = True
-            if new_info.frozen:
-                updated_to = f'{new_info.frozen} (frozen)'
+    config_repos = [
+        repo for repo in load_config(config_file)['repos']
+        if repo['repo'] not in {LOCAL, META}
+    ]
+
+    rev_infos: list[RevInfo | None] = [None] * len(config_repos)
+    jobs = jobs or xargs.cpu_count()  # 0 => number of cpus
+    jobs = min(jobs, len(repos) or len(config_repos))  # max 1-per-thread
+    jobs = max(jobs, 1)  # at least one thread
+    with concurrent.futures.ThreadPoolExecutor(jobs) as exe:
+        futures = [
+            exe.submit(
+                _update_one,
+                i, repo, tags_only=tags_only, freeze=freeze,
+            )
+            for i, repo in enumerate(config_repos)
+            if not repos or repo['repo'] in repos
+        ]
+        for future in concurrent.futures.as_completed(futures):
+            try:
+                i, old, new = future.result()
+            except RepositoryCannotBeUpdatedError as e:
+                output.write_line(str(e))
+                retv = 1
             else:
-                updated_to = new_info.rev
-            msg = f'updating {info.rev} -> {updated_to}.'
-            output.write_line(msg)
-            rev_infos.append(new_info)
-        else:
-            output.write_line('already up to date.')
-            rev_infos.append(None)
+                if new.rev != old.rev:
+                    changed = True
+                    if new.frozen:
+                        new_s = f'{new.frozen} (frozen)'
+                    else:
+                        new_s = new.rev
+                    msg = f'updating {old.rev} -> {new_s}'
+                    rev_infos[i] = new
+                else:
+                    msg = 'already up to date!'
+
+                output.write_line(f'[{old.repo}] {msg}')
 
     if changed:
         _write_new_config(config_file, rev_infos)
 
     return retv
```

### Comparing `pre_commit-3.2.2/pre_commit/commands/gc.py` & `pre_commit-3.3.0/pre_commit/commands/gc.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/hook_impl.py` & `pre_commit-3.3.0/pre_commit/commands/hook_impl.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/init_templatedir.py` & `pre_commit-3.3.0/pre_commit/commands/init_templatedir.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/install_uninstall.py` & `pre_commit-3.3.0/pre_commit/commands/install_uninstall.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/migrate_config.py` & `pre_commit-3.3.0/pre_commit/commands/migrate_config.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/run.py` & `pre_commit-3.3.0/pre_commit/commands/run.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/commands/try_repo.py` & `pre_commit-3.3.0/pre_commit/commands/try_repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/envcontext.py` & `pre_commit-3.3.0/pre_commit/envcontext.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/error_handler.py` & `pre_commit-3.3.0/pre_commit/error_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/file_lock.py` & `pre_commit-3.3.0/pre_commit/file_lock.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/git.py` & `pre_commit-3.3.0/pre_commit/git.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/hook.py` & `pre_commit-3.3.0/pre_commit/hook.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/lang_base.py` & `pre_commit-3.3.0/pre_commit/lang_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 import contextlib
-import multiprocessing
 import os
 import random
 import re
 import shlex
 from typing import Any
 from typing import ContextManager
 from typing import Generator
 from typing import NoReturn
 from typing import Protocol
 from typing import Sequence
 
 import pre_commit.constants as C
 from pre_commit import parse_shebang
+from pre_commit import xargs
 from pre_commit.prefix import Prefix
 from pre_commit.util import cmd_output_b
-from pre_commit.xargs import xargs
 
 FIXED_RANDOM_SEED = 1542676187
 
 SHIMS_RE = re.compile(r'[/\\]shims[/\\]')
 
 
 class Language(Protocol):
@@ -136,18 +135,15 @@
     if 'PRE_COMMIT_NO_CONCURRENCY' in os.environ:
         return 1
     else:
         # Travis appears to have a bunch of CPUs, but we can't use them all.
         if 'TRAVIS' in os.environ:
             return 2
         else:
-            try:
-                return multiprocessing.cpu_count()
-            except NotImplementedError:
-                return 1
+            return xargs.cpu_count()
 
 
 def _shuffled(seq: Sequence[str]) -> list[str]:
     """Deterministically shuffle"""
     fixed_random = random.Random()
     fixed_random.seed(FIXED_RANDOM_SEED, version=1)
 
@@ -167,15 +163,15 @@
         jobs = 1
     else:
         # Shuffle the files so that they more evenly fill out the xargs
         # partitions, but do it deterministically in case a hook cares about
         # ordering.
         file_args = _shuffled(file_args)
         jobs = target_concurrency()
-    return xargs(cmd, file_args, target_concurrency=jobs, color=color)
+    return xargs.xargs(cmd, file_args, target_concurrency=jobs, color=color)
 
 
 def hook_cmd(entry: str, args: Sequence[str]) -> tuple[str, ...]:
     return (*shlex.split(entry), *args)
 
 
 def basic_run_hook(
```

### Comparing `pre_commit-3.2.2/pre_commit/languages/conda.py` & `pre_commit-3.3.0/pre_commit/languages/conda.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/coursier.py` & `pre_commit-3.3.0/pre_commit/languages/coursier.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/dart.py` & `pre_commit-3.3.0/pre_commit/languages/dart.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/docker.py` & `pre_commit-3.3.0/pre_commit/languages/docker.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/docker_image.py` & `pre_commit-3.3.0/pre_commit/languages/docker_image.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/dotnet.py` & `pre_commit-3.3.0/pre_commit/languages/dotnet.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/fail.py` & `pre_commit-3.3.0/pre_commit/languages/fail.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/golang.py` & `pre_commit-3.3.0/pre_commit/languages/golang.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/lua.py` & `pre_commit-3.3.0/pre_commit/languages/lua.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/node.py` & `pre_commit-3.3.0/pre_commit/languages/node.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/perl.py` & `pre_commit-3.3.0/pre_commit/languages/perl.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/pygrep.py` & `pre_commit-3.3.0/pre_commit/languages/pygrep.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/python.py` & `pre_commit-3.3.0/pre_commit/languages/python.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/r.py` & `pre_commit-3.3.0/pre_commit/languages/r.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/ruby.py` & `pre_commit-3.3.0/pre_commit/languages/ruby.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/rust.py` & `pre_commit-3.3.0/pre_commit/languages/rust.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/script.py` & `pre_commit-3.3.0/pre_commit/languages/script.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/languages/swift.py` & `pre_commit-3.3.0/pre_commit/languages/swift.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/logging_handler.py` & `pre_commit-3.3.0/pre_commit/logging_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/main.py` & `pre_commit-3.3.0/pre_commit/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,17 +222,21 @@
         ),
     )
     autoupdate_parser.add_argument(
         '--freeze', action='store_true',
         help='Store "frozen" hashes in `rev` instead of tag names',
     )
     autoupdate_parser.add_argument(
-        '--repo', dest='repos', action='append', metavar='REPO',
+        '--repo', dest='repos', action='append', metavar='REPO', default=[],
         help='Only update this repository -- may be specified multiple times.',
     )
+    autoupdate_parser.add_argument(
+        '-j', '--jobs', type=int, default=1,
+        help='Number of threads to use.  (default %(default)s).',
+    )
 
     _add_cmd('clean', help='Clean out pre-commit files.')
 
     _add_cmd('gc', help='Clean unused cached repos.')
 
     init_templatedir_parser = _add_cmd(
         'init-templatedir',
@@ -364,18 +368,19 @@
 
         if args.command not in COMMANDS_NO_GIT:
             _adjust_args_and_chdir(args)
             store.mark_config_used(args.config)
 
         if args.command == 'autoupdate':
             return autoupdate(
-                args.config, store,
+                args.config,
                 tags_only=not args.bleeding_edge,
                 freeze=args.freeze,
                 repos=args.repos,
+                jobs=args.jobs,
             )
         elif args.command == 'clean':
             return clean(store)
         elif args.command == 'gc':
             return gc(store)
         elif args.command == 'hook-impl':
             return hook_impl(
```

### Comparing `pre_commit-3.2.2/pre_commit/meta_hooks/check_hooks_apply.py` & `pre_commit-3.3.0/pre_commit/meta_hooks/check_hooks_apply.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/meta_hooks/check_useless_excludes.py` & `pre_commit-3.3.0/pre_commit/meta_hooks/check_useless_excludes.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/output.py` & `pre_commit-3.3.0/pre_commit/output.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/parse_shebang.py` & `pre_commit-3.3.0/pre_commit/parse_shebang.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/repository.py` & `pre_commit-3.3.0/pre_commit/repository.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/resources/empty_template_LICENSE.renv` & `pre_commit-3.3.0/pre_commit/resources/empty_template_LICENSE.renv`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/resources/empty_template_activate.R` & `pre_commit-3.3.0/pre_commit/resources/empty_template_activate.R`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/resources/hook-tmpl` & `pre_commit-3.3.0/pre_commit/resources/hook-tmpl`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/resources/rbenv.tar.gz` & `pre_commit-3.3.0/pre_commit/resources/rbenv.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/resources/ruby-download.tar.gz` & `pre_commit-3.3.0/pre_commit/resources/ruby-download.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/staged_files_only.py` & `pre_commit-3.3.0/pre_commit/staged_files_only.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/store.py` & `pre_commit-3.3.0/pre_commit/store.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/util.py` & `pre_commit-3.3.0/pre_commit/util.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/pre_commit/xargs.py` & `pre_commit-3.3.0/pre_commit/xargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import concurrent.futures
 import contextlib
 import math
+import multiprocessing
 import os
 import subprocess
 import sys
 from typing import Any
 from typing import Callable
 from typing import Generator
 from typing import Iterable
@@ -18,14 +19,21 @@
 from pre_commit.util import cmd_output_b
 from pre_commit.util import cmd_output_p
 
 TArg = TypeVar('TArg')
 TRet = TypeVar('TRet')
 
 
+def cpu_count() -> int:
+    try:
+        return multiprocessing.cpu_count()
+    except NotImplementedError:
+        return 1
+
+
 def _environ_size(_env: MutableMapping[str, str] | None = None) -> int:
     environ = _env if _env is not None else getattr(os, 'environb', os.environ)
     size = 8 * len(environ)  # number of pointers in `envp`
     for k, v in environ.items():
         size += len(k) + len(v) + 2  # c strings in `envp`
     return size
```

### Comparing `pre_commit-3.2.2/pre_commit.egg-info/PKG-INFO` & `pre_commit-3.3.0/pre_commit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit
-Version: 3.2.2
+Version: 3.3.0
 Summary: A framework for managing and maintaining multi-language pre-commit hooks.
 Home-page: https://github.com/pre-commit/pre-commit
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit-3.2.2/pre_commit.egg-info/SOURCES.txt` & `pre_commit-3.3.0/pre_commit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pre_commit-3.2.2/setup.cfg` & `pre_commit-3.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pre_commit
-version = 3.2.2
+version = 3.3.0
 description = A framework for managing and maintaining multi-language pre-commit hooks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pre-commit/pre-commit
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

