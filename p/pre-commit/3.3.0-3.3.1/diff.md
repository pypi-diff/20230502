# Comparing `tmp/pre_commit-3.3.0.tar.gz` & `tmp/pre_commit-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit-3.3.0.tar", last modified: Mon May  1 22:23:57 2023, max compression
+gzip compressed data, was "pre_commit-3.3.1.tar", last modified: Tue May  2 14:07:33 2023, max compression
```

## Comparing `pre_commit-3.3.0.tar` & `pre_commit-3.3.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.773691 pre_commit-3.3.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:40.000000 pre_commit-3.3.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-05-01 22:23:57.773691 pre_commit-3.3.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      480 2022-12-31 16:55:07.000000 pre_commit-3.3.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.761690 pre_commit-3.3.0/pre_commit/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      127 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1357 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/all_languages.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12139 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/clientlib.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3219 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/color.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.765690 pre_commit-3.3.0/pre_commit/commands/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7022 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/commands/autoupdate.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/clean.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2804 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/gc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9391 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/commands/hook_impl.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/init_templatedir.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5408 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/install_uninstall.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2099 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/migrate_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14102 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/commands/run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      453 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/sample_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2578 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/try_repo.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      362 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/validate_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      368 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/commands/validate_manifest.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      282 2023-03-17 16:29:01.000000 pre_commit-3.3.0/pre_commit/constants.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1612 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/envcontext.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2624 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/error_handler.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/errors.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2369 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/file_lock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8509 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/git.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1504 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/hook.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5232 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/lang_base.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.769691 pre_commit-3.3.0/pre_commit/languages/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/languages/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2415 2023-03-05 21:04:19.000000 pre_commit-3.3.0/pre_commit/languages/conda.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2502 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/coursier.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3112 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/dart.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4630 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/docker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      827 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/docker_image.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3469 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/dotnet.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      676 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/fail.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4531 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/golang.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2529 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/lua.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3831 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/node.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2023-02-21 16:06:00.000000 pre_commit-3.3.0/pre_commit/languages/perl.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3811 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/pygrep.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6806 2023-03-05 21:04:19.000000 pre_commit-3.3.0/pre_commit/languages/python.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4863 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/r.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4396 2023-02-21 15:20:44.000000 pre_commit-3.3.0/pre_commit/languages/ruby.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5470 2023-03-25 18:01:33.000000 pre_commit-3.3.0/pre_commit/languages/rust.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      777 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/script.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1599 2023-04-03 20:26:07.000000 pre_commit-3.3.0/pre_commit/languages/swift.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2023-02-21 15:20:22.000000 pre_commit-3.3.0/pre_commit/languages/system.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1022 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/logging_handler.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    15466 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.769691 pre_commit-3.3.0/pre_commit/meta_hooks/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1193 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/check_hooks_apply.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2554 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/check_useless_excludes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      337 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/meta_hooks/identity.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/output.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2472 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/parse_shebang.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      495 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/prefix.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8327 2023-02-23 01:44:08.000000 pre_commit-3.3.0/pre_commit/repository.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.773691 pre_commit-3.3.0/pre_commit/resources/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/resources/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)        2 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_.npmignore
--rw-r--r--   0 asottile  (1000) asottile  (1000)       96 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_Cargo.toml
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1052 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_LICENSE.renv
--rw-r--r--   0 asottile  (1000) asottile  (1000)      104 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_Makefile.PL
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12037 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_activate.R
--rw-r--r--   0 asottile  (1000) asottile  (1000)      302 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_environment.yml
--rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_go.mod
--rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_main.go
--rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_main.rs
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_package.json
--rw-r--r--   0 asottile  (1000) asottile  (1000)      212 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
--rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
--rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_pubspec.yaml
--rw-r--r--   0 asottile  (1000) asottile  (1000)      351 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_renv.lock
--rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/resources/empty_template_setup.py
--rwxr-xr-x   0 asottile  (1000) asottile  (1000)      528 2022-04-30 16:59:40.000000 pre_commit-3.3.0/pre_commit/resources/hook-tmpl
--rw-r--r--   0 asottile  (1000) asottile  (1000)    32551 2023-04-29 17:03:06.000000 pre_commit-3.3.0/pre_commit/resources/rbenv.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)    75808 2023-04-29 17:07:26.000000 pre_commit-3.3.0/pre_commit/resources/ruby-build.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2023-04-29 17:03:06.000000 pre_commit-3.3.0/pre_commit/resources/ruby-download.tar.gz
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3922 2023-02-23 01:23:01.000000 pre_commit-3.3.0/pre_commit/staged_files_only.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9257 2023-02-23 01:44:08.000000 pre_commit-3.3.0/pre_commit/store.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6645 2023-03-05 21:04:19.000000 pre_commit-3.3.0/pre_commit/util.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5208 2023-05-01 22:20:01.000000 pre_commit-3.3.0/pre_commit/xargs.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      499 2023-02-20 22:54:27.000000 pre_commit-3.3.0/pre_commit/yaml.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-01 22:23:57.761690 pre_commit-3.3.0/pre_commit.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2947 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-05-01 22:23:57.000000 pre_commit-3.3.0/pre_commit.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1397 2023-05-01 22:23:57.773691 pre_commit-3.3.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-02-20 22:54:27.000000 pre_commit-3.3.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.299011 pre_commit-3.3.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:40.000000 pre_commit-3.3.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-05-02 14:07:33.299011 pre_commit-3.3.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      480 2022-12-31 16:55:07.000000 pre_commit-3.3.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.291011 pre_commit-3.3.1/pre_commit/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      127 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1357 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/all_languages.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12139 2023-03-17 16:29:01.000000 pre_commit-3.3.1/pre_commit/clientlib.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3219 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/color.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.295011 pre_commit-3.3.1/pre_commit/commands/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7148 2023-05-02 14:05:55.000000 pre_commit-3.3.1/pre_commit/commands/autoupdate.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/clean.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2804 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/gc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9391 2023-03-17 16:29:01.000000 pre_commit-3.3.1/pre_commit/commands/hook_impl.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/init_templatedir.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5408 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/install_uninstall.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2099 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/migrate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14102 2023-03-17 16:29:01.000000 pre_commit-3.3.1/pre_commit/commands/run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      453 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/sample_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2578 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/try_repo.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      362 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/validate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      368 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/commands/validate_manifest.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      282 2023-03-17 16:29:01.000000 pre_commit-3.3.1/pre_commit/constants.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1612 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/envcontext.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2624 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/error_handler.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/errors.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2369 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/file_lock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8509 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/git.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1504 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/hook.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5232 2023-05-01 22:20:01.000000 pre_commit-3.3.1/pre_commit/lang_base.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.295011 pre_commit-3.3.1/pre_commit/languages/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/languages/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2415 2023-03-05 21:04:19.000000 pre_commit-3.3.1/pre_commit/languages/conda.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2502 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/coursier.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3112 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/dart.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4630 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/docker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      827 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/docker_image.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3469 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/dotnet.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      676 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/fail.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4531 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/golang.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2529 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/lua.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3831 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/node.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2023-02-21 16:06:00.000000 pre_commit-3.3.1/pre_commit/languages/perl.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3811 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/pygrep.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6806 2023-03-05 21:04:19.000000 pre_commit-3.3.1/pre_commit/languages/python.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4863 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/r.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4396 2023-02-21 15:20:44.000000 pre_commit-3.3.1/pre_commit/languages/ruby.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5470 2023-03-25 18:01:33.000000 pre_commit-3.3.1/pre_commit/languages/rust.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      777 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/script.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1599 2023-04-03 20:26:07.000000 pre_commit-3.3.1/pre_commit/languages/swift.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2023-02-21 15:20:22.000000 pre_commit-3.3.1/pre_commit/languages/system.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1022 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/logging_handler.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    15466 2023-05-01 22:20:01.000000 pre_commit-3.3.1/pre_commit/main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.295011 pre_commit-3.3.1/pre_commit/meta_hooks/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/meta_hooks/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1193 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/meta_hooks/check_hooks_apply.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2554 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/meta_hooks/check_useless_excludes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      337 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/meta_hooks/identity.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/output.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2472 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/parse_shebang.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      495 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/prefix.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8327 2023-02-23 01:44:08.000000 pre_commit-3.3.1/pre_commit/repository.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.299011 pre_commit-3.3.1/pre_commit/resources/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/resources/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        2 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_.npmignore
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       96 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_Cargo.toml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1052 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_LICENSE.renv
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      104 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_Makefile.PL
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12037 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_activate.R
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      302 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_environment.yml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_go.mod
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_main.go
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_main.rs
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_package.json
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      212 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_pre-commit-package-dev-1.rockspec
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_pre_commit_placeholder_package.gemspec
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       78 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_pubspec.yaml
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      351 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_renv.lock
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/resources/empty_template_setup.py
+-rwxr-xr-x   0 asottile  (1000) asottile  (1000)      528 2022-04-30 16:59:40.000000 pre_commit-3.3.1/pre_commit/resources/hook-tmpl
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    32551 2023-04-29 17:03:06.000000 pre_commit-3.3.1/pre_commit/resources/rbenv.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    75808 2023-04-29 17:07:26.000000 pre_commit-3.3.1/pre_commit/resources/ruby-build.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2023-04-29 17:03:06.000000 pre_commit-3.3.1/pre_commit/resources/ruby-download.tar.gz
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3922 2023-02-23 01:23:01.000000 pre_commit-3.3.1/pre_commit/staged_files_only.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9257 2023-02-23 01:44:08.000000 pre_commit-3.3.1/pre_commit/store.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6645 2023-03-05 21:04:19.000000 pre_commit-3.3.1/pre_commit/util.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5208 2023-05-01 22:20:01.000000 pre_commit-3.3.1/pre_commit/xargs.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      499 2023-02-20 22:54:27.000000 pre_commit-3.3.1/pre_commit/yaml.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-02 14:07:33.291011 pre_commit-3.3.1/pre_commit.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1121 2023-05-02 14:07:33.000000 pre_commit-3.3.1/pre_commit.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2947 2023-05-02 14:07:33.000000 pre_commit-3.3.1/pre_commit.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-02 14:07:33.000000 pre_commit-3.3.1/pre_commit.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2023-05-02 14:07:33.000000 pre_commit-3.3.1/pre_commit.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2023-05-02 14:07:33.000000 pre_commit-3.3.1/pre_commit.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-05-02 14:07:33.000000 pre_commit-3.3.1/pre_commit.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1397 2023-05-02 14:07:33.299011 pre_commit-3.3.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-02-20 22:54:27.000000 pre_commit-3.3.1/setup.py
```

### Comparing `pre_commit-3.3.0/LICENSE` & `pre_commit-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/PKG-INFO` & `pre_commit-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre_commit
-Version: 3.3.0
+Version: 3.3.1
 Summary: A framework for managing and maintaining multi-language pre-commit hooks.
 Home-page: https://github.com/pre-commit/pre-commit
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit-3.3.0/pre_commit/all_languages.py` & `pre_commit-3.3.1/pre_commit/all_languages.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/clientlib.py` & `pre_commit-3.3.1/pre_commit/clientlib.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/color.py` & `pre_commit-3.3.1/pre_commit/color.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/autoupdate.py` & `pre_commit-3.3.1/pre_commit/commands/autoupdate.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,16 @@
             frozen = None
             if freeze:
                 exact = cmd_output(*_git, 'rev-parse', rev)[1].strip()
                 if exact != rev:
                     rev, frozen = exact, rev
 
             try:
+                # workaround for windows -- see #2865
+                cmd_output_b(*_git, 'show', f'{rev}:{C.MANIFEST_FILE}')
                 cmd_output(*_git, 'checkout', rev, '--', C.MANIFEST_FILE)
             except CalledProcessError:
                 pass  # this will be caught by manifest validating code
             try:
                 manifest = load_manifest(os.path.join(tmp, C.MANIFEST_FILE))
             except InvalidManifestError as e:
                 raise RepositoryCannotBeUpdatedError(f'[{self.repo}] {e}')
```

### Comparing `pre_commit-3.3.0/pre_commit/commands/gc.py` & `pre_commit-3.3.1/pre_commit/commands/gc.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/hook_impl.py` & `pre_commit-3.3.1/pre_commit/commands/hook_impl.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/init_templatedir.py` & `pre_commit-3.3.1/pre_commit/commands/init_templatedir.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/install_uninstall.py` & `pre_commit-3.3.1/pre_commit/commands/install_uninstall.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/migrate_config.py` & `pre_commit-3.3.1/pre_commit/commands/migrate_config.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/run.py` & `pre_commit-3.3.1/pre_commit/commands/run.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/commands/try_repo.py` & `pre_commit-3.3.1/pre_commit/commands/try_repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/envcontext.py` & `pre_commit-3.3.1/pre_commit/envcontext.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/error_handler.py` & `pre_commit-3.3.1/pre_commit/error_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/file_lock.py` & `pre_commit-3.3.1/pre_commit/file_lock.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/git.py` & `pre_commit-3.3.1/pre_commit/git.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/hook.py` & `pre_commit-3.3.1/pre_commit/hook.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/lang_base.py` & `pre_commit-3.3.1/pre_commit/lang_base.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/conda.py` & `pre_commit-3.3.1/pre_commit/languages/conda.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/coursier.py` & `pre_commit-3.3.1/pre_commit/languages/coursier.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/dart.py` & `pre_commit-3.3.1/pre_commit/languages/dart.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/docker.py` & `pre_commit-3.3.1/pre_commit/languages/docker.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/docker_image.py` & `pre_commit-3.3.1/pre_commit/languages/docker_image.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/dotnet.py` & `pre_commit-3.3.1/pre_commit/languages/dotnet.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/fail.py` & `pre_commit-3.3.1/pre_commit/languages/fail.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/golang.py` & `pre_commit-3.3.1/pre_commit/languages/golang.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/lua.py` & `pre_commit-3.3.1/pre_commit/languages/lua.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/node.py` & `pre_commit-3.3.1/pre_commit/languages/node.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/perl.py` & `pre_commit-3.3.1/pre_commit/languages/perl.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/pygrep.py` & `pre_commit-3.3.1/pre_commit/languages/pygrep.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/python.py` & `pre_commit-3.3.1/pre_commit/languages/python.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/r.py` & `pre_commit-3.3.1/pre_commit/languages/r.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/ruby.py` & `pre_commit-3.3.1/pre_commit/languages/ruby.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/rust.py` & `pre_commit-3.3.1/pre_commit/languages/rust.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/script.py` & `pre_commit-3.3.1/pre_commit/languages/script.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/languages/swift.py` & `pre_commit-3.3.1/pre_commit/languages/swift.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/logging_handler.py` & `pre_commit-3.3.1/pre_commit/logging_handler.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/main.py` & `pre_commit-3.3.1/pre_commit/main.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/meta_hooks/check_hooks_apply.py` & `pre_commit-3.3.1/pre_commit/meta_hooks/check_hooks_apply.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/meta_hooks/check_useless_excludes.py` & `pre_commit-3.3.1/pre_commit/meta_hooks/check_useless_excludes.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/output.py` & `pre_commit-3.3.1/pre_commit/output.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/parse_shebang.py` & `pre_commit-3.3.1/pre_commit/parse_shebang.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/repository.py` & `pre_commit-3.3.1/pre_commit/repository.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/resources/empty_template_LICENSE.renv` & `pre_commit-3.3.1/pre_commit/resources/empty_template_LICENSE.renv`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/resources/empty_template_activate.R` & `pre_commit-3.3.1/pre_commit/resources/empty_template_activate.R`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/resources/hook-tmpl` & `pre_commit-3.3.1/pre_commit/resources/hook-tmpl`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/resources/rbenv.tar.gz` & `pre_commit-3.3.1/pre_commit/resources/rbenv.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/resources/ruby-build.tar.gz` & `pre_commit-3.3.1/pre_commit/resources/ruby-build.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/resources/ruby-download.tar.gz` & `pre_commit-3.3.1/pre_commit/resources/ruby-download.tar.gz`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/staged_files_only.py` & `pre_commit-3.3.1/pre_commit/staged_files_only.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/store.py` & `pre_commit-3.3.1/pre_commit/store.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/util.py` & `pre_commit-3.3.1/pre_commit/util.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit/xargs.py` & `pre_commit-3.3.1/pre_commit/xargs.py`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/pre_commit.egg-info/PKG-INFO` & `pre_commit-3.3.1/pre_commit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit
-Version: 3.3.0
+Version: 3.3.1
 Summary: A framework for managing and maintaining multi-language pre-commit hooks.
 Home-page: https://github.com/pre-commit/pre-commit
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pre_commit-3.3.0/pre_commit.egg-info/SOURCES.txt` & `pre_commit-3.3.1/pre_commit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pre_commit-3.3.0/setup.cfg` & `pre_commit-3.3.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pre_commit
-version = 3.3.0
+version = 3.3.1
 description = A framework for managing and maintaining multi-language pre-commit hooks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pre-commit/pre-commit
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

